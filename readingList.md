<!-- readingList.html -->
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>My Reading List</title>
    <style>
        body { font-family: sans-serif; max-width: 800px; margin: auto; }
        .item { border: 1px solid #ccc; padding: 10px; margin: 10px 0; }
        img { max-width: 200px; }
    </style>
</head>
<body>
    <h1>My Reading List</h1>
    <div id="list">Loading...</div>

    <script>
        fetch('http://127.0.0.1:8080/api/readingList')
            .then(res => res.json())
            .then(data => {
                const list = document.getElementById('list');
                list.innerHTML = '';

                if (data.length === 0) {
                    list.innerHTML = '<p>No items yet.</p>';
                    return;
                }

                data.forEach(item => {
                    const div = document.createElement('div');
                    div.className = 'item';
                    div.innerHTML = `
                        <h2><a href="${item.url}" target="_blank">${item.title}</a></h2>
                        ${item.image ? `<img src="${item.image}">` : ''}
                        <p>${item.description}</p>
                    `;
                    list.appendChild(div);
                });
            });
    </script>
</body>
</html>

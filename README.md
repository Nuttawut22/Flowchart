<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flowchart ง่ายๆ</title>
    <!-- ดึงไลบรารี Mermaid.js มารันโฟลว์ชาร์ต -->
    <script type="module">
        import mermaid from 'https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.esm.min.mjs';
        mermaid.initialize({ startOnLoad: true });
    </script>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #f5f7fb;
        }
        h2 {
            color: #333;
            margin-bottom: 20px;
        }
        .flowchart-container {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
    </style>
</head>
<body>

    <h2>ตัวอย่าง Flowchart การตัดสินใจดื่มกาแฟ</h2>

    <div class="flowchart-container">
        <!-- เขียนโครงสร้างโฟลว์ชาร์ตตรงนี้ -->
        <pre class="mermaid">
            graph TD
                A([เริ่มทำงาน]) --> B{ง่วงนอนไหม?}
                B -- ใช่ --> C[ไปชงกาแฟ]
                B -- ไม่ --> D[ทำงานต่อ]
                C --> E([จบการทำงาน])
                D --> E
        </pre>
    </div>

</body>
</html>

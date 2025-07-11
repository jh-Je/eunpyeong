<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <title>현장대응 자료 다운로드</title>
  <script src="https://cdn.tailwindcss.com"></script>
</head>
<body class="bg-gray-100 flex items-center justify-center min-h-screen">
  <div class="text-center">
    <h1 class="text-2xl font-bold mb-6">현장대응 자료 다운로드</h1>
    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
      <!-- 다운로드 버튼 1: c1.pdf -->
      <button
        class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c1.pdf', '현장대응 가정폭력.pdf')"
      >
        현장대응 가정폭력 다운로드
      </button>

      <!-- 다운로드 버튼 2: c2.pdf -->
      <button
        class="bg-green-600 hover:bg-green-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c2.pdf', '보이스피싱 대응 요령.pdf')"
      >
        보이스피싱 대응 요령 다운로드
      </button>
    </div>
  </div>

  <script>
    function downloadFile(url, filename) {
      const a = document.createElement('a');
      a.href = url;
      a.download = filename;
      document.body.appendChild(a);
      a.click();
      document.body.removeChild(a);
    }
  </script>
</body>
</html>

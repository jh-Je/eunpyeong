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
      <!-- 다운로드 버튼 1 -->
      <button
        class="bg-blue-600 hover:bg-blue-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c1.pdf', '현장대응 가정폭력.pdf')"
      >
        현장대응 가정폭력 다운로드
      </button>

      <!-- 다운로드 버튼 2 -->
      <button
        class="bg-green-600 hover:bg-green-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c2.pdf', '보이스피싱 대응 요령.pdf')"
      >
        보이스피싱 대응 요령 다운로드
      </button>

      <!-- 다운로드 버튼 3 -->
      <button
        class="bg-purple-600 hover:bg-purple-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c3.pdf', '관계성 범죄 현장대응.pdf')"
      >
        관계성 범죄 현장대응 다운로드
      </button>

      <!-- 다운로드 버튼 4 -->
      <button
        class="bg-yellow-600 hover:bg-yellow-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c4.pdf', '불법체류자 업무처리 요령.pdf')"
      >
        불법체류자 업무처리 요령 다운로드
      </button>

      <!-- 다운로드 버튼 5 -->
      <button
        class="bg-red-600 hover:bg-red-700 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c5.pdf', '정신질환자 응급입원 대응.pdf')"
      >
        정신질환자 응급입원 대응 다운로드
      </button>

      <!-- 다운로드 버튼 6 -->
      <button
        class="bg-gray-700 hover:bg-gray-800 text-white font-bold py-3 px-6 rounded-2xl shadow"
        onclick="downloadFile('./c6.pdf', '피난명령 및 신고처리법.pdf')"
      >
        피난명령 및 신고처리법 다운로드
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

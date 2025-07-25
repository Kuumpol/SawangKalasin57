<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>ศูนย์กู้ภัยสว่างกาฬสินธุ์</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f9f9f9;
      color: #333;
    }

    header {
      background-color: #b71c1c;
      color: white;
      padding: 30px 20px;
      text-align: center;
    }

    header h1 {
      margin: 0;
      font-size: 2.5em;
    }

    header p {
      font-size: 1.2em;
      margin-top: 5px;
    }

    nav {
      background-color: #d32f2f;
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      padding: 10px 0;
      box-shadow: 0 2px 5px rgba(0,0,0,0.2);
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 10px 20px;
      font-weight: bold;
      padding: 8px 16px;
      border-radius: 20px;
      transition: background 0.3s;
      cursor: pointer;
    }

    nav a:hover {
      background-color: rgba(255,255,255,0.2);
    }

    main {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    section {
      background: white;
      margin-bottom: 40px;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.08);
      display: none;
    }

    section.active {
      display: block;
    }

    h2 {
      color: #c62828;
      margin-top: 0;
    }

    ul {
      list-style-type: none;
      padding-left: 0;
    }

    ul li {
      margin-bottom: 10px;
      padding-left: 20px;
      position: relative;
    }

    ul li::before {
      content: "✔️";
      position: absolute;
      left: 0;
      color: #4caf50;
    }

    .donation-info p {
      margin: 10px 0;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #c62828;
      color: white;
      margin-top: 50px;
    }

    .home {
      background: white;
      padding: 40px;
      text-align: center;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.08);
    }

    .home h2 {
      color: #c62828;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 1.8em;
      }

      nav {
        flex-direction: column;
        align-items: center;
      }

      nav a {
        margin: 5px 0;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>ศูนย์กู้ภัยสว่างกาฬสินธุ์</h1>
    <p>เราพร้อมช่วยเหลือ 24 ชั่วโมง ทุกชีวิตมีค่า</p>
  </header>

  <nav>
    <a onclick="showSection('home')">หน้าแรก</a>
    <a onclick="showSection('mission')">ภารกิจ</a>
    <a onclick="showSection('departments')">ฝ่ายต่างๆ</a>
    <a onclick="showSection('donation')">บริจาค</a>
    <a onclick="showSection('contact')">ติดต่อ</a>
  </nav>

  <main>
    <div id="home" class="home active">
      <h2>ยินดีต้อนรับสู่ศูนย์กู้ภัยสว่างกาฬสินธุ์</h2>
      <p>เราคือองค์กรจิตอาสาที่มุ่งมั่นในการช่วยเหลือชีวิตผู้ประสบภัยในทุกสถานการณ์<br>กรุณาเลือกหัวข้อจากด้านบนเพื่อดูข้อมูลเพิ่มเติม</p>
    </div>

    <section id="mission">
      <h2>ภารกิจหลักของเรา</h2>
      <ul>
        <li>ช่วยเหลือผู้ประสบอุบัติเหตุบนถนนและในพื้นที่ห่างไกล</li>
        <li>กู้ภัยน้ำท่วมและภัยพิบัติธรรมชาติในเขตจังหวัดกาฬสินธุ์</li>
        <li>สนับสนุนการขนส่งผู้ป่วยฉุกเฉินร่วมกับหน่วยงานอื่น</li>
        <li>ดับเพลิงและควบคุมเหตุเพลิงไหม้เบื้องต้นในชุมชน</li>
        <li>ฝึกอบรมและสร้างจิตอาสาด้านการปฐมพยาบาลและกู้ชีพ</li>
      </ul>
    </section>

    <section id="departments">
      <h2>ฝ่ายปฏิบัติงานภายในศูนย์</h2>
      <ul>
        <li>ฝ่ายปฏิบัติการภาคสนาม – รับผิดชอบการเข้าพื้นที่จริงและช่วยเหลือผู้ประสบเหตุ</li>
        <li>ฝ่ายสนับสนุนการแพทย์ – ดูแลเครื่องมือปฐมพยาบาลและประสานโรงพยาบาล</li>
        <li>ฝ่ายสื่อสารและควบคุม – รับแจ้งเหตุและประสานงานผ่านวิทยุสื่อสารและโทรศัพท์</li>
        <li>ฝ่ายพัฒนาและฝึกอบรม – จัดกิจกรรมฝึกซ้อมและฝึกอบรมจิตอาสา</li>
        <li>ฝ่ายบริหารและการเงิน – จัดการทรัพยากรและรายรับรายจ่ายขององค์กร</li>
      </ul>
    </section>

    <section id="donation">
      <h2>ร่วมบริจาคเพื่อสนับสนุนภารกิจกู้ภัย</h2>
      <div class="donation-info">
        <p>🙏 ศูนย์กู้ภัยสว่างกาฬสินธุ์ เปิดรับบริจาคเพื่อสนับสนุนอุปกรณ์กู้ชีพ รถพยาบาล และกิจกรรมจิตอาสา</p>
        <p><strong>บัญชีธนาคาร:</strong><br>
          ธนาคารกรุงเทพ<br>
          ชื่อบัญชี: มูลนิธิสว่างกาฬสินธุ์<br>
          เลขที่บัญชี: 315-4-34390-3<br>
        </p>
        <p>📞 สอบถามเพิ่มเติม: 080-228-1685 หรือ inbox เพจ Facebook: <a href="#" style="color: #c62828;">สว่างกาฬสินธุ์</a></p>
        <p>ทุกยอดบริจาคสามารถขอใบอนุโมทนาบัตรเพื่อลดหย่อนภาษีได้</p>
      </div>
    </section>

    <section id="contact">
      <h2>ข้อมูลติดต่อ</h2>
      <p>📞 โทรศัพท์: 043-840-243 (ศูนย์กลาง) | สายด่วน: 1669</p>
      <p>📧 อีเมล: sawangkalasin5757e@gmail.com</p>
      <p>📍 ที่อยู่: 456 ถ.ดงปอ ต.กาฬสินธุ์ อ.เมือง จ.กาฬสินธุ์ 46000</p>
      <p>🕒 เปิดบริการตลอด 24 ชั่วโมง ทุกวัน</p>
    </section>
  </main>

  <footer>
    &copy; 2025 ศูนย์กู้ภัยสว่างกาฬสินธุ์ | ร่วมด้วยช่วยกันเพื่อชีวิต
  </footer>

  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('section, .home');
      sections.forEach(sec => sec.classList.remove('active'));
      document.getElementById(id).classList.add('active');
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  </script>
</body>
</html>

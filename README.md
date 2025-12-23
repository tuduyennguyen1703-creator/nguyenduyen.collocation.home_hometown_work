Huyền_Speaking_1-100
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Luyện 200 Từ Vựng - Red Edition Pro</title>
    <style>
        :root {
            --primary-color: #d32f2f;
            --secondary-color: #b71c1c;
            --accent-light: #ffebee;
            --bg-color: #fdf2f2;
            --card-bg: #ffffff;
            --text-color: #333333;
            --success-color: #2e7d32;
            --warning-color: #f57f17;
            --gray-color: #757575;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            color: var(--text-color);
            padding: 10px;
            box-sizing: border-box;
        }

        .container {
            background-color: var(--card-bg);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(211, 47, 47, 0.15);
            width: 100%;
            max-width: 500px;
            text-align: center;
            border-top: 5px solid var(--primary-color);
            position: relative;
            box-sizing: border-box;
        }

        /* Header & Progress */
        .header-row {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }

        .header-controls {
            display: flex;
            gap: 10px;
        }

        .btn-icon {
            background: none;
            border: none;
            font-size: 22px; 
            cursor: pointer;
            color: var(--primary-color);
            padding: 5px;
            transition: transform 0.2s;
        }
        .btn-icon:hover { transform: scale(1.1); }

        .progress-bar {
            color: #ef5350;
            font-weight: 600;
            font-size: 14px;
            letter-spacing: 1px;
        }

        /* Card Area */
        .card {
            min-height: 280px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            position: relative;
        }

        .vietnamese-text {
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
            color: #2c3e50;
            line-height: 1.4;
            word-wrap: break-word; 
        }

        .hidden-content {
            display: none;
            animation: fadeIn 0.5s ease-out;
            width: 100%;
        }

        .english-row {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin: 5px 0;
            flex-wrap: wrap;
        }

        .english-word {
            font-size: 32px;
            color: var(--primary-color);
            font-weight: 800;
            text-shadow: 1px 1px 0px rgba(0,0,0,0.05);
            margin: 0;
            word-break: break-word; 
        }

        .ipa-text {
            font-family: 'Lucida Sans Unicode', 'Arial Unicode MS', sans-serif;
            font-size: 18px;
            color: #757575;
            margin-bottom: 10px;
            font-weight: 400;
        }

        .btn-audio-replay {
            background: white;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
            width: 40px; 
            height: 40px;
            border-radius: 50%;
            cursor: pointer;
            font-size: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.2s;
            flex-shrink: 0;
            -webkit-tap-highlight-color: transparent; 
        }
        .btn-audio-replay:hover {
            background: var(--primary-color);
            color: white;
            transform: scale(1.1);
        }

        .part-of-speech {
            font-style: italic;
            color: #c62828;
            margin-bottom: 5px;
            font-size: 14px;
            background: var(--accent-light);
            padding: 5px 12px;
            border-radius: 15px;
            display: inline-block;
            border: 1px solid #ffcdd2;
        }

        /* Buttons */
        .btn {
            border: none;
            padding: 14px 20px; 
            font-size: 16px;
            font-weight: 600;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s, box-shadow 0.2s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            color: white;
            -webkit-tap-highlight-color: transparent;
        }
        
        .btn:hover { transform: translateY(-2px); box-shadow: 0 6px 12px rgba(0,0,0,0.15); }
        .btn:active { transform: translateY(1px); }
        .btn:disabled { background: #bdbdbd !important; cursor: not-allowed; transform: none; box-shadow: none; color: #fff;}

        .btn-reveal {
            background: linear-gradient(135deg, var(--primary-color), var(--secondary-color));
            width: 100%;
            margin-top: 20px;
            font-size: 18px;
        }

        .nav-row {
            display: flex;
            justify-content: space-between;
            margin-top: 25px;
            gap: 15px;
        }

        .btn-nav {
            background-color: white;
            color: var(--primary-color);
            border: 2px solid var(--primary-color);
            width: 55px; 
            height: 55px;
            border-radius: 50%;
            font-size: 22px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0;
        }

        .review-actions {
            display: flex;
            gap: 10px;
            margin-top: 20px;
            justify-content: center;
        }

        .btn-learn { background-color: var(--warning-color); flex: 1; }
        .btn-success { background-color: var(--success-color); flex: 1; }

        .status-badge {
            font-size: 12px;
            padding: 4px 8px;
            border-radius: 4px;
            margin-bottom: 10px;
            display: inline-block;
            font-weight: bold;
        }
        .status-new { color: var(--gray-color); background: #eee; }
        .status-learned { color: var(--success-color); background: #e8f5e9; border: 1px solid #c8e6c9; }
        .status-learning { color: var(--warning-color); background: #fff3e0; border: 1px solid #ffe0b2; }

        .status-msg {
            font-size: 13px;
            margin-top: 10px;
            color: #e53935;
            font-style: italic;
            height: 20px;
        }

        /* Modal Global */
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.6);
            z-index: 100;
            justify-content: center;
            align-items: center;
            backdrop-filter: blur(2px);
        }

        .modal-content {
            background: white;
            width: 90%;
            max-width: 400px;
            max-height: 85vh; 
            border-radius: 15px;
            padding: 20px;
            display: flex;
            flex-direction: column;
            box-shadow: 0 20px 50px rgba(0,0,0,0.3);
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            border-bottom: 1px solid #eee;
            padding-bottom: 10px;
        }

        .list-container {
            overflow-y: auto;
            flex: 1;
            -webkit-overflow-scrolling: touch; 
        }

        .list-item {
            display: flex;
            justify-content: space-between;
            padding: 12px 10px; 
            border-bottom: 1px solid #f5f5f5;
            cursor: pointer;
            text-align: left;
            align-items: center;
        }
        .list-item:hover { background-color: #fce4ec; }
        .list-item.active { background-color: #ffcdd2; font-weight: bold; }

        .stats-summary {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            text-align: center;
        }
        .stat-box {
            padding: 10px;
            border-radius: 10px;
            width: 30%;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
        }
        .stat-val { font-size: 20px; font-weight: bold; display: block; }
        .stat-label { font-size: 12px; }
        
        .bg-learned { background: #e8f5e9; color: var(--success-color); }
        .bg-learning { background: #fff3e0; color: var(--warning-color); }
        .bg-new { background: #f5f5f5; color: var(--gray-color); }

        .recommend-section {
            text-align: left;
            margin-top: 10px;
            flex: 1;
            overflow-y: auto;
            -webkit-overflow-scrolling: touch;
        }
        .recommend-item {
            padding: 12px 8px;
            border-bottom: 1px solid #eee;
            cursor: pointer;
            color: var(--warning-color);
            font-weight: 500;
        }
        .recommend-item:hover { background: #fff3e0; }
        
        .settings-row {
            margin-bottom: 15px;
            text-align: left;
        }
        .settings-label {
            font-weight: 600;
            margin-bottom: 5px;
            display: block;
            color: #555;
        }
        select.settings-input {
            width: 100%;
            padding: 10px;
            border-radius: 8px;
            border: 1px solid #ccc;
            font-size: 14px;
            background: #fff;
        }
        input[type=range] {
            width: 100%;
            margin-top: 5px;
        }

        @media (max-width: 480px) {
            .container { padding: 20px; }
            .vietnamese-text { font-size: 20px; }
            .english-word { font-size: 26px; }
            .card { min-height: 240px; }
            .btn { font-size: 15px; padding: 12px; }
            .btn-nav { width: 45px; height: 45px; font-size: 18px; }
            .header-controls { gap: 8px; }
            .btn-icon { font-size: 22px; }
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body>

<div class="container">
    <div class="header-row">
        <div class="header-controls">
            <button class="btn-icon" onclick="toggleList()" title="Danh sách từ">☰</button>
            <button class="btn-icon" onclick="toggleStats()" title="Thống kê">📊</button>
            <button class="btn-icon" onclick="toggleSettings()" title="Cài đặt âm thanh">⚙️</button>
            <button class="btn-icon" onclick="shuffleVocabulary()" title="Đảo thứ tự">🔀</button>
        </div>
        <div id="progress" class="progress-bar">CÂU 1 / 200</div>
    </div>

    <div id="current-status" class="status-badge status-new">Mới</div>
    
    <div class="card">
        <div id="question-area">
            <div class="vietnamese-text" id="vn-text">Đang tải dữ liệu...</div>
        </div>

        <div id="answer-area" class="hidden-content">
            <div class="part-of-speech" id="pos-text"></div>
            
            <div class="english-row">
                <div class="english-word" id="en-text"></div>
                <button class="btn-audio-replay" onclick="playCurrentAudio()" title="Nghe lại">🔊</button>
            </div>
            
            <div class="ipa-text" id="ipa-text"></div>
        </div>
    </div>

    <div id="status-msg" class="status-msg"></div>

    <div id="main-actions">
        <button id="btn-reveal" class="btn btn-reveal" onclick="revealAnswer()">XEM ĐÁP ÁN</button>
    </div>

    <div id="review-actions" class="review-actions" style="display: none;">
        <button class="btn btn-learn" onclick="markStatus('learning')">Chưa thuộc 😕</button>
        <button class="btn btn-success" onclick="markStatus('learned')">Đã thuộc 😎</button>
    </div>

    <div class="nav-row">
        <button class="btn btn-nav" onclick="changeCard(-1)">❮</button>
        <button class="btn btn-nav" onclick="changeCard(1)">❯</button>
    </div>
</div>

<!-- Modal Danh Sách -->
<div id="list-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Danh Sách 200 Từ</h3>
            <button onclick="toggleList()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        <div class="list-container" id="vocab-list-content"></div>
    </div>
</div>

<!-- Modal Thống Kê -->
<div id="stats-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Thống Kê Học Tập</h3>
            <button onclick="toggleStats()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        
        <div class="stats-summary">
            <div class="stat-box bg-learned">
                <span class="stat-val" id="stat-learned">0</span>
                <span class="stat-label">Đã thuộc</span>
            </div>
            <div class="stat-box bg-learning">
                <span class="stat-val" id="stat-learning">0</span>
                <span class="stat-label">Chưa thuộc</span>
            </div>
            <div class="stat-box bg-new">
                <span class="stat-val" id="stat-new">0</span>
                <span class="stat-label">Mới</span>
            </div>
        </div>

        <hr style="border:0; border-top:1px solid #eee; width:100%; margin: 10px 0;">
        <h4 style="margin: 0 0 10px 0; color: #555;">💡 Từ cần học ngay:</h4>
        <div class="recommend-section" id="recommend-list"></div>
    </div>
</div>

<!-- Modal Cài Đặt -->
<div id="settings-modal" class="modal-overlay">
    <div class="modal-content">
        <div class="modal-header">
            <h3 style="margin:0; color:var(--primary-color)">Cài Đặt Âm Thanh</h3>
            <button onclick="toggleSettings()" style="border:none; background:none; font-size:24px; cursor:pointer;">&times;</button>
        </div>
        
        <div style="padding: 10px 0;">
            <div class="settings-row">
                <label class="settings-label">Chọn Giọng Đọc (Hệ thống):</label>
                <select id="voice-select" class="settings-input" onchange="updateVoiceSettings()">
                    <option value="-1">Tự động chọn (Tốt nhất)</option>
                </select>
                <p style="font-size: 12px; color: #666; margin-top: 5px;">* Chọn giọng "English" để nghe chuẩn.</p>
            </div>
            
            <div class="settings-row">
                <label class="settings-label">Tốc Độ Đọc: <span id="speed-display" style="color:var(--primary-color)">0.6</span></label>
                <input type="range" id="speed-range" min="0.4" max="1.5" step="0.1" value="0.6" oninput="updateSpeedSettings()">
                <div style="display:flex; justify-content:space-between; font-size:12px; color:#999; margin-top:5px;">
                    <span>Chậm (0.4)</span>
                    <span>Nhanh (1.5)</span>
                </div>
            </div>
            
            <button class="btn" style="width:100%; margin-top:10px;" onclick="testVoice()">🔊 Nghe thử</button>
        </div>
    </div>
</div>

<script>
    // === DỮ LIỆU TỪ VỰNG 200 CÂU (Đã thêm IPA) ===
    const initialVocabulary = [
        {id: 1, en: "Safe", pos: "(adj)", ipa: "/seɪf/", vi: "An toàn"},
        {id: 2, en: "view", pos: "v.", ipa: "/vjuː/", vi: "nhìn, xem"},
        {id: 3, en: "Environment", pos: "(n)", ipa: "/ɪnˈvaɪrənmənt/", vi: "Môi trường"},
        {id: 4, en: "Rain", pos: "(n)", ipa: "/reɪn/", vi: "Mưa"},
        {id: 5, en: "life", pos: "n.", ipa: "/laɪf/", vi: "cuộc sống"},
        {id: 6, en: "adventure", pos: "n.", ipa: "/ədˈventʃər/", vi: "cuộc phiêu lưu"},
        {id: 7, en: "Earth", pos: "(n)", ipa: "/ɜːθ/", vi: "Trái Đất"},
        {id: 8, en: "Use", pos: "(v)", ipa: "/juːz/", vi: "Sử dụng"},
        {id: 9, en: "Pollution", pos: "(n)", ipa: "/pəˈluːʃn/", vi: "Sự ô nhiễm"},
        {id: 10, en: "Factory", pos: "(n)", ipa: "/ˈfæktri/", vi: "Nhà máy"},
        {id: 11, en: "Bottle", pos: "(n)", ipa: "/ˈbɒtl/", vi: "Chai, lọ"},
        {id: 12, en: "punish", pos: "v.", ipa: "/ˈpʌnɪʃ/", vi: "trừng phạt"},
        {id: 13, en: "Recycle", pos: "(v)", ipa: "/ˌriːˈsaɪkl/", vi: "Tái chế"},
        {id: 14, en: "football", pos: "n.", ipa: "/ˈfʊtbɔːl/", vi: "bóng đá, bóng bầu dục"},
        {id: 15, en: "patient", pos: "adj.", ipa: "/ˈpeɪʃnt/", vi: "kiên nhẫn"},
        {id: 16, en: "fail", pos: "v.", ipa: "/feɪl/", vi: "thất bại"},
        {id: 17, en: "Burn", pos: "(v)", ipa: "/bɜːn/", vi: "Đốt, cháy"},
        {id: 18, en: "Can", pos: "(n)", ipa: "/kæn/", vi: "Lon, hộp kim loại"},
        {id: 19, en: "Global", pos: "(adj)", ipa: "/ˈɡləʊbl/", vi: "Toàn cầu"},
        {id: 20, en: "camera", pos: "n.", ipa: "/ˈkæmrə/", vi: "máy ảnh"},
        {id: 21, en: "Recyclable", pos: "(adj)", ipa: "/ˌriːˈsaɪkləbl/", vi: "Có thể tái chế"},
        {id: 22, en: "shout", pos: "v.", ipa: "/ʃaʊt/", vi: "la hét"},
        {id: 23, en: "several", pos: "adj.", ipa: "/ˈsevrəl/", vi: "một vài"},
        {id: 24, en: "experiment", pos: "n.", ipa: "/ɪkˈsperɪmənt/", vi: "thí nghiệm"},
        {id: 25, en: "bike", pos: "n.", ipa: "/baɪk/", vi: "xe đạp"},
        {id: 26, en: "Turn off", pos: "(phr. v)", ipa: "/tɜːn ɒf/", vi: "Tắt (điện, nước)"},
        {id: 27, en: "Air", pos: "(n)", ipa: "/eə(r)/", vi: "Không khí"},
        {id: 28, en: "chart", pos: "n.", ipa: "/tʃɑːt/", vi: "biểu đồ"},
        {id: 29, en: "Waste", pos: "(v)", ipa: "/weɪst/", vi: "Lãng phí"},
        {id: 30, en: "Natural", pos: "(adj)", ipa: "/ˈnætʃrəl/", vi: "Thuộc về tự nhiên"},
        {id: 31, en: "Plant", pos: "(n)", ipa: "/plɑːnt/", vi: "Thực vật, cây cối"},
        {id: 32, en: "content", pos: "adj.", ipa: "/kənˈtent/", vi: "hài lòng, mãn nguyện"},
        {id: 33, en: "golf", pos: "n.", ipa: "/ɡɒlf/", vi: "môn đánh gôn"},
        {id: 34, en: "habit", pos: "n.", ipa: "/ˈhæbɪt/", vi: "thói quen"},
        {id: 35, en: "behave", pos: "v.", ipa: "/bɪˈheɪv/", vi: "cư xử, hành xử"},
        {id: 36, en: "spread", pos: "v.", ipa: "/spred/", vi: "lan truyền, trải ra"},
        {id: 37, en: "Clean", pos: "(adj)", ipa: "/kliːn/", vi: "Sạch sẽ"},
        {id: 38, en: "Waste", pos: "(n)", ipa: "/weɪst/", vi: "Rác thải, chất thải"},
        {id: 39, en: "Plant", pos: "(v)", ipa: "/plɑːnt/", vi: "Trồng (cây)"},
        {id: 40, en: "Breathe", pos: "(v)", ipa: "/briːð/", vi: "Hít thở"},
        {id: 41, en: "Gas", pos: "(n)", ipa: "/ɡæs/", vi: "Khí đốt"},
        {id: 42, en: "Fresh", pos: "(adj)", ipa: "/freʃ/", vi: "Trong lành, tươi"},
        {id: 43, en: "Harmful", pos: "(adj)", ipa: "/ˈhɑːmfl/", vi: "Có hại"},
        {id: 44, en: "ever", pos: "adv.", ipa: "/ˈevə(r)/", vi: "đã từng"},
        {id: 45, en: "weight", pos: "n.", ipa: "/weɪt/", vi: "cân nặng"},
        {id: 46, en: "Nature", pos: "(n)", ipa: "/ˈneɪtʃə(r)/", vi: "Thiên nhiên, tự nhiên"},
        {id: 47, en: "Drop", pos: "(v)", ipa: "/drɒp/", vi: "Làm rơi, vứt"},
        {id: 48, en: "Farm", pos: "(n)", ipa: "/fɑːm/", vi: "Nông trại"},
        {id: 49, en: "shape", pos: "n.", ipa: "/ʃeɪp/", vi: "hình dạng"},
        {id: 50, en: "secret", pos: "n.", ipa: "/ˈsiːkrət/", vi: "bí mật"},
        {id: 51, en: "Quickly", pos: "(adv)", ipa: "/ˈkwɪkli/", vi: "Một cách nhanh chóng"},
        {id: 52, en: "On", pos: "(prep)", ipa: "/ɒn/", vi: "Ở trên"},
        {id: 53, en: "calm", pos: "adj.", ipa: "/kɑːm/", vi: "bình tĩnh"},
        {id: 54, en: "during", pos: "prep.", ipa: "/ˈdjʊərɪŋ/", vi: "trong suốt (thời gian)"},
        {id: 55, en: "Smoke", pos: "(n)", ipa: "/sməʊk/", vi: "Khói"},
        {id: 56, en: "Carefully", pos: "(adv)", ipa: "/ˈkeəfəli/", vi: "Một cách cẩn thận"},
        {id: 57, en: "loud", pos: "adj.", ipa: "/laʊd/", vi: "to, ồn ào"},
        {id: 58, en: "Reusable", pos: "(adj)", ipa: "/ˌriːˈjuːzəbl/", vi: "Có thể tái sử dụng"},
        {id: 59, en: "create", pos: "v.", ipa: "/kriˈeɪt/", vi: "tạo ra"},
        {id: 60, en: "Litter", pos: "(n)", ipa: "/ˈlɪtə(r)/", vi: "Rác vụn (vứt bừa bãi)"},
        {id: 61, en: "appropriate", pos: "adj.", ipa: "/əˈprəʊpriət/", vi: "thích hợp, phù hợp"},
        {id: 62, en: "Never", pos: "(adv)", ipa: "/ˈnevə(r)/", vi: "Không bao giờ"},
        {id: 63, en: "Noise", pos: "(n)", ipa: "/nɔɪz/", vi: "Tiếng ồn"},
        {id: 64, en: "Dirty", pos: "(adj)", ipa: "/ˈdɜːti/", vi: "Bẩn, dơ"},
        {id: 65, en: "Local", pos: "(adj)", ipa: "/ˈləʊkl/", vi: "Địa phương"},
        {id: 66, en: "agree", pos: "v.", ipa: "/əˈɡriː/", vi: "đồng ý"},
        {id: 67, en: "Reuse", pos: "(v)", ipa: "/ˌriːˈjuːz/", vi: "Tái sử dụng"},
        {id: 68, en: "Solar", pos: "(adj)", ipa: "/ˈsəʊlə(r)/", vi: "(Thuộc) mặt trời"},
        {id: 69, en: "adult", pos: "n.", ipa: "/ˈædʌlt/", vi: "người lớn, người trưởng thành"},
        {id: 70, en: "Bag", pos: "(n)", ipa: "/bæɡ/", vi: "Cái túi"},
        {id: 71, en: "laugh", pos: "n.", ipa: "/lɑːf/", vi: "tiếng cười"},
        {id: 72, en: "concern", pos: "n.", ipa: "/kənˈsɜːn/", vi: "mối quan tâm, sự lo lắng"},
        {id: 73, en: "nervous", pos: "adj.", ipa: "/ˈnɜːvəs/", vi: "lo lắng"},
        {id: 74, en: "approach", pos: "v.", ipa: "/əˈprəʊtʃ/", vi: "tiếp cận"},
        {id: 75, en: "Danger", pos: "(n)", ipa: "/ˈdeɪndʒə(r)/", vi: "Mối nguy hiểm"},
        {id: 76, en: "typical", pos: "adj.", ipa: "/ˈtɪpɪkl/", vi: "điển hình, tiêu biểu"},
        {id: 77, en: "travel", pos: "v.", ipa: "/ˈtrævl/", vi: "du lịch"},
        {id: 78, en: "alcohol", pos: "n.", ipa: "/ˈælkəhɒl/", vi: "cồn, rượu"},
        {id: 79, en: "choose", pos: "v.", ipa: "/tʃuːz/", vi: "lựa chọn"},
        {id: 80, en: "Paper", pos: "(n)", ipa: "/ˈpeɪpə(r)/", vi: "Giấy"},
        {id: 81, en: "River", pos: "(n)", ipa: "/ˈrɪvə(r)/", vi: "Con sông"},
        {id: 82, en: "Rubbish", pos: "(n)", ipa: "/ˈrʌbɪʃ/", vi: "Rác (tương tự trash)"},
        {id: 83, en: "Walk", pos: "(v)", ipa: "/wɔːk/", vi: "Đi bộ"},
        {id: 84, en: "Weather", pos: "(n)", ipa: "/ˈweðə(r)/", vi: "Thời tiết"},
        {id: 85, en: "Important", pos: "(adj)", ipa: "/ɪmˈpɔːtnt/", vi: "Quan trọng"},
        {id: 86, en: "boat", pos: "n.", ipa: "/bəʊt/", vi: "thuyền"},
        {id: 87, en: "visit", pos: "v.", ipa: "/ˈvɪzɪt/", vi: "thăm"},
        {id: 88, en: "Cycle", pos: "(v)", ipa: "/ˈsaɪkl/", vi: "Đạp xe"},
        {id: 89, en: "among", pos: "prep.", ipa: "/əˈmʌŋ/", vi: "ở giữa"},
        {id: 90, en: "breakfast", pos: "n.", ipa: "/ˈbrekfəst/", vi: "bữa sáng"},
        {id: 91, en: "Damage", pos: "(n)", ipa: "/ˈdæmɪdʒ/", vi: "Sự thiệt hại"},
        {id: 92, en: "Water", pos: "(n)", ipa: "/ˈwɔːtə(r)/", vi: "Nước"},
        {id: 93, en: "duck", pos: "n.", ipa: "/dʌk/", vi: "con vịt"},
        {id: 94, en: "Shower", pos: "(v)", ipa: "/ˈʃaʊə(r)/", vi: "Tắm (vòi sen)"},
        {id: 95, en: "Always", pos: "(adv)", ipa: "/ˈɔːlweɪz/", vi: "Luôn luôn"},
        {id: 96, en: "Beach", pos: "(n)", ipa: "/biːtʃ/", vi: "Bãi biển"},
        {id: 97, en: "worse", pos: "adj.", ipa: "/wɜːs/", vi: "tệ hơn"},
        {id: 98, en: "Grow", pos: "(v)", ipa: "/ɡrəʊ/", vi: "Trồng, phát triển"},
        {id: 99, en: "avoid", pos: "v.", ipa: "/əˈvɔɪd/", vi: "tránh, né tránh"},
        {id: 100, en: "Harm", pos: "(v)", ipa: "/hɑːm/", vi: "Gây hại"},
        {id: 101, en: "balance", pos: "n.", ipa: "/ˈbæləns/", vi: "sự cân bằng"},
        {id: 102, en: "Rainy", pos: "(adj)", ipa: "/ˈreɪni/", vi: "Có mưa"},
        {id: 103, en: "Animal", pos: "(n)", ipa: "/ˈænɪml/", vi: "Động vật"},
        {id: 104, en: "week", pos: "n.", ipa: "/wiːk/", vi: "tuần"},
        {id: 105, en: "love", pos: "v.", ipa: "/lʌv/", vi: "yêu"},
        {id: 106, en: "Trash", pos: "(n)", ipa: "/træʃ/", vi: "Rác (thường là đồ khô)"},
        {id: 107, en: "game", pos: "n.", ipa: "/ɡeɪm/", vi: "trò chơi"},
        {id: 108, en: "age", pos: "n.", ipa: "/eɪdʒ/", vi: "tuổi, tuổi tác"},
        {id: 109, en: "Healthy", pos: "(adj)", ipa: "/ˈhelθi/", vi: "Lành mạnh, khỏe"},
        {id: 110, en: "Energy", pos: "(n)", ipa: "/ˈenədʒi/", vi: "Năng lượng"},
        {id: 111, en: "Look after", pos: "(phr. v)", ipa: "/lʊk ˈɑːftə(r)/", vi: "Trông nom, chăm sóc"},
        {id: 112, en: "active", pos: "adj.", ipa: "/ˈæktɪv/", vi: "năng động, tích cực"},
        {id: 113, en: "Wind", pos: "(n)", ipa: "/wɪnd/", vi: "Gió"},
        {id: 114, en: "positive", pos: "adj.", ipa: "/ˈpɒzətɪv/", vi: "tích cực"},
        {id: 115, en: "suddenly", pos: "adv.", ipa: "/ˈsʌdnli/", vi: "đột ngột"},
        {id: 116, en: "increase", pos: "v.", ipa: "/ɪnˈkriːs/", vi: "tăng lên"},
        {id: 117, en: "Protect", pos: "(v)", ipa: "/prəˈtekt/", vi: "Bảo vệ"},
        {id: 118, en: "Soil", pos: "(n)", ipa: "/sɔɪl/", vi: "Đất"},
        {id: 119, en: "catch", pos: "v.", ipa: "/kætʃ/", vi: "bắt, chụp"},
        {id: 120, en: "Glass", pos: "(n)", ipa: "/ɡlɑːs/", vi: "Thủy tinh"},
        {id: 121, en: "bad", pos: "adj.", ipa: "/bæd/", vi: "tồi, tệ"},
        {id: 122, en: "project", pos: "n.", ipa: "/ˈprɒdʒekt/", vi: "dự án"},
        {id: 123, en: "instruct", pos: "v.", ipa: "/ɪnˈstrʌkt/", vi: "hướng dẫn, dạy"},
        {id: 124, en: "solve", pos: "v.", ipa: "/sɒlv/", vi: "giải quyết"},
        {id: 125, en: "village", pos: "n.", ipa: "/ˈvɪlɪdʒ/", vi: "làng, ngôi làng"},
        {id: 126, en: "report", pos: "n.", ipa: "/rɪˈpɔːt/", vi: "bài báo cáo"},
        {id: 127, en: "August", pos: "n.", ipa: "/ɔːˈɡʌst/", vi: "tháng Tám"},
        {id: 128, en: "Plastic", pos: "(n)", ipa: "/ˈplæstɪk/", vi: "Nhựa"},
        {id: 129, en: "Sea", pos: "(n)", ipa: "/siː/", vi: "Biển"},
        {id: 130, en: "suppose", pos: "v.", ipa: "/səˈpəʊz/", vi: "cho rằng, giả sử"},
        {id: 131, en: "library", pos: "n.", ipa: "/ˈlaɪbrəri/", vi: "thư viện"},
        {id: 132, en: "Tree", pos: "(n)", ipa: "/triː/", vi: "Cây xanh"},
        {id: 133, en: "understand", pos: "v.", ipa: "/ˌʌndəˈstænd/", vi: "hiểu"},
        {id: 134, en: "represent", pos: "v.", ipa: "/ˌreprɪˈzent/", vi: "đại diện"},
        {id: 135, en: "frequently", pos: "adv.", ipa: "/ˈfriːkwəntli/", vi: "thường xuyên"},
        {id: 136, en: "evil", pos: "adj.", ipa: "/ˈiːvl/", vi: "độc ác"},
        {id: 137, en: "Around", pos: "(prep)", ipa: "/əˈraʊnd/", vi: "Xung quanh"},
        {id: 138, en: "describe", pos: "v.", ipa: "/dɪˈskraɪb/", vi: "mô tả"},
        {id: 139, en: "Electricity", pos: "(n)", ipa: "/ɪˌlekˈtrɪsəti/", vi: "Điện"},
        {id: 140, en: "Care for", pos: "(phr. v)", ipa: "/keə(r) fɔː(r)/", vi: "Chăm sóc"},
        {id: 141, en: "Reduce", pos: "(v)", ipa: "/rɪˈdjuːs/", vi: "Cắt giảm"},
        {id: 142, en: "often", pos: "adv.", ipa: "/ˈɒfn/", vi: "thường"},
        {id: 143, en: "Green", pos: "(adj)", ipa: "/ɡriːn/", vi: "Xanh (liên quan đến MT)"},
        {id: 144, en: "fun", pos: "adj.", ipa: "/fʌn/", vi: "vui vẻ"},
        {id: 145, en: "Help", pos: "(v)", ipa: "/help/", vi: "Giúp đỡ"},
        {id: 146, en: "Pick up", pos: "(phr. v)", ipa: "/pɪk ʌp/", vi: "Nhặt lên"},
        {id: 147, en: "Forest", pos: "(n)", ipa: "/ˈfɒrɪst/", vi: "Khu rừng"},
        {id: 148, en: "Sun", pos: "(n)", ipa: "/sʌn/", vi: "Mặt trời"},
        {id: 149, en: "invite", pos: "v.", ipa: "/ɪnˈvaɪt/", vi: "mời"},
        {id: 150, en: "Throw away", pos: "(phr. v)", ipa: "/θrəʊ əˈweɪ/", vi: "Vứt đi"},
        {id: 151, en: "Windy", pos: "(adj)", ipa: "/ˈwɪndi/", vi: "Có gió"},
        {id: 152, en: "kilometer", pos: "n.", ipa: "/kɪˈlɒmɪtə(r)/", vi: "ki-lô-mét"},
        {id: 153, en: "instead", pos: "adv.", ipa: "/ɪnˈsted/", vi: "thay vì"},
        {id: 154, en: "grade", pos: "n.", ipa: "/ɡreɪd/", vi: "điểm số"},
        {id: 155, en: "kill", pos: "v.", ipa: "/kɪl/", vi: "giết"},
        {id: 156, en: "alien", pos: "n.", ipa: "/ˈeɪliən/", vi: "người ngoài hành tinh"},
        {id: 157, en: "capital", pos: "n.", ipa: "/ˈkæpɪtl/", vi: "thủ đô"},
        {id: 158, en: "Climate", pos: "(n)", ipa: "/ˈklaɪmət/", vi: "Khí hậu"},
        {id: 159, en: "shake", pos: "v.", ipa: "/ʃeɪk/", vi: "lắc, rung"},
        {id: 160, en: "issue", pos: "n.", ipa: "/ˈɪʃuː/", vi: "vấn đề"},
        {id: 161, en: "none", pos: "pron.", ipa: "/nʌn/", vi: "không ai, không cái gì"},
        {id: 162, en: "Destroy", pos: "(v)", ipa: "/dɪˈstrɔɪ/", vi: "Phá hủy"},
        {id: 163, en: "Flower", pos: "(n)", ipa: "/ˈflaʊə(r)/", vi: "Bông hoa"},
        {id: 164, en: "laboratory", pos: "n.", ipa: "/ləˈbɒrətri/", vi: "phòng thí nghiệm"},
        {id: 165, en: "cloud", pos: "n.", ipa: "/klaʊd/", vi: "đám mây"},
        {id: 166, en: "terrible", pos: "adj.", ipa: "/ˈterəbl/", vi: "khủng khiếp, tồi tệ"},
        {id: 167, en: "Save", pos: "(v)", ipa: "/seɪv/", vi: "Cứu, tiết kiệm"},
        {id: 168, en: "wine", pos: "n.", ipa: "/waɪn/", vi: "rượu vang"},
        {id: 169, en: "Ocean", pos: "(n)", ipa: "/ˈəʊʃn/", vi: "Đại dương"},
        {id: 170, en: "smell", pos: "v.", ipa: "/smel/", vi: "ngửi"},
        {id: 171, en: "month", pos: "n.", ipa: "/mʌnθ/", vi: "tháng"},
        {id: 172, en: "Sort", pos: "(v)", ipa: "/sɔːt/", vi: "Phân loại"},
        {id: 173, en: "Chemical", pos: "(n)", ipa: "/ˈkemɪkl/", vi: "Hóa chất"},
        {id: 174, en: "enjoy", pos: "v.", ipa: "/ɪnˈdʒɔɪ/", vi: "thích thú, tận hưởng"},
        {id: 175, en: "heart", pos: "n.", ipa: "/hɑːt/", vi: "trái tim"},
        {id: 176, en: "Drive", pos: "(v)", ipa: "/draɪv/", vi: "Lái xe"},
        {id: 177, en: "plenty", pos: "pron.", ipa: "/ˈplenti/", vi: "nhiều"},
        {id: 178, en: "expect", pos: "v.", ipa: "/ɪkˈspekt/", vi: "mong đợi, kỳ vọng"},
        {id: 179, en: "arrive", pos: "v.", ipa: "/əˈraɪv/", vi: "đến nơi"},
        {id: 180, en: "Fire", pos: "(n)", ipa: "/ˈfaɪə(r)/", vi: "Lửa"},
        {id: 181, en: "Clean", pos: "(v)", ipa: "/kliːn/", vi: "Dọn dẹp, làm sạch"},
        {id: 182, en: "Mountain", pos: "(n)", ipa: "/ˈmaʊntən/", vi: "Ngọn núi"},
        {id: 183, en: "doctor", pos: "n.", ipa: "/ˈdɒktə(r)/", vi: "bác sĩ"},
        {id: 184, en: "scare", pos: "v.", ipa: "/skeə(r)/", vi: "làm sợ hãi"},
        {id: 185, en: "In", pos: "(prep)", ipa: "/ɪn/", vi: "Ở trong"},
        {id: 186, en: "Bin", pos: "(n)", ipa: "/bɪn/", vi: "Thùng rác"},
        {id: 187, en: "photograph", pos: "n.", ipa: "/ˈfəʊtəɡrɑːf/", vi: "bức ảnh"},
        {id: 188, en: "Collect", pos: "(v)", ipa: "/kəˈlekt/", vi: "Thu gom"},
        {id: 189, en: "stroll", pos: "v.", ipa: "/strəʊl/", vi: "đi dạo"},
        {id: 190, en: "Planet", pos: "(n)", ipa: "/ˈplænɪt/", vi: "Hành tinh"},
        {id: 191, en: "Field", pos: "(n)", ipa: "/fiːld/", vi: "Cánh đồng"},
        {id: 192, en: "Polluted", pos: "(adj)", ipa: "/pəˈluːtɪd/", vi: "Bị ô nhiễm"},
        {id: 193, en: "Slowly", pos: "(adv)", ipa: "/ˈsləʊli/", vi: "Một cách chậm rãi"},
        {id: 194, en: "Sunny", pos: "(adj)", ipa: "/ˈsʌni/", vi: "Có nắng"},
        {id: 195, en: "history", pos: "(n)", ipa: "/ˈhɪstri/", vi: "lịch sử"},
        {id: 196, en: "past", pos: "(n)", ipa: "/pɑːst/", vi: "quá khứ"},
        {id: 197, en: "king", pos: "(n)", ipa: "/kɪŋ/", vi: "vua"},
        {id: 198, en: "queen", pos: "(n)", ipa: "/kwiːn/", vi: "nữ hoàng"},
        {id: 199, en: "castle", pos: "(n)", ipa: "/ˈkɑːsl/", vi: "lâu đài"},
        {id: 200, en: "war", pos: "(n)", ipa: "/wɔː(r)/", vi: "chiến tranh"}
    ];

    let vocabularyList = initialVocabulary.map(item => ({...item, status: 'new'}));
    
    let currentIndex = 0;
    let isRevealed = false;
    let availableVoices = [];
    
    // Global settings for audio
    let selectedVoiceIndex = -1; // -1 means auto-detect
    let readingRate = 0.6; // Default slow speed

    // Elements
    const elements = {
        vnText: document.getElementById('vn-text'),
        enText: document.getElementById('en-text'),
        ipaText: document.getElementById('ipa-text'), // New element for IPA
        posText: document.getElementById('pos-text'),
        // Remove exText since data doesn't have examples
        answerArea: document.getElementById('answer-area'),
        btnReveal: document.getElementById('btn-reveal'),
        reviewActions: document.getElementById('review-actions'),
        statusMsg: document.getElementById('status-msg'),
        progress: document.getElementById('progress'),
        currentStatus: document.getElementById('current-status'),
        listModal: document.getElementById('list-modal'),
        listContent: document.getElementById('vocab-list-content'),
        statsModal: document.getElementById('stats-modal'),
        statLearned: document.getElementById('stat-learned'),
        statLearning: document.getElementById('stat-learning'),
        statNew: document.getElementById('stat-new'),
        recommendList: document.getElementById('recommend-list'),
        settingsModal: document.getElementById('settings-modal'),
        voiceSelect: document.getElementById('voice-select'),
        speedRange: document.getElementById('speed-range'),
        speedDisplay: document.getElementById('speed-display')
    };

    // === SETUP AUDIO (PURE SYSTEM SPEECH) ===
    function loadVoices() {
        availableVoices = window.speechSynthesis.getVoices();
        
        // Populate Dropdown
        elements.voiceSelect.innerHTML = '';
        
        // Option Mặc định
        const defaultOption = document.createElement('option');
        defaultOption.value = -1;
        defaultOption.text = "Tự động chọn (Tốt nhất)";
        elements.voiceSelect.appendChild(defaultOption);

        availableVoices.forEach((voice, index) => {
            // Chỉ hiện các giọng có tiếng Anh để đỡ rối
            if(voice.lang.includes('en')) {
                const option = document.createElement('option');
                option.value = index;
                option.text = `${voice.name} (${voice.lang})`;
                // Đánh dấu nếu đang được chọn
                if (index === selectedVoiceIndex) option.selected = true;
                elements.voiceSelect.appendChild(option);
            }
        });
    }
    
    if (speechSynthesis.onvoiceschanged !== undefined) {
        speechSynthesis.onvoiceschanged = loadVoices;
    }
    // Gọi lần đầu (đôi khi trình duyệt đã load xong rồi)
    setTimeout(loadVoices, 100);

    function playAudio(text) {
        window.speechSynthesis.cancel();
        const utterance = new SpeechSynthesisUtterance(text);
        
        // Xác định giọng đọc
        if (selectedVoiceIndex !== -1 && availableVoices[selectedVoiceIndex]) {
            // Người dùng đã chọn giọng cụ thể
            utterance.voice = availableVoices[selectedVoiceIndex];
        } else {
            // Tự động chọn (Ưu tiên Google / Premium / UK)
            let preferredVoice = availableVoices.find(voice => 
                (voice.name.includes('Google') && voice.lang.includes('en')) || 
                (voice.name.includes('Premium') && voice.lang.includes('en')) ||
                (voice.name.includes('Samantha') && voice.lang.includes('en'))
            );

            if (!preferredVoice) {
                preferredVoice = availableVoices.find(voice => voice.lang === 'en-GB' || voice.lang === 'en_GB');
            }
            if (!preferredVoice) {
                preferredVoice = availableVoices.find(voice => voice.lang.includes('en'));
            }

            if (preferredVoice) utterance.voice = preferredVoice;
        }
        
        // Áp dụng tốc độ
        utterance.rate = readingRate; 
        utterance.pitch = 1.0;
        utterance.volume = 1.0;

        utterance.onerror = (e) => console.log('Speech error:', e);
        window.speechSynthesis.speak(utterance);
    }

    // --- SETTINGS FUNCTIONS ---
    function toggleSettings() {
        const isHidden = elements.settingsModal.style.display === 'none' || elements.settingsModal.style.display === '';
        if (isHidden) {
            elements.settingsModal.style.display = 'flex';
            // Refresh voice list in case it wasn't loaded
            if(availableVoices.length === 0) loadVoices();
        } else {
            elements.settingsModal.style.display = 'none';
        }
    }

    function updateVoiceSettings() {
        selectedVoiceIndex = parseInt(elements.voiceSelect.value);
        // Lưu ý: Không cần lưu localStorage vì đề bài không yêu cầu, 
        // nhưng biến selectedVoiceIndex là toàn cục nên sẽ áp dụng cho mọi từ.
    }

    function updateSpeedSettings() {
        readingRate = parseFloat(elements.speedRange.value);
        elements.speedDisplay.innerText = readingRate;
    }
    
    function testVoice() {
        playAudio("Hello, this is a test for English voice.");
    }

    // --- OTHER LOGIC ---
    function shuffleVocabulary() {
        for (let i = vocabularyList.length - 1; i > 0; i--) {
            const j = Math.floor(Math.random() * (i + 1));
            [vocabularyList[i], vocabularyList[j]] = [vocabularyList[j], vocabularyList[i]];
        }
        currentIndex = 0;
        loadCard(0);
        elements.statusMsg.innerText = "🔀 Đã đảo thứ tự từ vựng!";
        setTimeout(() => elements.statusMsg.innerText = "", 2000);
    }

    function loadCard(index) {
        if (index < 0) currentIndex = vocabularyList.length - 1;
        else if (index >= vocabularyList.length) currentIndex = 0;
        else currentIndex = index;

        const item = vocabularyList[currentIndex];

        elements.vnText.innerText = item.vi;
        elements.enText.innerText = item.en;
        elements.posText.innerText = item.pos;
        // elements.exText.innerText = ""; // REMOVED to fix error
        
        // Cập nhật IPA
        if (item.ipa) {
            elements.ipaText.innerText = item.ipa;
            elements.ipaText.style.display = 'block';
        } else {
            elements.ipaText.style.display = 'none';
        }
        
        elements.answerArea.style.display = 'none';
        elements.reviewActions.style.display = 'none';
        elements.btnReveal.style.display = 'block';
        elements.btnReveal.disabled = false;
        elements.btnReveal.innerText = "XEM ĐÁP ÁN";
        elements.statusMsg.innerText = "";
        
        elements.progress.innerText = `CÂU ${currentIndex + 1} / ${vocabularyList.length}`;
        updateStatusBadge(item.status);
        
        isRevealed = false;
    }

    function updateStatusBadge(status) {
        elements.currentStatus.className = 'status-badge';
        if (status === 'learned') {
            elements.currentStatus.innerText = "Đã thuộc";
            elements.currentStatus.classList.add('status-learned');
        } else if (status === 'learning') {
            elements.currentStatus.innerText = "Chưa thuộc";
            elements.currentStatus.classList.add('status-learning');
        } else {
            elements.currentStatus.innerText = "Mới";
            elements.currentStatus.classList.add('status-new');
        }
    }

    function revealAnswer() {
        isRevealed = true;
        elements.btnReveal.disabled = true;
        elements.answerArea.style.display = 'block';
        playAudio(vocabularyList[currentIndex].en);
        elements.btnReveal.style.display = 'none'; 
        elements.reviewActions.style.display = 'flex'; 
    }

    function playCurrentAudio() {
        playAudio(vocabularyList[currentIndex].en);
    }

    function markStatus(status) {
        vocabularyList[currentIndex].status = status;
        updateStatusBadge(status);
        setTimeout(() => { changeCard(1); }, 300);
    }

    function changeCard(step) {
        loadCard(currentIndex + step);
    }

    function toggleList() {
        const isHidden = elements.listModal.style.display === 'none' || elements.listModal.style.display === '';
        if (isHidden) {
            renderList();
            elements.listModal.style.display = 'flex';
        } else {
            elements.listModal.style.display = 'none';
        }
    }

    function renderList() {
        elements.listContent.innerHTML = '';
        vocabularyList.forEach((item, index) => {
            const div = document.createElement('div');
            div.className = `list-item ${index === currentIndex ? 'active' : ''}`;
            let statusIcon = '⚪';
            if (item.status === 'learned') statusIcon = '✅';
            if (item.status === 'learning') statusIcon = '🔸';
            div.innerHTML = `<div style="display:flex; align-items:center;"><span style="margin-right:8px; font-size: 12px;">${statusIcon}</span><strong>${item.en}</strong></div><div style="font-size:12px; color:#666;">${index + 1}</div>`;
            div.onclick = () => { currentIndex = index; loadCard(currentIndex); toggleList(); };
            elements.listContent.appendChild(div);
        });
    }

    function toggleStats() {
        const isHidden = elements.statsModal.style.display === 'none' || elements.statsModal.style.display === '';
        if (isHidden) { renderStats(); elements.statsModal.style.display = 'flex'; } else { elements.statsModal.style.display = 'none'; }
    }

    function renderStats() {
        const learnedCount = vocabularyList.filter(i => i.status === 'learned').length;
        const learningCount = vocabularyList.filter(i => i.status === 'learning').length;
        const newCount = vocabularyList.filter(i => i.status === 'new').length;
        elements.statLearned.innerText = learnedCount;
        elements.statLearning.innerText = learningCount;
        elements.statNew.innerText = newCount;
        let recommendItems = vocabularyList.map((item, index) => ({ ...item, originalIndex: index })).filter(i => i.status === 'learning');
        elements.recommendList.innerHTML = '';
        if (recommendItems.length === 0) {
            const newItems = vocabularyList.map((item, index) => ({ ...item, originalIndex: index })).filter(i => i.status === 'new').slice(0, 5);
            if (newItems.length > 0) {
                elements.recommendList.innerHTML = '<div style="color:#777; font-style:italic; padding:10px;">Bạn đã thuộc hết các từ cần ôn. Hãy học từ mới:</div>';
                newItems.forEach(item => createRecommendItem(item));
            } else {
                elements.recommendList.innerHTML = '<div style="color:green; padding:10px; text-align:center;">🎉 Tuyệt vời! Bạn đã thuộc hết toàn bộ danh sách.</div>';
            }
        } else {
            recommendItems.forEach(item => createRecommendItem(item));
        }
    }

    function createRecommendItem(item) {
        const div = document.createElement('div');
        div.className = 'recommend-item';
        div.innerHTML = `🔸 <strong>${item.en}</strong> <span style="font-size:12px; color:#999;">(${item.vi})</span>`;
        div.onclick = () => { currentIndex = item.originalIndex; loadCard(currentIndex); toggleStats(); };
        elements.recommendList.appendChild(div);
    }

    loadCard(0);
</script>

</body>
</html>

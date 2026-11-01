# maksab# ظˆط«ظٹظ‚ط© ظ…طھط¬ط± ط§ظ„طھط³ظˆظٹظ‚ ط¨ط§ظ„ط¹ظ…ظˆظ„ط© ط§ظ„ط°ظƒظٹ (Affiliate Store Setup)

ظ…ط±ط­ط¨ط§ظ‹ ط¨ظƒ! ظٹط­طھظˆظٹ ظ‡ط°ط§ ط§ظ„ظ…ظ„ظپ ط¹ظ„ظ‰ ط§ظ„ظ…ظ„ظپط§طھ ط§ظ„ط¨ط±ظ…ط¬ظٹط© ط§ظ„ظƒط§ظ…ظ„ط© ظˆط§ظ„ظ‡ظٹظƒظ„ ط§ظ„طھظ†ط¸ظٹظ…ظٹ ظ„ظ…طھط¬ط±ظƒ ط§ظ„ط¥ظ„ظƒطھط±ظˆظ†ظٹ ط§ظ„ط°ظƒظٹ ط§ظ„ظ…طھظˆط§ظپظ‚ ظ…ط¹ ط§ظ„ظ†ط·ط§ظ‚ط§طھ ط§ظ„ط§ط­طھط±ط§ظپظٹط© (ظ…ط«ظ„ ط¯ظˆظ…ظٹظ† .com). ظٹظ…ظƒظ†ظƒ ط­ظپط¸ ظ‡ط°ط§ ط§ظ„ظ…ظ„ظپ ط¹ظ„ظ‰ ظ‡ط§طھظپظƒ ظ„ظ„ط±ط¬ظˆط¹ ط¥ظ„ظٹظ‡ ط¹ظ†ط¯ ط±ظپط¹ ط§ظ„ظ…ظˆظ‚ط¹ ط¹ظ„ظ‰ ط§ظ„ط§ط³طھط¶ط§ظپط©.

---

## 1. ظ…ظ„ظپ ظˆط§ط¬ظ‡ط© ط§ظ„ظ…طھط¬ط± ط§ظ„ط±ط¦ظٹط³ظٹط© (index.html)
ظ‚ظ… ط¨ظ†ط³ط® ظ‡ط°ط§ ط§ظ„ظƒظˆط¯ ظˆط­ظپط¸ظ‡ ط¨ط§ط³ظ… `index.html` ط¹ظ†ط¯ ط±ظپط¹ ط§ظ„ظ…ظˆظ‚ط¹:

```html
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ظ…طھط¬ط±ظٹ ط§ظ„ط°ظƒظٹ ظ„ظ„ط£ظپظ„ظٹظٹطھ</title>
    <style>
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background-color: #f4f7f6; margin: 0; padding: 0; }
        header { background-color: #2c3e50; color: white; text-align: center; padding: 30px 20px; }
        .container { display: flex; flex-wrap: wrap; justify-content: center; padding: 20px; max-width: 1200px; margin: 0 auto; }
        .product-card { background: white; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); margin: 15px; width: 280px; overflow: hidden; text-align: center; transition: 0.3s; }
        .product-card:hover { transform: translateY(-5px); }
        .product-image { width: 100%; height: 200px; background-color: #eaeaea; display: flex; align-items: center; justify-content: center; color: #777; font-weight: bold; }
        .product-info { padding: 15px; }
        .product-title { font-size: 18px; margin: 10px 0; color: #333; }
        .product-price { color: #27ae60; font-weight: bold; font-size: 16px; margin-bottom: 15px; }
        .affiliate-btn { display: inline-block; background-color: #e67e22; color: white; padding: 10px 20px; text-decoration: none; border-radius: 5px; font-weight: bold; transition: 0.2s; width: 80%; }
        .affiliate-btn:hover { background-color: #d35400; }
        
        /* ط´ط§طھ ط¨ظˆطھ ط§ظ„ط°ظƒط§ط، ط§ظ„ط§طµط·ظ†ط§ط¹ظٹ */
        #ai-chat-box { position: fixed; bottom: 20px; left: 20px; width: 300px; background: white; border: 1px solid #ccc; border-radius: 10px; box-shadow: 0 4px 10px rgba(0,0,0,0.2); display: none; z-index: 9999; }
        .chat-header { background: #2c3e50; color: white; padding: 10px; border-top-left-radius: 10px; border-top-right-radius: 10px; font-weight: bold; }
        .chat-content { height: 200px; padding: 10px; overflow-y: auto; font-size: 14px; color: #333; }
        .chat-input-area { padding: 10px; border-top: 1px solid #eee; display: flex; }
        .chat-input { width: 75%; padding: 5px; border: 1px solid #ddd; border-radius: 3px; }
        .chat-btn { width: 22%; background: #e67e22; color: white; border: none; margin-right: 3%; cursor: pointer; border-radius: 3px; }
        .chat-toggle { position: fixed; bottom: 20px; left: 20px; background: #2c3e50; color: white; border: none; padding: 15px; border-radius: 50%; font-size: 20px; cursor: pointer; box-shadow: 0 4px 10px rgba(0,0,0,0.2); z-index: 9998; }
    </style>
</head>
<body>

    <header>
        <h1>ظ…ط±ط­ط¨ط§ظ‹ ط¨ظƒ ظپظٹ ظ…طھط¬ط±ظƒ ط§ظ„ط¥ظ„ظƒطھط±ظˆظ†ظٹ ط§ظ„ط¬ط¯ظٹط¯</h1>
        <p>ط£ظپط¶ظ„ ط§ظ„ظ…ظ†طھط¬ط§طھ ط§ظ„ظ…ط®طھط§ط±ط© ط°ظƒظٹط§ظ‹ ظ…ظ† ط£ظ…ط§ط²ظˆظ† ظˆط¹ظ„ظٹ ط¥ظƒط³ط¨ط±ظٹط³</p>
    </header>

    <div class="container">
        <!-- ظƒط±طھ ظ…ظ†طھط¬ ط£ظ…ط§ط²ظˆظ† -->
        <div class="product-card">
            <div class="product-image">ًں“¦ ظ…ظ†طھط¬ ظ…ظ† ط£ظ…ط§ط²ظˆظ†</div>
            <div class="product-info">
                <h3 class="product-title">ط³ط§ط¹ط© ط°ظƒظٹط© ظ…طھط·ظˆط±ط©</h3>
                <div class="product-price">35.00 ط¯ظˆظ„ط§ط±</div>
                <a href="#" target="_blank" class="affiliate-btn">طھط³ظˆظ‚ ط§ظ„ط¢ظ† ظ…ظ† ط£ظ…ط§ط²ظˆظ†</a>
            </div>
        </div>

        <!-- ظƒط±طھ ظ…ظ†طھط¬ ط¹ظ„ظٹ ط¥ظƒط³ط¨ط±ظٹط³ -->
        <div class="product-card">
            <div class="product-image">ًں›چï¸ڈ ظ…ظ†طھط¬ ظ…ظ† ط¹ظ„ظٹ ط¥ظƒط³ط¨ط±ظٹط³</div>
            <div class="product-info">
                <h3 class="product-title">ط³ظ…ط§ط¹ط§طھ ظ„ط§ط³ظ„ظƒظٹط© ط¹ط§ط²ظ„ط©</h3>
                <div class="product-price">12.99 ط¯ظˆظ„ط§ط±</div>
                <a href="#" target="_blank" class="affiliate-btn">طھط³ظˆظ‚ ط§ظ„ط¢ظ† ظ…ظ† AliExpress</a>
            </div>
        </div>
    </div>

    <!-- ظ†ط§ظپط°ط© ط§ظ„ط¯ط±ط¯ط´ط© ط§ظ„ط°ظƒظٹط© ظ„ظ„ط²ظˆط§ط± -->
    <div id="ai-chat-box">
        <div class="chat-header">
            ًں¤– ظ…ط³ط§ط¹ط¯ ط§ظ„ظ…طھط¬ط± ط§ظ„ط°ظƒظٹ
            <span onclick="toggleChat()" style="float: left; cursor: pointer;">âœ•</span>
        </div>
        <div id="chat-content" class="chat-content">
            <p style="color: #555; margin: 0;">ظ…ط±ط­ط¨ط§ظ‹ ط¨ظƒ! ط£ظ†ط§ ظ…ط³ط§ط¹ط¯ظƒ ط§ظ„ط°ظƒظٹ. ظƒظٹظپ ظٹظ…ظƒظ†ظ†ظٹ ظ…ط³ط§ط¹ط¯طھظƒ ظپظٹ ط§ط®طھظٹط§ط± ط§ظ„ظ…ظ†طھط¬ ط§ظ„ظٹظˆظ…طں</p>
        </div>
        <div class="chat-input-area">
            <input type="text" id="user-input" class="chat-input" placeholder="ط§ظƒطھط¨ ط³ط¤ط§ظ„ظƒ...">
            <button onclick="sendMessage()" class="chat-btn">ط¥ط±ط³ط§ظ„</button>
        </div>
    </div>

    <button onclick="toggleChat()" class="chat-toggle">ًں’¬</button>

    <script>
        function toggleChat() {
            var chat = document.getElementById('ai-chat-box');
            chat.style.display = (chat.style.display === 'none' || chat.style.display === '') ? 'block' : 'none';
        }
        function sendMessage() {
            var input = document.getElementById('user-input');
            var content = document.getElementById('chat-content');
            if(input.value.trim() !== "") {
                content.innerHTML += "<p style='margin:5px 0;'><b>ط£ظ†طھ:</b> " + input.value + "</p>";
                setTimeout(function() {
                    content.innerHTML += "<p style='color: #e67e22; margin:5px 0;'><b>ط§ظ„ط±ظˆط¨ظˆطھ:</b> ظٹط³ط¹ط¯ظ†ظٹ ظ…ط³ط§ط¹ط¯طھظƒ! طھطµظپط­ ط§ظ„ظ…ظ†طھط¬ط§طھ ط§ظ„ظ…طھظˆظپط±ط© ط£ط¹ظ„ط§ظ‡ ظ„ظ„ط­طµظˆظ„ ط¹ظ„ظ‰ ط£ظپط¶ظ„ ط§ظ„ط®طµظˆظ…ط§طھ.</p>";
                    content.scrollTop = content.scrollHeight;
                }, 800);
                input.value = "";
                content.scrollTop = content.scrollHeight;
            }
        }
    </script>
</body>
</html>
```

---

## 2. ظƒظˆط¯ ط§ظ„ط£طھظ…طھط© ظˆط§ظ„ط°ظƒط§ط، ط§ظ„ط§طµط·ظ†ط§ط¹ظٹ ط§ظ„ط®ظ„ظپظٹ (app.py)
ظ‚ظ… ط¨ط­ظپط¸ ظ‡ط°ط§ ط§ظ„ظƒظˆط¯ ظƒظ…ظ„ظپ ط¨ط§ط³ظ… `app.py` ظ„طھط´ط؛ظٹظ„ ط±ظˆط¨ظˆطھط§طھ ط¬ظ„ط¨ ط§ظ„ط¨ظٹط§ظ†ط§طھ ظˆط±ط¨ط· ط§ظ„ظ€ API:

```python
import os
import openai
from aliexpress_api import AliexpressApi

# ط§ط³طھط¯ط¹ط§ط، ط§ظ„ظ…طھط؛ظٹط±ط§طھ ط§ظ„ط£ظ…ظ†ظٹط© ظˆط§ظ„ظ…ظپط§طھظٹط­
openai.api_key = os.getenv("OPENAI_API_KEY")
ALI_API_KEY = os.getenv("ALIEXPRESS_APP_KEY")
ALI_SECRET = os.getenv("ALIEXPRESS_APP_SECRET")

print("ط§ظ„ظ…ظ†ط¸ظˆظ…ط© ط§ظ„ط°ظƒظٹط© ط¬ط§ظ‡ط²ط© ظ„ظ„ط±ط¨ط· ظ…ط¹ ط§ظ„ظ†ط·ط§ظ‚ ظˆط§ظ„ظ…ظˆظ‚ط¹ ط¨ظ†ط¬ط§ط­!")
```

---

## 3. ط®ط·ظˆط© ط±ط¨ط· ط§ظ„ظ†ط·ط§ظ‚ ط§ظ„ظ…ط®طµطµ (.com) ط¨ط§ظ„ظ…طھط¬ط±
ظ„طھظپط¹ظٹظ„ ظ…ظˆظ‚ط¹ظƒ ط¨ط§ظ„ط§ط³ظ… ط§ظ„ظ…ط®طµطµ ط§ظ„ط°ظٹ ط§ط®طھط±طھظ‡ (ظ…ط«ظ„ط§ظ‹: `AffiliateSmartStore.com`):
1. ظ‚ظ… ط¨ط´ط±ط§ط، ط§ظ„ط¯ظˆظ…ظٹظ† ظ…ظ† ط´ط±ظƒط© ط­ط¬ط² (ظ…ط«ظ„ Namecheap ط£ظˆ GoDaddy).
2. ط§ط­طµظ„ ط¹ظ„ظ‰ ط§ط³طھط¶ط§ظپط© ظˆظٹط¨ (Hosting) طھط¯ط¹ظ… طھط´ط؛ظٹظ„ ظ…ظ„ظپط§طھظƒ.
3. ظ‚ظ… ط¨طھط؛ظٹظٹط± ط¥ط¹ط¯ط§ط¯ط§طھ ط§ظ„ظ€ **DNS** (ط³ط¬ظ„ط§طھ A Record) ط¯ط§ط®ظ„ ظ„ظˆط­ط© طھط­ظƒظ… ط§ظ„ط¯ظˆظ…ظٹظ† ظ„طھط´ظٹط± ط¥ظ„ظ‰ ط¹ظ†ظˆط§ظ† ط§ظ„ظ€ IP ط§ظ„ط®ط§طµ ط¨ط§ظ„ط§ط³طھط¶ط§ظپط©.
4. ط§ط±ظپط¹ ظ…ظ„ظپ `index.html` ط¥ظ„ظ‰ ظ…ط¬ظ„ط¯ `public_html` ط§ظ„ط±ط¦ظٹط³ظٹ ظ„ظٹط¹ظ…ظ„ ظ…طھط¬ط±ظƒ ظ…ط¨ط§ط´ط±ط© ط¹ظ†ط¯ ظƒطھط§ط¨ط© ط§ظ„ط¯ظˆظ…ظٹظ† ظپظٹ ط§ظ„ظ…طھطµظپط­.
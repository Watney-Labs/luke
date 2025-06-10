<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luke - Watney Labs</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'SF Pro Display', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
        }

        .card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(20px);
            border-radius: 24px;
            padding: 48px;
            max-width: 600px;
            width: 100%;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 30px 80px rgba(0, 0, 0, 0.15);
        }

        .header {
            display: flex;
            align-items: center;
            gap: 24px;
            margin-bottom: 40px;
        }

        .logo {
            width: 80px;
            height: 80px;
            object-fit: contain;
            filter: drop-shadow(0 4px 12px rgba(0, 0, 0, 0.1));
        }

        .profile-section {
            flex: 1;
        }

        .name {
            font-size: 2.5rem;
            font-weight: 700;
            color: #2d3748;
            margin-bottom: 8px;
            background: linear-gradient(135deg, #667eea, #764ba2);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .company {
            font-size: 1.2rem;
            color: #718096;
            font-weight: 500;
        }

        .headshot {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid rgba(255, 255, 255, 0.8);
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
        }

        .links-section {
            display: grid;
            gap: 16px;
        }

        .link-item {
            display: flex;
            align-items: center;
            padding: 16px 20px;
            background: rgba(255, 255, 255, 0.6);
            border-radius: 16px;
            text-decoration: none;
            color: #2d3748;
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .link-item:hover {
            background: rgba(255, 255, 255, 0.9);
            transform: translateX(8px);
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
        }

        .link-icon {
            width: 24px;
            height: 24px;
            margin-right: 16px;
            opacity: 0.8;
        }

        .link-content {
            flex: 1;
        }

        .link-title {
            font-weight: 600;
            font-size: 1.1rem;
            margin-bottom: 4px;
            color: #2d3748;
        }

        .link-subtitle {
            font-size: 0.9rem;
            color: #718096;
        }

        .special-link {
            background: linear-gradient(135deg, #667eea, #764ba2);
            color: white;
        }

        .special-link:hover {
            background: linear-gradient(135deg, #5a67d8, #6b46c1);
            color: white;
        }

        .special-link .link-title,
        .special-link .link-subtitle {
            color: white;
        }

        @media (max-width: 768px) {
            .card {
                padding: 32px 24px;
            }

            .header {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }

            .name {
                font-size: 2rem;
            }

            .headshot {
                width: 100px;
                height: 100px;
            }

            .logo {
                width: 60px;
                height: 60px;
            }
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="header">
            <img src="watney_logo.png" alt="Watney Labs Logo" class="logo">
            <div class="profile-section">
                <h1 class="name">Luke</h1>
                <p class="company">Watney Labs</p>
            </div>
            <img src="IMG_7186.jpeg" alt="Luke's Headshot" class="headshot">
        </div>

        <div class="links-section">
            <a href="mailto:luke@watneylabs.com" class="link-item">
                <svg class="link-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                    <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/>
                    <polyline points="22,6 12,13 2,6"/>
                </svg>
                <div class="link-content">
                    <div class="link-title">Email</div>
                    <div class="link-subtitle">luke@watneylabs.com</div>
                </div>
            </a>

            <a href="https://pitch.com/v/watney-7ai63p" target="_blank" class="link-item">
                <svg class="link-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                    <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/>
                    <polyline points="14,2 14,8 20,8"/>
                    <line x1="16" y1="13" x2="8" y2="13"/>
                    <line x1="16" y1="17" x2="8" y2="17"/>
                    <polyline points="10,9 9,9 8,9"/>
                </svg>
                <div class="link-content">
                    <div class="link-title">More Information</div>
                    <div class="link-subtitle">View our pitch deck</div>
                </div>
            </a>

            <a href="https://calendly.com/luke-watneylabs/30min" target="_blank" class="link-item special-link">
                <svg class="link-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                    <rect x="3" y="4" width="18" height="18" rx="2" ry="2"/>
                    <line x1="16" y1="2" x2="16" y2="6"/>
                    <line x1="8" y1="2" x2="8" y2="6"/>
                    <line x1="3" y1="10" x2="21" y2="10"/>
                </svg>
                <div class="link-content">
                    <div class="link-title">Book a Meeting</div>
                    <div class="link-subtitle">Schedule 30 minutes with me</div>
                </div>
            </a>

            <a href="https://app.watneylabs.com" target="_blank" class="link-item">
                <svg class="link-icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                    <path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/>
                    <polyline points="3.27,6.96 12,12.01 20.73,6.96"/>
                    <line x1="12" y1="22.08" x2="12" y2="12"/>
                </svg>
                <div class="link-content">
                    <div class="link-title">Try the Platform</div>
                    <div class="link-subtitle">Sign up code: potatoes</div>
                </div>
            </a>
        </div>
    </div>
</body>
</html>

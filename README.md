# Sheena-demo-landing-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>From Military Service to Million-Dollar Government Contracts</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            line-height: 1.6;
            color: #2d3748;
            background: #f7fafc;
        }
        
        .container {
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .hero {
            background: linear-gradient(135deg, #1a365d 0%, #2c5282 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
        }
        
        .preheader {
            font-size: 14px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            color: #90cdf4;
            margin-bottom: 20px;
        }
        
        h1 {
            font-size: 48px;
            font-weight: 900;
            line-height: 1.2;
            margin-bottom: 20px;
        }
        
        .subheader {
            font-size: 22px;
            font-weight: 400;
            margin-bottom: 40px;
            color: #e2e8f0;
        }
        
        .vsl-container {
            margin: 40px 0;
            position: relative;
            display: inline-block;
            cursor: pointer;
        }
        
        .vsl-thumbnail {
            width: 400px;
            height: 225px;
            background: linear-gradient(45deg, #4a5568, #2d3748);
            border-radius: 8px;
            position: relative;
            border: 3px solid #90cdf4;
        }
        
        .play-button {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80px;
            height: 80px;
            background: rgba(255, 255, 255, 0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s;
        }
        
        .play-button::after {
            content: '';
            width: 0;
            height: 0;
            border-left: 25px solid #2c5282;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 5px;
        }
        
        .vsl-container:hover .play-button {
            background: white;
            transform: translate(-50%, -50%) scale(1.1);
        }
        
        .primary-cta {
            background: #e53e3e;
            color: white;
            padding: 18px 40px;
            font-size: 22px;
            font-weight: 700;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s;
            box-shadow: 0 8px 25px rgba(229, 62, 62, 0.3);
        }
        
        .primary-cta:hover {
            background: #c53030;
            transform: translateY(-2px);
            box-shadow: 0 12px 35px rgba(229, 62, 62, 0.4);
        }
        
        .section {
            padding: 80px 0;
            background: white;
            margin-bottom: 40px;
        }
        
        .section:nth-child(even) {
            background: #f7fafc;
        }
        
        .section h2 {
            font-size: 36px;
            font-weight: 800;
            margin-bottom: 30px;
            text-align: center;
            color: #1a365d;
        }
        
        .section h3 {
            font-size: 28px;
            font-weight: 700;
            margin-bottom: 20px;
            color: #2c5282;
        }
        
        p {
            font-size: 18px;
            margin-bottom: 20px;
            max-width: none;
        }
        
        .pain-point {
            background: #fed7d7;
            border-left: 5px solid #e53e3e;
            padding: 20px;
            margin: 30px 0;
            border-radius: 0 8px 8px 0;
        }
        
        .testimonial {
            background: #e6fffa;
            border-left: 5px solid #38b2ac;
            padding: 25px;
            margin: 40px 0;
            border-radius: 0 8px 8px 0;
            font-style: italic;
            font-size: 20px;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: #2c5282;
            margin-top: 15px;
            font-style: normal;
        }
        
        .bullet-points {
            list-style: none;
            margin: 30px 0;
        }
        
        .bullet-points li {
            background: white;
            padding: 20px;
            margin: 15px 0;
            border-left: 5px solid #3182ce;
            border-radius: 0 8px 8px 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        }
        
        .bullet-points li strong {
            color: #2c5282;
            display: block;
            margin-bottom: 8px;
        }
        
        .price-section {
            background: linear-gradient(135deg, #2c5282 0%, #1a365d 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
            margin: 40px 0;
        }
        
        .price {
            font-size: 48px;
            font-weight: 900;
            color: #90cdf4;
            margin: 20px 0;
        }
        
        .guarantee {
            background: #f0fff4;
            border: 2px solid #68d391;
            padding: 30px;
            border-radius: 12px;
            margin: 40px 0;
            text-align: center;
        }
        
        .guarantee h4 {
            color: #2f855a;
            font-size: 24px;
            margin-bottom: 15px;
        }
        
        .urgency-box {
            background: #fffaf0;
            border: 2px solid #ed8936;
            padding: 25px;
            border-radius: 8px;
            margin: 30px 0;
        }
        
        .faq {
            background: #edf2f7;
            padding: 25px;
            margin: 20px 0;
            border-radius: 8px;
        }
        
        .faq h4 {
            color: #2d3748;
            font-size: 20px;
            margin-bottom: 10px;
        }
        
        .bold { font-weight: 700; }
        .italic { font-style: italic; }
        .caps { text-transform: uppercase; }
        
        @media (max-width: 768px) {
            h1 { font-size: 32px; }
            .subheader { font-size: 18px; }
            .vsl-thumbnail { width: 320px; height: 180px; }
            .section { padding: 40px 0; }
            .section h2 { font-size: 28px; }
        }
    </style>
</head>
<body>
    <!-- HERO SECTION -->
    <section class="hero">
        <div class="container">
            <div class="preheader">For Retired Military & Veteran Entrepreneurs</div>
            
            <h1>From Zero Contracts to<br>3-Tier Government Contractor<br>in 90 Days</h1>
            
            <div class="subheader">
                Master federal, local, and corporate contracting without drowning in bureaucratic red tape or wasting months figuring it out alone
            </div>
            
            <div class="vsl-container">
                <div class="vsl-thumbnail">
                    <div class="play-button"></div>
                </div>
            </div>
            
            <button class="primary-cta">Get Instant Access Now</button>
        </div>
    </section>

    <!-- PROBLEM IDENTIFICATION -->
    <section class="section">
        <div class="container">
            <h2>The Government Contracting "Maze" That's Keeping You Broke</h2>
            
            <p>You served your country with honor.</p>
            
            <p>Now you're ready to build something of your own... but every time you try to crack the government contracting code, you hit another wall.</p>
            
            <div class="pain-point">
                <strong>Sound familiar?</strong> You've spent hours on SAM.gov only to get lost in a sea of confusing forms. You've watched YouTube videos that promise "easy government money" but leave out the critical details. You've even paid for courses that gave you generic advice without showing you the actual screens, the real templates, or the insider moves that separate winners from wannabes.
            </div>
            
            <p>Meanwhile, you're watching other contractors land $50K, $100K, even $500K+ deals...</p>
            
            <p>While you're still stuck trying to figure out what a UEI number even IS.</p>
            
            <p>Here's what nobody tells you: <span class="bold">The government contracting space isn't hard because the rules are complicated...</span></p>
            
            <p><span class="bold italic">It's hard because you're trying to navigate THREE completely different systems at once.</span></p>
            
            <p>And if you don't master all three? You'll never graduate from being a small-time vendor to becoming a <span class="caps bold">real contractor</span> with recurring, high-dollar deals.</p>
            
            <p>But what if I told you there's a way to cut through all the confusion... and position yourself as a serious player in 90 days or less?</p>
            
            <div class="testimonial">
                "I went from having no idea how to even register my business to landing my first city contract for $23,000 in just 6 weeks. The step-by-step guidance was exactly what I needed."
                <div class="testimonial-author">— Sarah M., Houston Facilities Contractor</div>
            </div>
        </div>
    </section>

    <!-- ORIGIN STORY -->
    <section class="section">
        <div class="container">
            <h2>How a Retired Signal Officer Cracked the "3-Tier Code"</h2>
            
            <p>Seven years ago, I was exactly where you are now.</p>
            
            <p>Retired from the Army. Ready to build something. But completely lost when it came to government contracting.</p>
            
            <p>I tried everything: attended expensive seminars, bought course after course, even hired a consultant who charged me $3,000 to basically Google search contracting opportunities for me.</p>
            
            <p><span class="bold">Nothing worked.</span></p>
            
            <p>That's when I had my breakthrough moment...</p>
            
            <p>I was sitting in a coffee shop, frustrated after another failed attempt at understanding sub-contracting, when I overheard two contractors talking. One was complaining about only getting small federal jobs. The other was bragging about his corporate contracts with major companies.</p>
            
            <p>It hit me like a lightning bolt: <span class="italic">They weren't competing in the same space at all.</span></p>
            
            <p>Most contractors focus on just ONE tier - usually federal - and wonder why they're stuck fighting for scraps.</p>
            
            <p>But the contractors making REAL money? They play in all three arenas:</p>
            
            <p><span class="bold">Federal contracts</span> (the big, prestigious deals everyone talks about)</p>
            <p><span class="bold">Local contracts</span> (the steady, relationship-based work nobody mentions)</p>
            <p><span class="bold">Corporate contracts</span> (the hidden goldmine that most veterans never even know exists)</p>
            
            <p>That night, I mapped out what would become the 3-Tier Contractor System...</p>
            
            <p>Within 18 months, my company 4SYT Industries was pulling contracts from all three tiers. Federal maintenance contracts. City buildout projects. Corporate facility management deals.</p>
            
            <p>Today, we're not just surviving - we're thriving across multiple revenue streams because we refused to put all our eggs in one contracting basket.</p>
        </div>
    </section>

    <!-- SOLUTION REVELATION -->
    <section class="section">
        <div class="container">
            <h2>The 3-Tier Contractor System That Changes Everything</h2>
            
            <p>Here's what I discovered: The contractors making six and seven figures aren't smarter than you.</p>
            
            <p>They just understand something most people don't...</p>
            
            <p><span class="bold">Each tier has its own language, its own systems, and its own secret handshakes.</span></p>
            
            <h3>Tier 1: Federal Mastery</h3>
            <p>This is where everyone starts... and where most get stuck. SAM registration, NAICS codes, past performance records. Yes, it's complex. But once you know the exact steps (and I mean EXACT - down to which buttons to click), you can position yourself for contracts worth hundreds of thousands.</p>
            
            <h3>Tier 2: Local Goldmine</h3>
            <p>Here's what shocked me: Cities and counties often have LESS competition than federal contracts. Why? Because most contractors never figure out how to find local solicitations. I'll show you the three websites that 90% of contractors never check... where contracts are practically waiting for qualified bidders.</p>
            
            <h3>Tier 3: Corporate Contracts</h3>
            <p>The hidden tier. Major corporations need facility maintenance, security services, and specialized work. But they don't advertise on government sites. I'll reveal the supplier portals and certification programs that open doors to steady, high-paying corporate work.</p>
            
            <p>When you master all three tiers, something incredible happens:</p>
            
            <p><span class="bold">You're no longer dependent on any single source of revenue.</span></p>
            
            <p>Federal contract delayed? Your local work keeps you going.</p>
            <p>City budget cuts? Your corporate contracts pick up the slack.</p>
            <p>Corporate client changes direction? Your federal pipeline keeps flowing.</p>
            
            <p>This isn't theory. This is exactly how 4SYT Industries has built a bulletproof contracting business over the past seven years.</p>
            
            <div class="testimonial">
                "The 3-tier approach completely changed my perspective. I was only looking at federal contracts and getting nowhere. Now I have active bids in all three areas and landed my first corporate contract last month."
                <div class="testimonial-author">— Marcus T., Army Veteran & Business Owner</div>
            </div>
        </div>
    </section>

    <!-- PRODUCT INTRODUCTION -->
    <section class="section">
        <div class="container">
            <h2>Introducing: The Complete 3-Tier Contractor Blueprint</h2>
            
            <p>After seven years of trial and error, wins and losses, I've distilled everything into a step-by-step system that takes you from zero to 3-tier contractor faster than I ever thought possible.</p>
            
            <p>This isn't another generic "government contracting 101" course.</p>
            
            <p>This is the <span class="bold">exact blueprint</span> I used to build 4SYT Industries from nothing into a multi-tier contracting business.</p>
            
            <p>Every screen share. Every template. Every insider secret I learned the hard way.</p>
            
            <p>Here's what makes this different from everything else you've seen:</p>
            
            <ul class="bullet-points">
                <li>
                    <strong>Real screen recordings of actual registration processes</strong>
                    No more guessing which buttons to click or forms to fill out - you'll watch over my shoulder as I navigate every government website and portal
                </li>
                <li>
                    <strong>My actual capability statement and proposal templates</strong>
                    The same documents that helped us win real contracts, not generic examples that look like they came from a textbook
                </li>
                <li>
                    <strong>Veteran-specific marketing strategies that actually work</strong>
                    How to leverage your military background in each tier without sounding like every other veteran-owned business
                </li>
                <li>
                    <strong>The "relationship blueprint" for local contracting</strong>
                    Discover the three key relationships in every city that can fast-track you to preferred vendor status
                </li>
                <li>
                    <strong>Corporate supplier portal walkthroughs</strong>
                    I'll show you exactly how to get registered with major corporations that need your services but never advertise publicly
                </li>
            </ul>
            
            <p>Plus, you're getting something no other course offers: <span class="bold">ongoing coaching and mentorship</span> to ensure you actually implement what you learn.</p>
            
            <p>Because let's be honest - information without implementation is just expensive entertainment.</p>
        </div>
    </section>

    <!-- OFFER STRUCTURE -->
    <section class="section">
        <div class="container">
            <h2>Everything You Get Inside the 3-Tier Contractor Blueprint</h2>
            
            <ul class="bullet-points">
                <li>
                    <strong>27 comprehensive video lessons (7.5 hours total)</strong>
                    Walk through every single step of the 3-tier system, from business setup to securing your first contracts in each tier
                </li>
                <li>
                    <strong>Federal Contracting Mastery Module</strong>
                    SAM registration, solicitation hunting, past performance building, certification strategies, and sub-contracting pros and cons
                </li>
                <li>
                    <strong>Local Government Goldmine Module</strong>
                    City and county bidding systems, local certifications, relationship building, and the three secret websites most contractors never find
                </li>
                <li>
                    <strong>Corporate Contracting Breakthrough Module</strong>
                    Supplier portal navigation, corporate relationship building, and the certification programs that open corporate doors
                </li>
                <li>
                    <strong>Veteran Marketing Advantage Module</strong>
                    Turn your military experience into a competitive edge in each contracting tier without falling into common veteran business traps
                </li>
                <li>
                    <strong>Essential Documents & Templates</strong>
                    Capability statements, proposal frameworks, and company registration documents - everything you need to look professional from day one
                </li>
                <li>
                    <strong>1-on-1 Virtual Coaching Sessions</strong>
                    Direct access to me for personalized guidance on your specific business and contracting goals
                </li>
                <li>
                    <strong>Bi-Monthly Office Hours</strong>
                    Group coaching sessions where you can get answers to your questions and learn from other contractors' challenges
                </li>
                <li>
                    <strong>Monthly Private Group Mentorship</strong>
                    Exclusive training sessions with fellow veterans and contractors working through the same system
                </li>
                <li>
                    <strong>Complimentary Strategy Consultation</strong>
                    Personal session to identify your best contracting opportunities and create your 90-day implementation plan
                </li>
            </ul>
            
            <div class="guarantee">
                <h4>My Personal Success Guarantee</h4>
                <p>Follow the system, implement the strategies, and show up to the coaching calls. If you don't see measurable progress toward your first contract within 90 days, I'll personally work with you until you do - at no additional cost.</p>
                <p><span class="bold">That's my promise to you as a fellow veteran.</span></p>
            </div>
        </div>
    </section>

    <!-- PRICING -->
    <section class="price-section">
        <div class="container">
            <h2>Your Investment in Your Contracting Future</h2>
            
            <p>I could easily charge $10,000 for this system.</p>
            
            <p>That's what most high-level government contracting consultants charge for far less comprehensive programs.</p>
            
            <p>But I remember what it was like starting out...</p>
            
            <p>Trying to make the transition from military service to business ownership without breaking the bank.</p>
            
            <div class="price">$2,500</div>
            
            <p><span class="bold">Payment plans available</span> to make this accessible for serious contractors ready to build their future.</p>
            
            <div class="urgency-box">
                <p style="color: black;"><span class="bold">Important:</span> I'm limiting this first group to 50 contractors maximum. Why? Because I personally review every application and provide individual coaching. Once we hit 50, the doors close until the next group is ready.</p>
                
                <p style="color: black;">Current enrollment: 37 of 50 spots filled.</p>
            </div>
            
            <button class="primary-cta">Secure Your Spot Now</button>
        </div>
    </section>

    <!-- FAQ SECTION -->
    <section class="section">
        <div class="container">
            <h2>Questions From Serious Contractors</h2>
            
            <div class="faq">
                <h4>Q: "I'm brand new to government contracting. Will this work for someone with zero experience?"</h4>
                <p>Absolutely. The system is designed to take you from complete beginner to competent contractor. I start with the basics and build up to advanced strategies. Plus, the coaching ensures you never get stuck.</p>
            </div>
            
            <div class="faq">
                <h4>Q: "I've tried other government contracting courses before and they didn't work. How is this different?"</h4>
                <p>Most courses give you generic theory. This gives you my actual process, with real screen recordings, actual templates, and ongoing support. Plus, the 3-tier approach means you're not putting all your eggs in the federal contracting basket.</p>
            </div>
            
            <div class="faq">
                <h4>Q: "What if my business isn't in facilities maintenance? Will this still apply?"</h4>
                <p>Yes. The 3-tier system works for any service-based business that can contract with government and corporate clients: IT services, security, consulting, construction, professional services, and more.</p>
            </div>
            
            <div class="faq">
                <h4>Q: "How much time will I need to dedicate to this?"</h4>
                <p>The video content is 7.5 hours, which you can complete at your own pace. Implementation takes 2-3 hours per week for most contractors. The key is consistency, not marathon sessions.</p>
            </div>
            
            <div class="faq">
                <h4>Q: "What if I can't afford the full payment right now?"</h4>
                <p>Payment plans are available for qualified contractors. During your consultation call, we'll discuss options that work for your situation.</p>
            </div>
            
            <div class="faq">
                <h4>Q: "Is this just for veterans, or can non-veterans benefit too?"</h4>
                <p>While there's specific content for leveraging veteran status, the 3-tier system works for any entrepreneur serious about government and corporate contracting. The core strategies are universal.</p>
            </div>
            
            <p style="text-align: center; margin-top: 40px; font-size: 20px;">
                <span class="bold">Ready to stop spinning your wheels and start building your contracting empire?</span>
            </p>
            
            <div style="text-align: center; margin-top: 30px;">
                <button class="primary-cta">Get Started Today</button>
            </div>
        </div>
    </section>
</body>
</html>

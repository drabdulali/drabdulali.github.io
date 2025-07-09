<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dr. Abdul Ali - Infectious Disease Ecologist</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Georgia', serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #2c5530, #4a7c59);
            color: white;
            padding: 2rem 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><circle cx="20" cy="20" r="2" fill="rgba(255,255,255,0.1)"/><circle cx="80" cy="40" r="1.5" fill="rgba(255,255,255,0.1)"/><circle cx="60" cy="70" r="1" fill="rgba(255,255,255,0.1)"/><circle cx="30" cy="80" r="2.5" fill="rgba(255,255,255,0.1)"/></svg>');
            pointer-events: none;
        }

        .header-content {
            position: relative;
            z-index: 1;
        }

        h1 {
            font-size: 3rem;
            margin-bottom: 0.5rem;
            font-weight: 300;
        }

        .subtitle {
            font-size: 1.3rem;
            font-weight: 300;
            opacity: 0.9;
        }

        /* Navigation */
        nav {
            background: #1a3d20;
            padding: 1rem 0;
            position: sticky;
            top: 0;
            z-index: 100;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
        }

        nav li {
            margin: 0 1rem;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            transition: background-color 0.3s;
            display: block;
        }

        nav a:hover {
            background: #2c5530;
        }

        /* Main Content */
        main {
            padding: 2rem 0;
        }

        .section {
            background: white;
            margin: 2rem 0;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .section h2 {
            color: #2c5530;
            margin-bottom: 1rem;
            font-size: 2rem;
            border-bottom: 3px solid #4a7c59;
            padding-bottom: 0.5rem;
        }

        .concept-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }

        .concept-card {
            background: #f8f9fa;
            padding: 1.5rem;
            border-radius: 8px;
            border-left: 4px solid #4a7c59;
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .concept-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        .concept-card h3 {
            color: #2c5530;
            margin-bottom: 0.5rem;
        }

        .concept-card p {
            color: #666;
            margin-bottom: 1rem;
        }

        .read-more {
            color: #4a7c59;
            text-decoration: none;
            font-weight: bold;
            display: inline-flex;
            align-items: center;
            transition: color 0.3s;
        }

        .read-more:hover {
            color: #2c5530;
        }

        .read-more::after {
            content: '→';
            margin-left: 0.5rem;
        }

        /* Research Areas */
        .research-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1rem;
            margin-top: 1.5rem;
        }

        .research-item {
            background: linear-gradient(135deg, #e8f5e8, #f0f8f0);
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            border: 2px solid #4a7c59;
        }

        .research-item h3 {
            color: #2c5530;
            margin-bottom: 0.5rem;
        }

        /* Recent Posts */
        .post-preview {
            border-bottom: 1px solid #eee;
            padding: 1.5rem 0;
        }

        .post-preview:last-child {
            border-bottom: none;
        }

        .post-date {
            color: #666;
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
        }

        .post-title {
            color: #2c5530;
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
        }

        .post-excerpt {
            color: #666;
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            background: #1a3d20;
            color: white;
            text-align: center;
            padding: 2rem 0;
            margin-top: 3rem;
        }

        .social-links {
            margin-top: 1rem;
        }

        .social-links a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
            transition: opacity 0.3s;
        }

        .social-links a:hover {
            opacity: 0.7;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav li {
                margin: 0.25rem 0;
            }
            
            .concept-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <h1>Dr. Abdul Ali</h1>
                <p class="subtitle">Infectious Disease Ecologist</p>
            </div>
        </div>
    </header>

    <nav>
        <div class="container">
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#research">Research</a></li>
                <li><a href="#concepts">Concepts</a></li>
                <li><a href="#publications">Publications</a></li>
                <li><a href="#blog">Blog</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <main class="container">
        <section id="home" class="section">
            <h2>Welcome to Infectious Disease Ecology</h2>
            <p>Exploring the complex relationships between pathogens, hosts, and their environments. This site serves as a resource for understanding how ecological principles shape disease dynamics and inform public health strategies.</p>
            <p>Here you'll find insights into disease ecology, pathogen evolution, host-pathogen interactions, and the environmental factors that influence infectious disease emergence and spread.</p>
        </section>

        <section id="about" class="section">
            <h2>About</h2>
            <p>As an Infectious Disease Ecologist, I study the intricate connections between pathogens, their hosts, and the environment. My research focuses on understanding how ecological processes influence disease transmission, evolution, and control strategies.</p>
            <p>This interdisciplinary field combines principles from ecology, epidemiology, evolution, and environmental science to address some of the most pressing health challenges of our time.</p>
        </section>

        <section id="research" class="section">
            <h2>Research Areas</h2>
            <div class="research-grid">
                <div class="research-item">
                    <h3>Disease Ecology</h3>
                    <p>Studying pathogen-host-environment interactions</p>
                </div>
                <div class="research-item">
                    <h3>Vector Ecology</h3>
                    <p>Understanding vector-borne disease dynamics</p>
                </div>
                <div class="research-item">
                    <h3>Zoonotic Diseases</h3>
                    <p>Investigating wildlife-human disease interfaces</p>
                </div>
                <div class="research-item">
                    <h3>Climate & Health</h3>
                    <p>Assessing climate change impacts on disease</p>
                </div>
            </div>
        </section>

        <section id="concepts" class="section">
            <h2>Key Concepts in Disease Ecology</h2>
            <div class="concept-grid">
                <div class="concept-card">
                    <h3>Basic Reproductive Number (R₀)</h3>
                    <p>The average number of secondary infections caused by one infected individual in a completely susceptible population. A fundamental metric in epidemiology.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
                <div class="concept-card">
                    <h3>Dilution Effect</h3>
                    <p>The phenomenon where increased biodiversity can reduce disease transmission by diluting the concentration of competent hosts.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
                <div class="concept-card">
                    <h3>Spillover Events</h3>
                    <p>The transmission of pathogens from animal reservoirs to humans, often leading to emerging infectious diseases.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
                <div class="concept-card">
                    <h3>Vector Competence</h3>
                    <p>The ability of arthropod vectors to acquire, maintain, and transmit pathogens to susceptible hosts.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
                <div class="concept-card">
                    <h3>Disease Reservoir</h3>
                    <p>The natural habitat or host population where pathogens normally live and reproduce without causing disease.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
                <div class="concept-card">
                    <h3>One Health Approach</h3>
                    <p>An integrated approach recognizing the interconnection between human, animal, and environmental health.</p>
                    <a href="#" class="read-more">Learn More</a>
                </div>
            </div>
        </section>

        <section id="publications" class="section">
            <h2>Recent Publications</h2>
            <div class="post-preview">
                <div class="post-date">2024</div>
                <h3 class="post-title">Climate Change and Vector-Borne Disease Expansion</h3>
                <p class="post-excerpt">An analysis of how changing temperature and precipitation patterns affect the geographic distribution of disease vectors...</p>
                <a href="#" class="read-more">Read Full Paper</a>
            </div>
            <div class="post-preview">
                <div class="post-date">2024</div>
                <h3 class="post-title">Biodiversity Loss and Emerging Infectious Diseases</h3>
                <p class="post-excerpt">Examining the relationship between habitat fragmentation, species diversity, and disease emergence risk...</p>
                <a href="#" class="read-more">Read Full Paper</a>
            </div>
        </section>

        <section id="blog" class="section">
            <h2>Latest Blog Posts</h2>
            <div class="post-preview">
                <div class="post-date">January 15, 2025</div>
                <h3 class="post-title">Understanding Pathogen Evolution in Changing Environments</h3>
                <p class="post-excerpt">How environmental pressures drive the evolution of infectious agents and what this means for disease control strategies...</p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="post-preview">
                <div class="post-date">January 10, 2025</div>
                <h3 class="post-title">The Role of Wildlife in Disease Surveillance</h3>
                <p class="post-excerpt">Exploring how wildlife monitoring can serve as an early warning system for emerging infectious diseases...</p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="post-preview">
                <div class="post-date">January 5, 2025</div>
                <h3 class="post-title">Ecological Niche Modeling for Disease Prediction</h3>
                <p class="post-excerpt">Using computational models to predict disease distribution based on environmental and ecological factors...</p>
                <a href="#" class="read-more">Read More</a>
            </div>
        </section>

        <section id="contact" class="section">
            <h2>Contact & Collaboration</h2>
            <p>Interested in collaborating on research or have questions about infectious disease ecology? I'm always open to discussing new ideas and potential partnerships.</p>
            <p>Feel free to reach out for:</p>
            <ul style="margin-top: 1rem; margin-left: 2rem;">
                <li>Research collaborations</li>
                <li>Guest lectures or seminars</li>
                <li>Manuscript reviews</li>
                <li>Graduate student mentoring</li>
            </ul>
        </section>
    </main>

    <footer>
        <div class="container">
            <p>&copy; 2025 Dr. Abdul Ali - Infectious Disease Ecologist. All rights reserved.</p>
            <div class="social-links">
                <a href="#">ResearchGate</a>
                <a href="#">ORCID</a>
                <a href="#">Twitter</a>
                <a href="#">LinkedIn</a>
                <a href="https://github.com/drabdulali">GitHub</a>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Add some interactivity to concept cards
        document.querySelectorAll('.concept-card').forEach(card => {
            card.addEventListener('click', function() {
                // You can add modal functionality here later
                console.log('Clicked on:', this.querySelector('h3').textContent);
            });
        });
    </script>
</body>
</html>

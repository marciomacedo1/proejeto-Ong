<!DOCTYPE html>
<html lang="pt-BR" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Festival de Iniciação Artística Comunitária</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Merriweather:wght@700;900&display=swap" rel="stylesheet">
    <!-- Chosen Palette: Amazonian Earth -->
    <!-- Application Structure Plan: A single-page application with a sticky top navigation bar for easy access to all key sections. The flow is designed to guide the user from initial impact (Home) to detailed understanding (O Festival), direct action (Inscrições), and finally to informational/support sections (Imprensa, Apoio). This non-linear but guided structure allows different user types (participant, press, sponsor) to find what they need quickly, maximizing usability. -->
    <!-- Visualization & Content Choices: The project's content is primarily qualitative and informational. Goal: Inform/Engage -> Method: Thematic Sections with clear typography and iconography. Interaction: Smooth scrolling and an interactive registration form. Justification: This approach is best for storytelling and guiding users toward the main call to action (registration) without overwhelming them with complex data visualizations, which are not central to this report's content. Goal: Action -> Method: HTML Form + JS. Interaction: Form submission with dynamic feedback. Justification: Provides a seamless, single-page registration experience. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #FDFBF8;
            color: #3D2B1F;
        }
        h1, h2, h3 {
            font-family: 'Merriweather', serif;
        }
        .nav-link.active {
            color: #A55A2A;
            font-weight: 700;
        }
        .hero-bg {
            background-image: linear-gradient(to bottom, rgba(253, 251, 248, 0.5), rgba(253, 251, 248, 1)), url('https://images.unsplash.com/photo-1616333983249-95242a8b3e2a?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header & Navigation -->
    <header id="header" class="bg-white/80 backdrop-blur-md sticky top-0 z-50 shadow-sm">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#inicio" class="text-2xl font-bold text-[#4A3F35]">
                Festival
            </a>
            <div class="hidden md:flex space-x-8">
                <a href="#festival" class="nav-link text-gray-600 hover:text-[#A55A2A] transition-colors duration-300">O Festival</a>
                <a href="#inscricoes" class="nav-link text-gray-600 hover:text-[#A55A2A] transition-colors duration-300">Oficinas & Inscrições</a>
                <a href="#imprensa" class="nav-link text-gray-600 hover:text-[#A55A2A] transition-colors duration-300">Imprensa</a>
            </div>
            <a href="#apoio" class="hidden md:block bg-[#A55A2A] text-white px-5 py-2 rounded-full hover:bg-[#8e4d23] transition-colors duration-300">Apoie o Projeto</a>
            <button id="mobile-menu-button" class="md:hidden text-2xl">☰</button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white/90 backdrop-blur-md">
            <a href="#festival" class="block text-center py-2 px-4 text-gray-600 hover:bg-gray-100">O Festival</a>
            <a href="#inscricoes" class="block text-center py-2 px-4 text-gray-600 hover:bg-gray-100">Oficinas & Inscrições</a>
            <a href="#imprensa" class="block text-center py-2 px-4 text-gray-600 hover:bg-gray-100">Imprensa</a>
            <a href="#apoio" class="block text-center py-4 px-4 bg-[#A55A2A] text-white hover:bg-[#8e4d23]">Apoie o Projeto</a>
        </div>
    </header>

    <main>
        <!-- Home Section -->
        <section id="inicio" class="hero-bg pt-24 pb-32">
            <div class="container mx-auto px-6 text-center">
                <h1 class="text-4xl md:text-6xl font-black text-[#4A3F35] mb-4 leading-tight">Festival de Iniciação Artística Comunitária</h1>
                <p class="text-lg md:text-xl text-[#6B4F4F] max-w-3xl mx-auto mb-8">Democratizando o acesso à cultura em Belém através de oficinas gratuitas, shows e uma grande celebração da arte paraense.</p>
                <a href="#inscricoes" class="bg-[#A55A2A] text-white px-8 py-4 rounded-full text-lg font-bold hover:bg-[#8e4d23] transition-colors duration-300 shadow-lg">Inscreva-se nas Oficinas</a>
            </div>
        </section>

        <!-- O Festival Section -->
        <section id="festival" class="py-20">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-4xl font-bold text-[#4A3F35]">Conheça o Coração do Projeto</h2>
                    <p class="text-lg text-[#6B4F4F] mt-2 max-w-2xl mx-auto">Nossa missão é usar a arte como ferramenta de transformação social e valorização da nossa identidade cultural.</p>
                </div>

                <div class="grid md:grid-cols-2 gap-12 items-center">
                    <div>
                        <h3 class="text-2xl font-bold text-[#4A3F35] mb-4">Justificativa e Objetivos</h3>
                        <p class="text-gray-700 mb-6">Este festival nasce da necessidade de criar espaços de aprendizado e expressão artística em nossas comunidades. Alinhado à Lei Rouanet, nosso objetivo é estimular a formação cultural, valorizar os talentos locais e facilitar o acesso de todos à arte, fortalecendo a cidadania e a economia criativa de Belém.</p>
                        <div class="space-y-3">
                           <p><strong><span class="text-[#A55A2A]">PARA QUÊ?</span></strong> Para democratizar o acesso à cultura, fomentar a expressão artística local e promover a inclusão social.</p>
                           <p><strong><span class="text-[#A55A2A]">QUAIS?</span></strong> Realizaremos 9 turmas de oficinas, 1 evento final de 2 dias com mostra cultural, feira criativa, shows locais e 1 atração nacional.</p>
                        </div>
                    </div>
                    <div class="bg-white p-8 rounded-lg shadow-md border border-gray-200">
                        <h3 class="text-2xl font-bold text-center text-[#4A3F35] mb-6">Programação do Evento Final</h3>
                        <div class="space-y-4">
                            <div class="text-center">
                                <p class="font-bold text-lg text-[#A55A2A]">Dia 1 (Sábado)</p>
                                <p>16h - Abertura da Feira Criativa</p>
                                <p>17h - Mostra Cultural das Oficinas</p>
                                <p>19h - Shows com Bandas de Abertura Locais</p>
                            </div>
                            <hr class="my-4">
                            <div class="text-center">
                                <p class="font-bold text-lg text-[#A55A2A]">Dia 2 (Domingo)</p>
                                <p>16h - Feira Criativa e Atividades Infantis</p>
                                <p>18h - Sarau de Poesia</p>
                                <p>20h - Show com Atração Nacional</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Oficinas e Inscrições Section -->
        <section id="inscricoes" class="py-20 bg-white">
            <div class="container mx-auto px-6">
                <div class="text-center mb-12">
                    <h2 class="text-4xl font-bold text-[#4A3F35]">Oficinas Gratuitas: Venha Criar!</h2>
                    <p class="text-lg text-[#6B4F4F] mt-2 max-w-2xl mx-auto">As inscrições estão abertas! Escolha sua oficina e garanta sua vaga. Totalmente gratuito.</p>
                </div>
                
                <div class="grid md:grid-cols-3 gap-8 mb-12">
                    <!-- Card Oficina 1 -->
                    <div class="border border-gray-200 p-8 rounded-lg text-center hover:shadow-xl transition-shadow duration-300">
                        <div class="text-4xl mb-4 text-[#A55A2A]">🎵</div>
                        <h3 class="text-2xl font-bold mb-2">Percussão Paraense</h3>
                        <p class="text-gray-600">Aprenda os ritmos contagiantes do Pará, como o Carimbó e o Lundu, em uma oficina prática e cheia de energia.</p>
                    </div>
                    <!-- Card Oficina 2 -->
                    <div class="border border-gray-200 p-8 rounded-lg text-center hover:shadow-xl transition-shadow duration-300">
                        <div class="text-4xl mb-4 text-[#A55A2A]">✍️</div>
                        <h3 class="text-2xl font-bold mb-2">Escrita Criativa</h3>
                        <p class="text-gray-600">Explore sua criatividade e transforme suas vivências em poemas e crônicas, descobrindo sua voz literária.</p>
                    </div>
                    <!-- Card Oficina 3 -->
                    <div class="border border-gray-200 p-8 rounded-lg text-center hover:shadow-xl transition-shadow duration-300">
                        <div class="text-4xl mb-4 text-[#A55A2A]">🎨</div>
                        <h3 class="text-2xl font-bold mb-2">Arte em Miriti</h3>
                        <p class="text-gray-600">Mergulhe na tradição do artesanato paraense, criando brinquedos e esculturas a partir da palmeira do miriti.</p>
                    </div>
                </div>

                <div id="form-container" class="max-w-2xl mx-auto">
                    <form id="registration-form" class="bg-gray-50 p-8 rounded-lg shadow-inner border">
                        <h3 class="text-2xl font-bold text-center mb-6">Formulário de Inscrição</h3>
                        <div class="grid grid-cols-1 gap-6">
                            <input type="text" id="name" placeholder="Nome Completo" class="w-full p-3 border rounded-md focus:ring-2 focus:ring-[#A55A2A]" required>
                            <input type="email" id="email" placeholder="Seu Melhor E-mail" class="w-full p-3 border rounded-md focus:ring-2 focus:ring-[#A55A2A]" required>
                            <input type="tel" id="phone" placeholder="Telefone (WhatsApp)" class="w-full p-3 border rounded-md focus:ring-2 focus:ring-[#A55A2A]" required>
                            <select id="workshop" class="w-full p-3 border rounded-md bg-white" required>
                                <option value="" disabled selected>Escolha a oficina desejada</option>
                                <option value="percussao">Oficina de Percussão Paraense</option>
                                <option value="escrita">Oficina de Escrita Criativa</option>
                                <option value="miriti">Oficina de Arte em Miriti</option>
                            </select>
                            <button type="submit" class="w-full bg-[#A55A2A] text-white p-4 rounded-md text-lg font-bold hover:bg-[#8e4d23] transition-colors duration-300">Enviar Inscrição</button>
                        </div>
                    </form>
                    <div id="success-message" class="hidden mt-6 p-4 bg-green-100 text-green-800 border border-green-200 rounded-md text-center">
                        <p class="font-bold">Inscrição enviada com sucesso!</p>
                        <p>Entraremos em contato em breve para confirmar sua vaga. Obrigado!</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Imprensa Section -->
        <section id="imprensa" class="py-20">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-4xl font-bold text-[#4A3F35]">Espaço da Imprensa</h2>
                <p class="text-lg text-[#6B4F4F] mt-2 max-w-2xl mx-auto mb-8">Informações, releases e materiais de divulgação para veículos de comunicação.</p>
                <div class="max-w-lg mx-auto bg-white p-8 rounded-lg shadow-md border">
                    <p class="mb-4">Para entrevistas, pautas e mais informações, entre em contato com nossa assessoria.</p>
                    <p class="font-bold">Contato: <a href="mailto:imprensa@festivalcomunitario.com.br" class="text-[#A55A2A] hover:underline">imprensa@festivalcomunitario.com.br</a></p>
                    <a href="#" class="mt-6 inline-block bg-gray-700 text-white px-6 py-3 rounded-full hover:bg-gray-800 transition-colors">Baixar Press Kit</a>
                </div>
            </div>
        </section>

        <!-- Apoio Section -->
        <section id="apoio" class="py-20 bg-gray-50">
            <div class="container mx-auto px-6 text-center">
                <h2 class="text-4xl font-bold text-[#4A3F35]">Apoio e Patrocínio</h2>
                <p class="text-lg text-[#6B4F4F] mt-2 max-w-2xl mx-auto mb-12">Este projeto só é possível graças ao apoio de empresas e instituições que acreditam na cultura como motor de desenvolvimento.</p>
                
                <div class="space-y-10">
                    <div>
                        <h3 class="text-xl font-semibold text-gray-500 mb-4 tracking-widest">APRESENTA</h3>
                        <div class="flex justify-center items-center h-20 bg-gray-200 rounded-md max-w-sm mx-auto">
                            <span class="text-gray-500">Logo Patrocinador Master</span>
                        </div>
                    </div>
                    <div>
                        <h3 class="text-xl font-semibold text-gray-500 mb-4 tracking-widest">PATROCÍNIO</h3>
                        <div class="grid grid-cols-2 md:grid-cols-4 gap-8 max-w-3xl mx-auto">
                            <div class="flex justify-center items-center h-16 bg-gray-200 rounded-md"><span class="text-gray-500 text-sm">Logo</span></div>
                            <div class="flex justify-center items-center h-16 bg-gray-200 rounded-md"><span class="text-gray-500 text-sm">Logo</span></div>
                            <div class="flex justify-center items-center h-16 bg-gray-200 rounded-md"><span class="text-gray-500 text-sm">Logo</span></div>
                            <div class="flex justify-center items-center h-16 bg-gray-200 rounded-md"><span class="text-gray-500 text-sm">Logo</span></div>
                        </div>
                    </div>
                     <div>
                        <h3 class="text-xl font-semibold text-gray-500 mb-4 tracking-widest">REALIZAÇÃO</h3>
                        <div class="flex justify-center items-center h-20 bg-gray-200 rounded-md max-w-sm mx-auto">
                            <span class="text-gray-500">[Sua ONG/Proponente]</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-[#4A3F35] text-white py-12">
        <div class="container mx-auto px-6 text-center">
            <p class="font-bold text-lg mb-4">Festival de Iniciação Artística Comunitária</p>
            <div class="flex justify-center space-x-6 mb-6">
                <a href="#" class="text-2xl hover:text-[#A55A2A] transition-colors">◉</a> <!-- Instagram -->
                <a href="#" class="text-2xl hover:text-[#A55A2A] transition-colors">◉</a> <!-- Facebook -->
                <a href="#" class="text-2xl hover:text-[#A55A2A] transition-colors">◉</a> <!-- YouTube -->
            </div>
            <p class="text-gray-400">Contato Geral: <a href="mailto:contato@festivalcomunitario.com.br" class="hover:underline">contato@festivalcomunitario.com.br</a></p>
            <p class="text-sm text-gray-500 mt-4">&copy; 2026. Todos os direitos reservados.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // Mobile menu toggle
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
            });

            // Close mobile menu on link click
            document.querySelectorAll('#mobile-menu a').forEach(link => {
                link.addEventListener('click', () => {
                    mobileMenu.classList.add('hidden');
                });
            });
            
            // Smooth scroll for navigation links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });

            // Form submission handler
            const form = document.getElementById('registration-form');
            const successMessage = document.getElementById('success-message');
            form.addEventListener('submit', (e) => {
                e.preventDefault();
                // Basic validation check
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const workshop = document.getElementById('workshop').value;
                if (name && email && workshop) {
                    form.classList.add('hidden');
                    successMessage.classList.remove('hidden');
                } else {
                    alert('Por favor, preencha todos os campos obrigatórios.');
                }
            });

            // Active nav link highlighting on scroll
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-link');
            const headerHeight = document.getElementById('header').offsetHeight;

            window.addEventListener('scroll', () => {
                let current = '';
                sections.forEach(section => {
                    const sectionTop = section.offsetTop - headerHeight - 50;
                    if (pageYOffset >= sectionTop) {
                        current = section.getAttribute('id');
                    }
                });

                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${current}`) {
                        link.classList.add('active');
                    }
                });
            });
        });
    </script>
</body>
</html>

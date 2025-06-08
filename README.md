import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { motion } from "framer-motion"; import { FaGithub, FaLinkedin, FaEnvelope } from "react-icons/fa";

const Portfolio = () => { return ( <div className="min-h-screen bg-gray-100 text-gray-900"> <header className="bg-white shadow p-6"> <div className="container mx-auto flex justify-between items-center"> <h1 className="text-2xl font-bold">Meu Portfólio</h1> <nav> <a href="#about" className="px-4 py-2 hover:underline">Sobre</a> <a href="#projects" className="px-4 py-2 hover:underline">Projetos</a> <a href="#contact" className="px-4 py-2 hover:underline">Contato</a> </nav> </div> </header>

<main>
    {/* Hero Section */}
    <section className="bg-gray-200 py-20 text-center">
      <div className="container mx-auto">
        <motion.h1
          className="text-4xl font-bold mb-4"
          initial={{ opacity: 0, y: -50 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.5 }}
        >
          Olá, eu sou [Seu Nome]
        </motion.h1>
        <p className="text-lg mb-6">Desenvolvedor Moderno e Criativo</p>
        <Button className="px-6 py-3 text-white bg-blue-500 rounded-full hover:bg-blue-600">
          Veja Meus Projetos
        </Button>
      </div>
    </section>

    {/* About Section */}
    <section id="about" className="py-20 container mx-auto">
      <h2 className="text-3xl font-bold text-center mb-6">Sobre Mim</h2>
      <p className="text-center max-w-2xl mx-auto text-lg">
        Sou apaixonado por tecnologia e design. Com [anos de experiência] na criação de soluções modernas, estou sempre em busca de novos desafios.
      </p>
    </section>

    {/* Projects Section */}
    <section id="projects" className="bg-gray-100 py-20">
      <div className="container mx-auto">
        <h2 className="text-3xl font-bold text-center mb-6">Meus Projetos</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          {[1, 2, 3].map((project) => (
            <Card key={project} className="hover:shadow-lg transition">
              <CardContent>
                <img
                  src={`https://via.placeholder.com/300x200?text=Projeto+${project}`}
                  alt={`Projeto ${project}`}
                  className="mb-4 rounded-lg"
                />
                <h3 className="text-xl font-bold">Projeto {project}</h3>
                <p className="text-gray-700">Descrição breve do projeto {project}.</p>
              </CardContent>
            </Card>
          ))}
        </div>
      </div>
    </section>

    {/* Contact Section */}
    <section id="contact" className="py-20 bg-gray-200">
      <div className="container mx-auto text-center">
        <h2 className="text-3xl font-bold mb-6">Contato</h2>
        <p className="mb-4">Gostaria de trabalhar comigo? Entre em contato!</p>
        <div className="flex justify-center space-x-4">
          <a href="https://github.com" target="_blank" rel="noreferrer">
            <FaGithub className="text-3xl text-gray-700 hover:text-black" />
          </a>
          <a href="https://linkedin.com" target="_blank" rel="noreferrer">
            <FaLinkedin className="text-3xl text-blue-700 hover:text-blue-900" />
          </a>
          <a href="mailto:email@example.com">
            <FaEnvelope className="text-3xl text-gray-700 hover:text-black" />
          </a>
        </div>
      </div>
    </section>
  </main>

  <footer className="bg-gray-800 text-white text-center py-4">
    <p>&copy; {new Date().getFullYear()} Seu Nome. Todos os direitos reservados.</p>
  </footer>
</div>

); };

export default Portfolio;


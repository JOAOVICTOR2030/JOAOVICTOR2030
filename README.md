import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Facebook, Instagram, Phone } from "lucide-react";

export default function ChronoBeats() { return ( <main className="bg-black text-white min-h-screen"> {/* Header */} <header className="p-6 flex justify-between items-center border-b border-gray-800"> <h1 className="text-3xl font-bold text-white">ChronoBeats</h1> <nav className="space-x-6"> <a href="#home" className="hover:text-purple-400">Home</a> <a href="#about" className="hover:text-purple-400">Sobre</a> <a href="#products" className="hover:text-purple-400">Produtos</a> <a href="#contact" className="hover:text-purple-400">Contato</a> </nav> </header>

{/* Hero Section */}
  <section id="home" className="p-10 text-center bg-gradient-to-br from-purple-900 to-black">
    <h2 className="text-4xl font-bold mb-4">Estilo que pulsa no seu ritmo</h2>
    <p className="text-lg text-gray-300">Fones, relógios e muito mais em um só lugar</p>
  </section>

  {/* Sobre */}
  <section id="about" className="p-10 bg-black">
    <h2 className="text-2xl font-bold mb-4 text-purple-300">Sobre a ChronoBeats</h2>
    <p className="text-gray-400 max-w-3xl">
      A ChronoBeats é uma loja especializada em eletrônicos modernos como fones, relógios e smartwatches. Com produtos de alta qualidade e um atendimento personalizado, buscamos sempre oferecer o melhor para você que vive no ritmo do tempo.
    </p>
  </section>

  {/* Produtos */}
  <section id="products" className="p-10 bg-black">
    <h2 className="text-2xl font-bold mb-6 text-purple-300">Nossos Produtos</h2>
    <div className="grid md:grid-cols-3 gap-6">
      <Card>
        <CardContent className="p-4">
          <img src="/fones.jpg" alt="Fone de Ouvido" className="rounded-xl mb-4" />
          <h3 className="text-xl font-semibold">Fones de Ouvido</h3>
          <p className="text-sm text-gray-400">Qualidade sonora para o seu dia a dia.</p>
        </CardContent>
      </Card>
      <Card>
        <CardContent className="p-4">
          <img src="/relogio.jpg" alt="Relógio" className="rounded-xl mb-4" />
          <h3 className="text-xl font-semibold">Relógios Estilosos</h3>
          <p className="text-sm text-gray-400">Estilo e funcionalidade no seu pulso.</p>
        </CardContent>
      </Card>
      <Card>
        <CardContent className="p-4">
          <img src="/smartwatch.jpg" alt="Smartwatch" className="rounded-xl mb-4" />
          <h3 className="text-xl font-semibold">Smartwatches</h3>
          <p className="text-sm text-gray-400">Tecnologia conectada ao seu tempo.</p>
        </CardContent>
      </Card>
    </div>
  </section>

  {/* Contato */}
  <section id="contact" className="p-10 bg-gradient-to-tr from-black to-purple-900">
    <h2 className="text-2xl font-bold mb-6 text-purple-200">Fale com a gente</h2>
    <div className="flex flex-col md:flex-row gap-4">
      <Button variant="outline" className="flex items-center gap-2">
        <Phone className="w-5 h-5" /> WhatsApp
      </Button>
      <Button variant="outline" className="flex items-center gap-2">
        <Facebook className="w-5 h-5" /> Facebook
      </Button>
      <Button variant="outline" className="flex items-center gap-2">
        <Instagram className="w-5 h-5" /> Instagram
      </Button>
    </div>
  </section>
</main>

); }



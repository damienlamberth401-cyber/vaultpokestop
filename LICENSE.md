export default function VaultPokeStopWebsite() {
  const products = [
    {
      title: "Singles",
      description:
        "Browse rare Pokémon singles, modern hits, vintage cards, and collector favorites.",
    },
    {
      title: "Graded",
      description:
        "High-quality graded cards for collectors who want authenticity and protection.",
    },
    {
      title: "Packs / Boxes",
      description:
        "Sealed Pokémon packs, booster boxes, ETBs, and special collection products.",
    },
    {
      title: "Bulk",
      description:
        "Affordable bulk cards for deck builders, collectors, and trade stock.",
    },
  ];

  return (
    <div className="min-h-screen bg-black text-white font-sans">
      {/* Header */}
      <header className="border-b border-red-900 bg-zinc-950 sticky top-0 z-50">
        <div className="max-w-7xl mx-auto px-6 py-5 flex flex-col md:flex-row items-center justify-between">
          <h1 className="text-4xl font-bold tracking-wide text-red-700">
            Vault PokéStop
          </h1>

          <nav className="flex gap-6 mt-4 md:mt-0 text-lg">
            <a href="#vault" className="hover:text-red-500 transition">
              In the Vault
            </a>
            <a href="#backstory" className="hover:text-red-500 transition">
              Backstory
            </a>
            <a href="#contact" className="hover:text-red-500 transition">
              Contact
            </a>
          </nav>
        </div>
      </header>

      {/* Hero Section */}
      <section className="relative py-28 px-6 text-center bg-gradient-to-b from-zinc-950 to-black">
        <div className="max-w-4xl mx-auto">
          <h2 className="text-5xl md:text-7xl font-extrabold text-red-700 mb-6">
            Welcome to the Vault
          </h2>

          <p className="text-xl text-zinc-300 leading-relaxed">
            Pokémon cards for real collectors. Built by a fan, not a scalper.
          </p>

          <div className="flex flex-col sm:flex-row justify-center gap-4 mt-10">
            <a
              href="#vault"
              className="bg-red-800 hover:bg-red-700 transition px-8 py-4 rounded-2xl text-lg font-semibold shadow-lg"
            >
              Explore the Vault
            </a>

            <a
              href="#backstory"
              className="border border-red-800 hover:bg-red-950 transition px-8 py-4 rounded-2xl text-lg font-semibold"
            >
              Read the Backstory
            </a>
          </div>
        </div>
      </section>

      {/* Shop Section */}
      <section id="vault" className="py-24 px-6 bg-zinc-950">
        <div className="max-w-7xl mx-auto">
          <div className="text-center mb-14">
            <h2 className="text-5xl font-bold text-red-700 mb-4">
              In the Vault
            </h2>
            <p className="text-zinc-400 text-lg">
              Find the cards and products you are looking for.
            </p>
          </div>

          <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
            {products.map((item, index) => (
              <div
                key={index}
                className="bg-black border border-red-900 rounded-3xl p-8 shadow-2xl hover:scale-105 transition duration-300"
              >
                <h3 className="text-3xl font-bold text-red-600 mb-4">
                  {item.title}
                </h3>

                <p className="text-zinc-300 leading-relaxed mb-6">
                  {item.description}
                </p>

                <button className="w-full bg-red-800 hover:bg-red-700 transition py-3 rounded-xl font-semibold">
                  View Collection
                </button>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Backstory Section */}
      <section id="backstory" className="py-24 px-6 bg-black">
        <div className="max-w-5xl mx-auto">
          <div className="bg-zinc-950 border border-red-900 rounded-3xl p-10 md:p-14 shadow-2xl">
            <h2 className="text-5xl font-bold text-red-700 mb-8 text-center">
              Backstory
            </h2>

            <div className="space-y-6 text-lg leading-relaxed text-zinc-300">
              <p>
                My name is Damien, and I started Vault PokéStop because I love Pokémon cards and collecting. I am 14 years old and wanted to build a place where collectors can buy cards without dealing with scalpers who overprice products and ruin the hobby for real fans.
              </p>

              <p>
                Scalping has become a huge issue in the Pokémon community. Many people buy large amounts of products just to resell them at much higher prices, making it harder for collectors and younger fans to enjoy the hobby.
              </p>

              <p>
                Here are a few websites and articles discussing Pokémon scalping and its impact on collectors:
              </p>

              <ul className="list-disc list-inside space-y-2 text-red-400">
                <li>
                  <a
                    href="https://www.polygon.com"
                    target="_blank"
                    rel="noreferrer"
                    className="hover:underline"
                  >
                    Polygon - Pokémon Card Scalping Articles
                  </a>
                </li>

                <li>
                  <a
                    href="https://www.ign.com"
                    target="_blank"
                    rel="noreferrer"
                    className="hover:underline"
                  >
                    IGN - Pokémon TCG Market News
                  </a>
                </li>

                <li>
                  <a
                    href="https://www.pokebeach.com"
                    target="_blank"
                    rel="noreferrer"
                    className="hover:underline"
                  >
                    PokéBeach - Pokémon TCG Community Updates
                  </a>
                </li>
              </ul>

              <p>
                Outside of Pokémon, I am also a huge metal fan. My favorite band is Slipknot, and I wanted the website theme to match that darker heavy-metal style with matte black and dark red colors.
              </p>

              <p>
                Vault PokéStop is built for collectors, players, and fans who genuinely enjoy the hobby.
              </p>
            </div>
          </div>
        </div>
      </section>

      {/* Contact Section */}
      <section id="contact" className="py-24 px-6 bg-zinc-950">
        <div className="max-w-4xl mx-auto text-center">
          <h2 className="text-5xl font-bold text-red-700 mb-8">
            Contact & Socials
          </h2>

          <div className="grid md:grid-cols-2 gap-8">
            <div className="bg-black border border-red-900 rounded-3xl p-10 shadow-xl">
              <h3 className="text-3xl font-bold mb-4 text-red-500">
                TikTok
              </h3>

              <p className="text-zinc-300 text-lg mb-6">
                Follow for card updates, openings, and new inventory.
              </p>

              <a
                href="https://www.tiktok.com/@vaultpokestop"
                target="_blank"
                rel="noreferrer"
                className="inline-block bg-red-800 hover:bg-red-700 transition px-6 py-3 rounded-xl font-semibold"
              >
                @vaultpokestop
              </a>
            </div>

            <div className="bg-black border border-red-900 rounded-3xl p-10 shadow-xl">
              <h3 className="text-3xl font-bold mb-4 text-red-500">
                Gmail
              </h3>

              <p className="text-zinc-300 text-lg mb-6">
                Reach out for questions, trades, or customer support.
              </p>

              <a
                href="mailto:damienlamberth401@gmail.com"
                className="inline-block bg-red-800 hover:bg-red-700 transition px-6 py-3 rounded-xl font-semibold"
              >
                Email Damien
              </a>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t border-red-950 bg-black py-8 text-center text-zinc-500">
        <p>
          © 2026 Vault PokéStop — Built for collectors, not scalpers.
        </p>
      </footer>
    </div>
  );
}

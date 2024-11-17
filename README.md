import Link from "next/link"
import Image from "next/image"
import { Sun, Heart, Briefcase, Moon, Plane, Mail } from 'lucide-react'

export default function Component() {
  return (
    <div className="min-h-screen bg-zinc-950 text-zinc-100">
      <header className="p-4">
        <h1 className="text-xl font-semibold">Francisco</h1>
      </header>
      <div className="relative h-[300px] w-full">
        <Image
          src="https://images.unsplash.com/photo-1533104816931-20fa691ff6ca?w=1200&h=300&fit=crop&crop=focalpoint&auto=format&q=80"
          alt="Mediterranean coastline with clear blue water and rocky shore"
          className="object-cover"
          fill
          priority
        />
      </div>
      <main className="mx-auto max-w-3xl px-4 py-16">
        <div className="space-y-12">
          <div className="space-y-4">
            <div className="flex items-center gap-2">
              <h2 className="text-4xl font-bold">Hi there, I&apos;m Francisco!</h2>
              <Sun className="h-8 w-8 text-yellow-400" aria-hidden="true" />
            </div>
            <p className="text-zinc-300">
              Right now, I&apos;m balancing my life in London, UK, where I moved almost five years ago from Mallorca, the Mediterranean paradise I still call home. 
            </p>
            <p className="text-zinc-300">
              As they say, &quot;When a man is tired of London, he is tired of life.&quot; I&apos;ve embraced the city&apos;s energy and diversity, and it&apos;s become the perfect place to grow both personally and professionally. <Heart className="inline h-5 w-5 text-red-500" />
            </p>
          </div>

          <div className="space-y-4">
            <h3 className="text-2xl font-semibold flex items-center gap-2">
              <Briefcase className="h-6 w-6" />
              What I Do
            </h3>
            <p className="text-zinc-300">
              By day, I&apos;m a Consultant at{" "}
              <Link href="https://www.synpulse.com" className="text-purple-400 hover:text-purple-300 underline underline-offset-4">
                Synpulse
              </Link>
              , helping FTSE 100 companies solve their most complex tech challenges. It&apos;s a role that keeps me curious, collaborative, and always learning.
            </p>
            <p className="text-zinc-300">
              By night (and sometimes day), I'm driving the evolution of{" "}
              <Link href="https://www.linkedin.com/company/opera-group-hospitality/?viewAsMember=true" className="text-purple-400 hover:text-purple-300 underline underline-offset-4">
                Opera Hospitality Group
              </Link>
              , modernizing our brand and sharpening our marketing strategy for our restaurants in Mallorca. I focus on:
            </p>
            <ul className="list-disc list-inside text-zinc-300 space-y-2 pl-4">
              <li>Enhancing paid media campaigns for greater reach.</li>
              <li>Improving online reviews and staying top-ranked on platforms like TripAdvisor.</li>
              <li>Collaborating with marketing providers to optimize communication across our portfolio.</li>
            </ul>
            <p className="text-zinc-300">
              And as a Venture Scout for{" "}
              <Link href="https://flashpoint.vc" className="text-purple-400 hover:text-purple-300 underline underline-offset-4">
                Flashpoint Ventures
              </Link>
              , I&apos;m always on the lookout for B2B SaaS founders with $1–5M in ARR and 2x+ growth. If that sounds like you, let&apos;s connect—I&apos;d love to hear your story!
            </p>
          </div>

          <div className="space-y-4">
            <h3 className="text-2xl font-semibold flex items-center gap-2">
              <Moon className="h-6 w-6" />
              In My Free Time
            </h3>
            <p className="text-zinc-300">When I&apos;m not working, you&apos;ll find me:</p>
            <ul className="list-disc list-inside text-zinc-300 space-y-2 pl-4">
              <li>Training Jiu-Jitsu—grappling my way to mindfulness.</li>
              <li>Exploring Startups—diving into the latest innovations and entrepreneurial trends.</li>
              <li>Traveling the World—collecting stamps in my passport and stories for a lifetime.</li>
            </ul>
          </div>

          <div className="space-y-4">
            <p className="text-zinc-300">
              Let&apos;s chat about scaling SaaS, hospitality innovations, or even share travel tips! Drop me a message—I&apos;m always up for a conversation.
            </p>
            <Link 
              href="mailto:fgostscagliarini@gmail.com" 
              className="inline-flex items-center px-4 py-2 bg-purple-600 text-white rounded hover:bg-purple-700 transition-colors"
            >
              <Mail className="mr-2 h-5 w-5" />
              Get in Touch
            </Link>
          </div>
        </div>
      </main>
    </div>
  )
}

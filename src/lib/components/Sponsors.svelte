<script lang="ts">
  import { Linkedin, MapPin, Calendar } from 'lucide-svelte';

  const founders = [
    {
      name: 'Eric Thimba',
      role: 'CEO & Co-Founder',
      bio: 'Eric built East Africa\'s leading ticketing platform serving 8,000+ creators. His deep understanding of event economics and capital barriers positions him to revolutionize creative financing.',
      linkedin: 'https://linkedin.com/in/ericthimbagichuki/'
    },
    {
      name: 'George "Porgie" Gachui',
      role: 'Director & Co-Founder',
      bio: 'George co-built MOOKH\'s platform infrastructure processing $50M+ in creative revenues. His operational expertise in event-tech enables scalable, automated financing solutions for underserved creators.',
      linkedin: 'https://linkedin.com/in/georgegachui/'
    }
  ];

  const partners = [
    { name: 'Pata Flow', type: 'Financing Partner' },
    { name: 'Heva', type: 'Financing Partner' },
    { name: 'Sony Innovation Fund', type: 'Target Strategic Partner' }
  ];

  const coverage = [
    { country: 'Kenya', status: 'Active', description: 'ACEF financing currently available' },
    { country: 'Uganda', status: 'Platform Active', description: 'MOOKH platform operational, ACEF expanding' },
    { country: 'Rwanda', status: 'Platform Active', description: 'MOOKH platform operational, ACEF expanding' }
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-16 text-[#110F28]">About ACEF</h2>

  <!-- Mission Statement -->
  <div class="mb-20">
    <p class="text-2xl leading-relaxed text-[#110F28] font-normal max-w-4xl mb-8">
      We're on a mission to democratize access to creative financing across Africa, empowering youth-led enterprises and emerging talent who lack access to traditional financial systems.
    </p>
    <p class="text-base leading-relaxed text-gray-600 max-w-3xl">
      Since 2015, MOOKH has facilitated 8,000+ events and generated $50M+ in economic value for Africa's creative sectors. ACEF represents the next evolution—the world's first tokenized creative industry bond that combines blockchain technology with receivables-backed financing.
    </p>
  </div>

  <!-- Founders -->
  <div class="mb-20">
    <h3 class="text-xl font-medium text-[#110F28] mb-8">Meet the founders</h3>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
      {#each founders as founder}
        <div class="bg-white p-8 rounded-2xl border border-gray-100">
          <div class="flex items-start justify-between mb-6">
            <div>
              <h4 class="text-xl font-medium text-[#110F28] mb-1">{founder.name}</h4>
              <p class="text-sm text-gray-600">{founder.role}</p>
            </div>
            <a 
              href={founder.linkedin} 
              target="_blank" 
              rel="noopener noreferrer"
              class="w-10 h-10 rounded-full bg-gray-100 flex items-center justify-center hover:bg-gray-200 transition-colors"
            >
              <Linkedin size={18} class="text-gray-600" />
            </a>
          </div>
          <p class="text-sm text-gray-600 leading-relaxed">{founder.bio}</p>
        </div>
      {/each}
    </div>
  </div>

  <!-- Geographic Coverage -->
  <div class="mb-20">
    <h3 class="text-xl font-medium text-[#110F28] mb-8">Geographic coverage</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      {#each coverage as location}
        <div class="bg-gray-50 p-6 rounded-xl">
          <div class="flex items-center gap-2 mb-3">
            <MapPin size={18} class="text-[#110F28]" />
            <h4 class="text-lg font-medium text-[#110F28]">{location.country}</h4>
          </div>
          <div class="inline-block bg-green-100 text-green-700 text-xs font-medium px-3 py-1 rounded-full mb-3">
            {location.status}
          </div>
          <p class="text-sm text-gray-600">{location.description}</p>
        </div>
      {/each}
    </div>
  </div>

  <!-- Partners -->
  <div>
    <h3 class="text-xl font-medium text-[#110F28] mb-8">Our partners</h3>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      {#each partners as partner}
        <div class="bg-[#110F28] p-8 rounded-xl text-white flex flex-col justify-center items-center text-center min-h-[160px]">
          <h4 class="text-xl font-medium mb-2">{partner.name}</h4>
          <p class="text-sm text-white/70">{partner.type}</p>
        </div>
      {/each}
    </div>
  </div>
</section>

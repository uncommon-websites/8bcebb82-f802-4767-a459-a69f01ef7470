<script lang="ts">
  import { TrendingUp, Users, DollarSign, Globe } from 'lucide-svelte';
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-16 text-[#110F28]">Our impact</h2>

  <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-20">
    <!-- Stat 1 -->
    <div class="bg-white p-8 rounded-2xl border border-gray-100">
      <div class="w-12 h-12 rounded-full bg-[#110F28] flex items-center justify-center mb-6">
        <TrendingUp size={24} class="text-white" />
      </div>
      <h3 class="text-4xl font-medium text-[#110F28] mb-2">8,000+</h3>
      <p class="text-sm text-gray-600">Creative entrepreneurs served across East Africa</p>
    </div>

    <!-- Stat 2 -->
    <div class="bg-white p-8 rounded-2xl border border-gray-100">
      <div class="w-12 h-12 rounded-full bg-[#110F28] flex items-center justify-center mb-6">
        <Users size={24} class="text-white" />
      </div>
      <h3 class="text-4xl font-medium text-[#110F28] mb-2">10,000+</h3>
      <p class="text-sm text-gray-600">Emerging businesses impacted in Kenya and Uganda</p>
    </div>

    <!-- Stat 3 -->
    <div class="bg-white p-8 rounded-2xl border border-gray-100">
      <div class="w-12 h-12 rounded-full bg-[#110F28] flex items-center justify-center mb-6">
        <DollarSign size={24} class="text-white" />
      </div>
      <h3 class="text-4xl font-medium text-[#110F28] mb-2">$50M+</h3>
      <p class="text-sm text-gray-600">Economic value generated for Africa's creative sectors</p>
    </div>

    <!-- Stat 4 -->
    <div class="bg-white p-8 rounded-2xl border border-gray-100">
      <div class="w-12 h-12 rounded-full bg-[#110F28] flex items-center justify-center mb-6">
        <Globe size={24} class="text-white" />
      </div>
      <h3 class="text-4xl font-medium text-[#110F28] mb-2">$76B</h3>
      <p class="text-sm text-gray-600">African events market by 2028 at 6% annual growth</p>
    </div>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
    <!-- Left Content -->
    <div>
      <h3 class="text-2xl font-medium mb-6 text-[#110F28]">Democratizing access to creative financing</h3>
      <p class="text-base leading-relaxed text-gray-600 mb-6">
        Since 2015, we've been on a mission to empower Africa's creative economy. Through MOOKH's platform and ACEF's innovative financing, we're breaking down barriers that have kept talented event organizers from accessing the capital they need to grow.
      </p>
      <p class="text-base leading-relaxed text-gray-600 mb-6">
        Our receivables-backed financing model replaces traditional credit requirements with performance-based eligibility, opening doors for youth-led enterprises and emerging talent who lack access to conventional banking.
      </p>
      <div class="bg-gray-100 p-6 rounded-lg">
        <p class="text-sm font-medium text-[#110F28] mb-2">World's first achievement</p>
        <p class="text-sm text-gray-600">
          ACEF represents the world's first tokenized creative industry bond, positioning us as pioneers in combining blockchain technology with creative industry financing.
        </p>
      </div>
    </div>

    <!-- Right Content -->
    <div class="bg-[#110F28] rounded-2xl p-12 text-white flex flex-col justify-center">
      <blockquote class="text-xl leading-relaxed mb-6">
        "We're not just providing loans—we're building infrastructure that enables Africa's creative economy to thrive. Every event funded is a step toward economic empowerment for the next generation."
      </blockquote>
      <div class="flex items-center gap-4">
        <div class="w-12 h-12 rounded-full bg-white/10"></div>
        <div>
          <p class="font-medium">Eric Thimba</p>
          <p class="text-sm text-white/70">CEO & Co-Founder, ACEF</p>
        </div>
      </div>
    </div>
  </div>
</section>

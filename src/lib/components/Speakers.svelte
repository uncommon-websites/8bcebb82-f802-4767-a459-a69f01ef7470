<script lang="ts">
  import { TrendingUp, Lock, Zap, Award } from 'lucide-svelte';

  const benefits = [
    {
      icon: TrendingUp,
      title: '12% estimated APY',
      description: 'Attractive risk-adjusted returns backed by automated ticket sales receivables',
      color: 'green'
    },
    {
      icon: Lock,
      title: 'Secured by receivables',
      description: '100% collateralization through ticket sales with automatic repayment deduction',
      color: 'blue'
    },
    {
      icon: Zap,
      title: 'Tokenized access',
      description: "World's first tokenized creative industry bond enables fractional investment",
      color: 'purple'
    },
    {
      icon: Award,
      title: 'Social impact',
      description: 'Support youth-led enterprises and emerging African creative talent',
      color: 'orange'
    }
  ];

  const riskMitigation = [
    'Direct control of revenue stream through MOOKH platform',
    'Automatic deduction from ticket sales eliminates manual collection',
    '100% collateralization provides strong investor protection',
    '180-day grace period with multi-layered enforcement mechanisms',
    'Credit bureau reporting and legal action for defaults',
    'Platform suspension and industry blacklisting consequences'
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="for-investors">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-8 text-[#110F28]">For investors</h2>
  
  <p class="text-xl leading-relaxed text-gray-600 mb-16 max-w-3xl">
    Invest in Africa's creative economy through the world's first tokenized creative industry bond. Access attractive returns while supporting the next generation of African event organizers.
  </p>

  <!-- Benefits Grid -->
  <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-20">
    {#each benefits as benefit}
      <div class="bg-white p-8 rounded-2xl border border-gray-100 hover:shadow-md transition-shadow">
        <div class={[
          'w-12 h-12 rounded-full flex items-center justify-center mb-6',
          benefit.color === 'green' ? 'bg-green-100' : '',
          benefit.color === 'blue' ? 'bg-blue-100' : '',
          benefit.color === 'purple' ? 'bg-purple-100' : '',
          benefit.color === 'orange' ? 'bg-orange-100' : ''
        ]}>
          <svelte:component 
            this={benefit.icon} 
            size={24} 
            class={[
              benefit.color === 'green' ? 'text-green-600' : '',
              benefit.color === 'blue' ? 'text-blue-600' : '',
              benefit.color === 'purple' ? 'text-purple-600' : '',
              benefit.color === 'orange' ? 'text-orange-600' : ''
            ]} 
          />
        </div>
        <h3 class="text-xl font-medium text-[#110F28] mb-3">{benefit.title}</h3>
        <p class="text-sm text-gray-600 leading-relaxed">{benefit.description}</p>
      </div>
    {/each}
  </div>

  <!-- Two Column Layout -->
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
    <!-- Left: Risk Mitigation -->
    <div>
      <h3 class="text-2xl font-medium text-[#110F28] mb-6">Built-in risk management</h3>
      <p class="text-base text-gray-600 mb-6 leading-relaxed">
        Our unique model provides multiple layers of investor protection through automated systems and enforcement mechanisms.
      </p>
      <ul class="space-y-4">
        {#each riskMitigation as item}
          <li class="text-sm text-gray-600 flex items-start gap-3">
            <div class="w-1.5 h-1.5 rounded-full bg-[#110F28] mt-2 flex-shrink-0"></div>
            <span>{item}</span>
          </li>
        {/each}
      </ul>
    </div>

    <!-- Right: Market Opportunity -->
    <div class="bg-[#110F28] rounded-2xl p-10 text-white">
      <h3 class="text-2xl font-medium mb-6">Market opportunity</h3>
      <div class="space-y-8">
        <div>
          <p class="text-4xl font-medium mb-2">$76B</p>
          <p class="text-sm text-white/70">African events market by 2028</p>
        </div>
        <div>
          <p class="text-4xl font-medium mb-2">6%</p>
          <p class="text-sm text-white/70">Year-over-year growth rate</p>
        </div>
        <div>
          <p class="text-4xl font-medium mb-2">Thousands</p>
          <p class="text-sm text-white/70">Underserved organizers lacking capital access</p>
        </div>
      </div>
      <div class="mt-10 pt-8 border-t border-white/10">
        <p class="text-sm text-white/70 mb-4">
          ACEF captures this massive opportunity through automated, scalable receivables financing backed by MOOKH's proven platform.
        </p>
        <a href="#apply" class="inline-block bg-white text-[#110F28] text-sm font-medium px-8 py-3 rounded-full hover:bg-gray-100 transition-colors">
          Invest with us
        </a>
      </div>
    </div>
  </div>
</section>

<script lang="ts">
  import { FileText, CheckCircle, Banknote, RotateCcw } from 'lucide-svelte';

  const organizerSteps = [
    {
      icon: FileText,
      number: '01',
      title: 'Apply for funding',
      description: 'Submit your application with event details and track record. Currently 15 days to approval, targeting 3 days through automation.',
      details: ['Event information', 'Historical performance', 'MOOKH platform integration', 'Business documentation']
    },
    {
      icon: CheckCircle,
      number: '02',
      title: 'Get approved',
      description: 'Performance-based eligibility assessment replaces traditional credit checks. Your event success is what matters.',
      details: ['Track record review', 'Loan amount determination', 'Terms agreement', 'Data sharing consent']
    },
    {
      icon: Banknote,
      number: '03',
      title: 'Receive capital',
      description: 'Funds disbursed directly to your account. Use the capital to create an unforgettable event experience.',
      details: ['Immediate disbursement', 'KES 100K - 5M range', '9% annual interest', 'Up to 12 months term']
    },
    {
      icon: RotateCcw,
      number: '04',
      title: 'Automatic repayment',
      description: 'Seamless deduction from ticket sales through MOOKH platform. No manual payments or collection hassles.',
      details: ['Auto-deduction from sales', 'Real-time tracking', '180-day grace period', 'Transparent reporting']
    }
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="how-it-works">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-16 text-[#110F28]">How it works</h2>

  <div class="mb-20">
    <p class="text-xl leading-relaxed text-gray-600 max-w-3xl mb-4">
      Our streamlined process gets capital into the hands of event organizers quickly, with automated repayment through ticket sales.
    </p>
  </div>

  <!-- Steps -->
  <div class="space-y-8">
    {#each organizerSteps as step, index}
      <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 pb-8 border-b border-gray-200 last:border-b-0">
        <!-- Left: Number and Icon -->
        <div class="lg:col-span-2 flex lg:flex-col items-start gap-4">
          <div class="text-5xl font-medium text-gray-200">{step.number}</div>
          <div class="w-12 h-12 rounded-full bg-[#110F28] flex items-center justify-center lg:mt-4">
            <svelte:component this={step.icon} size={24} class="text-white" />
          </div>
        </div>

        <!-- Middle: Content -->
        <div class="lg:col-span-6">
          <h3 class="text-2xl font-medium text-[#110F28] mb-4">{step.title}</h3>
          <p class="text-base text-gray-600 leading-relaxed mb-6">{step.description}</p>
          <ul class="grid grid-cols-2 gap-3">
            {#each step.details as detail}
              <li class="text-sm text-gray-600 flex items-center gap-2">
                <div class="w-1 h-1 rounded-full bg-[#110F28]"></div>
                {detail}
              </li>
            {/each}
          </ul>
        </div>

        <!-- Right: Visual Element -->
        <div class="lg:col-span-4 bg-gradient-to-br from-gray-50 to-gray-100 rounded-2xl p-8 flex items-center justify-center min-h-[200px]">
          <div class="text-center">
            <div class="w-16 h-16 rounded-full bg-white shadow-sm flex items-center justify-center mx-auto mb-4">
              <svelte:component this={step.icon} size={32} class="text-[#110F28]" />
            </div>
            <p class="text-xs font-medium text-gray-500">Step {index + 1} of 4</p>
          </div>
        </div>
      </div>
    {/each}
  </div>

  <!-- CTA -->
  <div class="mt-16 bg-[#110F28] rounded-2xl p-12 text-center text-white">
    <h3 class="text-3xl font-medium mb-4">Ready to fund your next event?</h3>
    <p class="text-lg text-white/80 mb-8 max-w-2xl mx-auto">
      Join 8,000+ creative entrepreneurs who have accessed capital through our platform.
    </p>
    <a href="#apply" class="inline-block bg-white text-[#110F28] text-sm font-medium px-10 py-4 rounded-full hover:bg-gray-100 transition-colors">
      Start your application
    </a>
  </div>
</section>

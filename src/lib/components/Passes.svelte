<script lang="ts">
  import { Check, Clock, Percent, Shield } from 'lucide-svelte';
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="for-organizers">
  <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium mb-16 text-[#110F28]">For event organizers</h2>

  <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
    <!-- Main Content -->
    <div class="lg:col-span-8">
      <p class="text-xl leading-relaxed text-gray-600 mb-12">
        Get the upfront capital you need to create unforgettable events. Our receivables-backed loans are secured by your ticket sales, with automatic repayment through MOOKH's platform.
      </p>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6 mb-12">
        <!-- Benefit 1 -->
        <div class="bg-white p-6 rounded-2xl border border-gray-100">
          <div class="w-10 h-10 rounded-full bg-green-100 flex items-center justify-center mb-4">
            <Percent size={20} class="text-green-600" />
          </div>
          <h3 class="text-lg font-medium text-[#110F28] mb-2">40-60% lower rates</h3>
          <p class="text-sm text-gray-600">
            9% per annum interest rate versus 15-25% from traditional banks. Save thousands on financing costs.
          </p>
        </div>

        <!-- Benefit 2 -->
        <div class="bg-white p-6 rounded-2xl border border-gray-100">
          <div class="w-10 h-10 rounded-full bg-blue-100 flex items-center justify-center mb-4">
            <Clock size={20} class="text-blue-600" />
          </div>
          <h3 class="text-lg font-medium text-[#110F28] mb-2">Fast approval</h3>
          <p class="text-sm text-gray-600">
            Currently 15 days from application to disbursement, targeting 3 days through automation.
          </p>
        </div>

        <!-- Benefit 3 -->
        <div class="bg-white p-6 rounded-2xl border border-gray-100">
          <div class="w-10 h-10 rounded-full bg-purple-100 flex items-center justify-center mb-4">
            <Shield size={20} class="text-purple-600" />
          </div>
          <h3 class="text-lg font-medium text-[#110F28] mb-2">No traditional collateral</h3>
          <p class="text-sm text-gray-600">
            Performance-based eligibility replaces credit scores. Your event track record is what matters.
          </p>
        </div>

        <!-- Benefit 4 -->
        <div class="bg-white p-6 rounded-2xl border border-gray-100">
          <div class="w-10 h-10 rounded-full bg-orange-100 flex items-center justify-center mb-4">
            <Check size={20} class="text-orange-600" />
          </div>
          <h3 class="text-lg font-medium text-[#110F28] mb-2">Automated repayment</h3>
          <p class="text-sm text-gray-600">
            Seamless deduction from ticket sales through MOOKH platform. No manual payments needed.
          </p>
        </div>
      </div>

      <!-- Loan Details -->
      <div class="bg-gray-50 p-8 rounded-2xl">
        <h3 class="text-lg font-medium text-[#110F28] mb-6">Loan details</h3>
        <div class="grid grid-cols-2 gap-6">
          <div>
            <p class="text-xs text-gray-500 mb-1">Loan range</p>
            <p class="text-base font-medium text-[#110F28]">KES 100,000 - 5,000,000</p>
            <p class="text-xs text-gray-500 mt-1">($1,000 - $50,000 USD)</p>
          </div>
          <div>
            <p class="text-xs text-gray-500 mb-1">Average loan</p>
            <p class="text-base font-medium text-[#110F28]">$10,000 USD</p>
          </div>
          <div>
            <p class="text-xs text-gray-500 mb-1">Interest rate</p>
            <p class="text-base font-medium text-[#110F28]">9% per annum</p>
          </div>
          <div>
            <p class="text-xs text-gray-500 mb-1">Repayment period</p>
            <p class="text-base font-medium text-[#110F28]">Up to 12 months</p>
          </div>
        </div>
      </div>
    </div>

    <!-- Eligibility Sidebar -->
    <div class="lg:col-span-4 pl-0 lg:pl-12 pt-4">
      <h3 class="text-sm font-medium text-[#110F28] mb-6">Eligibility requirements</h3>
      <ul class="space-y-4 mb-8">
        {#each [
          'Active event organizer in Kenya',
          'Track record of successful events',
          'Use MOOKH ticketing platform',
          'Consent to data sharing',
          'Valid business documentation'
        ] as item}
          <li class="text-sm text-gray-600 flex items-start gap-3">
            <Check size={16} class="text-green-600 mt-0.5 flex-shrink-0" />
            <span>{item}</span>
          </li>
        {/each}
      </ul>

      <a href="#apply" class="block w-full bg-[#110F28] text-white py-3 rounded-full text-sm font-medium hover:bg-opacity-90 transition-opacity text-center">
        Apply for funding
      </a>
    </div>
  </div>
</section>

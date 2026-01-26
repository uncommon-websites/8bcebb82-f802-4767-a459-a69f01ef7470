<script lang="ts">
  import { Plus } from 'lucide-svelte';

  const organizerFaqs = [
    "What are the eligibility requirements for ACEF financing?",
    "How long does the application process take?",
    "What loan amounts are available?",
    "What happens if my event doesn't sell enough tickets?",
    "Do I need collateral or a credit score?",
    "What are the interest rates and fees?",
    "Can I get financing for multiple events?",
    "What happens if I need to cancel my event?"
  ];

  const investorFaqs = [
    "What returns can I expect from investing in ACEF?",
    "How is my investment secured?",
    "What is tokenization and how does it work?",
    "What are the risks involved?",
    "How do I start investing with ACEF?",
    "Can I invest from outside Africa?",
    "What is the minimum investment amount?",
    "How liquid is my investment?"
  ];
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto border-t border-gray-200" id="faq">
  <div class="grid grid-cols-1 lg:grid-cols-12 gap-12">
    <div class="lg:col-span-4">
      <h2 class="text-[clamp(2.5rem,5vw,4rem)] leading-none font-medium text-[#110F28]">FAQs</h2>
    </div>

    <div class="lg:col-span-8 space-y-12">
      <!-- Organizer FAQs -->
      <div>
        <h3 class="text-lg font-medium text-[#110F28] mb-6">For event organizers</h3>
        <div class="border-t border-gray-200">
          {#each organizerFaqs as question}
            <div class="py-5 border-b border-gray-200 flex justify-between items-center cursor-pointer group hover:bg-gray-50 transition-colors px-2 -mx-2 rounded-sm">
              <h4 class="text-sm font-medium text-[#110F28] pr-8">{question}</h4>
              <div class="text-gray-400 group-hover:text-[#110F28] transition-colors">
                <Plus size={16} />
              </div>
            </div>
          {/each}
        </div>
      </div>

      <!-- Investor FAQs -->
      <div>
        <h3 class="text-lg font-medium text-[#110F28] mb-6">For investors</h3>
        <div class="border-t border-gray-200">
          {#each investorFaqs as question}
            <div class="py-5 border-b border-gray-200 flex justify-between items-center cursor-pointer group hover:bg-gray-50 transition-colors px-2 -mx-2 rounded-sm">
              <h4 class="text-sm font-medium text-[#110F28] pr-8">{question}</h4>
              <div class="text-gray-400 group-hover:text-[#110F28] transition-colors">
                <Plus size={16} />
              </div>
            </div>
          {/each}
        </div>
      </div>

      <!-- Contact -->
      <div class="bg-gray-50 p-8 rounded-2xl">
        <h3 class="text-lg font-medium text-[#110F28] mb-3">Still have questions?</h3>
        <p class="text-sm text-gray-600 mb-6">
          Our team is here to help. Reach out and we'll get back to you as soon as possible.
        </p>
        <a href="mailto:info@acef.africa" class="inline-block bg-[#110F28] text-white text-sm font-medium px-8 py-3 rounded-full hover:bg-opacity-90 transition-opacity">
          Contact us
        </a>
      </div>
    </div>
  </div>
</section>

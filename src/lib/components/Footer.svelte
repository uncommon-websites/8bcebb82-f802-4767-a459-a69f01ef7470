<script lang="ts">
  import { Linkedin, Mail, MapPin } from 'lucide-svelte';
</script>

<footer class="bg-[#110F28] text-white pt-20 pb-12 px-6" id="apply">
  <div class="max-w-[1400px] mx-auto">
    
    <!-- Top Section -->
    <div class="flex flex-col md:flex-row justify-between items-start mb-24">
      <div class="flex items-center gap-2 mb-8 md:mb-0">
        <span class="font-bold text-2xl tracking-tight">ACEF</span>
      </div>

      <div class="flex flex-col md:flex-row gap-8 md:gap-32 text-sm font-medium text-white/80">
        <div>
          <p>World's first</p>
          <p>tokenized creative bond</p>
        </div>
        <div>
          <p>Kenya, Uganda,</p>
          <p>and Rwanda</p>
        </div>
      </div>
    </div>

    <!-- Big Title -->
    <h2 class="text-[clamp(2.5rem,6vw,5rem)] leading-[0.95] tracking-tight font-medium max-w-5xl mb-12">
      Fueling Africa's new generation of creators
    </h2>

    <!-- CTA Buttons -->
    <div class="mb-32 flex flex-col sm:flex-row gap-4">
      <button class="bg-white text-[#110F28] text-sm font-medium px-12 py-4 rounded-full hover:bg-opacity-90 transition-opacity">
        Apply for funding
      </button>
      <button class="bg-white/10 backdrop-blur-sm text-white text-sm font-medium px-12 py-4 rounded-full hover:bg-white/20 transition-colors border border-white/20">
        Invest with us
      </button>
    </div>

    <!-- Contact & Links Section -->
    <div class="grid grid-cols-1 md:grid-cols-3 gap-12 mb-16 border-t border-white/10 pt-12">
      <!-- Contact -->
      <div>
        <h3 class="text-sm font-medium text-white mb-4">Contact</h3>
        <div class="space-y-3">
          <a href="mailto:info@acef.africa" class="flex items-center gap-2 text-sm text-white/70 hover:text-white transition-colors">
            <Mail size={16} />
            info@acef.africa
          </a>
          <div class="flex items-start gap-2 text-sm text-white/70">
            <MapPin size={16} class="mt-0.5" />
            <span>Nairobi, Kenya</span>
          </div>
        </div>
      </div>

      <!-- Quick Links -->
      <div>
        <h3 class="text-sm font-medium text-white mb-4">Quick links</h3>
        <div class="space-y-3">
          <a href="#how-it-works" class="block text-sm text-white/70 hover:text-white transition-colors">How it works</a>
          <a href="#for-organizers" class="block text-sm text-white/70 hover:text-white transition-colors">For organizers</a>
          <a href="#for-investors" class="block text-sm text-white/70 hover:text-white transition-colors">For investors</a>
          <a href="#faq" class="block text-sm text-white/70 hover:text-white transition-colors">FAQ</a>
        </div>
      </div>

      <!-- Connect -->
      <div>
        <h3 class="text-sm font-medium text-white mb-4">Connect with founders</h3>
        <div class="space-y-3">
          <a 
            href="https://linkedin.com/in/ericthimbagichuki/" 
            target="_blank" 
            rel="noopener noreferrer"
            class="flex items-center gap-2 text-sm text-white/70 hover:text-white transition-colors"
          >
            <Linkedin size={16} />
            Eric Thimba
          </a>
          <a 
            href="https://linkedin.com/in/georgegachui/" 
            target="_blank" 
            rel="noopener noreferrer"
            class="flex items-center gap-2 text-sm text-white/70 hover:text-white transition-colors"
          >
            <Linkedin size={16} />
            George Gachui
          </a>
        </div>
      </div>
    </div>

    <!-- Bottom Legal -->
    <div class="flex flex-col md:flex-row justify-between items-center border-t border-white/10 pt-8 text-xs text-white/60">
      <p>© 2024 ACEF. All rights reserved.</p>
      <div class="flex flex-wrap gap-6 mt-4 md:mt-0">
        <a href="/" class="hover:text-white transition-colors">Privacy Policy</a>
        <a href="/" class="hover:text-white transition-colors">Terms of Service</a>
        <a href="/" class="hover:text-white transition-colors">Financing Agreement</a>
      </div>
    </div>

  </div>
</footer>

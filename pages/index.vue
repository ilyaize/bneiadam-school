<template>
  <div class="mx-auto px-4">
    <!-- Hero Section -->
    <div class="hero pt-5">
      <section class="">
        <div class="max-w-xl text-center">
          <h1 class="text-5xl font-bold tracking-wider text-yellow-50">
            {{ $t('home_title') }}
          </h1>
          <h2 class="text-1xl mb-5 text-yellow-300">{{ $t('home_tag') }}</h2>
          <img class="video-image mb-6 mt-6 rounded-3xl" src="/assets/image.jpg" />
          <section class="blurred-bg rounded-3xl">
            <p class="mb-5 text-yellow-50">
              {{ $t('home_p1.1') }}
              <!-- TODO: keep one-liner -->
              <span class="font-bold text-yellow-300">{{ $t('home_p1.2') }}</span>
              <span class="text-yellow-50">{{ $t('home_p1.3') }}</span>
            </p>

            <a href="tel:+972555694652" class="btn btn-lg btn-wide mx-4 border-0 bg-yellow-500 text-xl font-bold text-black hover:bg-yellow-400">
              {{ $t('home_btn') }}
            </a>
            <div class="flex flex-wrap justify-center gap-10">
              <div class="mt-10 flex justify-center">
                <a href="#" class="px-5 text-gray-400 hover:text-gray-300">
                  <span class="sr-only"></span>
                  <i class="fa-brands fa-whatsapp fa-lg"></i>
                </a>
                <a href="#" class="px-5 text-gray-400 hover:text-gray-300">
                  <span class="sr-only"></span>
                  <i class="fa-brands fa-facebook fa-lg"></i>
                </a>
                <a href="#" class="px-5 text-gray-400 hover:text-gray-300">
                  <span class="sr-only"></span>
                  <i class="fa-brands fa-youtube fa-lg"></i>
                </a>
              </div>
            </div>
          </section>
        </div>
      </section>
    </div>
    <div class="py-20 text-yellow-50">
      <div class="container mx-auto px-6 md:px-12 xl:px-32">
        <div class="mb-16 text-center">
          <h2 class="mb-4 text-center text-2xl font-bold md:text-4xl">{{ $t('team_title') }}</h2>
          <p class="lg:mx-auto lg:w-8/12">{{ $t('team_p1') }}</p>
        </div>
        <div class="grid items-center gap-12 md:grid-cols-3">
          <div class="space-y-4 text-center">
            <img class="mx-auto h-64 w-64 rounded-xl object-cover md:h-40 md:w-40 lg:h-64 lg:w-64" src="../assets/ilya.jpg" alt="woman" loading="lazy" width="640" height="805" />
            <div>
              <h4 class="text-2xl">{{ $t('team_c1.1') }}</h4>
              <span class="block text-sm">{{ $t('team_c1.2') }}</span>
            </div>
          </div>
          <div class="space-y-4 text-center">
            <img class="mx-auto h-64 w-64 rounded-xl object-cover md:h-64 md:w-48 lg:h-80 lg:w-64" src="../assets/michael.jpg" alt="Michael Amar" loading="lazy" width="1000" height="667" />
            <div>
              <h4 class="text-2xl">{{ $t('team_c2.1') }}</h4>
              <span class="block text-sm">{{ $t('team_c2.2') }}</span>
            </div>
          </div>
          <div class="space-y-4 text-center">
            <img class="mx-auto h-64 w-64 rounded-xl object-cover md:h-40 md:w-40 lg:h-64 lg:w-64" src="https://tailus.io/sources/blocks/classic/preview/images/woman1.jpg" alt="woman" loading="lazy" width="1000" height="667" />
            <div>
              <h4 class="text-2xl">{{ $t('team_c3.1') }}</h4>
              <span class="block text-sm">{{ $t('team_c3.2') }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- About Me Section -->
    <section id="about" class="text-yellow-50">
      <div class="text-center">
        <h2 class="mb-2 text-4xl font-bold">
          {{ $t('about_title') }}
        </h2>
        <p class="relative mb-4 px-3 py-1 text-xs leading-6">
          {{ $t('about_tag') }}
        </p>
      </div>
      <div class="flex flex-wrap justify-center">
        <div class="max-w-lg">
          <p>{{ $t('about_p1') }}</p>
          <p class="pt-5">{{ $t('about_p2') }}</p>
        </div>
      </div>
    </section>
  </div>

  <!-- Feature section -->
  <div class="mt-16 text-yellow-50 sm:mt-28">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-3xl sm:text-center">
        <p class="mt-2 text-3xl font-bold tracking-tight sm:text-4xl">Dive deeper into our unique approach:</p>
        <p class="mt-6 text-lg leading-8 text-yellow-50">In our practice, we believe that the mind and body are intricately connected and that true healing requires addressing both. This is why we've chosen to integrate the power of psychology and osteopathy to treat the whole person, not just their symptoms.</p>
      </div>
    </div>
    <div class="relative overflow-hidden pt-16">
      <!-- <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <img src="../assets/osteopathy.webp" alt="App screenshot" class="mb-[-12%] rounded-xl shadow-2xl ring-1 ring-gray-900/10" width="2432" height="1442" />
        <div class="relative" aria-hidden="true">
          <div class="absolute -inset-x-20 bottom-0 bg-gradient-to-t from-white pt-[7%]" />
        </div>
      </div> -->
    </div>
    <div class="mx-auto mt-16 max-w-7xl px-6 sm:mt-20 md:mt-24 lg:px-8">
      <dl class="mx-auto grid max-w-2xl grid-cols-1 gap-x-6 gap-y-10 text-base leading-7 text-gray-600 sm:grid-cols-2 lg:mx-0 lg:max-w-none lg:grid-cols-3 lg:gap-x-8 lg:gap-y-16">
        <div class="">
          <dt class="inline font-semibold text-yellow-50">Psychological factors manifest in physical ways:&nbsp;</dt>
          <dd class="inline text-yellow-50">Stress, anxiety, and trauma can create tension in muscles, affect posture, and contribute to pain. For example, chronic stress can manifest as headaches, back pain, or digestive issues.</dd>
        </div>
        <div class="">
          <dt class="inline font-semibold text-yellow-50">Physical discomfort impacts mental well-being:&nbsp;</dt>
          <dd class="inline text-yellow-50">Chronic pain, discomfort, and limitations in mobility can lead to depression, anxiety, and decreased self-esteem. The cycle can go both ways, making it crucial to address both aspects.</dd>
        </div>
        <div class="">
          <dt class="inline font-semibold text-yellow-50">Osteopathic treatment promotes emotional well-being:&nbsp;</dt>
          <dd class="inline text-yellow-50">By releasing physical tension, improving circulation, and restoring balance to the musculoskeletal system, osteopathy can create a sense of calm and relaxation, impacting the nervous system and reducing stress.</dd>
        </div>
        <div class="">
          <dt class="inline font-semibold text-yellow-50">Psychological tools can enhance osteopathic treatment:&nbsp;</dt>
          <dd class="inline text-yellow-50">Techniques like mindfulness, stress management, and cognitive-behavioral therapy can help patients become more aware of their body's sensations and work with the osteopath to optimize treatment outcomes.</dd>
        </div>
        <div class="">
          <dt class="inline font-semibold text-yellow-50">Your osteopath and psychologist work together:&nbsp;</dt>
          <dd class="inline text-yellow-50">They share information, create a personalized treatment plan, and adjust it based on your progress.</dd>
        </div>
        <div class="">
          <dt class="inline font-semibold text-yellow-50">You, the patient, are an active participant:&nbsp;</dt>
          <dd class="inline text-yellow-50">You'll learn about the mind-body connection and be equipped with tools to manage your physical and emotional health.</dd>
        </div>
      </dl>
    </div>
    <div class="mx-auto max-w-2xl py-8 sm:py-12 lg:py-14">
      <div class="text-center">
        <p class="mt-2 text-3xl font-bold tracking-tight text-yellow-50 sm:text-4xl">In summary,</p>
        <p class="mt-6 text-lg leading-8 text-yellow-50">by combining the strengths of osteopathy and psychology, we offer a more holistic and effective approach to wellness. We address the root causes of your symptoms, improve your physical and emotional well-being, and empower you to live a healthier, happier life.</p>
      </div>
    </div>
  </div>

  <!-- Coming Soon Section -->
  <section id="coming_soon" class="">
    <div class="text-center">
      <h2 class="mt-20 text-4xl font-bold text-yellow-50">{{ $t('coming_soon') }}</h2>
    </div>
  </section>
</template>

<style scoped>
.video-image {
  transition: filter 0.3s ease;
}

.video-image:hover {
  filter: brightness(1.2);
}

.blurred-bg {
  background-color: rgba(0, 0, 0, 0.3);
  -webkit-backdrop-filter: blur(5px);
  backdrop-filter: blur(5px);
  padding: 50px;
}
</style>

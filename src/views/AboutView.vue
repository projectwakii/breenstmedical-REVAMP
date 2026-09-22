<!--
  This example requires Tailwind CSS v2.0+ 
  
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/aspect-ratio'),
    ],
  }
  ```
-->
<template>
  <div class="bg-white">
    <div class="mx-auto py-12 px-4 max-w-7xl sm:px-6 lg:px-8 lg:py-24">
      <div class="space-y-12 lg:grid lg:grid-cols-3 lg:gap-8 lg:space-y-0">
        <div class="space-y-5 sm:space-y-4">
          <h2 class="text-3xl font-extrabold tracking-tight sm:text-4xl">Our Team</h2>
          <p class="text-xl text-gray-500">Meet our friendly and experienced General Practitioners, Nurses, and Allied Health staff. Here you'll also find a list of special areas of interest.</p>
        </div>
        <div class="lg:col-span-2">
          <ul role="list" class="space-y-12 sm:grid sm:grid-cols-2 sm:gap-x-6 sm:gap-y-12 sm:space-y-0 lg:gap-x-8">
            <li v-for="person in people" :key="person.name">
              <div class="space-y-4">
                <div v-if="person.imageUrl" class="aspect-w-3 aspect-h-5">
                  <img class="object-cover shadow-lg rounded-lg" :src="person.imageUrl" alt="" />
                </div>
                <div class="text-lg leading-6 font-medium space-y-1">
                  <h3>{{ person.name }}</h3>
                  <p class="text-indigo-600">{{ person.role }}</p>
                </div>
                <div class="text-lg space-y-4">
                  <p v-for="(paragraph, index) in person.bio.split('\n\n')" :key="index" class="text-gray-500">{{ paragraph }}</p>
                </div>

              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const people = [
  {
    name: 'Dr Hariom Thaker (Harry)',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drhariom.JPG',
    bio: 'Dr Hariom Thaker (Dr Harry) is a full-time General Practitioner who relocated from Melton to Bendigo. He enjoys all areas of general practice, and his special interests are Preventative medicine & Weight management, Chronic disease management, Children\'s Health, Men\'s Health and Sexual Health. Dr Harry is multi-lingual and is fluent in Gujarati and Hindi.',
    twitterUrl: '#',
    linkedinUrl: '#',
  },

{
    name: 'Dr. Piraneetha Hall',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drpiraneetha.jpg',
    bio: 'Dr Piranee Hall grew up in Sydney before completing her medical training at the University ofNewcastle in NSW. Since the completion of her training she has worked at The Austin Hospital, The Royal Children\'s Hospital in Melbourne as well as at the Royal Darwin Hospital in the Northern Territory. Her GP training was completed in Brisbane, Queensland becoming a fellow of the Royal Australian College of General Practitioners. Dr Hall has an interest in paediatrics and women\'s health, having completed her Diploma of Obstetrics and Gynaecology. Men\'s health has become an area she is familiar with through the work of her husband, Mr Rohan Hall, who is a local Urological surgeon. When not at work, Piranee is kept busy looking after her two young children.',
    twitterUrl: '#',
    linkedinUrl: '#',
  },

    {
    name: 'Dr Rosamund Stobie',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drrosamund.jpg',
    bio: 'Rosamund Stobie is a female General Practitioner. She graduated from Monash University, and is a fellow of the RACGP and Skin cancer College Australasia. She has completed her Diploma of Obstetrics and Gynaecology.\nShe is caring, competent and thorough.\nSpecial interests- Women\'s Health, Skin Cancer,Antenatal , Contraception and Implanon, Children\'s Health, Men\'s Health, Chronic Disease, Preventative Health, Mental Health',
    twitterUrl: '#',
    linkedinUrl: '#',
  },

  {
    name: 'Dr. Mina Kouhzad',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drmina.jpg',
    bio: 'I am a caring and compassionate doctor who takes pride in being a good listener and trying to share as much medical information as practical to my patients, giving them the opportunity to take part in their treatment.',
    twitterUrl: '#',
    linkedinUrl: '#',
  },
  {
    name: 'Dr Muhammad Ilyas Shazi',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drshazi.jpg',
    bio: 'Dr Shazi is an experienced GP with over 22 years of international practice, including 8 years in Pakistan and 14 years in Saudi Arabia. He holds MRCGP INT (UK) and MCPS (Family Medicine) qualifications. His special interests include chronic disease management, geriatrics, mental health, and paediatrics, with a keen interest in exploring all areas of general practice.\n\nDr Shazi is fluent in multiple languages including English, Urdu, Hindi, Punjabi and Arabic(Saudi).',
    twitterUrl: '#',
    linkedinUrl: '#',
  },
  {
    name: 'Dr Sethunge Manoj Sethunge',
    role: 'General Practitioner (GP)',
    imageUrl:
      '/img/drsethunge.jpg',
    bio: 'Dr Sethunge is a dedicated General Practitioner committed to providing comprehensive, patient-centered care. He enjoys all areas of general practice, with special interests in preventative medicine, chronic disease management, and family health. Dr Sethunge takes the time to listen to his patients and works collaboratively with them to achieve the best health outcomes.',
    twitterUrl: '#',
    linkedinUrl: '#',
  },
  {
    name: 'Dr. Shaheen',
    role: 'General Practitioner (GP)',
    imageUrl: '/img/drshaheen.png',
    bio: `Dr. Shaheen obtained her MBBS in 2008 and has built a people-focused medical career shaped by diverse clinical experiences across Malaysia, Borneo, Australia, and clinical observerships in the United Kingdom. Her international background has helped her develop into an adaptable and culturally attuned clinician who connects easily with patients from all walks of life.

She has special interests in ENT, chronic disease management, paediatrics, mental health, and preventive medicine. Passionate about helping patients feel heard, understood, and empowered, she is undertaking further training with the Royal Australian College of General Practitioners (RACGP), reflecting her commitment to comprehensive, patient-centred and community-based care.

Known for her warm and approachable manner, Dr. Shaheen believes that good healthcare starts with good conversations. She takes the time to listen, explain, and work collaboratively with her patients to support their health and wellbeing. She places particular emphasis on prevention, early intervention, and caring for both physical and mental health.

Fluent in English, Malay, and Tamil, Dr. Shaheen enjoys bridging language and cultural gaps to make healthcare more accessible, personal, and less intimidating for her patients.

Outside of medicine, Dr. Shaheen enjoys spending quality time with her husband and their three cats. She has a love for travelling and discovering new places, as well as cooking and exploring different cuisines. She also enjoys expressing her creative side through art and music. These interests provide her with a balance between her professional life and the things she values most personally—creativity, connection, family, and lifelong learning.`,
  },
  // More people...
]

export default {
  setup() {
    return {
      people
    }
  }
}

</script>
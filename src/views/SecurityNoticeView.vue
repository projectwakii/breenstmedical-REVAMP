<template>
  <main class="bg-red-50">
    <section class="mx-auto max-w-4xl px-4 py-12 sm:px-6 lg:px-8 lg:py-16">
      <div class="overflow-hidden rounded-2xl border border-red-200 bg-white shadow-sm">
        <div class="border-b border-red-200 bg-red-700 px-6 py-5 sm:px-8">
          <div class="flex justify-center">
            <div class="flex h-16 w-16 items-center justify-center rounded-full bg-white/10 ring-1 ring-white/20">
              <svg
                class="h-10 w-10 text-white"
                viewBox="0 0 24 24"
                fill="none"
                stroke="currentColor"
                stroke-width="1.8"
                aria-hidden="true"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M10.29 3.86 1.82 18a2 2 0 0 0 1.72 3h16.92a2 2 0 0 0 1.72-3L13.71 3.86a2 2 0 0 0-3.42 0Z"
                />
                <path stroke-linecap="round" stroke-linejoin="round" d="M12 8.5v5.25" />
                <circle cx="12" cy="16.75" r="0.9" fill="currentColor" stroke="none" />
              </svg>
            </div>
          </div>

          <p class="mt-4 text-center text-sm font-semibold uppercase tracking-[0.2em] text-red-100">
            Security Notice
          </p>
          <h1 class="mt-2 text-center text-2xl font-extrabold text-white sm:text-3xl">
            Important Security Notice — 23 April 2026
          </h1>
        </div>

        <div class="space-y-6 px-6 py-8 text-base leading-7 text-gray-700 sm:px-8">
          <p>
            On 22 April 2026, Breen Street Medical Practice experienced a security
            incident involving our email system. An unauthorised email was sent to
            some patients with the subject line
            <strong>'Review And Acknowledge Medical Form'</strong>.
          </p>

          <p class="text-lg font-bold text-red-700">
            This email did NOT come from our practice.
          </p>

          <div>
            <h2 class="text-lg font-bold text-gray-900">If you received this email:</h2>
            <ul class="mt-3 list-disc space-y-2 pl-6 marker:text-red-700">
              <li><strong>Delete it immediately</strong></li>
              <li><strong>Do NOT click any links</strong> in the email</li>
              <li><strong>Do NOT open any attachments</strong></li>
              <li>
                <strong>Do NOT enter any personal information</strong> on any page
                it links to
              </li>
              <li><strong>Do NOT install any software</strong> it prompts you to</li>
            </ul>
          </div>

          <p>
            Our practice will never ask you to install software or provide remote
            access to your computer.
          </p>

          <div>
            <h2 class="text-lg font-bold text-gray-900">
              If you have already clicked the link, opened the attachment, or entered
              any information:
            </h2>
            <ol class="mt-3 list-decimal space-y-2 pl-6 marker:font-semibold marker:text-red-700">
              <li>
                <strong>Change any passwords</strong> you may have entered, as well
                as any other accounts using the same password
              </li>
              <li>
                <strong>Contact your bank</strong> immediately if you entered
                financial or credit card details
              </li>
              <li>
                <strong>Run an antivirus scan</strong> on your device if you
                downloaded or opened the attachment
              </li>
              <li>
                <strong>Monitor your accounts</strong> for any unusual activity over
                the coming weeks
              </li>
            </ol>
          </div>

          <p>
            We are investigating this incident thoroughly and taking steps to secure
            our systems. We sincerely apologise for any concern this has caused.
          </p>

          <p>
            If you have any questions or are unsure whether an email is genuine,
            please call us directly on <strong>(03) 5444 0689</strong>.
          </p>

          <div class="border-t border-gray-200 pt-6">
            <p>Kind regards,</p>
            <p class="mt-3 font-semibold text-gray-900">Administration Team</p>
            <p>Breen Street Medical Practice</p>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>

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
          <p>Dear patient,</p>

          <p>
            We are writing to inform you that we have reason to believe there has
            been a breach involving the email addresses of patients from our
            practice. As a result, you may have received a suspicious email from
            this address dated <strong>22 April</strong> with the subject line
            <strong>&ldquo;Review &amp; Acknowledge Medical Form&rdquo;</strong>.
          </p>

          <p class="text-lg font-bold text-red-700">
            This email was not sent by us.
          </p>

          <p>
            If you received it, please <strong>delete the email</strong>. Do not
            click any links, open any attachments, or provide any details in
            response.
          </p>

          <p>
            Based on our investigation so far, we have no evidence that any
            healthcare information has been accessed or taken. We will contact you
            again if this position changes.
          </p>

          <p>
            We have taken steps to secure our email accounts and are updating our
            broader security systems to reduce the risk of this occurring again.
          </p>

          <div class="rounded-lg border-l-4 border-indigo-600 bg-indigo-50 px-5 py-4">
            <p class="text-sm font-semibold uppercase tracking-wide text-indigo-700">
              Our new email address
            </p>
            <p class="mt-1 text-lg font-bold text-gray-900">
              admin@breenstmedical.com.au
            </p>
          </div>

          <p>
            We apologise for any inconvenience this may have caused.
          </p>

          <div class="border-t border-gray-200 pt-6">
            <p>Kind regards,</p>
            <p class="mt-3 font-semibold text-gray-900">Administration Team</p>
            <p>Breen St Medical Practice</p>
          </div>
        </div>
      </div>
    </section>
  </main>
</template>


<main class="text-white relative flex min-h-screen flex-col items-center justify-center">
  <h1
    class="pt-4 pb-8  text-white bg-clip-text text-center text-4xl font-medium tracking-tight text-transparent md:text-7xl"
  >
    Blob on Vercel
  </h1>
  <div
    class="flex flex-col items-center w-full max-w-xl p-12 mx-auto rounded-lg shadow-xl bg-slate-800 ring-1 ring-gray-900/5 backdrop-blur-lg"
  >
    <form
      class="grid gap-6 w-full "
      action="?/upload"
      method="POST"
      enctype="multipart/form-data"
    >
      <div>
        <div class="space-y-1 mb-4 ">
          <h2 class="text-xl font-semibold ">Upload a file</h2>
          <p class="text-sm text-gray-500">
            Accepted formats: .png, .jpg, .gif, .mp4
          </p>
        </div>
        <label
          for="image-upload"
          class=" group relative mt-2 flex h-72 cursor-pointer flex-col items-center justify-center rounded-md border border-gray-300 shadow-sm transition-all hover:bg-gray-900"
        >
          
            <div class="absolute z-[5] h-full w-full rounded-md bg-transparent">
              <div
                class={`${''} bg-transparent absolute z-[3] flex h-full w-full flex-col items-center justify-center rounded-md px-10 transition-all `}
              >
                <svg
                  class={`${'scale-100'} h-7 w-7 text-gray-500 transition-all duration-75 group-hover:scale-110 group-active:scale-95`}
                  xmlns="http://www.w3.org/2000/svg"
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  stroke="currentColor"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                >
                  <path
                    d="M4 14.899A7 7 0 1 1 15.71 8h1.79a4.5 4.5 0 0 1 2.5 8.242"
                  />
                  <path d="M12 12v9" />
                  <path d="m16 16-4-4-4 4" />
                </svg>
                <p class="mt-2 text-center text-sm text-gray-500">
                  Click to upload.
                </p>
                <p class="mt-2 text-center text-sm text-gray-500">
                  Max file size: 50MB
                </p>
                <span class="sr-only">Photo upload</span>
              </div>
            </div>

        </label>
        <div class="bg-transparent mt-1 flex rounded-md shadow-sm">
          <input
            id="image-upload"
            name="image-upload"
            type="file"
            accept="image/*"
            class="sr-only"
            
          />
        </div>
      </div>

      <button

        class="bg-transparent flex h-10 w-full items-center justify-center rounded-md border text-sm transition-all focus:outline-none"
      >
        <p class="text-sm">Confirm upload</p>
      </button>

    </form>
  </div>
 
</main>

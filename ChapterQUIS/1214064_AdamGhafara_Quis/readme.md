# Membuat Frontend
+++
Pada Quis ini, kita akan membuat tampilan frontend terlebih dahulu. Ini adalah Frontend form registrasi untuk Test API registrasi.
![image](https://github.com/adam-ghafara/WS/blob/main/ChapterQUIS/1214064_AdamGhafara_Quis/foto/Screenshot_2674.png?raw=true)
Codingannya:
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Punya Adam</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap">
    <link rel="stylesheet" href="css/tailwind/tailwind.min.css">
    <link rel="icon" type="image/png" sizes="32x32" href="shuffle-for-tailwind.png">
    <script src="js/main.js"></script>
    <script src="js/apihook.js"></script>
</head>
<body class="antialiased bg-body text-body font-body">
    <div class="">
                
      <section class="relative bg-white">
        <nav class="flex xl:hidden items-center justify-between py-3.5 px-7 bg-light">
          <div class="w-full xl:w-auto px-2 xl:mr-10">
            <div class="flex items-center justify-between"><a class="inline-flex items-center h-7" href="#"><img src="dashy-assets/logos/dashy-circle2-logo.svg" alt=""></a>
              <div class="xl:hidden">
                <button class="navbar-burger text-gray-400 hover:text-gray-300 focus:outline-none">
                  <svg width="20" height="12" viewbox="0 0 20 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 2H19C19.2652 2 19.5196 1.89464 19.7071 1.70711C19.8946 1.51957 20 1.26522 20 1C20 0.734784 19.8946 0.48043 19.7071 0.292893C19.5196 0.105357 19.2652 0 19 0H1C0.734784 0 0.48043 0.105357 0.292893 0.292893C0.105357 0.48043 0 0.734784 0 1C0 1.26522 0.105357 1.51957 0.292893 1.70711C0.48043 1.89464 0.734784 2 1 2ZM19 10H1C0.734784 10 0.48043 10.1054 0.292893 10.2929C0.105357 10.4804 0 10.7348 0 11C0 11.2652 0.105357 11.5196 0.292893 11.7071C0.48043 11.8946 0.734784 12 1 12H19C19.2652 12 19.5196 11.8946 19.7071 11.7071C19.8946 11.5196 20 11.2652 20 11C20 10.7348 19.8946 10.4804 19.7071 10.2929C19.5196 10.1054 19.2652 10 19 10ZM19 5H1C0.734784 5 0.48043 5.10536 0.292893 5.29289C0.105357 5.48043 0 5.73478 0 6C0 6.26522 0.105357 6.51957 0.292893 6.70711C0.48043 6.89464 0.734784 7 1 7H19C19.2652 7 19.5196 6.89464 19.7071 6.70711C19.8946 6.51957 20 6.26522 20 6C20 5.73478 19.8946 5.48043 19.7071 5.29289C19.5196 5.10536 19.2652 5 19 5Z" fill="currentColor"></path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
        </nav>
        <div class="navbar-menu relative z-50 hidden xl:flex xl:flex-col">
          <div class="navbar-backdrop fixed xl:hidden inset-0 bg-gray-800 opacity-10"></div>
          
        </div>
        <div class="mx-auto xl:ml-xss xl:pl-4"></div>
      </section>
                
      <section class="overflow-hidden">
        <nav class="flex items-center justify-between py-3.5 xl:py-2.5 px-7 bg-neutral-50">
          <div class="w-full xl:w-auto px-2 xl:mr-10">
            <div class="flex items-center justify-between"><a class="inline-flex items-center h-7" href="#"><img src="dashy-assets/logos/dashy-logo-dark.svg" alt=""></a>
              <div class="xl:hidden">
                <button class="navbar-burger text-gray-400 hover:text-gray-300 focus:outline-none">
                  <svg width="20" height="12" viewbox="0 0 20 12" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M1 2H19C19.2652 2 19.5196 1.89464 19.7071 1.70711C19.8946 1.51957 20 1.26522 20 1C20 0.734784 19.8946 0.48043 19.7071 0.292893C19.5196 0.105357 19.2652 0 19 0H1C0.734784 0 0.48043 0.105357 0.292893 0.292893C0.105357 0.48043 0 0.734784 0 1C0 1.26522 0.105357 1.51957 0.292893 1.70711C0.48043 1.89464 0.734784 2 1 2ZM19 10H1C0.734784 10 0.48043 10.1054 0.292893 10.2929C0.105357 10.4804 0 10.7348 0 11C0 11.2652 0.105357 11.5196 0.292893 11.7071C0.48043 11.8946 0.734784 12 1 12H19C19.2652 12 19.5196 11.8946 19.7071 11.7071C19.8946 11.5196 20 11.2652 20 11C20 10.7348 19.8946 10.4804 19.7071 10.2929C19.5196 10.1054 19.2652 10 19 10ZM19 5H1C0.734784 5 0.48043 5.10536 0.292893 5.29289C0.105357 5.48043 0 5.73478 0 6C0 6.26522 0.105357 6.51957 0.292893 6.70711C0.48043 6.89464 0.734784 7 1 7H19C19.2652 7 19.5196 6.89464 19.7071 6.70711C19.8946 6.51957 20 6.26522 20 6C20 5.73478 19.8946 5.48043 19.7071 5.29289C19.5196 5.10536 19.2652 5 19 5Z" fill="currentColor"></path>
                  </svg>
                </button>
              </div>
            </div>
          </div>
          <div class="hidden xl:block w-full md:w-auto px-2 mr-auto">
            <ul class="flex items-center">
              <li class="mr-10"><a class="group inline-block" href="#"><span class="text-sm text-neutral-600 font-medium group-hover:text-transparent group-hover:bg-gradient-purple-top bg-clip-text">Home</span></a></li>
              <li class="mr-10"><a class="group inline-block" href="#"><span class="text-sm font-medium text-transparent bg-gradient-purple-top bg-clip-text">Projects</span></a></li>
              <li class="mr-10"><a class="group inline-block" href="#"><span class="text-sm text-neutral-600 font-medium group-hover:text-transparent group-hover:bg-gradient-purple-top bg-clip-text">What is Dashy?</span></a></li>
            </ul>
          </div>
          <div class="hidden xl:block w-full md:w-auto px-2">
            <div class="md:flex items-center">
              <div class="w-full md:w-auto mb-6 md:mb-0">
                <div class="flex flex-wrap items-center">
                  <div class="relative flex items-center mr-4 w-52 border border-neutral-100 rounded-lg focus-within:border-neutral-600 hover:bg-gray-50">
                    <input class="w-full px-4 pr-12 py-2 text-sm text-neutral-400 placeholder-neutral-400 bg-transparent outline-none" id="horizontalNav4-1" type="text" placeholder="Search...">
                    <div class="absolute right-4">
                      <svg width="18" height="18" viewbox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M15.2197 16.2803C15.5126 16.5732 15.9874 16.5732 16.2803 16.2803C16.5732 15.9874 16.5732 15.5126 16.2803 15.2197L15.2197 16.2803ZM11.7803 10.7197C11.4874 10.4268 11.0126 10.4268 10.7197 10.7197C10.4268 11.0126 10.4268 11.4874 10.7197 11.7803L11.7803 10.7197ZM12 7.5C12 9.98528 9.98528 12 7.5 12V13.5C10.8137 13.5 13.5 10.8137 13.5 7.5H12ZM7.5 12C5.01472 12 3 9.98528 3 7.5H1.5C1.5 10.8137 4.18629 13.5 7.5 13.5V12ZM3 7.5C3 5.01472 5.01472 3 7.5 3V1.5C4.18629 1.5 1.5 4.18629 1.5 7.5H3ZM7.5 3C9.98528 3 12 5.01472 12 7.5H13.5C13.5 4.18629 10.8137 1.5 7.5 1.5V3ZM16.2803 15.2197L11.7803 10.7197L10.7197 11.7803L15.2197 16.2803L16.2803 15.2197Z" fill="#B8C1CC"></path>
                      </svg>
                    </div>
                  </div><a class="inline-block mr-4" href="#">
                    <div class="flex items-center justify-center w-8 h-8 bg-neutral-100 rounded-full">
                      <svg width="18" height="18" viewbox="0 0 18 18" fill="none" xmlns="http://www.w3.org/2000/svg">
                        <path d="M15 12.75V13.5C15.3033 13.5 15.5768 13.3173 15.6929 13.037C15.809 12.7568 15.7448 12.4342 15.5303 12.2197L15 12.75ZM3 12.75L2.46967 12.2197C2.25517 12.4342 2.191 12.7568 2.30709 13.037C2.42318 13.3173 2.69665 13.5 3 13.5V12.75ZM4.0537 11.6963L4.58403 12.2266H4.58403L4.0537 11.6963ZM7.5 4.00606L7.74993 4.71319C8.04963 4.60726 8.25 4.32392 8.25 4.00606H7.5ZM10.5 4.00606H9.75C9.75 4.32392 9.95037 4.60726 10.2501 4.71319L10.5 4.00606ZM3.53033 13.2803L4.58403 12.2266L3.52337 11.166L2.46967 12.2197L3.53033 13.2803ZM5.25 10.6188V8.25H3.75V10.6188H5.25ZM12.75 8.25V10.6188H14.25V8.25H12.75ZM13.416 12.2266L14.4697 13.2803L15.5303 12.2197L14.4766 11.166L13.416 12.2266ZM4.58403 12.2266C5.01044 11.8002 5.25 11.2219 5.25 10.6188H3.75C3.75 10.8241 3.66848 11.0209 3.52337 11.166L4.58403 12.2266ZM12.75 10.6188C12.75 11.2219 12.9896 11.8002 13.416 12.2266L14.4766 11.166C14.3315 11.0209 14.25 10.8241 14.25 10.6188H12.75ZM7.25007 3.29893C5.21199 4.01929 3.75 5.96295 3.75 8.25H5.25C5.25 6.6184 6.29243 5.22834 7.74993 4.71319L7.25007 3.29893ZM10.2501 4.71319C11.7076 5.22834 12.75 6.6184 12.75 8.25H14.25C14.25 5.96295 12.788 4.01929 10.7499 3.29893L10.2501 4.71319ZM11.25 4.00606V3.75H9.75V4.00606H11.25ZM6.75 3.75V4.00606H8.25V3.75H6.75ZM9 1.5C7.75736 1.5 6.75 2.50736 6.75 3.75H8.25C8.25 3.33579 8.58579 3 9 3V1.5ZM11.25 3.75C11.25 2.50736 10.2426 1.5 9 1.5V3C9.41421 3 9.75 3.33579 9.75 3.75H11.25ZM10.5 13.5C10.5 14.3284 9.82843 15 9 15V16.5C10.6569 16.5 12 15.1569 12 13.5H10.5ZM9 15C8.17157 15 7.5 14.3284 7.5 13.5H6C6 15.1569 7.34315 16.5 9 16.5V15ZM15 12H11.25V13.5H15V12ZM12 13.5V12.75H10.5V13.5H12ZM11.25 12H6.75V13.5H11.25V12ZM6.75 12H3V13.5H6.75V12ZM7.5 13.5V12.75H6V13.5H7.5Z" fill="#0C1523"></path>
                      </svg>
                    </div></a><a class="inline-flex items-center" href="#"><img class="mr-2" src="dashy-assets/images/avatar4.png" alt="">
                    <svg width="16" height="16" viewbox="0 0 16 16" fill="none" xmlns="http://www.w3.org/2000/svg">
                      <path d="M12.6668 6L8.00016 10.6667L3.3335 6" stroke="#0C1523" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"></path>
                    </svg></a>
                </div>
              </div>
            </div>
          </div>
        </nav>
        <div class="navbar-menu fixed top-0 left-0 bottom-0 z-50 hidden">
          <div class="navbar-backdrop fixed top-0 left-0 w-full h-full bg-gray-800 opacity-50"></div>
          <nav class="fixed w-full h-full max-w-xss bg-white">
            <div class="flex flex-wrap items-center justify-between px-7 py-2 pb-1 border-b border-gray-200">
              <div class="w-auto"><a class="inline-block" href="#"><img src="dashy-assets/logos/dashy-logo-dark.svg" alt=""></a></div>
              <div class="w-auto"><a class="text-neutral-300 hover:text-neutral-400" href="#">
                  <svg width="23" height="22" viewbox="0 0 23 22" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M6.97944 7.71965C6.68654 8.01254 6.68654 8.48742 6.97944 8.78031C7.27233 9.0732 7.7472 9.0732 8.0401 8.78031L6.97944 7.71965ZM11.1764 4.58331L11.7068 4.05298C11.4139 3.76009 10.939 3.76009 10.6461 4.05298L11.1764 4.58331ZM14.3128 8.78031C14.6057 9.0732 15.0805 9.0732 15.3734 8.78031C15.6663 8.48742 15.6663 8.01254 15.3734 7.71965L14.3128 8.78031ZM15.3734 14.2803C15.6663 13.9874 15.6663 13.5125 15.3734 13.2196C15.0805 12.9268 14.6057 12.9268 14.3128 13.2196L15.3734 14.2803ZM11.1764 17.4166L10.6461 17.947C10.939 18.2399 11.4139 18.2399 11.7068 17.947L11.1764 17.4166ZM8.0401 13.2196C7.7472 12.9268 7.27233 12.9268 6.97944 13.2196C6.68654 13.5125 6.68654 13.9874 6.97944 14.2803L8.0401 13.2196ZM8.0401 8.78031L11.7068 5.11364L10.6461 4.05298L6.97944 7.71965L8.0401 8.78031ZM10.6461 5.11364L14.3128 8.78031L15.3734 7.71965L11.7068 4.05298L10.6461 5.11364ZM14.3128 13.2196L10.6461 16.8863L11.7068 17.947L15.3734 14.2803L14.3128 13.2196ZM11.7068 16.8863L8.0401 13.2196L6.97944 14.2803L10.6461 17.947L11.7068 16.8863Z" fill="currentColor"></path>
                  </svg></a></div>
            </div>
            <div class="py-6 h-full overflow-y-auto">
              <div class="flex flex-col flex-wrap px-7 -m-2.5">
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/home-2.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Dashboard</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center mb-3.5" href="#"><img class="mr-3" src="dashy-assets/images/gear.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">People &amp; Settings</p></a>
                  <div class="ml-8">
                    <div class="flex flex-wrap -m-1">
                      <div class="w-auto p-1"><a class="font-medium text-neutral-500 hover:text-neutral-600" href="#">
                          Help with
                          Sketch</a></div>
                      <div class="w-auto p-1"><a class="font-medium text-neutral-500 hover:text-neutral-600" href="#">
                          All
                          Documents</a></div>
                      <div class="w-auto p-1"><a class="font-medium text-neutral-500 hover:text-neutral-600" href="#">
                          Shared with
                          Me</a></div>
                      <div class="w-auto p-1"><a class="font-medium text-neutral-500 hover:text-neutral-600" href="#">Libraries</a></div>
                    </div>
                  </div>
                </div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/loader-rec.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Discover</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/lifebuoy.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Help with Sketch</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/folder-open.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">All Documents</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/user-circle.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Shared with Me</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/link-2-rec.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Libraries</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/list-unordered-3-rec.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">My Drafts</p></a></div>
                <div class="w-auto p-2.5"><a class="flex flex-wrap items-center" href="#"><img class="mr-3" src="dashy-assets/images/trash.svg" alt="">
                    <p class="hover:text-neutral-700 font-medium">Trash</p></a></div>
              </div>
            </div>
          </nav>
        </div>
      </section>
      <section id="formsignup" class="py-4 overflow-hidden"><div class="container px-4 mx-auto">
        <div class="pb-12 pt-8 px-6 text-center bg-white overflow-hidden border rounded-xl">
          <h3 class="mb-1 text-xl font-semibold">Register</h3>
          <p class="mb-11 text-neutral-500">Register to the site to join the Community.</p>
          <div class="flex flex-wrap justify-center max-w-xs mx-auto -m-2">
            <div class="w-full p-2">      <div class="mb-6">
              <label class="block font-heading mb-2.5 text-sm font-semibold">Username</label>
              <input id="username" class="py-2.5 px-3.5 text-sm w-full hover:bg-gray-50 outline-none placeholder-neutral-400 border border-neutral-200 rounded-lg focus-within:border-neutral-600" type="text" placeholder="Input Your Name"></div>
            </div>
            <div class="mb-6">
              <label class="block font-heading mb-2.5 text-sm font-semibold">Email</label>
              <input id="email" class="py-2.5 px-3.5 text-sm w-full hover:bg-gray-50 outline-none placeholder-neutral-400 border border-neutral-200 rounded-lg focus-within:border-neutral-600" type="text" placeholder="Input Your Email"></div>
            <div class="mb-6">
              <label class="block font-heading mb-2.5 text-sm font-semibold">Password</label>
              <input id="password" class="py-2.5 px-3.5 text-sm w-full hover:bg-gray-50 outline-none placeholder-neutral-400 border border-neutral-200 rounded-lg focus-within:border-neutral-600" type="password" placeholder="Input Your Password"></div>
          </div>
          <button onclick="PushReg()" class="inline-flex flex-wrap items-center px-5 py-3.5 text-sm text-neutral-50 font-medium bg-gradient-purple-left hover:bg-gradient-purple-left-dark rounded-lg transition duration-300" type="submit">Submit</button>
        </div>
        </div>
      </section>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/apexcharts"></script>
    <script src="js/charts-demo.js"></script>
</body>
</html>
```
Didalam terdapat 3 textbox yang ditambah id, id ini akan digunakan sebagai input untuk API. Dan ada button submit yang ditambahkan "PushReg()" agar JS berjalan ke API saat di pencet.

# Membuat JS dan Sambungkan dengan Web
Kita buat terlebih dahulu API nya di Pipedream..
Selanjutnya kita membuat JS untuk disambungkan dengan Web, Kita menggunakan codingan js berikut:
```
function PushReg(){
    username=document.getElementById("username").value;
    email=document.getElementById("email").value;
    password=document.getElementById("password").value;
    PostSignUp(username,email,password);
}

function PostSignUp(username,email,password){
var myHeaders = new Headers();
myHeaders.append("reghook", "$^[xhF9;V&w#CR'huKj;xGm-;~^S:EE!,Xpt;a*kU%7>vKLSw:&28`VyGFxuWuZ)z%yZH&-f");
myHeaders.append("Content-Type", "application/json");

var raw = JSON.stringify({
  "username": username,
  "email": email,
  "password": password
});

var requestOptions = {
  method: 'POST',
  headers: myHeaders,
  body: raw,
  redirect: 'follow'
};

fetch("https://eo218ccadktgtds.m.pipedream.net", requestOptions)
  .then(response => response.text())
  .then(result => console.log(result))
  .catch(error => console.log('error', error));  
}
function GetResponse(result){
  document.getElementById("formsignup").style.display = 'none';
  document.getElementById("formsignup").style.display = 'block';
  document.getElementById("formsignup").innerHTML = result;
}
```

Hasilnya seperti berikut:
![image](https://github.com/adam-ghafara/WS/blob/main/ChapterQUIS/1214064_AdamGhafara_Quis/foto/Screenshot_2671.png?raw=true)
Hasil dalam Pipedream:
![image](https://github.com/adam-ghafara/WS/blob/main/ChapterQUIS/1214064_AdamGhafara_Quis/foto/Screenshot_2673.png?raw=true)

# Membuat BACKEND GO

Kegiatan kedua kita akan membuat Backend GO. Sebelumnya kita perlu membuat Database nya terlebih dahulu menggunakan MONGODB di Atlas, selanjutnya sambungkan database tersebut dengan aplikasi mongodb compass. Setelah semuanya selesai, kita dapat langsung membuat backend go.
Berikut adalah tahapannya.

## Membuat Mod

Kita akan membuat Mod terlebih dahulu untuk Backend GO.
Pertama buat folder backend, kita push terlebih dahulu folder backend tersebut kedalam git.
Selanjutnya, buka terminal di VS Code, dan jalankan perintah seperti contoh:
```
go mod init github.com/adam-ghafara/WS/edit/main/ChapterQUIS/1214064_AdamGhafara_Quis/golang
```
Pada kasus, disini foldernya namanya golang, namun hal ini tidak masalah selama kita push dengan folder yang benar dan dapat digunakan untuk backend GO.
Selanjutnya kita akan membuat beberapa codingan Go berikutnya.
## Membuat Type.Go
Type.go menggunakan codingan berikut:
```
package adamquis

import (
	"go.mongodb.org/mongo-driver/bson/primitive"
)

type Karyawan struct {
	ID           primitive.ObjectID `bson:"_id,omitempty" json:"_id,omitempty"`
	Nama         string             `bson:"nama,omitempty" json:"nama,omitempty"`
	Phone_number string             `bson:"phone_number,omitempty" json:"phone_number,omitempty"`
	Jabatan      string             `bson:"jabatan,omitempty" json:"jabatan,omitempty"`
	Jam_kerja    []JamKerja         `bson:"jam_kerja,omitempty" json:"jam_kerja,omitempty"`
	Hari_kerja   []string           `bson:"hari_kerja,omitempty" json:"hari_kerja,omitempty"`
}

type JamKerja struct {
	Durasi     int      `bson:"durasi,omitempty" json:"durasi,omitempty"`
	Jam_masuk  string   `bson:"jam_masuk,omitempty" json:"jam_masuk,omitempty"`
	Jam_keluar string   `bson:"jam_keluar,omitempty" json:"jam_keluar,omitempty"`
	Gmt        int      `bson:"gmt,omitempty" json:"gmt,omitempty"`
	Hari       []string `bson:"hari,omitempty" json:"hari,omitempty"`
	Shift      int      `bson:"shift,omitempty" json:"shift,omitempty"`
	Piket_tim  string   `bson:"piket_tim,omitempty" json:"piket_tim,omitempty"`
}

type Presensi struct {
	ID           primitive.ObjectID `bson:"_id,omitempty" json:"_id,omitempty"`
	Longitude    float64            `bson:"longitude,omitempty" json:"longitude,omitempty"`
	Latitude     float64            `bson:"latitude,omitempty" json:"latitude,omitempty"`
	Location     string             `bson:"location,omitempty" json:"location,omitempty"`
	Phone_number string             `bson:"phone_number,omitempty" json:"phone_number,omitempty"`
	Datetime     primitive.DateTime `bson:"datetime,omitempty" json:"datetime,omitempty"`
	Checkin      string             `bson:"checkin,omitempty" json:"checkin,omitempty"`
	Biodata      Karyawan           `bson:"biodata,omitempty" json:"biodata,omitempty"`
}

type Lokasi struct {
	ID       primitive.ObjectID `bson:"_id,omitempty" json:"_id,omitempty"`
	Nama     string             `bson:"nama,omitempty" json:"nama,omitempty"`
	Batas    Geometry           `bson:"batas,omitempty" json:"batas,omitempty"`
	Kategori string             `bson:"kategori,omitempty" json:"kategori,omitempty"`
}

type Geometry struct {
	Type        string      `json:"type" bson:"type"`
	Coordinates interface{} `json:"coordinates" bson:"coordinates"`
}
```
SAVE!
Selanjutnya jalankan:
```
go mod tidy
```
Tunggu hingga selesai.
## Membuat package
Selanjutnya kita akan membuat package, berikut adalah codingan untuk package.go yang akan dibuat:
```
package adamquis

import (
	"context"
	"fmt"
	"os"
	"time"

	"go.mongodb.org/mongo-driver/bson/primitive"
	"go.mongodb.org/mongo-driver/mongo"
	"go.mongodb.org/mongo-driver/mongo/options"
	"gopkg.in/mgo.v2/bson"
)

var MongoString string = os.Getenv("MONGOSTRING")

func MongoConnect(dbname string) (db *mongo.Database) {
	client, err := mongo.Connect(context.TODO(), options.Client().ApplyURI(MongoString))
	if err != nil {
		fmt.Printf("MongoConnect: %v\n", err)
	}
	return client.Database(dbname)
}

func InsertOneDoc(db string, collection string, doc interface{}) (insertedID interface{}) {
	insertResult, err := MongoConnect(db).Collection(collection).InsertOne(context.TODO(), doc)
	if err != nil {
		fmt.Printf("InsertOneDoc: %v\n", err)
	}
	return insertResult.InsertedID
}

func InsertPresensi(long float64, lat float64, lokasi string, phonenumber string, checkin string, biodata Karyawan) (InsertedID interface{}) {
	var presensi Presensi
	presensi.Latitude = long
	presensi.Longitude = lat
	presensi.Location = lokasi
	presensi.Phone_number = phonenumber
	presensi.Datetime = primitive.NewDateTimeFromTime(time.Now().UTC())
	presensi.Checkin = checkin
	presensi.Biodata = biodata
	return InsertOneDoc("ChapterQuis", "presensi", presensi)
}

func GetKaryawanFromPhoneNumber(phone_number string) (staf Presensi) {
	karyawan := MongoConnect("ChapterQuis").Collection("presensi")
	filter := bson.M{"phone_number": phone_number}
	err := karyawan.FindOne(context.TODO(), filter).Decode(&staf)
	if err != nil {
		fmt.Printf("getKaryawanFromPhoneNumber: %v\n", err)
	}
	return staf
}
```
jalan perintah **go mod tidy** sebelumnya hingga selesai.
## Membuat package_test.go dan test Backend

Selanjutnya di tahap akhir kita akan melakukan test Backend, sebelumnya kita perlu membuat codingan test nya. berikut adalah codingan untuk package_test.go
```
package adamquis

import (
	"fmt"
	"testing"
)

func TestInsertPresensi(t *testing.T) {
	long := 98.345345
	lat := 123.561651
	lokasi := "Gedung"
	phonenumber := "89673581578"
	checkin := "Ya"
	biodata := Karyawan{
		Nama:         "Adam",
		Phone_number: "89673581578",
		Jabatan:      "Developer",
	}
	hasil := InsertPresensi(long, lat, lokasi, phonenumber, checkin, biodata)
	fmt.Println(hasil)

}

func TestGetKaryawanFromPhoneNumber(t *testing.T) {
	phonenumber := "89673581578"
	biodata := GetKaryawanFromPhoneNumber(phonenumber)
	fmt.Println(biodata)
}
```
Setelah itu, jalankan perintah berikut:
```
go test
```
Hasil dari terminal dan dalam MongoDB Compass setelah dilakukan semua kegiatan tersebut:
![image](https://github.com/adam-ghafara/WS/blob/main/ChapterQUIS/1214064_AdamGhafara_Quis/foto/Screenshot_2675.png?raw=true)
![image](https://github.com/adam-ghafara/WS/blob/main/ChapterQUIS/1214064_AdamGhafara_Quis/foto/Screenshot_2676.png?raw=true)
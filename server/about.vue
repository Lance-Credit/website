<template>
    <div>
        <MainMenu class="group black"/>
        <div class="bg-[#FBFBFB] pt-[194px] sm:pt-[254px] sm:px-40 pb-0 sm:pb-[104px] text-center">
            <p class="px-8 mb-6 text-[#021E1C] text-[32px] sm:text-[40px] leading-[30px] sm:leading-[42px] font-medium">
                Providing the best lending services<br>through multiple channels
            </p>
            <p class="px-8 mb-10 sm:mb-16 max-w-[623px] mx-auto text-[#5C6C67] font-gelion-l text-base sm:text-lg leading-[26px]">
                At Lance, We're turning dreams into reality by fueling dreams, aspirations, and
                driving progress like never before.
            </p>
            <div class="max-w-[1120px] h-[324px] mx-auto bg-[#D8D6D6] sm:rounded-[10px]"></div>
        </div>
        <div class="bg-[#1C2928] py-20 sm:py-[104px] px-8 sm:px-[160px]">
            <div class="max-w-[1120px] mx-auto">
                <div class="mb-10 sm:mb-24 text-center sm:text-left">
                    <p class="mb-4 text-white text-[22px] sm:text-[32px] leading-[28px] sm:leading-[40px] tracking-[-0.22px] sm:tracking-[-0.32px]">
                        Meet the Lance Credit Team
                    </p>
                    <p class="max-w-[453px] text-[#9FB8A8] text-base sm:text-lg leading-[26px] tracking-[0.16px] sm:tracking-[0.18px] font-gelion-r">
                        Lance’s mission is to improve the financial happiness of underserved Africans, starting with making credit more accessible.
                    </p>
                    <p class="max-w-[453px] text-[#9FB8A8] text-base sm:text-lg leading-[26px] tracking-[0.16px] sm:tracking-[0.18px] font-gelion-r">
                        The team is made up of a combination of some of the top technologists on the African continent. We are deeply passionate and share deep values around using technology to bring amazing solutions to reality for Africans.
                    </p>
                </div>
                <ul class="flex gap-x-6 sm:gap-x-16 gap-y-16 sm:gap-y-20 text-center flex-wrap justify-center">
                    <li v-for="(member, key) in teamMembers" :key="key" class="w-[151px] sm:w-auto">
                        <div class="rounded-full mb-4 sm:mb-6 bg-[#2A3B39] w-24 sm:w-[232px] h-24 sm:h-[232px] mx-auto">
                            <img v-if="member.img" :src="member.img" alt="" class="w-full h-full rounded-full">
                        </div>
                        <p class="mb-1 text-[#C8E993] text-base sm:text-lg leading-[24px] tracking-[-0.16px] sm:tracking-[-0.18px]">
                            {{ member.name }}
                        </p>
                        <p class="text-[#ACBD91] font-gelion-l text-sm sm:text-base sm:leading-[24px] tracking-[-0.14px] sm:tracking-[-0.16px]">
                            {{ member.title }}
                        </p>
                    </li>
                </ul>
            </div>
        </div>
        <MainFooter/>
    </div>
</template>

<script setup lang="ts">
    
    const teamMembers = [
        {
            name: 'Yewande Odumosu',
            title: 'Co-Founder',
            img: '/assets/img/team/yewande.png'
        },
        {
            name: 'Adebayo Opesanya',
            title: 'Co-Founder/Engineering',
            img: ''
        },
        {
            name: 'Albert Oboh',
            title: 'Engineering',
            img: ''
        },
        {
            name: 'Nwagba Okechukwu',
            title: 'Engineering',
            img: ''
        },
        {
            name: 'Yanmife Akeju',
            title: 'Engineering',
            img: ''
        },
        {
            name: 'Ndebe Wisdom',
            title: 'Design',
            img: ''
        },
        {
            name: 'Oluwatimilehin Lawal',
            title: 'Design',
            img: ''
        }
    ]

</script>
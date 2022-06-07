<template>
  <div class="flex flex-col justify-center items-center mt-12">
    <a
      href="#"
      class="flex items-center bg-gray-900 text-white px-6 py-3 rounded-md text-base font-medium my-2"
    >
      <HomeIcon /> <span class="pl-2">Home</span>
    </a>

    <a
      href="#"
      class="flex items-center text-gray-300 hover:bg-gray-700 hover:text-white px-6 py-3 rounded-md text-base font-medium my-2"
    >
      <GroupIcon /> <span class="pl-2">Groups</span>
    </a>

    <a
      href="#"
      class="flex items-center text-gray-300 hover:bg-gray-700 hover:text-white px-6 py-3 rounded-md text-base font-medium my-2"
    >
      <SettingsIcon /> <span class="pl-2">Settings</span>
    </a>

    <a
      href="#"
      class="flex items-center text-gray-300 hover:bg-gray-700 hover:text-white px-6 py-3 rounded-md text-base font-medium my-2"
      ><InviteIcon /> <span class="pl-2">Invite</span>
    </a>

    <a
      href="#"
      class="flex items-center text-gray-300 hover:bg-gray-700 hover:text-white px-6 py-3 rounded-md text-base font-medium my-2"
      ><LogoutIcon /> <span class="pl-2">Logout</span>
    </a>
  </div>
</template>
<script>
import HomeIcon from "@/assets/svgs/home-svg.vue";
import GroupIcon from "@/assets/svgs/groups-svg.vue";
import InviteIcon from "@/assets/svgs/invite-svg.vue";
import LogoutIcon from "@/assets/svgs/logout-svg.vue";
import SettingsIcon from "@/assets/svgs/settings-svg.vue";
export default {
  name: "Navbar",
  components: {
    HomeIcon,
    GroupIcon,
    InviteIcon,
    LogoutIcon,
    SettingsIcon,
  },
};
</script>

<template>
    <main class="w-100 h-100">
      <NavBar/>
      <div class="d-flex justify-content-center">
        <ProfilePage />
        <DataBase />
      </div>
      <TableView />
      <FooterView/>
    </main>
</template>

<script>
import NavBar from '@/components/Navbar'
import ProfilePage from '@/components/Profile'
import DataBase from '@/components/Database'
import TableView from '@/components/Table'
import FooterView from '@/components/Footer'

export default {
  name: 'HomeView',
  components: {
    NavBar,
    ProfilePage,
    DataBase,
    TableView,
    FooterView,
  },
}
</script>
<style lang="scss">
body{
  overflow-x:hidden;
}
main{
  border: 1px solid #A9ADCC;
  padding-top:  7px ;
  border-left: 20px solid #D5D5D5 !important;
  border-right: 20px solid #D5D5D5 !important;

}
</style>

<template>
  <div class="profile-pics-cover py-2 d-flex px-1">
      <div class="profile-pics text-sm text-blue-20 d-flex align-items-center justify-content-center pointer">
        (Profile Pic)
      </div>
      <div class="details d-flex flex-column align-items-start">
        <p class="text-sm text-black-10">Logged in as:</p>
        <div class="d-flex justify-content-between align-items-center">
            <p class="michel text-md text-black-10">Michel B. Jordan</p>
            <img src="../assets/Icon-user-edit.svg" alt="" width="31" height="22" class="mb-3 pointer">
        </div>
        <p class="text-sm-2">Sales Manager</p>
        <p class="text-sm-2">Fouler Automotive</p>
        <div class="office-cell">
          <p class="text-sm-2">Office: <span>(703) 123-4567</span></p>
          <p class="text-sm-2">Cell: <span>&nbsp;&nbsp; (571) 123-4567</span></p>
        </div>
      </div>
    </div>
</template>

<script>

export default{
    name: 'ProfilePage',

}

</script>

<style lang="scss">
  .profile-pics-cover{
  font-family: 'Open Sans';
  border:1px solid rgba(169, 173, 204, 1);
  width: auto;
  height: 225px;
    .profile-pics{
    background: rgba(206, 201, 201, 1);
    width: 147px;
    height: 207px;
    }
    .details{
    line-height: 18px;
    margin-left: 20px;
    .office-cell{
      line-height:10px;
      span{
      margin-left:20px;
      }
    }
    .michel{
      margin-right: 45px;
    }
    }
  }
  
</style>
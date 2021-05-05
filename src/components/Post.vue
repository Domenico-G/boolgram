<template>
  <div class="post">
    <!-- header post -->
    <div class="head-post">
      <div class="user-post">
        <div class="pic-user">
          <img src="../assets/img/profile.jpg" alt="pic user" />
        </div>
        <p>Miss Maye Pfeffer</p>
      </div>
      <font-awesome-icon class="icon" :icon="['fas', 'ellipsis-h']" />
    </div>
    <!-- immagine post -->
    <div class="post-img">
      <img src="../assets/img/landscape.png" alt="" />
    </div>
    <!-- informazioni post -->
    <div class="info-post">
      <div class="like-chat-icon">
        <font-awesome-icon class="icon" :icon="['far', 'heart']" />
        <font-awesome-icon class="icon" :icon="['far', 'comment']" />
      </div>
      <div class="users-like">
        <div class="users-pic">
          <img src="../assets/img/profile.jpg" alt="pic user" />
        </div>
        <p>Piace a <b>trudie35</b> e <b>4 altri</b></p>
      </div>
      <div class="comments">
        <p class="show-comments">Mostra tutti e 4 commenti</p>
        <p><b>krajcik.leonard</b> I get".</p>
        <p><b>schulist.sabryna</b> Lory, as.</p>
        <p><b>meaghan91</b> D, she.</p>
      </div>
      <div class="time">
        <p>33 Ore fa</p>
      </div>
    </div>
    <!-- input agigunta commento -->
    <div class="add-comment">
      <input type="text" placeholder="Aggingi un commento" />
      <div class="button-comment">
        <p>Pubblica</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Post",
  props: {},
};
</script>

<style lang="scss" scoped>
.post {
  margin-top: 30px;

  .head-post {
    border-radius: 5px 5px 0 0;
    border: 1px solid #e6e6e6;
    padding: 10px 10px;
    @include flex-center;

    .user-post {
      @include flex-center;

      .pic-user {
        width: 40px;
        margin-right: 15px;
        height: 40px;
        border: 2px solid red;
        border-radius: 50%;
        padding: 1px;

        img {
          border-radius: 50%;
          width: 100%;
        }
      }

      p {
        font-weight: 600;
      }
    }
  }

  .post-img {
    width: 100%;
    height: 500px;

    img {
      width: 100%;
      height: 100%;
    }
  }

  .info-post {
    padding: 20px 10px;
    border: 1px solid #e6e6e6;

    .icon {
      font-size: 25px;
      margin-right: 20px;
    }

    .users-like {
      margin: 15px 0;
      display: flex;

      .users-pic {
        width: 20px;
        margin-right: 10px;

        img {
          width: 110%;
          border-radius: 50%;
        }
      }
    }

    .comments {
      p {
        font-size: 14px;
        line-height: 1.6;
      }

      .show-comments {
        color: #bfbfbf;
      }
    }

    .time {
      margin: 15px 0 0 0;
      font-size: 14px;
      color: #bfbfbf;
    }
  }

  .add-comment {
    @include flex-center;
    padding: 10px 10px;
    border: 1px solid #e6e6e6;
    border-top: 0px;

    input {
      border: 0px;
      &:focus {
        outline: 0px;
      }

      &::placeholder {
        // text-align: center;
      }
    }

    .button-comment {
      color: #4da6ff;
      font-size: 15px;
      font-weight: 600;
      cursor: pointer;
    }
  }
}
</style>

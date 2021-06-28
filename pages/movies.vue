<template>
  <div>
    
    <div class="chat-banner chat-banner--danger" v-if="isNetwork">

      <div class="chat-banner--left">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        xmlns:xlink="http://www.w3.org/1999/xlink"
        width="32px"
        height="32px"
        viewBox="0 0 32 32"
        class="chat-banner--icon"
        style="fill: currentcolor"
      >
        <path
          d="M27.7 12.943c-.302 0-.606-.104-.852-.318a15.296 15.296 0 0 0-2.271-1.638 1.3 1.3 0 0 1 1.318-2.242c.928.546 1.822 1.19 2.658 1.917a1.3 1.3 0 0 1-.853 2.28m-3.758 4.868c-.3 0-.6-.102-.845-.312a11.092 11.092 0 0 0-2.797-1.763 1.3 1.3 0 1 1 1.035-2.385 13.7 13.7 0 0 1 3.453 2.173 1.3 1.3 0 0 1-.846 2.287m-3.758 4.838c-.296 0-.592-.1-.837-.306-.96-.808-2.15-1.253-3.347-1.253h-.137a1.3 1.3 0 0 1 0-2.6H16c1.81 0 3.594.662 5.022 1.865a1.298 1.298 0 0 1-.838 2.294M7.053 24.586a1.3 1.3 0 0 1-.945-2.193l6.678-7.07a11.03 11.03 0 0 0-3.878 2.172 1.3 1.3 0 0 1-1.7-1.97c2.394-2.064 5.404-3.23 8.504-3.3L18.93 8.82A16.39 16.39 0 0 0 16 8.557c-3.937 0-7.792 1.447-10.854 4.073a1.3 1.3 0 1 1-1.692-1.973c3.532-3.03 7.988-4.7 12.546-4.7 1.707 0 3.386.225 5 .67l1.626-1.72a1.3 1.3 0 1 1 1.889 1.786l-7.283 7.71c-.016.019-.032.035-.05.052l-9.184 9.723c-.256.27-.6.408-.945.408m9.359 2.914c-.138 0-.277-.022-.412-.067a1.3 1.3 0 0 1-1.212-2.26 1.998 1.998 0 0 1 2.424 0 1.3 1.3 0 0 1-.8 2.327"
        ></path>
      </svg>
      </div>

      <div class="chat-banner--center">
        <div class="chat-banner--text-section">
          <h4 class="chat-banner--title">Network connection is unstable.</h4>
          <div class="chat-banner--description-container">
            <span class="chat-banner--main-description body2">
              Please retry your internet connection and refresh the page. </span
            >
          </div>
        </div>
      </div>
    </div>
    <h1>This Movies</h1>
  </div>
</template>


<script>
export default {
  data(){
    return {
      isNetwork: true
    }
  }
}
</script>


<style scoped>
  .chat-banner{
    width: 100%;
    display: flex;
    padding: 12px 16px; 
  }

  .chat-banner--danger{
    background-color: #feedef;
  }
  .chat-banner--danger .chat-banner--title,
  .chat-banner--danger .chat-banner--icon {
      color: #e5172f;
  }
  .chat-banner--left{
    padding-right: 12px;
  }
  .chat-banner--center{
    width: 100%;
    padding-right: 8px;
    display: flex;
    align-items: center;
  }
</style>

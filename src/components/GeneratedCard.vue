<!-- Generated Card UI added here -->
<template>
  <div class="section-container section-right col-6">
    <div class="id-card-container" id="collegeCard">
      <div class="text-center subtitle-card">Preview carte générée</div>
      <div class="card-container">
        <div class="card-wrapper" id="generatedIdCard">
          <div class="profile-card">
            
              <div class="user-card">
                <span class="user-photo">
              
                </span>
              </div>
              <div>
              <div class="general-information">
                <div class="card-element card-name">
                  <span class="card-title"></span>
                  <span class="card-input dafont" id="cardName">{{formData.fullName}}</span>
                </div>
                <div class="card-element card-name">
                  <span class="card-title"></span>
                  <span class="card-input dafont" id="cardName">{{formData.clubName}}</span>
                </div>
              </div>
              </div>

              
              <div class="general-information text-left">
                <div class="card-element card-name">
                  <span class="card-title">Licence : </span>
                  <span class="card-input dafont" id="cardName">{{formData.licenceNum}}</span>
                </div>
                <div class="card-element college-name">
                  <span class="card-title">Groupe Sanguin : </span>
                  <span class="card-input dafont" id="cardCollegeName">{{formData.groupeSanguin}}</span>
                </div>
                <div class="card-element college-name">
                  <span class="card-title">Email : </span>
                  <span class="card-input dafont" id="cardLocation">{{formData.email}}</span>
                </div>
                <div class="card-element college-name">
                  <span class="card-title">Téléphone : </span>
                  <span class="card-input dafont" id="cardNumber">{{formData.phoneNum}}</span>
              </div>
                <div class="card-element college-name">
                  <span class="card-title">Adresse : </span>
                  <span class="card-input dafont" id="cardNumber">{{formData.locationName}}</span>
              </div>
            
          </div>

          
          </div>
        </div>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: 'GeneratedCard',
  props: {
      formData: Object
  }
}
</script>












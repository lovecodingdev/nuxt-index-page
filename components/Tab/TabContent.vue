<template>
  <div id="panels" class="relative">
    <Tab1
      :active="openTab === tabs[0].id"
      :title="tabs[0].title"
      :steps="tabs[0].steps"
    />
    <Tab2
      :active="openTab === tabs[1].id"
      :title="tabs[1].title"
      :steps="tabs[1].steps"
    />
    <Tab3
      :active="openTab === tabs[2].id"
      :title="tabs[2].title"
      :steps="tabs[2].steps"
    />
  </div>
</template>
<script>

export default {
  props: ['openTab'],
  data() {
    return {
      tabs: [
        {
          id: 1,
          title: "Drei einfache Schritte zu deinem neuen Job",
          steps: [
            {
              id: 1, 
              desc: "Erstellen dein Unternehmensprofil",
              img: "/img/undraw_Profile_data_re_v81r.svg"
            },
            {
              id: 2, 
              desc: "Erstellen dein Unternehmensprofil",
              img: "/img/undraw_task_31wc.svg"
            },
            {
              id: 3, 
              desc: "Erstellen dein Unternehmensprofil",
              img: "/img/undraw_personal_file_222m.svg"
            },
          ]
        },
        {
          id: 2,
          title: "Drei einfache Schritte zu deinem neuen Mitarbeiter",
          steps: [
            {
              id: 1, 
              desc: "Erstellen dein Unternehmensprofil",
              img: "/img/undraw_Profile_data_re_v81r.svg"
            },
            {
              id: 2, 
              desc: "Erstellen ein Jobinserat",
              img: "/img/undraw_about_me_wa29.svg"
            },
            {
              id: 3, 
              desc: "Wähle deinen neuen Mitarbeiter aus",
              img: "/img/undraw_swipe_profiles1_i6mr.svg"
            },
          ]
        },
        {
          id: 3,
          title: "Drei einfache Schritte zur Vermittlung neuer Mitarbeiter",
          steps: [
            {
              id: 1, 
              desc: "Erstellen dein Unternehmensprofil",
              img: "/img/undraw_Profile_data_re_v81r.svg"
            },
            {
              id: 2, 
              desc: "Erhalte Vermittlungs- angebot von Arbeitgeber",
              img: "/img/undraw_job_offers_kw5d.svg"
            },
            {
              id: 3, 
              desc: "Vermittlung nach Provision oder Stundenlohn",
              img: "/img/undraw_business_deal_cpi9.svg"
            },
          ]
        }
      ]
    }
  }
}
</script>

<style>
#panels {
  /* top: 781px; */
  width: 360px;
  /* height: 956px; */
  opacity: 1;
  margin: 0px auto;
}

#panels > .circle-1 {
  position: absolute;
  top: 127px;
  left: -34px;
  width: 208px;
  height: 208px;
  border-radius: 50%;
  background: #F7FAFC 0% 0% no-repeat padding-box;
  opacity: 0.5;
}

#panels > .circle-3 {
  position: absolute;
  top: 629px;
  left: -54px;
  width: 304px;
  height: 303px;
  border-radius: 50%;
  background: #F7FAFC 0% 0% no-repeat padding-box;
  opacity: 1;
}

.tab-content {
  position: relative;
  display: none;
  width: 360px;
  /* height: 956px; */
  opacity: 1;
}
</style>
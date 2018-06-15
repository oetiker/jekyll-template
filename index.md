---
layout: default
title: Home
---

# Hello World

Bla Bla Bla

<div class="container omniad">
    <div class="row">
       <div class="features col s12">
           <div class="row">
               <div class="col s12">
                   <h3>Key Features</h3>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-database"></i>
		       <span class="card-title">Storage Platform</span>
                       <p>
ZFS, OmniOS' native file-system, combines a volume manager and file-system with strong data-integrity protection. Easily share volumes via iSCSI, CIFS and NFS.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-clone"></i>
                       <span class="card-title">Lightweight Virtualisation</span>
                       <p>
Run lightweight OmniOS or Linux virtual machines in containers without the
overhead of a traditional hypervisor and with full resource control.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="fas fa-lg fa-pull-left fa-clone"></i>
                       <span class="card-title">Hardware Virtualisation</span>
                       <p>
OmniOS also provides full hardware virtualisation via KVM for running guests
such as Microsoft Windows, FreeBSD and many others.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-sitemap"></i>
                       <span class="card-title">Software-Defined Networking</span>
                       <p>
Virtualise your network infrastructure through Crossbow
virtual interfaces and switches and even allocate dedicated resources for
specific services.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-stethoscope"></i>
                       <span class="card-title">In-depth Tracing</span>
                       <p>
DTrace provides a comprehensive dynamic tracing framework to aid
troubleshooting across the whole software stack. Always available,
instrument anything on demand.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="fab fa-lg fa-pull-left fa-github"></i>
                       <span class="card-title">Open Source</span>
                       <p>
OmniOS is open-source, self-hosting and maintained on GitHub. All development
is done out in the open with pull-requests and anyone can grab the source and
build OmniOS themselves.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-fire-extinguisher"></i>
                       <span class="card-title">Commercial Support</span>
                       <p>
Commercial support packages are available to provide custom assistance
and direct access to the OmniOS developers in case of any problems.
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-fighter-jet"></i>
                       <span class="card-title">Rapid Deployment</span>
                       <p>
OmniOS' revolutionary installation framework - Kayak - is blindingly fast,
whether installing 100s of servers over the network or just building a single
VM (in less than 2 minutes).
                       </p>
                  </div>
                  </div>
               </div>
               <div class="col s12 m12 l6 xl4">
                  <div class="card">
                  <div class="card-content">
                       <i class="far fa-lg fa-pull-left fa-cogs"></i>
                       <span class="card-title">Seamless Updates</span>
                       <p>
Easily manage installed packages with digitally-signed updates. LTS releases
receive updates for three years so you can schedule upgrades when convenient.
                       </p>
                  </div>
                  </div>
               </div>
           </div>
        </div>
    </div>
</div>

<script>
jQuery(document).ready(function(){
    var resizer = function (){
        var width = jQuery(window).width();
        var height = 0;
        var cards = jQuery('.features .row .col .card');
        cards.css('height','auto');
        if (width < 600){
            return;
        }
        cards.each(function(){
            height = Math.max(height,$(this).height());
            return this;
        })
        .css('height',height);
    };
    resizer();
    jQuery(window).on('resize',resizer);
});
</script>

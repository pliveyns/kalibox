# kalibox

## Description

Customized toolbox/distrobox container for Kali Linux Rolling.

Based on Universal Blue's boxkit: https://github.com/ublue-os/boxkit

### Create Box

If you use distrobox:

    distrobox create -i ghcr.io/pliveyns/kalibox -n kalibox
    distrobox enter kalibox
    
If you use toolbx:

    toolbox create -i ghcr.io/pliveynss/kalibox -c kalibox
    toolbox enter boxkit

### Pull down your config

Use `chezmoi` to pull down your dotfiles and set up git sync.


### Make your own

The user experience is much nicer if you [set your terminal open right in the container](https://distrobox.privatedns.org/useful_tips/#using-distrobox-as-main-cli) and is the intended experience. 

Check out the amazing projects    
Universal Blue: https://universal-blue.org/    
Blue Build: https://blue-build.org/

## Verification

These images are signed with sisgstore's [cosign](https://docs.sigstore.dev/cosign/overview/). You can verify the signature by downloading the `cosign.pub` key from this repo and running the following command:

    cosign verify --key cosign.pub ghcr.io/pliveyns/kalibox


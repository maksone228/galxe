const elementsToClick = document.querySelectorAll("div[data-state=\"closed\"] .cursor-pointer");
function clickElement(_0x3d1f2b) {
  const _0x11d130 = new MouseEvent("click", {
    view: window,
    bubbles: true,
    cancelable: true
  });
  _0x3d1f2b.dispatchEvent(_0x11d130);
}
function closePopup() {
  const _0x3a861c = document.querySelector("button.absolute.rounded-sm.opacity-70.right-5.top-6.sm\\:right-9.sm\\:top-9");
  if (_0x3a861c) {
    clickElement(_0x3a861c);
    console.log("Popup closed.");
  }
}
function checkClaimButton() {
  const _0x14d370 = document.querySelector("button.bg-primary:not([disabled]).w-full");
  if (_0x14d370) {
    clickElement(_0x14d370);
    console.log("Claim button clicked. Subscribe: https://t.me/h0ld_er");
    setTimeout(closePopup, 2000);
    return true;
  }
  return false;
}
function checkConditionsAndRetry() {
  const _0x1fd4cd = document.querySelectorAll(".text-size-14.font-bold");
  const _0x1ca349 = document.querySelectorAll("svg[data-state=\"closed\"] .ml-4.flex.gap-4.items-center");
  if (_0x1fd4cd.length > 0 || _0x1ca349.length !== elementsToClick.length) {
    setTimeout(processElements, 60000);
  } else {
    checkClaimButton();
  }
}
function processElements() {
  alert("Galxe Auto Complete tasks – H0LD_ER\n\nSubscribe: https://t.me/h0ld_er");
  if (!checkClaimButton()) {
    elementsToClick.forEach(clickElement);
    setTimeout(() => {
      const _0x522696 = document.querySelectorAll("button[data-state=\"closed\"] svg");
      _0x522696.forEach(clickElement);
      setTimeout(checkConditionsAndRetry, 2000);
    }, 2000);
  } else {
    alert("All tasks has been completed!\n\nSubscribe: https://t.me/h0ld_er");
  }
}
processElements();

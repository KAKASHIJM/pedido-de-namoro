<!DOCTYPE html>
<html lang="pt-BR"><head><meta charset="UTF-8"><meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover"><meta name="theme-color" content="#310009"><title>Uma pergunta para você ❤️</title>
<style>
[hidden]{display:none!important}*{box-sizing:border-box}html,body{margin:0;min-height:100%;font-family:Arial,sans-serif}body{min-height:100vh;min-height:100svh;min-height:100dvh;display:grid;place-items:center;background:#310009;overflow-x:hidden;overflow-y:auto;padding:22px;padding:max(18px,env(safe-area-inset-top)) max(18px,env(safe-area-inset-right)) max(18px,env(safe-area-inset-bottom)) max(18px,env(safe-area-inset-left));color:#302633;background-image:radial-gradient(ellipse at 50% 35%,#650b26 0%,#310009 60%,#170006 100%)}
#hearts{position:fixed;inset:0;overflow:hidden;pointer-events:none}.heart{position:absolute;color:#ff346c;filter:drop-shadow(0 0 7px #ff0057);animation:float var(--duration) linear infinite;animation-delay:var(--delay);opacity:0;font-size:var(--size);left:var(--x)}@keyframes float{0%{transform:translateY(108vh) rotate(-15deg);opacity:0}12%,85%{opacity:var(--opacity)}100%{transform:translateY(-15vh) rotate(22deg);opacity:0}}
.card{position:relative;width:min(100%,580px);min-height:365px;border-radius:40px;background:#eae6fc;box-shadow:0 20px 80px #0005,0 0 0 1px #fff6;padding:30px 25px 25px;text-align:center;z-index:1}.bear{display:block;width:145px;height:157px;margin:0 auto 16px;animation:breathe 2.6s ease-in-out infinite;transform-origin:50% 100%}@keyframes breathe{50%{transform:translateY(-3px) rotate(2deg)}}h1{font-size:clamp(19px,4.5vw,24px);line-height:1.4;margin:0 0 12px;font-weight:700}.note{color:#b32350;font-size:13px;min-height:20px;margin:0 0 12px;line-height:1.5}.choices{display:flex;justify-content:center;gap:14px;min-height:44px}button{touch-action:manipulation;-webkit-tap-highlight-color:transparent;user-select:none;-webkit-user-select:none;border:0;border-radius:5px;color:#fff;font-weight:700;font-size:14px;min-width:98px;min-height:48px;padding:12px 22px;cursor:pointer;box-shadow:0 3px 5px #0002}button:focus-visible{outline:3px solid #5f2e96;outline-offset:4px}#yes{background:#2fbc59}#yes:hover{background:#239d47}#no{background:#d92350;z-index:5}#no:hover{background:#c01c45}.accepted .bear{animation:happy .6s ease-in-out infinite alternate}@keyframes happy{to{transform:translateY(-9px) rotate(-5deg)}}#restart{display:none;background:#8d548a;margin:6px auto 0;min-width:130px}.accepted #restart{display:block}.signature{font-size:11px;color:#a184a0;margin:17px 0 0;letter-spacing:.06em}
@media(max-width:480px){.card{border-radius:30px;padding:25px 18px;min-height:355px}.bear{width:135px;height:147px}}@media(max-height:480px){.card{min-height:0;padding:15px}.bear{width:85px;height:92px;margin-bottom:6px}h1{font-size:18px}.signature{display:none}}
@media(prefers-reduced-motion:reduce){.heart,.bear,.accepted .bear{animation:none}.heart{top:var(--y);opacity:.35}}

/* Fluid layout: narrow phones, tablets, desktop and short landscape screens. */
html{-webkit-text-size-adjust:100%;text-size-adjust:100%}
body{display:flex;justify-content:center;align-items:center;padding:clamp(12px,3.5vw,32px);padding-top:max(clamp(12px,3.5vw,32px),env(safe-area-inset-top));padding-bottom:max(clamp(12px,3.5vw,32px),env(safe-area-inset-bottom));padding-left:max(clamp(12px,3.5vw,32px),env(safe-area-inset-left));padding-right:max(clamp(12px,3.5vw,32px),env(safe-area-inset-right))}
.card{flex:0 1 580px;min-width:0;min-height:0;margin:auto;padding:clamp(20px,4.5vw,36px);border-radius:clamp(24px,5vw,40px);display:grid;grid-template-areas:"bear" "question" "message" "choices" "restart" "signature";justify-items:center;row-gap:12px}
.bear{grid-area:bear;width:clamp(105px,27vw,155px);height:auto;aspect-ratio:180/195;margin:0 0 4px;max-width:100%}
h1{grid-area:question;max-width:100%;margin:0;font-size:clamp(18px,4.8vw,25px);overflow-wrap:anywhere;text-wrap:balance}
.note{grid-area:message;margin:0;min-height:40px;font-size:clamp(12px,3vw,14px);max-width:100%;overflow-wrap:anywhere}
.choices{grid-area:choices;width:100%;flex-wrap:wrap;gap:clamp(10px,3vw,18px);min-height:48px}
button{max-width:100%;min-width:88px;min-height:48px;font-size:clamp(13px,3vw,15px);padding:12px clamp(18px,5vw,30px)}
#restart{grid-area:restart;margin:0}.signature{grid-area:signature;display:block;margin:2px 0 0;line-height:1.5}
@media(min-width:768px){.card{padding:38px 44px;row-gap:16px}.bear{width:160px}}
@media(max-height:500px) and (min-width:480px){
 .card{flex-basis:650px;grid-template-columns:minmax(110px,.7fr) minmax(0,1.5fr);grid-template-areas:"bear question" "bear message" "bear choices" "bear restart" "signature signature";padding:18px 24px;column-gap:24px;row-gap:9px}
 .bear{width:clamp(100px,22vh,145px);align-self:center}h1{font-size:clamp(18px,3vw,23px)}.note{min-height:24px}.signature{font-size:10px}
}
@media(max-width:320px){.card{padding:20px 14px;row-gap:10px}.bear{width:105px}.choices{gap:10px}button{min-width:84px;padding:12px 18px}}
@media(max-height:360px){body{align-items:flex-start}.card{margin-block:0}.signature{display:none}}

.summary{list-style:none;padding:0;margin:0;width:100%;text-align:left;display:grid;gap:10px}.summary[hidden]{display:none}.summary li{display:flex;justify-content:space-between;gap:16px;background:#fff7;padding:12px 14px;border-radius:12px;font-size:14px;line-height:1.4}.summary strong{color:#9a2450;white-space:nowrap}
</style></head><body>
<noscript><p style="position:fixed;inset:15px 15px auto;z-index:20;background:white;padding:16px;border-radius:12px">Abra este arquivo em um navegador com JavaScript ativado para os botões funcionarem.</p></noscript>
<div id="hearts" aria-hidden="true"></div>
<main class="card" id="card">
<svg class="bear" viewBox="0 0 180 195" role="img" aria-label="Ursinho fofo segurando uma rosa vermelha">
<defs><radialGradient id="fur" cx="35%" cy="25%" r="85%"><stop stop-color="#dba991"/><stop offset="1" stop-color="#bc846d"/></radialGradient></defs>
<g stroke="#674038" stroke-width="3" stroke-linejoin="round">
<circle cx="48" cy="30" r="17" fill="#c79179"/><circle cx="132" cy="30" r="17" fill="#c79179"/><circle cx="48" cy="30" r="9" fill="#8a574c"/><circle cx="132" cy="30" r="9" fill="#8a574c"/>
<path d="M61 121 Q43 137 47 174 L45 191 H132 L130 168 Q139 147 121 124" fill="url(#fur)"/>
<path d="M32 75 C29 33 57 19 89 20 C126 18 150 41 149 77 C153 110 135 138 91 140 C52 140 29 116 32 75Z" fill="url(#fur)"/>
<path d="M120 145 Q147 140 143 155 Q140 168 125 163" fill="#c79179"/>
</g>
<ellipse cx="54" cy="105" rx="14" ry="10" fill="#efb28e"/><ellipse cx="125" cy="105" rx="14" ry="10" fill="#efb28e"/>
<ellipse cx="66" cy="88" rx="4.5" ry="5.5" fill="#4c2c2d"/><ellipse cx="113" cy="88" rx="4.5" ry="5.5" fill="#4c2c2d"/>
<circle cx="67" cy="86" r="1.2" fill="#fff"/><circle cx="114" cy="86" r="1.2" fill="#fff"/>
<path d="M85 96 Q90 91 95 96 Q91 104 85 96" fill="#613a34"/><path d="M90 100 Q85 108 80 101 M90 100 Q95 108 100 101" stroke="#613a34" stroke-width="2" fill="none" stroke-linecap="round"/>
<path d="M53 173 Q51 139 44 111" fill="none" stroke="#4f7048" stroke-width="4"/><path d="M49 145 Q31 145 33 132 Q46 131 49 145 M51 153 Q66 139 70 148 Q65 158 51 153" fill="#70945d" stroke="#4e7046" stroke-width="2"/>
<path d="M43 118 C24 115 24 102 30 98 C26 86 41 84 47 89 C60 83 66 96 61 104 C64 114 51 122 43 118Z" fill="#e95b75" stroke="#793347" stroke-width="2"/>
<path d="M32 98 Q44 105 55 93 M33 110 Q54 112 55 100 Q43 92 40 99 Q37 109 50 110 M43 89 Q40 94 46 98" fill="none" stroke="#943247" stroke-width="2"/>
<ellipse cx="52" cy="156" rx="14" ry="10" transform="rotate(-18 52 156)" fill="#d5a088" stroke="#674038" stroke-width="2.5"/>
<path d="M153 49 C144 40 137 52 153 62 C169 51 160 41 153 49" fill="#e14368" stroke="none"/>
</svg>
<h1 id="question">Você aceita ser minha namorada?</h1>
<p class="note" id="message" role="status" aria-live="polite">Tenho uma pergunta especial para você… ❤️</p>
<div class="choices" id="choices"><button id="yes" type="button">SIM</button><button id="no" type="button">NÃO</button><ul class="summary" id="summary" aria-label="Suas respostas" hidden></ul></div>
<button id="restart" type="button">Ver de novo</button>
<p class="signature">Com carinho, para você ♡</p>
</main>
<script>
'use strict';
const hearts=document.getElementById('hearts'),card=document.getElementById('card'),yes=document.getElementById('yes'),no=document.getElementById('no'),message=document.getElementById('message'),question=document.getElementById('question');
for(let i=0;i<45;i++){const h=document.createElement('span');h.className='heart';h.textContent=i%4?'♥':'✦';h.style.cssText='--x:'+Math.random()*100+'%;--y:'+Math.random()*100+'%;--size:'+(10+Math.random()*23)+'px;--duration:'+(8+Math.random()*13)+'s;--delay:-'+Math.random()*21+'s;--opacity:'+(.2+Math.random()*.6);hearts.appendChild(h);}
let accepted=false,moved=false,attempts=0,lastEscape=-Infinity;
let step=-1;
const answers=[];
const followups=[
 {question:'Quer ir ao cinema comigo? 🎬',label:'Cinema juntos'},
 {question:'Topa um jantar a dois? 🍕',label:'Jantar a dois'},
 {question:'Vamos passear juntinhos? 🌷',label:'Passeio juntos'},
 {question:'Posso te surpreender com um encontro especial? 🎁',label:'Encontro surpresa'},
 {question:'Topa tomar um sorvete comigo? 🍦',label:'Sorvete juntos'},
 {question:'Vamos assistir ao pôr do sol juntinhos? 🌅',label:'Pôr do sol'},
 {question:'Quer fazer uma maratona de filmes comigo? 🍿',label:'Maratona de filmes'},
 {question:'Topa cozinhar uma receita comigo? 👩‍🍳',label:'Cozinhar juntos'},
 {question:'Vamos tirar uma foto bem fofa juntos? 📸',label:'Foto juntos'},
 {question:'Quer montar uma playlist só nossa? 🎶',label:'Nossa playlist'},
 {question:'Topa um piquenique comigo? 🧺',label:'Piquenique'},
 {question:'Posso te dar um abraço bem apertado? 🥰',label:'Abraço apertado'}
];
const summary=document.getElementById('summary');
const phrases=['Tem certeza? 🥺','Olha lá, hein… ❤️','Dá mais uma pensadinha…','Acho que você clicou errado… 😅','O SIM está te esperando! 💚'];
function escapeNo(event){
 if(accepted)return;
 if(event&&event.cancelable)event.preventDefault();
 const now=Date.now();if(event&&now-lastEscape<180)return;lastEscape=now;
 const old=no.getBoundingClientRect(),safe=yes.getBoundingClientRect(),pad=12,w=old.width,h=old.height;
 const vv=window.visualViewport;
 const viewX=vv?vv.offsetLeft:0,viewY=vv?vv.offsetTop:0;
 const minX=viewX+pad,minY=viewY+pad;
 const maxX=Math.max(minX,viewX+(vv?vv.width:innerWidth)-w-pad);
 const maxY=Math.max(minY,viewY+(vv?vv.height:innerHeight)-h-pad);
 let best={x:minX,y:minY},score=-Infinity;
 for(let i=0;i<80;i++){
 const x=minX+Math.random()*(maxX-minX),y=minY+Math.random()*(maxY-minY);
 if(x<safe.right+18&&x+w>safe.left-18&&y<safe.bottom+18&&y+h>safe.top-18)continue;
 const px=event&&Number.isFinite(event.clientX)?event.clientX:old.left+w/2,py=event&&Number.isFinite(event.clientY)?event.clientY:old.top+h/2;
 const d=Math.hypot(x+w/2-px,y+h/2-py);if(d>score){best={x,y};score=d;}
 }
 if(!moved){document.body.appendChild(no);moved=true;}
 Object.assign(no.style,{position:'fixed',left:best.x+'px',top:best.y+'px',margin:'0'});
 message.textContent=phrases[attempts++%phrases.length];
}
if('PointerEvent' in window){
 no.addEventListener('pointerenter',event=>{if(event.pointerType==='mouse')escapeNo(event);});
 no.addEventListener('pointerdown',escapeNo);
}else{
 no.addEventListener('mouseenter',escapeNo);
 no.addEventListener('touchstart',event=>{if(accepted)return;const t=event.touches[0];if(event.cancelable)event.preventDefault();escapeNo({clientX:t.clientX,clientY:t.clientY});},{passive:false});
}
no.addEventListener('click',event=>{if(accepted)reply(false);else escapeNo(event);});
if(window.visualViewport)window.visualViewport.addEventListener('resize',()=>{if(moved&&!accepted)escapeNo();});
addEventListener('resize',()=>{if(moved&&!accepted)escapeNo();});
function dockNo(){no.removeAttribute('style');document.getElementById('choices').appendChild(no);moved=false;}
function showStep(){
 if(step>=followups.length){
  yes.hidden=true;no.hidden=true;summary.hidden=false;
  question.textContent='Nosso próximo capítulo! ❤️';message.textContent='Suas respostas ficaram assim. Vamos combinar os detalhes juntos!';
  summary.replaceChildren();
  followups.forEach((item,i)=>{const li=document.createElement('li'),label=document.createElement('span'),value=document.createElement('strong');label.textContent=item.label;value.textContent=answers[i]?'Sim ❤️':'Não';li.appendChild(label);li.appendChild(value);summary.appendChild(li);});
  document.getElementById('restart').hidden=false;
  return;
 }
 question.textContent=followups[step].question;
 message.textContent=(step===0?'Você me fez muito feliz! ❤️ · ':'')+'Pergunta '+(step+1)+' de '+followups.length;
 yes.hidden=false;no.hidden=false;summary.hidden=true;
}
function reply(value){if(!accepted||step>=followups.length)return;answers.push(value);step++;showStep();}
yes.onclick=()=>{
 if(accepted){reply(true);return;}
 accepted=true;step=0;dockNo();card.classList.add('accepted');document.getElementById('restart').hidden=true;showStep();
};
document.getElementById('restart').onclick=()=>{
 accepted=false;attempts=0;step=-1;answers.length=0;summary.replaceChildren();summary.hidden=true;moved=false;lastEscape=-Infinity;dockNo();no.hidden=false;yes.hidden=false;card.classList.remove('accepted');document.getElementById('restart').hidden=false;question.textContent='Você aceita ser minha namorada?';message.textContent='Tenho uma pergunta especial para você… ❤️';
};
</script></body></html>

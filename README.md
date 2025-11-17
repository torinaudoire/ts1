<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Miss Mu and the Canary</title>

<style>
    body {
        font-family: system-ui, sans-serif;
        max-width: 700px;
        margin: 40px auto;
        line-height: 1.6;
        padding: 0 15px;
    }

  /* Footnote marker */
.fn {
    color: #005bbb;
    cursor: pointer;
    font-weight: normal;     
    font-size: 1em;       
    vertical-align: super;
    margin-left: 2px;
    text-decoration: none;   /* no underline */
}

    }

    /* Hidden panel container */
    .footnote-panel {
        max-height: 0;
        overflow: hidden;
        background: #f0f4ff;
        border-left: 3px solid #005bbb;
        padding: 0 12px;
        margin: 6px 0 12px;
        transition: max-height 0.25s ease, padding 0.25s ease;
    }

    /* Active (expanded) state */
    .footnote-panel.open {
        padding: 12px;
        max-height: 300px; /* Enough for several lines; can increase */
    }

    .footnote-label {
        font-size: 0.85em;
        font-weight: bold;
    }
</style>
</head>

<body>

<h1>Miss Mu and the Canary</h1>

<p>
“<span class="fn" data-fn="1">Yan’er</span>, I’m not like you. I was sold into this cesspit when I was ten years old. I’ve seen everything there is to see. In a place as dark and corrupt as this, for whores and clients alike, the rarest treasure is a taste of true affection. How happy you were when you were with her – I saw it all.” Fei Hua spoke clearly and deliberately. “But love can’t be eaten at the end of the day. Never mind her reasons for deceiving you – even if she really has feelings for you, what kind of future can you have together? She might keep you for a time, even buy your freedom from this place. But she’s the eldest daughter of the Mu family. Eventually the day will come when she must marry. If it were to a man, he might take you as a <span class="fn" data-fn="2">concubine</span>… But would you really marry into his household along with her? Then what would you do? Come back here to the brothel?”
</p>

<p>
The hand holding the letter tightened abruptly. The paper could not withstand the force, and began to crumple inch by inch.
</p>

<p>Yes… Bai Yan thought absently. Were these days of anguish because she couldn’t accept Mu Xing’s gender? Or because she was wounded by Mu Xing’s betrayal? Or was it that…?</p>

<p>Mu Xing… was getting married.</p>

<p>No matter how she felt or how Mu Xing felt, that opulent wedding gown had made the choice for both of them long ago, hadn’t it?</p>

<p>Fei Hua patted her shoulder and spoke each word carefully: “They say whores are heartless and actors faithless. Yan’er, whether you can accept her or not, think about your original intentions. We don’t take clients for love and sentiment. At such a crucial moment, don’t go astray. Miss Mu can act without restraint, but for you and me, there’s long since been no such second path.”</p>

<p>Bai Yan stared blankly into space for a moment, and then let out a mocking laugh.</p>

<p>
That was right. She, too, hadn’t gotten close to Mu Xing out of love; she had only <span class="fn" data-fn="3">found a stage upon which to act out her performance</span>. It was true that Mu Xing had lied to her, but had she herself been sincere from the beginning?
</p>

<p>How could she have forgotten? Her original motive had simply been to find some kind of refuge.</p>

<p>
Once, she had been able to use that nobleman’s name as a stepping stone without regard for face or feeling; had discarded <span class="fn" data-fn="4">Cui-shaoye</span> with no hesitation; now, surely, she could do so again.
</p>

<p>
No matter how humiliating the ending of this farce might be, Mu Xing could still escape unscathed, return to her <span class="fn" data-fn="5">unassailable</span> life, clad herself in wedding finery, and become someone else’s wife.
</p>

<p>And what about Bai Yan? What would she be left with in the end?</p>

<p>A wedding dress, a ring, and a memory without closure?</p>

<p>At least this affair ending here meant she could still keep the sweetness of the past, and in the dark days to come might avail herself of its comfort.</p>

<!-- Footnote panels -->
<div id="footnote-1" class="footnote-panel">
    艳儿 Yan'er, a diminutive and affectionate nickname for Bai Yan.
</div>

<div id="footnote-2" class="footnote-panel">
    In the Republican era it was still legal for men to take additional concubines alongside their primary wife, but concubines were of lower status. Many elite families viewed the practice as old-fashioned compared to increasingly popular Western monogamy.
</div>

<div id="footnote-3" class="footnote-panel">
    逢场作戏 (“find a stage and put on a show”). An idiom referring to performing, playing along, or going through the motions without true feeling.
</div>

<div id="footnote-4" class="footnote-panel">
    少爷, a polite form of address for the young master of a wealthy or noble family.
</div>

<div id="footnote-5" class="footnote-panel">
    固若金汤 (“solid as metal walls and boiling soup”), meaning firmly protected or unassailable.
</div>

<script>
    // Toggle corresponding panel
    document.querySelectorAll('.fn').forEach(marker => {
        marker.addEventListener('click', () => {
            const num = marker.dataset.fn;
            const panel = document.getElementById('footnote-' + num);

            // close others
            document.querySelectorAll('.footnote-panel').forEach(p => {
                if (p !== panel) p.classList.remove('open');
            });

            // toggle this one
            panel.classList.toggle('open');

            // scroll into view if needed
            if (panel.classList.contains('open')) {
                setTimeout(() => panel.scrollIntoView({ behavior: 'smooth', block: 'start' }), 200);
            }
        });
    });
</script>

</body>
</html>

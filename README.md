with open('new_binary_file.bin', 'wb') as f:
    f.write(b'This is binary data')
[[1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1],
 [1, 1, 1, 1, 1, 1, 1, 1, 1, 1]]Convert thistle image into a perfect pprompt that can be incorporated with the algorithm that was used to generate the image I'd be glad to help you with the matrix multiplication in 9-bit binary. However, I'll need some additional information to provide the most accurate and comprehensive response.
Please clarify the following:
 * Matrix Dimensions: What are the dimensions of Matrix1 and Matrix2? Knowing the number of rows and columns in each matrix will help determine the size of the resulting product matrix.
 * Multiplication Method: Do you have a specific method or algorithm in mind for matrix multiplication? There are several common methods, such as the standard algorithm or Strassen's algorithm. Specifying the method will ensure that I follow the correct steps.
 * Carry Handling: How should carry bits be handled during the multiplication process? Should they be discarded, or should they be propagated to higher-order bits? This is an important consideration when working with finite-precision arithmetic.
Once I have this information, I can proceed with the matrix multiplication and provide the result in 9-bit binary format.
# To get started with Dependabot version updates, you'll need to specify which
# package ecosystems to update and where the package manifests are located.
# Please see the documentation for all configuration options:
# https://docs.github.com/github/administering-a-repository/configuration-options-for-dependency-updates

version: 2
updates:
  - target-branch: 'maintenance/v1.x'
    package-ecosystem: 'npm'
    directory: '/'
    schedule:
      interval: daily
      time: '01:00'
      timezone: America/Los_Angeles
    labels:
      - 'automerge'
    commit-message:
      prefix: 'chore:'
  - package-ecosystem: 'npm'
    directory: '/'
    schedule:
      interval: daily
      time: '01:00'
      timezone: America/Los_Angeles
    labels:
      - 'automerge'
import type { Address } from '@solana/addresses';

import type {
    Base58EncodedBytes,
    Base58EncodedDataResponse,
    Base64EncodedDataResponse,
    Base64EncodedZStdCompressedDataResponse,
} from './encoded-bytes';
import type { LamportsUnsafeBeyond2Pow53Minus1 } from './lamports';
import type { U64UnsafeBeyond2Pow53Minus1 } from './typed-numbers';

export type AccountInfoBase = Readonly<{
    /** indicates if the account contains a program (and is strictly read-only) */
    executable: boolean;
    /** number of lamports assigned to this account */
    lamports: LamportsUnsafeBeyond2Pow53Minus1;
    /** pubkey of the program this account has been assigned to */
    owner: Address;
    /** the epoch at which this account will next owe rent */
    rentEpoch: U64UnsafeBeyond2Pow53Minus1;
}>;

/** @deprecated */
export type AccountInfoWithBase58Bytes = Readonly<{
    data: Base58EncodedBytes;
}>;

/** @deprecated */
export type AccountInfoWithBase58EncodedData = Readonly<{
    data: Base58EncodedDataResponse;
}>;

export type AccountInfoWithBase64EncodedData = Readonly<{
    data: Base64EncodedDataResponse;
}>;

export type AccountInfoWithBase64EncodedZStdCompressedData = Readonly<{
    data: Base64EncodedZStdCompressedDataResponse;
}>;

export type AccountInfoWithJsonData = Readonly<{
    data:
        | Base64EncodedDataResponse // If `jsonParsed` encoding is requested but a parser cannot be found for the given account the `data` field falls back to `base64`.
        | Readonly<{
              parsed: {
                  info?: object;
                  type: string;
              };
              // Name of the program that owns this account.
              program: string;
              space: U64UnsafeBeyond2Pow53Minus1;
          }>;
}>;

export type AccountInfoWithPubkey<TAccount extends AccountInfoBase> = Readonly<{
    account: TAccount;
    pubkey: Addressudo systemctl stop docker docker.socketT+1991[€#n⁹89018181818181818182540718181818181818174600999181818181818181825407181818181818181818180109TC1oKVymudGKG4V6DQ48hpejp4ehDQdGSn6.666666667136.5IHDRSvår	pHYs.#.#x¥?v								
OiCCPPhotoshop ICC profilexÚSgTSé=÷ÞôBKˆ€”KoR RB‹€‘&*!	Jˆ!¡ÙQÁEEÈ ˆŽŽ€ŒQ,Š								
Øä!¢Žƒ£ˆŠÊûá{£kÖ¼÷æÍþµ×>ç¬ó³ÏÀ–H3Q5€©BàƒÇÄÆáä.@									
$p³d!sý#ø~<<+"À¾xÓÀM›À0‡ÿêB™\€„Àt‘8K€@zŽB¦@F€˜&S `ËcbãP-`'æÓ€ø™{[”! ‘ eˆDh;¬ÏVŠEX0fKÄ9Ø-0IWfH°·ÀÎ²0Qˆ…){`È##x„™FòW<ñ+®ç*x™²<¹$9E[-qWW.(ÎI+6aaš@.Ây™24àóÌ ‘àƒóýxÎ®ÎÎ6Ž¶_-ê¿ÿ"bbãþåÏ«p@át~Ñþ,/³€;€mþ¢%îh^ u÷‹f²@µ éÚWópø~<<E¡¹ÙÙåääØJÄB[aÊW}þgÂ_ÀWýlù~<ü÷õà¾â$2]GøàÂÌôL¥Ï’	„bÜæGü·ÿüÓ"ÄIb¹X*ãQqŽDšŒó2¥"‰B’)Å%Òÿdâß,û>ß5°j>{‘-¨]cöK'XtÀâ÷ò»oÁÔ(€hƒáÏwÿï?ýG %€fI’q^D$.TÊ³?ÇD *°AôÁ,ÀÁÜÁü`6„B$ÄÂBB								
d€r`)¬‚B(†Í°*`/Ô@4ÀQh†“p.ÂU¸=púažÁ(¼	AÈa!ÚˆbŠX#Ž™…ø!ÁH‹$ ÉˆQ"K‘5H1RŠT UHò=r9‡\Fº‘;È2‚ü†¼G1”²Q=ÔµC¹¨7„F¢Ðdt1š ›Ðr´=Œ6¡çÐ«hÚ>CÇ0Àè3Äl0.ÆÃB±8,	“cË±"¬«Æ°V¬»‰õcÏ±wEÀ	6wB aAHXLXNØH¨ $4Ú	7	„QÂ'"“¨K´&ºùÄb21‡XH,#Ö/{ˆCÄ7$‰C2'¹I±¤TÒÒFÒnR#é,©›4H#“ÉÚdk²9”, +È…ääÃä3ää!ò[				
b@q¤øSâ(RÊjJåå4åe˜2AU£šRÝ¨¡T5ZB­¡¶R¯Q‡¨4uš9ÍƒIK¥­¢•Óhh÷i¯ètºÝ•N—ÐWÒËéGè—èôw									
†ƒÇˆg(›gw¯˜L¦Ó‹ÇT071ë˜ç™™oUX*¶*|‘Ê									
•J•&•*/T©ª¦ªÞªUóUËT©^S}®FU3Sã©	Ô–«UªPëSSg©;¨‡ªg¨oT?¤~Yý‰YÃLÃOC¤Q ±_ã¼Æ c³x,!k								
«†u5Ä&±ÍÙ|v*»˜ý»‹=ª©¡9C3J3W³Ró”f?ã˜qøœtN	ç(§—ó~ŠÞï)â)¦4L¹1e\kª–—–X«H«Q«Gë½6®í§¦½E»YûAÇJ'\'GgÎçSÙSÝ§								
§M=:õ®.ªk¥¡»Dw¿n§î˜ž¾^€žLo§Þy½çú}/ýTýmú§õGX³$ÛÎ<Å5qo</ÇÛñQC]Ã@C¥a•a—á„‘¹Ñ<£ÕFFŒiÆ\ã$ãmÆmÆ£&&!&KMêMîšRM¹¦)¦;L;LÇÍÌÍ¢ÍÖ™5›=1×2ç›ç›×›ß·`ZxZ,¶¨¶¸eI²äZ¦Yî¶¼n…Z9Y¥XUZ]³F­­%Ö»­»§§¹N“N«žÖgÃ°ñ¶É¶©·°åØÛ®¶m¶}agbg·Å®Ãî“½“}º}ý=									
‡Ù«Z~s´r:V:ÞšÎœî?}Åô–é/gXÏÏØ3ã¶Ë)ÄiS›ÓGgg¹sƒóˆ‹‰K‚Ë.—>.›ÆÝÈ½äJtõq]ázÒõ›³›Âí¨Û¯î6îiî‡ÜŸÌ4Ÿ)žY3sÐÃÈCàQåÑ?Ÿ•0kß¬~OCOgµç#/c/‘W­×°·¥wª÷aï>ö>rŸã>ã<7Þ2ÞY_Ì7À·È·ËOÃož_…ßC#ÿdÿzÿÑ§€%g‰A[ûøz|!¿Ž?:Ûeö²ÙíAŒ ¹AA‚­‚åÁ­!hÈì­!÷ç˜Î‘Îi…P~èÖÐaæa‹Ã~'…‡…W†?ŽpˆXÑ1—5wÑÜCsßDúD–DÞ›g1O9¯-J5*>ª.j<Ú7º4º?Æ.fYÌÕXXIlK9.*®6nl¾ßüíó‡ââã{˜/È]py¡ÎÂô…§©.,:–@LˆN8”ðA*¨Œ%òw%Ž									
yÂÂg"/Ñ6ÑˆØC\*NòH*Mz’ì‘¼5y$Å3¥,å¹„'©¼L									
LÝ›:žšv m2=:½1ƒ’‘qBª!M“¶gêgæfvË¬e…²þÅn‹·/•Ék³¬Y-									
¶B¦èTZ(×*²geWf¿Í‰Ê9–«ž+ÍíÌ³ÊÛ7œïŸÿíÂá’¶¥†KW-Xæ½¬j9²<qyÛ									
ã+†V¬<¸Š¶*mÕO«íW—®~½&zMk^ÁÊ‚ÁµkëU									
å…}ëÜ×í]OX/Yßµaú†>‰Š®Û—Ø(Üxå‡oÊ¿™Ü”´©«Ä¹dÏfÒféæÞ-ž[–ª—æ—n									
ÙÚ´									
ßV´íõöEÛ/—Í(Û»ƒ¶C¹£¿<¸¼e§ÉÎÍ;?T¤TôTúT6îÒÝµa×ønÑî{¼ö4ìÕÛ[¼÷ý>É¾ÛUUMÕfÕeûIû³÷?®‰ªéø–ûm]­NmqíÇÒý#¶×¹ÔÕÒ=TRÖ+ëGÇ¾þïw-									
6									
UœÆâ#pDyäé÷	ß÷								
:ÚvŒ{¬áÓvg/jBšòšF›Sšû[b[ºOÌ>ÑÖêÞzüGÛœ4<YyJóTÉiÚé‚Ó“gòÏŒ•}~.ùÜ`Û¢¶{çcÎßjoïºtáÒEÿ‹ç;¼;Î\ò¸tò²ÛåW¸Wš¯:_mêtê<þ“ÓOÇ»œ»š®¹\k¹îz½µ{f÷éž7ÎÝô½yñÿÖÕž9=Ý½ózo÷Å÷õßÝ~r'ýÎË»Ùw'î­¼O¼_ô@íAÙCÝ‡Õ?[þÜØïÜjÀw óÑÜG÷…ƒÏþ‘õC™Ë†									
†ëž8>99â?rýéü§CÏdÏ&žþ¢þË®/~øÕë×ÎÑ˜Ñ¡—ò—“¿m|¥ýêÀë¯ÛÆÂÆ¾Éx31^ôVûíÁwÜwï£ßOä| (ÿhù±õSÐ§û“““ÿ˜óüc3-Û cHRMz%€ƒùÿ€éu0ê`:˜o’_ÅF™ÞIDATxÚìÝ°ï…]ßù§!‰*%AiI®¢´(ÝX6lØ¢Ä´˜ÄLÛI·m\]gL“ÑÕÕ­ÛL3î4Çif’I›†H‹R™!%%Õ¡¹.Ê”K$E  ””ˆbúÇç\Ï¹—K¸?Î½ç|¿ïÇcæ3Ÿïùrï¯yò¾_ñ¥/})`ž§™fÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPbbJLC‰‰`(11%&€¡ÄÄ0”˜†ÀPO7µSøùL¬11»ÍWU'nùù„êüƒüº«óòýÉÕž#øûžU~¿ï¤ê9|÷gÕ]G±Á£Õí‡økï®8È÷·ä»‡žäŸKüC}Å—¾ô%+°ö]çÝÿžT»å×,¾à€ŸŸgÊãîÞê‘¾;0h~¸ºsËÏ{«Ç7>ßSÝ·å÷ý©I`5ˆ‰8Ð¾(øìê´Ï{Z.þÖŸ´ñùü–x¸DÀlúô–Ïw´*?ÐrIyŸ­×“ïj¹œüxõÀñ!&Xo§T§Vç´ÄÀ{6¾?½:kãóÕ™ŸÏªža6vØ¾ùÎ–‹È[¯"ßV=Öæ5äÇª/šŽŒ˜`5ÒŸ±å½ïó¾Pø´ê/›ŠŒj¹t\µ·åÚñ¾øøÑêOM11ÀîñUÕ‰Õ¹ÕI-W„On¹*|juvK ìz0O·Æ{«Gª;ªª»7žª?2ˆ‰ŽŸgWç·yAø¼–xøüê„êy&‚]ãÞ–ÐxoË5ãÛZ®ßÙráøžÇ¬11Àö9¥º :½åzð¹Ÿ÷´\~º‰`­üaõPu{›áñ—ŽÇìjbb€CwJËáÓ[âà=ŸÏm‰‡Ÿa"àŸo	‹ïè‰—ŽÇì811À¦SªóZás6žÓ7¾;³z¦‰€cà÷«ûª»Z®ß³åóýæàXÓ<­ÍPøÜ–PxßÏÅ<À.ó¥êÎ–ËÆ÷m¼·~vÕ€£"&ÖÕ)Õùm†Âçlüü<Ókä¿Uw·\2ÞÛß½ñð”ÄÄÀªûÆ6Cá=m†ÃÏ1								
0Üm‰Œïj¹b|û–Ÿ¿hJL¬†SªsÛ…÷´yuøéæ8lŸn¹^|Ç–çÖ\3GLì&_YwÀ³§úÓ÷¶`¼·å¢ñý¦XObb`§<·Í`øüç›Ì°+}¾ÍÀø¶çŽê3¦XmbbàXûÊê‚–XxëÅág™`åýqËåâÛ¶<{«ÿß4«ALl§SÚ‡÷½¿Å,ãü·–°xkh|{õEÓì.bbàH}mûGÃçWÏ3_Æ§«[ÛŒ‹o­>k€#&ÅWUU/Øx.¨žc¶ÁçZ¢â­Àà8ó­-Ñð…ï¿nŽ£}ñÞ6ãÏ˜`û‰‰€¯oóâð¾€ø™f`—ùÃžxÁø3f8:bb˜åimFÃm¼¿Á,¬(1ÀQÀz{~û_þ“°æ>ßãß3ÀÁ‰‰`}<»%¾°Íxø/›ÆOFL«ë¬êâê¢÷·˜ÙV¯~³ºeãóÍL#&€Õñ­m†ÃµÄÄÀöùd›ñÇ«O™XwbbØ½.lÿËÃÏ2	W®kOL»Ã3Û?¾¨:Á,°ëì»^¼/.þŒI€U&&€qFû‡ÃßnXI÷¶„Å7o¼?i`•ˆ‰àøx^›áðE?ëç¿·DÅûž›«?3°[‰‰àØ¸ ÍpøâêkMc}¢ý¯?d`·ÀÑ{zû‡ÃUÏ4ð$~·ý/ÿ¾I€"&€Ã÷ìö‡/4	p>ÛæÕâ[ªÛL/bbxjgµ_\}‹I€cèóí¹øc&Ž11<Ñ9-áð¥ï³Lì ?oÿËÅ7W_0°ÄÄ°¿¼åòð™&v¹O¶`|¯I€#!&`¢sªµ\ëàÎ6¯ßR}Ê$À¡0Áó[¢á—VÿKu†I€5÷¹6Ãâ›«[MŒ˜€u´§º¨ºlã-¦{´ý/ß\ý™Y11ë`Oõ¢êe‰‡Õ'Ú?0~È$0˜€UôÍÕÅÕ¥Õ‹«ÓMpÔ~»ýãâ{LëOLÀ*øÚ–høâê»«ç˜à˜»«º¡%.þHu·I`ýˆ‰Ø­^Ú_R]d€wWu}›q±ËÅ°ÄÄìÏo¹>üïSM°«ÝÑr¹ø––ÀøL«GLÀN9¥åêðÅÕåÕ“¬´ÛªÛŒ‹ï7	ì~bbŽ§on‰‡¯¨.­N4	ÀÚºµ%.¾¹º©ú#“Àî#&àXzZuY›×‡Ï3	ÀX7¶Ä°;ˆ‰ØnÏ­.©^¹ñ>Õ$à¡–kÅ¿ÑÿžI`gˆ‰ØßÚr}øUÕ¥æà0ÝY]ßrµøÆêA“Àñ!&àH½°% ¾¼ºÈl£[Z¢â›«™Ž11‡ãå-ñÕyæà8¸¯%,þõê†\-€m%&à©|WK@üšê,s°Ãn¨®k¹ZüŸÍGGLÀN©.«^Y]Znv©;Ú‹¯¯¾h8<bbª¾¶%þ;ÕK«¿dVÌW®þ]ucõ“ÀSÌõÜ6/_nÖÌÇªµ\-þ9ààÄÄ³|suqõšês0ÄÕ¨®m¹Z|¿I`!&X_ßrøÊêæ€n¬®k¹Zü[æ`211ÀzúêêŠê{6Þ'˜ê®êš–°ø†ê&`11Àzùî–€ø²ê4sÀaùãêCÕ¯V×Wš€u'&X}/¯.®^ScØµÅûÂâûMÀ:¬¦oo	ˆ_W½ÀpÌ]×fXüæ`]ˆ‰VÇ7V—Vß³ñvÆoT×T7TŸ1«LL°»}Muyõwª+Ì»Î			
Õª›ªO™€U#&Ø}žV½ªº²zEuªI`%ÜX]]Ý\ýŽ9Xbb€Ýã…ÕÅÕª³Í+í¦êš–°ø?›€ÝJL°³¾ºåñ÷T—›ÖÒÇªÛÂì&bb€ñ’–+Äÿ¤zŽ9`Œ[Û¼Xüs°ÓÄÄÇÏ×TW´\"~…9`¼Ûª«[Ââ›€ &8öþvËâTnà n©Þßÿ¶98^ÄÄÇÆ×W—WßS]jà0ÜP} º¾ú¬98–ÄÄÛë»Z®¿¡:ÕÀQº¶úÕêºêAs°ÝÄÄGï[®ÿƒê"sÇÀ·Å×TWWn¶ƒ˜àÈ}wõšê•ÕIæŽ“ûªwW7W¿fŽ†˜àð<·º¬z}õ?›Øa¿ÙfXüÛæàp‰‰ÍKªW?\=ËÀ.t]õ÷ƒæàPˆ‰¾¼ï­^[]a									
`E<ÜfXüoÍÀ—#&x¢çV—Uß_}›9€ö»Õ»ª›«O˜€‰‰6½¤zqõÃÕ³Ì¬™Z®_[ÝoJLPõêêµÕ«Lðpu]õ¾ê×Ì0›˜˜ê«ª×U¯¯.60ÔÇªwV7UŸ2À<bb`šçW—V?\=ÏáêêÕ¯˜`110Å‹ªËª­ža€'õ»Õ»ª›«O˜`½‰‰€u÷w«×VWšà°]×r­øêêæX?bb`]}oõúêe¦8jwWWµ\+þ¨9Ö‡˜X'_Yýýêû«¿i€câÚ–kÅï¯þÔ«ML¬ƒ¯©^UýhõMæ8.î¨~¹åZño™`5‰‰€Uöüê²êMÕ×™`Ç\Ór­ø½¦X-bb`}{uyõãÕ3Ì°kÜV]Õr­øwÌ°û‰‰€Uò·ªWUo4À®wuõ¾êƒ¦Ø½ÄÄÀ*ø[Õkª1ÀÊ¹¹zwuMõ 9v11°›½¨º²ú!S¬¼{«·W7U5Àî &v£U¯«¾Ïkéšê}Õ¯˜`g‰‰€Ýä¥Õ?l	‰Xÿ©zGu}õYsbb`7xaõúê›`¤ÏWÿouSõas?bb`'ý–+Äo4®©þMõAS{bb`'|cõšê-¦àIÜ\½£zõEsbbàx:¥åñ[«¿dÁ§«·U7VŸ2ÀöÇËÿVýdõ								
¦àüIKT|}õsl11p¬ý½êÇª¿n									
¶ÉÕÕûªšàèˆ‰€cåÕÕV›€£ôxµ÷ ß?VÝvï©î8‚¿ÏÝÕGðû­n?à»Óª³âßù¤êÜCüµgU§äûòÝÑþsÀnó«wVï©þÔ‡OLl·ïªþQõJSŒµ5þ=0´=X|ë?ß¶ñë8~öT'ðÝAó©Õ9[~>¿:aãó™Õf`ý—êmÕû«?2À¡Ûå%Õª×š`mÜU=´ñùŽ–‹¿µÄÁn|ÞÛ×£`f:0BÞ*ŸÞrIyŸ­×“Ïn¹œGã÷«Ÿ«®­>k€§&&ŽÖÿT½¾úSìZWw¶ÄÀwl|÷@u÷Æçûª{6>ß½ñ×`§œÐrõ¸–KÈ§¶ÿUäóªs									
€/ïóÕ[ªëªß1À“GêùÕß¯~Â;æž6Càû¶|Þ									
?Ôr]ÖÙ‰-qmÆÇ§µ\:®%L>!ñ1ÀT_ª~¶%*þ„9žHL®§Uo¨~¡z†9Ž‰Û«G[®?ÒrUøá–0ø¡\†£qRun›O®öT§Wgm<§›	`-ý‹êÚêC¦Ø$&Ç««Ÿ¬¾ÅGäñjo›„o«Ûøîñ-?;oOKh|~K€|^ËÕãsZ.Ÿi"€•õ¾êÝÕ¿7€˜84/¬~°z­)žÒ­-Wƒïn¹0ü@Ë…á}W…õqvuZË¥ã}áñ—ŽØ½®©þMõAS“‰‰€/çkªï¯~ÆaoK |WK$ü@K4|÷Æg€­Îj	‹véXp°;üFË¥â÷š˜HL<™¿W½µú:SÃÜÖß¹ñ<°ñÝ=Õ}æŽóª3Z.Ÿ[¹åóIæ8n>Výrõ.S“ˆ‰€½¼ú±ê5°Æîk	…oo	…ïÜòì&§Vç´\6>cã½õ3Ûïÿ«Þ^½§ú‚9€u'&öy~õƒÕ™X#{Û?Þ[ÝQ=b`Mœ[ÕrÉøü–ðø¬7Gç¿Vo©®­î7°®ÄÄ@Õÿ^ýBõS+è¡ö…÷…Ã·›îü–Èøì–+Æçn|>Ó4‡ås-QñuÕ§Ì¬11ÌöêêMÕ·™X··					
ßÑæÕá‡LpXN¬Îk¹^¼gËsi¾¬?©~ªº&Q1°FÄÄ0Ó«¨^g									
`º³ºmËsÇÆ€coÏÏù-O2									
À_ø“êÍÕµÕï™Xubb˜åÙÕZþxV€öp›ÁðÞç¶êQÓì:gµŸ·ñì©N3									
0Ø¯~¢ººú¬9€U%&€9¾·zkõS;àö6cá}ÏÝfXyg¶\.>oËs~u‚i€A>_ýTKTüæV˜Ößß¨ÞT½ÖÀqrkK8¼ï½7×†¦Ùo									
Ï1°æþ°Í¨ø~s«BLëíªiày´'FÃ·š€'qbKT|A›¡ñÕ©¦ÖÌçÚŒŠ4°Û‰‰`=½¨úñêe¦¶Ñonyn­n7	Ûàœ–¨xë#0ÖÁ½-Qñ»«/šØ­ÄÄ°~ÞTýs3Géî–høãmÄ™€ãd_`|~›ñifVÔ§«Ÿ­Þe								
`7ÀúxyõÓÕw˜8L´ÿÕáW÷™€]æìžxÁX`¬’OV?W½×Àn"&€Õ÷ÕÕ?­þOS‡èö–hø–÷m&`E	ŒUô««ª_1°ˆ‰`µ}wõóÕ_5ð$îë‰W‡1kì¬žŸn`úÕêÕ¯™ØIbbXMÏ­~¬ú!S[<Þf0¼/¾Ë, 0vµ÷Tÿªú°)€ &€Õó½Õ/VÏ2Œ÷XuKuÓÆû–ï€§vvuaõ‚ê¢–À`'ýbË¥âß2p<‰‰`u|kõãÕkMc‰‡àØ9±%.Þ_Xa`¼©zGõ )€ãAL«áûª«ª¯0ŒòXû‡Ã7U›Ž×‹roõæê]¦Ž511ìn/j¹Fü2SÀ¶8|KâaØM¶^/¾hã}šY€cè“Õ[ª_1p¬ˆ‰`÷zSõÏÍkm_<¼õú°xVËžêÅÏ…-×Œ¶ÛZþÄ¢›ØnbbØ}Î¬~©úNSÀÚy´ýÃá›LkçŒ–«ÅU—VçšØFo­ÞQ}ÊÀvÀîòê–KCþ¨dX7¶DÃ7¶ÄÀ,§µ\,¾hËp4þ¤ú‘ê—«?7p´ÄÄ°{üBõÃf€•wWuýÆsSõ°I€-Nª^Üï{‰ß­~¶z¯)€£!&€÷’–?¦ôošVÒÃ-Ñð¾€ø.“‡áä6£âKª˜8L¿Þr¥ø×L	11ì¬¯þ™`åüfK8|cKH°]Nmójñ¥Õù&Ñ¿j‰ŠËÀáÀÎøkÕ¿¨^a							
X	U7T×´Ä˜8NNk3.¾¬:×$ÀSxSõŽêAS‡BLÇß?¨®ªži								
ØÕöV×¶DÄ·˜Ø%Îh	‹/¯.©Î4	p÷Vo®Þe							
à©ˆ‰àøùÊ–kÄßg									
Ø•i¹:|mu}uI€°§Í°øÅÕÉ&¶øXõ¶êƒ¦žŒ˜Ž—¶„Äßd									
ØUî«®®®k	‰3	°âöEÅ—VšØðžê«š8˜Ž½Ÿªþ/3À®qWõþ–Ä7°ÆNm‰‹/­.«Î6	Œ÷ÓÕÛ«Mì#&€cç…ÕOV/3ì¸½Õ5-Wˆo70ÔÙÕ•-qñ%Õ	&‘î­ÞXýkS%&€cåÇª·švÔMÕu-Wˆï6À~Nn‰Š¯h¹Z|†I`œ_¯ÞV}Ø0›˜¶××UWU¯4wW7´\ ¾¶ºÏ$‡ì‚êòçæ€Q~ºz{õ )`&11lŸ¿ÛŸn					
8ni	ˆß_]_=l€£vzËµâWU—T§šÖÞ½Õ«m								
˜GLÛãç«5U×UW·„Äšà˜9¡%(¾¤º²:Ç$°Ö~½z[õaSÀbb8:ßÖrø;LÇÔ=Õ5-ñõæØ1gWW´\.¾¤:Ñ$°–þYõöê~SÀúÀ‘û?ZþÃpl<P½ã¹Å»ÎÉ-AñåÏ™&µò¹êGª÷šÖ›˜ß)-×ˆ_g									
ØvT×Vïi¹@ü¸IVÆù-W‹/­.2¬÷µüÏÔ5¬'11žW´„Äß`									
Ø6·„Ãïi	‰1	ÀÊ;½%*¾rã}²I`å½±ú93ÀúÀ¡û¿«Ÿ0l›·Äï¯0ÀÚ:©º¬zÍÆûT“ÀÊúOÕÏTÿÞ°>ÄÄðÔž_ýRõSÀQ»£% ~gu·9Æ9±%(¾²º¼:Í$°’~¾åJñý¦€Õ'&€/ïVWUÏ0±ûªw·\ ¾Õl8¡%,~UuEuºI`¥|®ú‘ê½¦€Õ&&€ƒ{zKDüMGäáêš–+Ä7˜€CpiKXüªêsÀÊøÕêmÕGM«ILOô¢ê—ªo6–Çªë«wV×müGâÅ-Qñ•Õ™æ€•ðÆêçÌ«GLû{sõÿ˜Ë--ñ5ÕCæ`›]X]Q½®:Ë°«ý‡êgª˜V‡˜Ï©®ª¾ÓpHj	ˆßQÝnŽ“Z.¿¦:Ç°k½¹z‹`5ˆ‰`ùÐWUÏ6<¥[â««ÇÌÀ:¯ºrã9×°ë¸R+BLüöþ>ÞÒº ÷ÿ_Ãà‚ (ˆ‚(ˆw ŠB(						
á}¦ïC!ï TŽ<=öÅ#?M$Ey$MŽ¤É‰25Š¢PÊRI£È)’¤(¥°ÑÑi~\›¸‡¹Ùkïk­õ|>ë±73ƒàkß°×Zïõ¹`Þ^½A¸S×6ˆÏªVËÀ=¬á…¢‡WûÉ£â”b9cbæÕ									
§ Ü¡ó«TŸ¬ÖÉÀ”Ø«:rá¶‡0									
N)€3&`½¼úp»®i ºZ¦ÜÕ									
§ï",;§À0oN¯Þ ÜÆ'ÄŸ–€õÌ†QñáÕrÀ²qJ1ŒŒ11óâ€êÌ…·ÀàÊê¬…Û5r0'VU‡UG.¼]%	,§ÀH0^\}L¨jm7B|Ì¹ª,Üo|º°äþ zGõ‡RÀò1&`Ö½µz»Ðê†ñ‡«kå€ÛØ¥zùÂíarÀ’:¥aT,cbfÕŽÕ™Õ‹¤`Î_¾ðØ0VGVG,Ü¿&ïªŸÍ)Å°äŒ‰˜E‡5‰ sêú†ˆÏh8‘Ø4«îc¾|áíJI`âœRKÌ˜€YsBõ.˜S—7ˆÏ®nÕNÝtZñþrÀD}®z[N)€%aLÀ,yOõ&˜CçW§/¼&oß†ÓŠ¨v‘&Æ)Å°Œ‰˜»WgV?.sä†ê¬†“ˆWËËæ9ÕÑÕaÕJ9`ÑýNÃ ø¥€É0&`ÚÞ0$¾¯Ì‰«N!þ@u½0»4œV|tµ—°èÞR½[X|ÆÄL³ªwÉÀœ¸¤aD|NµNµCFÅ/¨¶‘ÍoUÇTÿ(,cb¦Õ{ª7ÉÀødõÞê")`êìP½¸zMµ¿°(®mÿ?)`q0mv¯Î¬~\								
fØšêÃ									
'_!Ì„}FÅGT;Ê›í½Õ›e€ÍgLÀ4yzÃøÁR0£®kŸ±ð>0{VU/h*l–?k8¥øËRÀ¦3&`Z]}PfÔÕÕi									
§ß Ì½FÅ/¯v6ÙqÕ/È›Æ˜€ipruªÌ +FÄgWëä€¹µMõâ†V”6É9_Cÿ*lcbÆî}Õe`Æ|¡aD|žÀ­ì×0ˆ<¢ÚNØ(ßXøúù)`Ã0V;VgV/’‚rAõŽê")€»°]udõš†1°áN­þ‡°aŒ‰£ƒ†Ä–‚q^Ãˆø)€M¼ŸüšêÅÕ6rÀùÃêuÕ_KwÎ˜€±9¢ú¨Ìˆ7Œˆ/“X;VGWÇU»ËwéûÕ1Õ‡¤€;fLÀ˜W½_fÀ9Õi“søÂýè§Hwéƒ									
£âJ·eLÀXœ\*SîÃ									
#â+¤–ÈÞ									
£â#«íä€;ô—ÕëªÏJ·dLÀ¼«:A¦ÔºêìŒˆ€åµCõò†añ^rÀú™ê2ÀMŒ‰Xnïox¢¦ÑYÕ;ª+¥Fä™ÕÞ·õ©ê˜ê›R€11Ëg»êÌêeR0…Î«N©.—±½ª7UG.Ünòí†AñÇ¥`Þ°öm?Q									
¦ÌEÕ[ª/HL‘«£†Å»È·ðó									
'yÀÜ2&`©Ú0$~„L‘KFÄHL±UÕ‹FÅûÉÿéK									
§I									
æ‘11KééÕïÉÀY]’Kž³çÐ†Qñs¤€ÿôêêƒ20oŒ‰X*‡UŸ’)qMõ¶ê¬jÀ{XõÆêåÕ6r@j8¥øûR0/Œ‰X									
/®>&Sàºê´êŒjÀÙ±zMÃiÅ;ÉÁœ»¢aPü‡R0Œ‰˜´#«ÈÀÈÝÐ0 >­º^`Ž­ªŽ¨Nl8µæÙÿ¨N•€YgLÀ$½¦úe±µÕYÕÏV×Èp/®N¨ö—‚9ö;									
§C									
f•11“rLõ‹20bg7ŒˆWKp§žÙpRñ¡R0§®ox¬ë×¤`0	oªÞ##õéê”êR)6ÊAÕÉÕaR0§~¡:Nf11‹íÄê20B—VÇWI°Yö]¸ÿ„Ì¡/7œRügR0+Œ‰XL'W§ÊÀÈ\W½¥:K								
€EµGÃ¨øåÕ*9˜3¯Êc									
ÌcbËÛ«·ÊÀˆ¬«Î¨ÞV]/ÀÄìZ½©zMµÌ‘ÿÓpJñ:)˜fÆÄ,†SN%†±¸ :¾º\									
€%³cõÆê¸…÷aüEÃ øsR0­Œ‰Ø\ïªN‘¸²zsužËf»†SŠO¨v‘ƒ9qbõÿ“€idLÀæxOÃeLa¹ÝPV½·Z#À(¬ª^Þ0²ÜCæÀ'N)þ)˜&ÆÄlª÷5\º–Û9ÕIÕURŒÖ									
£â}¥`Æ}«aP|®L‹-$`¼+Cb–ß¥Õ“ª—fH0vçTªž[}^fØ}ªOTo—€iádb6Ö;N‚år]uJu¦SëÐ†±å¡R0ÃÎi8¥ø_¥`ÌŒ‰Ø§V'ËÀ2YW} :©º^€™phÃ—’‚õw									
ƒâó¥`¬¶€									
ôÖ‰Y>5\÷Ø‰fíþÞª§VŸ—ƒô êwª¤`¬œLÀ†8¹áTbXjWUo®Î•`.<³z{u Ì _¨Ž“€±q21wå„‰Y§WûdH0OÎ¯W=»ºDfÌOW¾ð9£ádbîÌqÕûe`‰]^½¢ú‚sï9									
'ï'3æµÕd`œLÀ9:Cb–ÖÚêmÕc2$`ðÉ…û‰Ï«.“ƒòËÕ;e`œLÀí9¬ú”,¡ÏW¯j8•îÈ‘									
'ï!3â×ªcªë¥`¹pkU"Kä†ê”êt)Ø@«®¨ôÖj9˜Ý0(¾P									
–ƒ117·Gu^õh)XçW¯­®’€M°]u\ubµƒÌ€c«3e`©p£m†Ä?&vmu|uŽ,‚ª“†ÅÛÈÁ”;­:I–’117úpõS20aç4‰¯•€E¶KõÖê5ÕJ9˜b¿ZS­‘€¥`L@ÕûNïI¹ªzmu¾LØ^									
£â#¥`Š}­aP|±LÚÌ½weHÌd^í“!1KcuuTõ˜ê"9˜R¬>W-“fL0ßNX¸Á$\^=¡:¾ºA–Ø¥Õ“ªç5Œa}°z»LÒŠõë×«0Ÿ^\}L&`mõŽê´…÷`¹­j8áõÔjG9˜B§7¼`11À|: ú¢LÀÕK«K¤`„v¨ÞZ×00†iò™ê˜ê*)XL[H0wVVgÊÀ| zL†ÄŒ×õÕ›«}ªóä`Êüxuaõt)XLÆÄóçÌ†“‰a±\[=·zmµF¦ÀêêyÕ“ªKå`Š<¸ú½êh)X,ÆÄóåÕ«e`_=ªú¤L¡‹®²óªê9˜"¬N–€Å°býúõ*Ì‡7Uï‘E²¦:©:]									
fÄvÕ‰									
¡l#Sâ½Õ›e`sÌ‡Ã«ßErYõ’êr)˜A»T§VGKÁ”øõê˜ê:)ØÆÄ³ï€ê‹2°HÞÛp"ñZ)˜qûUï«•‚)ð¥†Añ—¤`cÌ¾/6Šas\]U](sæðê]Õ^R0ž[}R6ÆÌ´33$fóWí“!1ó}¿øÍÕõr0r¿U-Ã˜`vZ½N6Ã									
Õ+ªçåÉRæÛÚê½Õž									
/Þ^'	#öÁêØP+Ö¯_¯Àì9®z¿l†/T/©®”ncïê=Õ3¥`ÄN«N’€»bL0{žÓp9CØëªwT?›S–à®^½¯Ú]								
Fêôêx¸3ÆÄ³e§êÒêþR°	®j8øóRÀÛ¦:¹:¡Z%#ô+Õ1ÕZ)¸=[H0SÎÌ˜MsAu@†Ä°±ÖT§TûTçËÁ½rásóaRp{Œ‰fÇÛ«çËÀFZW½­zFu­°ÉVWÏªž×põ“'WçU‡JÀ­­X¿~½								
ÓïÅÕÇd`#][½¤ºP									
XTÛT'WoZxÆäy									
Ãb¨Œ‰fÁÕe`#]Ü0$¾Z									
˜˜½ª÷U‡IÁÈ¼¢ú°Tm!ÀÔ;S6ÒiÕ“2$€I[]=»znu•ŒÈ‡ªãd Œ‰¦Ýé									
'Ã†¸¾áÉË“ªurÀ’ùdµOÃc9î“3ï¯N–€ë×¯W`:Q}T6Ðå									
CâÕRÀ²Ú¯ú`µ¿ŒÄÏVo“`~L§ª/ÊÀ:¯:ªºA									
7V§VÛIÁ¼»z‹ói	¦Ò™°N©ž—!1ŒÍéÕÃ«s¥`N¨Þ'À|2&˜>§7œLwæúêYÕ;¤€ÑººzaõÜê*9Xfo¬~Q€ù³býúõ*LW“»pyÃ“«¥€©±]õÖêMÕJ9XFgVÇÊ0?Œ‰¦ÇnÕW«{IÁ8¯:ªºA								
˜JûV]xËåÿTÇTë¤˜}[H05ÎÌ˜;wJõ¼‰`š]V°p?­,“WWgW;H0ûœL0Nªþ—Ü5									
§Ÿ+Ì”}«TûIÁ2ù									
'_+Àì2&¿­.’;pMõÜêRÀLZYX½µZ%Ëà3									
ƒâ«¤˜MÆÄã¶eõÕêRp;.«ž'r`ì[}¨Ú_									
–Áï7ŠWK0{¶`ÔÎÌ˜Ûwnõ¸‰`^\ÖðXÀ)ÕZ9XbO«ÎÉ˜`&9™`¼^QýŠÜŽÓª“d€¹µoõÁê@)XbÞpBñ¤˜ÆÄãôÐê«ÕVRp3k«×V–æÞÊêÄê­Õ*9XBÅ3Æ˜`œ.¬ž,7s}õÜê")€›Ù»úPN)fiýyutu©Óo	FçÿË˜[ºª:$Cbà¶.¯žPR­‘ƒ%òØêÌj?)¦Ÿ“‰ÆåYÕgdàf.«žÝ0(¸3«>’SŠY:ÚpBñåRL/'ŒÇö								
§yÀ.j8‘ØØW4œR|RN)fi<¾á1Í½¥˜^N&VGÈÀ‚WGUk¥6SŠYJŸ­^Ó0hg¾l¿æ_e€q3&‡Ÿ®Îï­Þ,°™VVoªÞ^m#ö‡ÕÑÕ•RŒÆCß]ª]Þß¦[ž$½cµÇíü½{oÀ÷•Õžðïñ·Õº»ø3kªËoç×¯¬®»Ù__ÞM'¯_]]³ð¾Á2lcb€å÷˜êÏe`Áë3,—SŠY*¿ÛpBñURLÌöÕªjßj»…¯ïª½~¿†‘ï6ÕnsÔå›									
#ãuÕ¥¿¶ºº¾áÄìªË®gx·bL°üþ´zœso]uTuŽÀ¬l8¡øÄ…÷aR>S½¼ºVŠ¶}Ã8x»n:x¿…¯ÙýÛð“€¹s7ž”|I7o<ù††ñ±Á1sÅ˜`y½§áR“Ì·µÕK«s¥&ìÐê£Õ®R0Aÿ¯:²a É-Ý¿a0¼oµGµûÂû{U+äõ									
'_ÖpÒö•ï_Qýƒ<Ìcb€åóüŒGžPyIõI)€%²cõÁêp)˜ _m8¡xÝ«áDá½Ã{4œ,¼{µ•O©÷ý†ñ%									
#ã+†Ç—Vß–€idL°<îW}¥ÚIŠ¹¶¦zvu¡À28¦áÊYÛHÁ„œY;ÃÿÿÔ0Þ·Ú{á¶Guú¹õo									
ãâËn—5ŒŒÿNÆÌ˜`yüfõ\æÚ									
Õ³ª‹¥–ÑÞÕÇÆ0	gT¯Ÿÿlßüvo^6Ð¿4ŒŠo~ûš,Œ…11ÀÒ;¡z—síºê								
—ÁXnÛ4<^uœLÈéÕñSòïºm·									
ïWméÃÈ"ûa·_Z}W–š11ÀÒzbN¢w×6‰/•™çT¬v’‚	xwõ–þ{=¾:¸Úáö*–Ù×¢¸¤áù„?•€I3&XZ¿Û0$e>]]=µºB								
`¤v­>R=E									
&àÕ)ËøÏ¿OuPÃxøÆ·+|X¹õ									
£âÏßìí·d`1,·Vo—an]U=©ºR									
`									
œÜðxÖ*)Xd§4ŒŠ—Âƒ®wðÂíò3#þ²aX|qõÇÕßHÀæ0&XO«.an­n8‘ø*)€)r`õ±j)Xd¯¯Î˜ÀÿîÕ!Ý4ÞYjæÄ?wÓ¸øsÕ—$`c,¯T’a.]Þ0$¾F									
`									
mWýru„,²—TßŒ¿«†ÁðÍÇÃ[É									
U}¿[Ž‹/^ø5¸]ÆÄ“÷Õ±2Ì¥K«gT×JL¹#«_lÃbyRuÑþÙûtËáðòÁFùB·KndL0Y/­þ¯séóÕ³ªë¥fÄ^ÕÇªý¥`‘üeuXuåíüÞžÝ4>¤z¸\°¨þª›N-¾¸ú[Iæ—11Àä<¨úju)æÎÅ									
Câ¤fÌªêíÕ‰R°H~·:¢z@7									
‡®v•–ÔÕÝtjñÅÕW$˜ÆÄ“óN&f¾\\=£Z#0Ãž^}¤ÚE									
Á¿åPã×åÃâß0£Œ‰&ã¨êWe˜;_h_/0v©>ÑpŠ,³ïæÃâ‹«•`6,¾W_­î.Å\¹¬zRuÀYY½«z“sç+Ýr`|µ$ÓÉ˜`ñýJõ									
æÊå									
Câk¥æÔáÕGªí¤˜[WvÓ°øsÕ_I0Œ‰×‘									
Oš0?V7‰¸Ì»½ªß¨ö•€ê[Ýòäâ/H0NÆÄ‹gÏê«Õ¶RÌ««'TWIPÕ6Õ/7¼ènîû									
£â›Œ¿/Àò3&X<ÿ§z•sãê†‰WKp¯©Þ_­’€;ñ…n90þ–$KÏ˜`q¼¬:[†¹q}uHu™whÿê7ªÝ¥`]\]Ô0,þ]9–†11ÀæÛ£újµsaMÃ‰Ä_à.íX}´z¦l¤5ÕU¿ß0.þ¢$“aL°ùN¯Þ Ã\XW=¯ú¤leõÎê)Øß¬~³aX|AõmI‡11ÀæyQõqæÆ+ªË°I^\}¨ÚF									
ÁÕù9µ`³lºUÕW«‡I1NªN“`³ìWýVµ»,¢Ë®*ø¹êwåØ8ÆÄ›î5L™}§WÇË°(v¬~£:T									
&`uunÃ°ø3rÜ5cb€MsXõ)æÂ9ÕKeXT+«÷To”€	º¦áqþÏ5œ\ü’Ü–11À¦ù\u°3ïÂêYÕZ)&âÈê—«m¤`Â®«Î¯~«útõ]IÆÄïÄê2Ì¼ÕÕÕõRLÔÕ'ªÝ¥`‰\_]PýFÃÀøÛ’óÌ˜`ãR}V†™w}ÃxµKb—†“"”€%v}ÃIÅŸ¨~S`lœs«çË0ÓÖUÏ¨.”`ImS}¤z,“Ëª³«ÏU*0/Œ‰6Ü1Õ/Ê0ó^_!À²9¹:U–Ù								
§ºú9€YfL°aU}E†™wfu¬Ëî									
§o#ËlMõ[ÕyÕ¯ËÌ"cb€									
szõfÚ…Õ³ªµRŒÂ									
ã­]¤`$VWçTŸ«~_`VÜµU—a¦­®W]'À¨ì^}ªÚW									
FæÂêc									
'K`šÜ¹•ÕW«½¥˜Y×7‰¯`”¶«>Q=S									
Fè«3ª‹ª?–˜F[Hp§Þ’!ñ,[W½$Cb€1»¡zvušŒÐýªwTW¿Uý¤$À´q21ÀûÑ†W‘3»Ž¯N—`jS½¿áŠb0V_®Î¬.¬þF`ìŒ‰îØoVÏ•af} z­Sç°êÕ6R0rkªóªU¿-0VÆÄ·ïÕ¯È0³.¬žU­•`*Øp)ù]¤`JüNõñ…Û÷äÆÄ˜à¶Z}µÚJŠ™´ºzBu­Sm¯†aÖ^R0EVW¿X_ý¥ÀÜÖ/U¯•a&]_R]&ÀLØ±úTuL™Vï¨>]}Q`9ÜÒó«se˜YÏnxP€Ù±Mõ‘êR0¥Þ_}²ú})€å`LpK^=F†™ôŽêfÒÊê}ÕqR0Å>V}¼úM)€¥dLp“ªwÉ0“.ªžZ­“`¦½©zL¹OV­~]									
`)žX],ÃLº¶zTusáˆêCÕ*)˜rP}¸ú¿R“´…U+ÁLZW½$Cb€yrNõÜjL¹§VgW_¬^YÝM`Œ‰êù									
§•0{ÞV](ÀÜ9¿a€uÌ€ª³ª¯V?%°ØV¬_¿^`Þýiõ8fÎùÕ³N'`>í[ý^µ‹Ì/Wï®~M									
`1óî§ªË0s®®S]+ÀÜÛ½úƒj/)˜1TYýºÀæ0&æÙý.uo)fÊº†KX^$v©~§ÚO									
fÐo5žó›R›b	€9vt†Ä³è´‰¸¥kª'åq#fÓs«óª_«~L`c9™˜WO¬.–aæ|¡:¤Z+·c›êcÕs¤`†SýbõÇRÂÉÄÀ¼:V‚™sCuT†ÄÜ±5ÕóFV0«Žh8TççªÇÊÜ'óèÇ«OË0s^[}@6ÀÊêƒÕË¥`œXQ}W								
àö8™˜GGK0sÎË€									
·®zEu¦ÌÓª¯V/“¸=N&æÍó«se˜)×TûT×IÀ&xWu‚Ì‰ß©N¯~W									
àFN&æÍqÌœ£2$`Ó½¥z‡Ì‰gUçW?W=T Œ‰€ùò“Õ“d˜)gTÈÀf:eáóâÍÕW«×I¬X¿~½									
À¼øóê12ÌŒ+«GU7HÀ"9¡z—Ì™/W§U¿.Ì''óâ•ÏšWeHÀâzwõZ˜3©>^}´z¢0œLÌƒí.Óô@)fÆò¤“stõA˜S'VgTß•æƒ“‰€ypD†Ä³äªê¿ÊÀÕpe,˜G§5Ôó_¤€ùàdb`Ö= áÁŽ{J13žVý,cª_”€9öþ†qñ?H³ËÉÄÀ¬;2CâYrV†Ä,3«ce`Ž½¾áàžŸ”f—“‰€Yöà†7î.ÅL¸ºzhõïR°ÄÞX½OæÜG«wT)Ì–-%fØáÏ’—gHP7=¦·rá¶Eu·…_[¿ðþ·úó[,üÞ=ª]þÌT÷«î³ðç¶ªv«¶]ø³Uë~}÷…¿÷‡wòïõƒ†«‚Ü¯Úúfÿ7º¦úç…çÛ³Eµ¦áEd7,üõŠÛùs+«oUÿ¸ðïs·ê{Õ•oW4\zõÛ7ûÿ°îf}~p«ÿëþžßÿ…›S€›;}áíû¤`Ž½´zquLõA9`v8™˜U÷o8•øÞRÌ„ß®ž#0ƒnËnY­jÆnÙ0à½ÛÂÛÇÂ[4}ï[m×0Ú½gµMµÇÂß÷Ãjç…Ÿ‡°ð÷Ý¯›ÆÆóè{Õ?5Œƒ×T×M£áo6ŒŽ·¬®m)·aôü¯îÕÚ…·ß_hüƒ›ÝþcáŸãV˜oªÞ#ô©êÝÕg¥€égLÌªŸ®Îa&ÜÐpBÞõRSbÅÍÞnÑp’îÖ									
£ßm®ž±ÍÂmË…·÷m8!xç†ÄÝøö~Þ‹ä–Ç«ëNUþ—†±ñ¿4Œ¿Ý0FþNÃèxmÃØøû									
æ5ï¯Yø½u									
ƒãoÀô:±z§PÕIÕi2Àt3&fÑ}N%¾Ÿ3áåÕ¯ÊŒÈÝ4Þ¢›ÁÛU÷Xx»CÃx»jûê									
ƒá]~N½ñTafÇÚ†Óÿ¥a€ü­†ÁñÕ									
ããïTÿÞðb¹mx±Ü									
·›ÿ£›N;ÆëäêT ª?©ÞVý¾0Œ‰€Yôêê2Ì„/Uæä6`éÝx¢ð–ÕÝÆÂ÷lïØ0Þqá×·¯î_í´ðö>									
£á»ËÈí¸®ú‡†‘ñµÕU¿öï									
ãï,üõõ									
cäïW?h8%ù?nöX~§6ŒŠ€Áÿ¬Þ.Lcb`ÖÜ«áTâÝ¤˜	»6-&eËjÕÍnÛV;7‚ï»pÛaá¯w«î]í²ðvùXdÿÑpŠñ?6œpüÍ†Añ¿5œfüí†¯­®i8Õø								
'¯mKë}Õe€ÿôÕÏVŸ•¦‡110k^Y%ÃL8¡ú9€E²MµUµuÃ‰ÁÛ6‚w­Øpªð=ÞîÖMcâ­¤cD¾ß0&þç†¯mßxÂñßwÓ)Çß­ÖTßk“óÁêhàNªN“¦ƒ110K¶m8•xO)¦ÞßUÎå›€·²Ú®a|ÏnïÕ0Þ¹Úqá¶SÃ ø>²1¾UýSÃ°øú†“ÿ~ávõÂïÿ[ÃiÆßm¯•									
ígÐV/–náSÕñÕßHãfLÌ§ÏŽGT%pV6Œ…w¼Ùm·†áðž									
Ãá{5Œ…ïÓp*1Ì›ï,Ü®m8µø_ª¨®l8Íøú…ß¿náí¿W4€·ªúê0)àþ½:¦úˆ0^ÆÄÀ¬Ø¢áTâ}¤˜z?W p+«NÞ¹a¼cu¿j†ñð.									
'									
ßkáÏ­îÔ¿Ußî¦SŒ¯j_ÙMÃãZø½ïVë$€»´Mõ{ÕÁRÀmürÃ¨ØP	FÈ˜˜?U}X†©wMµ{õ)`nmÑp‚ð½ª]«û7Œ‡wnïYÝ·aL¼}µ­d°hÖUÿÚpBñ¿Tßì¦Œÿyáçõßÿ÷ê‡’ÀmìPýQµŸp—UÇUŸ•ÆÅ˜˜Ÿ­‘aê=¾ú3`®¬ªîÞ0Þ«zÐÂû»7Œ‡ïÛpÒð¶Õ–rÁ²ø^ÃÈøÚ†1ñêênß¨þ¶á”ãïUkå€vªþdáç[à¶NªN“ÆÃ˜˜/ª>.ÃÔûÄÂÇ˜]+.ý¼mÃ	Ãmï¶ð×j^l'ŒÞÚ†Œÿ¹áôâ««j_Qý]õÝjMÃ‰Ç0ovoï*Ü®OU¯[¸?	,3cb`üFu¸Sí††ÑõRÀLÙ¦áÔá{6œÊ¶wõê~ÕÞîØp:10ýÖVÿÒM'ÿSõ7Õ_4œfü…Ÿý×HÀœØ·ú\µƒp»®«Ž©~]						
X^ÆÄÀ´û±ê|¦ÞÑÕ¯ÈSï^									
§									
ß§zxõ¨êÁÕ}«]ª†ÅÀü¸¾º¶a`üÏÕ×«¯UÙ06þ×êßd`†=¥ú¼€îÌéÕñ2Àò1&¦ÝG«#d˜jW?ZùÁ¦Ïv									
áûV¨×pñNÕ½NÞZ&àf¾×pòÔu									
ã¿¬.i_{³ß€YrDÃã˜ÀûRõº…ûˆÀ3&¦Ù£«Ke˜jkN,¼B									
˜									
+«,ÜXí_=¦º_Ã©Ä÷ª¶”	ØÈûßn8Áø[ÕåÕ«Õ								
'_]}G&fÀ‰Õ;e€»ôÆêçe€¥eLL³ÿZ½W†©vZu’0j»Uj?¢zlõ°†S‰·ÏÉÃÀâúAõoÕ¿6œTü•†Ó©¾Ñ0,^]­‘	€)õÎ†Q1pç>^ÓðâS`	Ójûê«							
£¦Óêjï†±0÷n?¸Ú«Úwá¶Cµmuw‰€%ôƒê†êß«¿¯þ¼ú‹…÷ÿ:W9`ú|´:B¸Kß¬^W}Z									
˜<cb`Z½²:K†©ö¤ê"`Ù­¨ö«UíY=¼zdµKÃ©Ã[W[ÈŒÄÚê{·Ë^dúõêkï_'#·ªúê)RÀygõ32ÀdÓê³Õ!2L­W¯–ÍvÕªÇVmïQmÓ0nX)0Ö7œ\ü½ê«¿j8­ø/ªKÞz€1Ú¡ú\Ã@€»vQuLõ—RÀdÓè¿TçÉ0µ®«’Ã`©íR=¹:°Ú«áâûU[U[ÊÌ€uÕ«ï6œV|eõ·Õ7¼ õ‰‘]«/-üœÜµ6Š?(,>cb`}¢zSëØêL`I<¢áòÉ?R=xávŸ†“‡·˜aë«ÿh8¹øFÅÛ0*þ£ê›0.üwi)`ƒ}¨aTü})`ñÓæ±									
—«e:]ZÐpb°ø¶«ö«žÖ0L¸õ€†Ë(oQ­˜Sëî‡|«aHü·ÕŸT¿_­Î“Ð,ŸÃ«ß6Ê									
ƒâ?”‡110mÞX½O†©´®z\Æà°XVT[U;U©ž^=¾Ú±Ú¹Ú6ãa€Û³~áv}õOÕ?TŸ«~¯úzu]Ã©Æ<`©œX½SØhÿ£:UØ|ÆÄÀ4Ùºújõ)¦Ò™Õ±2ÀfÙbág¢ûUûV?QÔ0 ¾WµJ"€Mòï									
#âkª‹N·ú‹†±ñšŒ‹˜¼U/—6Úï4œRü									
)`ÓÓäeÕÙ2L¥ëFà×ImeÃHxÏêaÕUO®î]m_m)À¢ú~õÝêÛ									
'®º¬º²á4ãfXÀâ[Õ0†zŠ°Ñ®oÿš°iŒ‰€iò™êY2L¥ã«Óe€									
¶eµUõÀ†ˆŸØ0"Þ¥Ú¶a`Àä­«¾W}§úãê³									
WÌ¹¼º¡Z›a1‹gÇêÏª½¤€MòÕq2ÀÆ3&¦Å“«e˜J««}ždîØÝª­«ÝªnOk8‘xkyFamumuqõ…ê’†S‹×4ŒŽ=àÀæÚ«ú“j')`“|¹á”â?“6œ110-ÞZ½]†©ôìêÓ2ÀíÚ²ºGµsõ„êÀêq									
/ÄY%Àè]Ý0*þó†“‹ÿ¢áÄâ—€Íð”ê÷rEØÇVgÊÆ˜˜ÛVÕpJÓå‚ê2ÀmìPÝ§:¨a(°oõÈœ@0Í¾Y]Z}±úýêÊêÛ									
'ÀÆzcõ>`³üBuœp×Œ‰€ið²êl¦Îº†Ë³_*TµUµKµgõœê‰Õ#ªí¤˜9ßh8¥ønÿP][ýP6ÂGª#e`\ÓpE…ª5Õå7û½ë^uk—/üÙ;³®									
{üw¿îú¤ímª½oç×÷¨v¼Ù_ï½ðg«v]¸Ÿ									
pg¾\Sý™pÇŒ‰€ið™êY2LT¯•º_õÀêêÙÕÃ«e˜ëª¿oÙünõ¥êªêŸ¥`lS}®Ú_									
nemuYuCuEu}µzá÷.]øäÖ£áYwãÈxeÃx¹j¯†+=¬á…¼ûV«|úÀÜzUu–pûŒ‰€±ûÑê"¦Îšê!ÝtÚÌ›m«W­žßp									
ñ®ÕÒÌ­Vß¬.¬~»úzõ×Õ¤àNìÚp¢âNRÌ+FÂ7ž|iÃ8ø’6ü$`îÜ~									
£ãý»i||ãÉÈÛ5ŒÙôŽêà¶Œ‰€±;¹:U†©óîê-20‡XíÓp									
ñ3«GT[ÉÀ­¬©¾Z}ªúbõµ¼€;vpõ9QuVÜxšðeÕ•									
W-¸¬ádáëåN6Þ·Ú½ÚcáýO9¦×ÿ«Ž©®•nbLŒÙ									
ªî%ÅT¹®áTâë¤`NÜ½: zTõÔêIÕ=e`][ýauAõÕN€›;®z¿SãÆ„W7†¯l8YøªŒ×fÁN									
ãýFÆ{4<±_ÃIÇÀøý}Ã øÓRÀÀ˜³U—aêœT&s`÷†áðª§4¼˜6Ç×FÅ_®>Wý$ÜÌ«£e•ëFÃ—U—/Ü®ÌæÙ®									
ãâ½nû6ŒŒw”Fé-									
WÛ€¹gLŒÙ'ªÈ0U®®Þp©>˜UVÏlZm-	‹ì†êOª?«>[]\}O€¹·ªú£ê )–ÅU								
Ãá›ß®”…									
´GÃ¨øæ·ÝeQø…†+À\3&ÆêAy v[)3hÛê									
#âžô€¥ðõ†±ÒŸ4\‚÷ë’ÌµÝ«/U;I1Q—uÛáðu²°Èvì¶ã}eeñåê˜†tÀ\2&Æê•ÕY2L•Õ									
§¯“€±¢Ú«zNõ”êÑ									
—+€åðýêÏ«¯UŸl8±ø_e˜KÏ¬>U­”bQ\Þp€Kn—æ1N–ÏÊ†Qñþ·ƒ«½e%sTu¶Ì#cb`¬þ¨á²áL—T—€°}õ¨êEÕã«}ª»ËÀˆ|£º¢aHö™†Ë®ÿ@€¹rju²mmõù†ñðo¯—…‘Û¡aT|ÐÍÞ®’&æ”ê20oŒ‰€1zbÃƒ¸LK«ÇÈÀÛ¢árÁO¨^Ð0 ~HÃéÄ0Vß©®\¸}^Ã%Ù¿%À\XYý^ÃUT¸c×vÛñ0Ì‚[‹w’Õ»«·ÈÀ<1&ÆèÄê2L•gUçËÀº{Ãpø©Õó«Ýª]d`Êü úfÃ˜øÜêÏª¿É%ÚfÝNÕWÝ‡¹…Õ									
£á†Ã«%aNìÕ0,>táí^’Àf;£z½Ìcb`Œ¾Zí+ÃÔ¸°a€ÓäžÕÕaÕOT÷®¶—€pmõê7ªÏV_©n`f\ýQÃIÅóèÊê‚†ƒ.^øï 0¼Øààê™ÕÓ«=$Mò»Õ1ÿ½€™fLŒÍWŸ–aª<µaPÓà>Õ“ªkß«ÚZfÐ¿UÿRývÃ¨ø¢¬fÕ<]éíÚ…ÿ¦Ý8 ¾Ê‡6ÈîÝ4,>´all˜¿i_ ³Ì˜›VGÈ05.®‘€)ð€êi									
Oš=½áâU²0¾ßp2ñïUŸ«þ áÉðuÒÌ”O5¼`r]¸p;¿ºÄ‡Å~ß3ž²pîÚ«ª³d`Vcr·†“$v‘bj<;'I0^[T¬žÓ0 ~BujKi˜C?¬þ½úRÃC?]]Z­•`&ìX}¹áôÑiwMÃéŸl_çÃµCÃã&7>~â9¸c'U§ÉÀ,2&ÆäùÕ¹2LKªd`„¶ªR=·zjµµmµRè?N+¾¢a õ©†ñ¿I0õžÒpý4Þ÷¹´:¯a@|©%,«ý†Å‡/¼ÜÒi									
£b˜)ÆÄÀ˜|¢zSãy
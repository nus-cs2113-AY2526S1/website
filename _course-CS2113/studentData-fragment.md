{% set staff = [] %}
{% set tutors = [

]%}

{% set tutorials = [
"CS2113-W10",
"CS2113-W12",
"CS2113-W13",
"CS2113-W14",
"CS2113-T10",
"CS2113-T11"
]%}

{% set students = [
['EMAN.. YUE', 'CS2113-T10-1', 'Emannuel-Tan'],
['GOH .. WEE', 'CS2113-T10-1', 'gbinw128'],
["L'KE..NAIR", 'CS2113-T10-1', 'Rezelix'],
['LAI ..REMY', 'CS2113-T10-1', 'MinionWolf'],
['ROYD.. REN', 'CS2113-T10-1', 'roydenlyr'],
['DARS..RESH', 'CS2113-T10-2', 'darshhs'],
['HUAN..NGRU', 'CS2113-T10-2', 'AmandaHuang'],
['PANG..SHER', 'CS2113-T10-2', 'ashpasa'],
['SEAN.. JIE', 'CS2113-T10-2', 'seantankj'],
['YEOH..EONG', 'CS2113-T10-2', 'Yeoh-Soo-Leong'],
['CHEN..EFAN', 'CS2113-T10-3', 'W1ndB10w'],
['CHIU.. CHI', 'CS2113-T10-3', 'ycdaniel326'],
['MROZ..TRYK', 'CS2113-T10-3', 'patrykmrozek'],
['PACZ..LIAN', 'CS2113-T10-3', 'sandrej09'],
['SEAH..G LI', 'CS2113-T10-3', 'seahsongli'],
['ANG .. BIN', 'CS2113-T10-4', 'AWeiBin'],
['HIEW.. T G', 'CS2113-T10-4', 'HiewTheG'],
['NOCH..ANSH', 'CS2113-T10-4', 'sivanshno'],
['ONG ..O YU', 'CS2113-T10-4', 'osy4477'],
['ZHU ..ENBO', 'CS2113-T10-4', 'mendax1234'],
['ALUN..TOSH', 'CS2113-T11-1', 'ashutoshalung'],
['JALI..EYLI', 'CS2113-T11-1', 'ljalilova'],
['MUKH.. ISA', 'CS2113-T11-1', 'mukhtarcal'],
['NGUY.. DUC', 'CS2113-T11-1', 'k1b1t0'],
['ADRI.. HNG', 'CS2113-T11-2', 'aydrienlaw'],
['AHME..HEER', 'CS2113-T11-2', 'saheer17'],
['GU M..UJIA', 'CS2113-T11-2', 'gumingyoujia'],
['LIM ..ERUI', 'CS2113-T11-2', 'limzerui'],
['MUAD..TAFA', 'CS2113-T11-2', 'muadzyamani'],
['JEWE.. LIM', 'CS2113-T11-3', 'Jeweljace'],
['LEE ..HENG', 'CS2113-T11-3', 'Lee-YiSheng'],
['ONG .. JIE', 'CS2113-T11-3', 'yujie-o'],
['RYAN..FONG', 'CS2113-T11-3', 'rsiowkf'],
['SHOU..MOUD', 'CS2113-T11-3', 'Ibrashoukry'],
['GADD..IRAM', 'CS2113-T11-4', 'argadde'],
['GOH ..LING', 'CS2113-T11-4', 'gohjieling834'],
['PAVI..ASAN', 'CS2113-T11-4', 'Pavithra6-Srinivasan'],
['SRIV..SHIT', 'CS2113-T11-4', 'HarshitSrivastavaHS'],
['ZHEN..IWEN', 'CS2113-T11-4', 'Kevin88866'],
['IRWA..NOOR', 'CS2113-W10-1', 'irw9n'],
['JIAN..XUAN', 'CS2113-W10-1', 'jyx0615'],
['LIU ..QUAN', 'CS2113-W10-1', 'LJQ2001'],
['TAN ..N YI', 'CS2113-W10-1', 'Tanjy55'],
['FAHA..ADER', 'CS2113-W10-2', 'fahadmohaideen'],
['KEVI..I YI', 'CS2113-W10-2', 'kevinlokewy'],
['WILL..DREW', 'CS2113-W10-2', 'Mack34021'],
['XU H..GHAO', 'CS2113-W10-2', 'XuHh03'],
['BREN.. HAN', 'CS2113-W12-1', 'BTslayer761'],
['GOH .. ANH', 'CS2113-W12-1', 'JeanPerrierIII'],
['HE P.. SAN', 'CS2113-W12-1', 'Kennahh'],
['JOSH.. TZE', 'CS2113-W12-1', 'Ekko-Technology'],
['KENN..N WI', 'CS2113-W12-1', 'Kurokishi592'],
['ABE .. YIN', 'CS2113-W12-2', 'abefqy'],
['CAI ..NGZE', 'CS2113-W12-2', 'andrewcai8'],
['ONG .. KAI', 'CS2113-W12-2', 'EggsKay'],
['TAN ..NDEN', 'CS2113-W12-2', 'ZT712002'],
['MA H..YANG', 'CS2113-W12-3', 'm-xrtin'],
['ONG .. YAO', 'CS2113-W12-3', 'chongyaoo'],
['RAYA..WONG', 'CS2113-W12-3', 'Rayan-Wong'],
['RYAN.. HAO', 'CS2113-W12-3', 'ry-koh'],
['GAO ..NETH', 'CS2113-W12-4', 'duckyfuz'],
['JORD..HENG', 'CS2113-W12-4', 'JordanTwz'],
['RYAN..GKAI', 'CS2113-W12-4', 'goodguyryan'],
['SANJ..UMAR', 'CS2113-W12-4', 'sanjay-shiva-kumar'],
['THEN..ELLE', 'CS2113-W12-4', 'noellethen'],
['CHEO.. HAO', 'CS2113-W13-1', 'JianHao24'],
['DANI.. WEI', 'CS2113-W13-1', 'danielkwan2004'],
['GORD.. JIE', 'CS2113-W13-1', 'gordonajajar'],
['SHAU.. REN', 'CS2113-W13-1', 'shauntsr'],
['VENK..THAN', 'CS2113-W13-1', 'shira421'],
['CHEW.. JEN', 'CS2113-W13-2', 'zeeeing'],
['LEE ..SEAN', 'CS2113-W13-2', 'sean6369'],
['XYLO..HONG', 'CS2113-W13-2', 'xylonc'],
['YANG..ZHAO', 'CS2113-W13-2', 'Zhenzha0'],
['YAO ..IANG', 'CS2113-W13-2', 'Yxiang-828'],
['CELE.. TAN', 'CS2113-W13-3', 'xelisce'],
['LI M..EIYI', 'CS2113-W13-3', 'limeiy1'],
['MICH.. ZHI', 'CS2113-W13-3', 'Michael-Low'],
['SHEN.. TAY', 'CS2113-W13-3', 'shennontay'],
['TAN .. JIE', 'CS2113-W13-3', 'zhengjie2002'],
['BRIE..HONG', 'CS2113-W13-4', 'blimc1'],
['CHEW.. WEI', 'CS2113-W13-4', 'enwei29'],
['JOSH.. YUI', 'CS2113-W13-4', 'tam308'],
['MENG..HONG', 'CS2113-W13-4', 'msc-123456'],
['REVA..MIKA', 'CS2113-W13-4', 'samika2005'],
['COKE.. CAN', 'CS2113-W14-1', 'Sheeeesh-code'],
['HANS..OONG', 'CS2113-W14-1', 'ChangIkJoong'],
['MA Z..HENG', 'CS2113-W14-1', 'mazh25'],
['TOH ..IZEN', 'CS2113-W14-1', 'Izen9835'],
['YEUN..G HO', 'CS2113-W14-1', 'hyeungac'],
['FOO ..KANG', 'CS2113-W14-2', 'fookang'],
['GAN ..HIEN', 'CS2113-W14-2', 'asytrix99'],
['LIM .. JIN', 'CS2113-W14-2', 'yikjin'],
['OOI .. REE', 'CS2113-W14-2', 'Wrooi'],
['T. K..SAMI', 'CS2113-W14-2', 't-kandasami'],
['NGUY..LOAN', 'CS2113-W14-3', 'bennyy117'],
['NITI..ITIN', 'CS2113-W14-3', 'nitin19011'],
['RAJA..THIK', 'CS2113-W14-3', 'Kart04'],
['VU D..KHOI', 'CS2113-W14-3', 'Exceptional-Khoi'],
['ZHON..AODE', 'CS2113-W14-3', 'ZhongBaode'],
['BENJ..KIET', 'CS2113-W14-4', 'BenyAlbatross'],
['JUNG..YEON', 'CS2113-W14-4', 'Joannaj00'],
['LUKE.. TAN', 'CS2113-W14-4', 'lukeai-tan'],
['LUO ..GXUN', 'CS2113-W14-4', 'BestBearrr'],
['VITO..ALIM', 'CS2113-W14-4', 'V1T0bh']
]%}

{% set org_replacements = {

}%}

{% set teams = {

}%}

{% set products = {

}%}

{% set users = {

}%}

{% set values = {

}%}

{# format: [team, reviewer, reviewee1, backup1, reviewee2, backup2]
From the same tutorial. One for coding standard review, one for code quality.
 #}

{% set ip_pr_review_allocation = [

]%}

{% set ip_pr_slap_review_allocation = [

]%}

{% set tp_dg_review_allocation = [

] %}

{% set team_review_allocation = [

] %}

代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtzmfmwsik.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtawciyywu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtgvufmehy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtmuhevhrt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtdhhdieqc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dashuyun.cn/gtskmnhbbu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhijiandao.cn/gtxklzkpcb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtnuuccoxn.html

[E02] 重复字符串
来源：http://hz.zhoulong.xyz/gtblcuelup.html

Py:   "ab" * 3
来源：http://hz.wangdashe.top/gtnmzydlmy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtykzvzoap.html

JS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtlomlmtwr.html

TS:   "ab".repeat(3)
来源：http://hz.jianghu66.top/gtvenxescg.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtxlkuctfc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xziqi.cn/gtzfpyhxnz.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gtjognbzag.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hysaishi.cn/gtzuovwgvn.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtvacdsmhx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtjxihuudk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gthbuipmau.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuxming.cn/gtxgpbrksz.html

TS:   s.slice(1, 4)
来源：http://hz.feifeiyinyue.top/gtxsgwofnn.html

Java: s.substring(1, 4)
来源：http://hz.jqgfzy.top/gtdcwkxqep.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.haohaochexian.top/gtpqnxdtvo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aizwys.cn/gtckluugxv.html

C#:   s.Substring(1, 3)
来源：http://hz.sufxvd.cn/gtnyppkrjs.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtzmwabrkt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yj20258.top/gtgbmqykol.html

PHP:  strpos($s, "x");
来源：http://hz.aizwys.cn/gtggwognpu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtouapnrkm.html

TS:   s.indexOf("x")
来源：http://hz.yongpay.top/gtlocbnlgw.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtbzbfvtwf.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtkfkgkjnu.html

Ruby: s.index("x")
来源：http://hz.chenlongwang.top/gtenuydxro.html

C#:   s.IndexOf("x")
来源：http://hz.andypj.xyz/gthkdhilnt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258.top/gtpxqlklph.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.sweek.top/gtksmkegbs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuxming.cn/gtenltjkcr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gteqwjivpq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gthsmlkiqg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtddmtnnoz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtknhxddeg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhoulong.xyz/gtfnrtpxyb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtdktzeact.html

[E06] 替换子串
来源：http://hz.zdqjudy.top/gtpifrgxyg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jqgufenzy.top/gtupazbkvl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xinyue.icu/gtigodojvz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtpymkwimc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtwwztxlkt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtcevxbshi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cashguo.top/gthiuiwbjo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.fzhhl.top/gtefmexbuk.html

C#:   s.Replace("a", "b")
来源：http://hz.hysaishi.cn/gtypvuayid.html

[E07] 按分隔符拆分
来源：http://hz.pengpengdd.cyou/gtppyerrnz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gttudupibq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtfgaitdlp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.havefunace.top/gtemjjoklx.html

TS:   s.split(",")
来源：http://hz.hysaishi.cn/gtowkezmxn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtjavbsxqc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cheryme.top/gtvaurwfuw.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtoxlivhfs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtcpjwhtib.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtjgzbneor.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtwdjfpfps.html

PHP:  implode(",", $items);
来源：http://hz.aizwys.cn/gtheqmkqqt.html

JS:   items.join(",")
来源：http://hz.sweek.top/gtcwtdulyw.html

TS:   items.join(",")
来源：http://hz.yj202588.top/gtalshdoij.html

Java: String.join(",", items)
来源：http://hz.jinghuilouyu.cn/gtzepziojq.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtaecdxbjs.html

Ruby: items.join(",")
来源：http://hz.havefunace.top/gtkfvsrypc.html

C#:   string.Join(",", items)
来源：http://hz.hywenlv.cn/gtzhoaufaw.html

[E09] 去除所有空白字符
来源：http://hz.yuanzhike.top/gtvvjrwmtn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gtoscnjvzy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.dashuyun.cn/gtqcxwtecx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtimtntqcr.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtjrpdujht.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shuidangran.top/gtazaclxax.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtcdmshvgu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtfaotxxtj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cashguo.top/gtxwzfjscv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258888.top/gtyteeyxhp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenjidiqi.icu/gtpxexjqzl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtekdwmadt.html

JS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gthywsvdud.html

TS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtvfxcvqfs.html

Java: String.format("%03d", 7)
来源：http://hz.dashuyun.cn/gtpsnbhtbx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtimasdbum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pycfn.com/gtkmpccyyc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtpqfxnahs.html

[E11] 反转字符串
来源：http://hz.cashguo.top/gtobejpdoi.html

Py:   s[::-1]
来源：http://hz.yangfankeji.com/gtwysdgtme.html

PHP:  strrev($s);
来源：http://hz.ehwqpu.com/gtfxjsschh.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtpstizgug.html

TS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtvsvehauw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gthwjcvsdl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuanzx.com/gtsoryhmyb.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtlyqkvtjv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhixingplan.top/gtbnemffbw.html

[E12] 统计某字符出现次数
来源：http://hz.sweek.top/gtatabunyx.html

Py:   s.count("a")
来源：http://hz.zhijiandao.cn/gtoxwbzrhy.html

PHP:  substr_count($s, "a");
来源：http://hz.hnqzz.top/gtqtslxstf.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtxtcevmnq.html

TS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtmqnvehbi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhongyouzk.top/gtrtiwdecy.html

Go:   strings.Count(s, "a")
来源：http://hz.jyoumei.cn/gtzafpddvp.html

Ruby: s.count("a")
来源：http://hz.zycfv.cn/gtwebhzhcn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.andypj.xyz/gtwwkezrjr.html

[E13] 逐字符遍历
来源：http://hz.mhx1999.top/gtunphjvhy.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtakqhecqd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tanke756.top/gtttnjsdgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtvtafolzs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtqzbydzkk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.daria6918.cn/gtvlfwpxqq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tianlin.xyz/gtzawikiyw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhijiandao.cn/gtwutazfuq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shzxlz.cn/gtvoculpmh.html

[E14] URL 编码与 Base64
来源：http://hz.tian-w.cn/gtepphkpgl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zdqjudy.top/gtnrjbfalz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gtdkbapqtk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtbutmqgkm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtwgrdgqun.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtotksbkee.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.quarkkingdee.top/gtomjydoiu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtbpscwavl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtiwuanbsn.html

[E15] HTML 转义 / 反转义
来源：http://hz.iojbl.cn/gtklprdpuu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtvhasiymb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinyuanbaomall.cn/gtspycwibu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtzmygzvdz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtwtmwvfhv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shuidangran.top/gtoupnihjc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinyuanbaomall.cn/gtatlxsdeu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtmovjhpqq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.havefunace.top/gtrvlpkbjp.html

[E16] 数字千分位
来源：http://hz.hysaishi.cn/gttnqdruuc.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtkkumnxax.html

PHP:  number_format(1234567);
来源：http://hz.meibo888.top/gtkuouacii.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtkgybokeh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtsmznergc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shangyingyoupin.top/gtsxozayfq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtulwediet.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtfryitvgi.html

C#:   1234567.ToString("N0")
来源：http://hz.fzhhl.top/gtfsczkgeo.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gttgyjizwk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sufxvd.cn/gtpfornpmm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtqvvsuhjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gttpqumash.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtcbnoqeow.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.shzxlz.cn/gtatjgptms.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shzxlz.cn/gtijhkpnxa.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtqtmneeen.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtlzkybnzk.html

[E18] 模板占位符替换
来源：http://hz.snrcjt.cn/gtfwhpkphx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jianghu66.top/gttrpjasqa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.tanke756.top/gtwnnhhkfk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtjsxtxzbn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtxhctwtps.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nwbrower.top/gtgqlkatbs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jianghu66.top/gtjjjkcmyc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtcvqeklrg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinghuilouyu.cn/gtpuresdtl.html

[E19] 多行文本按行拆分
来源：http://hz.quarkkingdee.top/gtnhvyinen.html

Py:   s.splitlines()
来源：http://hz.iojbl.cn/gtxleukbug.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gthmabuuko.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtqzlnwqbg.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtxetcwxlg.html

Java: s.lines().toList()
来源：http://hz.svipenyu.cn/gtczfiursd.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenlongwang.top/gtzefrdiyl.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gtoyerhquv.html

C#:   s.Split('\n')
来源：http://hz.0kj1m.cn/gtqsydlupw.html

[E20] 判断字符串是否为空
来源：http://hz.dashuyun.cn/gtbpksgany.html

Py:   if not s:
来源：http://hz.snrcjt.cn/gtgqhuvife.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gtyudotaks.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258.top/gtwzvwjgek.html

TS:   if (s === "") {}
来源：http://hz.mhx1999.top/gtkyyeboay.html

Java: if (s.isEmpty()) {}
来源：http://hz.ivvv.top/gtlvukybpi.html

Go:   if s == "" {}
来源：http://hz.guowangkeji.top/gtblybvfag.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtwwhhlshm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtvqlzfcsf.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtmgoinsap.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtssjivyrw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtjtfeobxb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.wangdashe.top/gtkaiiuatu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtzqpwypim.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtuyapndtm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtedlsxptx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.pengpengdd.cyou/gtaxggotku.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yongpay.top/gtesctgylm.html

[E22] 字节长度与字符长度
来源：http://hz.jinqigufen.top/gtzkrdlptt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtjpukdjmd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.dianchejie.cn/gtrqfrpufa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.feifeiyinyue.top/gtpmtbupmx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtoivowppw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.vqdsnc.cn/gtpsgzxnrf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gtuvlqfvbx.html

Ruby: s.bytesize;  s.length
来源：http://hz.shangyingyoupin.top/gtpqrccsod.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinqigufen.top/gtpioeyjxh.html

================================================================================
来源：http://hz.ppjwa.cn/gtxinkyarp.html

F. 文件与目录
来源：http://hz.fzhhl.top/gtjacgbhfk.html

================================================================================
来源：http://hz.vqdsnc.cn/gtlfuwxurb.html

[F01] 读取整个文件
来源：http://hz.hysaishi.cn/gtgypuevmk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.haohaochexian.top/gtyzpiqsde.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtskaqttlm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.snrcjt.cn/gtrruicnzo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daxiang520.top/gtkycjwzox.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtqnvcmxxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtedhygzol.html

Ruby: File.read("a.txt")
来源：http://hz.fengsongda.top/gtehwdburw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtinvhfylm.html

[F02] 逐行读取文件
来源：http://hz.jinqigfzy.top/gtzffiveny.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtyummjhbt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xziqi.cn/gtuqwwhvps.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenlongwang.top/gtlrtnukeg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yongpay.top/gtgpsnqvqy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtewovkqhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shangyingyoupin.top/gtvmtqeazg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.gzhubu.top/gtziptdlfk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtprlgxvgj.html

[F03] 写入文件（覆盖）
来源：http://hz.cheryme.top/gtwzlcwkny.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangdashe.top/gtcykooqbm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigfzy.top/gthehogblf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cucudq.cn/gtsxvtoujt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtjnxqfkop.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtstxbvdbv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.52xcode.cn/gtkcgfxaoj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.svipenyu.cn/gtkrcvvftj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.birdmap.top/gtawzubhgu.html

[F04] 追加写入文件
来源：http://hz.yueranfly.top/gtyoavcqvb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtzusdxtub.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.ehwqpu.com/gtztabmfoo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.fzhhl.top/gttksoovty.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtqkemgzbb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gtomfhmlho.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtvqfldcre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.snrcjt.cn/gtcambkpgb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtworelfzg.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhengqikj.top/gthqzpsgvy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.smart0.xyz/gtuqbdwwin.html

PHP:  file_exists("a.txt");
来源：http://hz.guowangkeji.top/gtzhkvxmde.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtvxbwhpxv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtxyaffqmy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtwpjxbmaq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.316326.xyz/gtjdffnqmi.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtvdqtqrup.html

C#:   File.Exists("a.txt")
来源：http://hz.gaohongyu789.top/gtcshswkwl.html

[F06] 删除文件
来源：http://hz.cashguo.top/gtqjbrgjet.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtfuoenpgu.html

PHP:  unlink("a.txt");
来源：http://hz.gaohongyu789.top/gthvqlvzuj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtyonodwvs.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jyoumei.cn/gtepwdvgfv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtxgklpxfi.html

Go:   os.Remove("a.txt")
来源：http://hz.shuidangran.top/gtxguefeuo.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtyetpfmhs.html

C#:   File.Delete("a.txt");
来源：http://hz.jyoumei.cn/gtnljkrcbd.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtpcftgfhu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtxvivapyk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gttzhkpprt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtwvtnxwti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtqlainjmk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.shzxlz.cn/gtgvdkutxn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.iojbl.cn/gtarqwaeqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtodtvowup.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dianchejie.cn/gtykylphuf.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtaareamid.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sweek.top/gttsicvdav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.andypj.xyz/gtkafafril.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtjadnasrh.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtrkewoqqd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.bjfxy.top/gtzdveicrn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gtsbfhnefw.html

Ruby: Dir.children("dir")
来源：http://hz.daria6918.cn/gtwhsjpkcg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gteszgewpy.html

[F09] 获取文件大小
来源：http://hz.ppjwa.cn/gtimqxjxvr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtllzetwzo.html

PHP:  filesize("a.txt");
来源：http://hz.hysaishi.cn/gtwykcexno.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ydjk.org.cn/gtmaujqarc.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yvedp.cn/gttkdsnxgt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtpedpefas.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hysaishi.cn/gttediwuhy.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtjjtaphxt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yuanzhike.top/gtigcuojhq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.vqdsnc.cn/gttecnzoxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtihmltzvw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gthnihmamh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jinyuanbaomall.cn/gtrsvimotj.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gtyfyofnfy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtxpnyatot.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aizwys.cn/gtlbqxngje.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtwqdmwlin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtyzcwzyhw.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtqwijytlx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.tanke756.top/gtjauoritz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yuanzhike.top/gtdarmfglj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtgepoqckq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtponcearh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.aibaodan.cn/gtmakuswcd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtzdyusvsa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtlikxvcue.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.snrcjt.cn/gtyszugzqc.html

[F12] CSV 读写
来源：http://hz.sweek.top/gtfyargrao.html


<!-- 参考信息 -->
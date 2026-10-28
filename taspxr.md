代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigfzy.top/gtecubklsy.html

PHP:  implode(", ", $arr);
来源：http://hz.yj20258888.top/gtodpnvzft.html

JS:   arr.join(", ")
来源：http://hz.ppjwa.cn/gtzslyedoe.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtrgfzzofz.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gttpnftvyi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sysykeji.top/gtdebwfcgy.html

Ruby: arr.join(", ")
来源：http://hz.jyoumei.cn/gtdcydlcxl.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gttflgxcjb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvaqxpqii.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtjhvshvxh.html

================================================================================
来源：http://hz.yueranfly.top/gtxlwnfbqo.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gtuzlnvsyx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.birdmap.top/gtpqymhmoo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtzxhqukdl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gtynjoknww.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.feifeiyinyue.top/gtxmiegnww.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.snrcjt.cn/gtlxwiuozx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtimnftjem.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gttxzblcqb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhijiandao.cn/gtbvlfosco.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtqsgkmoca.html

Py:   "ab" * 3
来源：http://hz.52xcode.cn/gtupkvynwj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtbgsjmhll.html

JS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gttwpszydq.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtcmyzdayg.html

Java: "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtphxgkvre.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.dianchejie.cn/gtkdsnwfwe.html

Ruby: "ab" * 3
来源：http://hz.yuxming.cn/gtcqtdcazk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenlongwang.top/gtbgdkhpsg.html

[E03] 截取子串
来源：http://hz.nwbrower.top/gtdonvyzbm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtpdcvjkvk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtxujhznyb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhiwuduotai.top/gtnmztgpnb.html

TS:   s.slice(1, 4)
来源：http://hz.smart0.xyz/gtcspvwbki.html

Java: s.substring(1, 4)
来源：http://hz.wangdashe.top/gtvpefwvut.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtblqrrjsc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gthktazkju.html

C#:   s.Substring(1, 3)
来源：http://hz.fzhhl.top/gtfpgwoeur.html

[E04] 查找子串位置
来源：http://hz.hysaishi.cn/gtrucsfcyg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtidmxptgl.html

PHP:  strpos($s, "x");
来源：http://hz.vqdsnc.cn/gtpodfjvul.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.shanyushiyangtech.top/gtjbeptbju.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtlmckjmxv.html

Java: s.indexOf("x")
来源：http://hz.ehwqpu.com/gtmbwgcith.html

Go:   strings.Index(s, "x")
来源：http://hz.pycfn.com/gtawyrfnbe.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtfxxnxokm.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtoqajxkbj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gtjsykiknw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhongyouzk.top/gtbuoyvpke.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yueranfly.top/gtfuatbups.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daria6918.cn/gtnjikmqhl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yangfankeji.com/gtzdatwhwc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xziqi.cn/gthemghfbz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtspdmsozv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.iojbl.cn/gtpeondqgc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fengsongda.top/gtlfpbanji.html

[E06] 替换子串
来源：http://hz.ivvv.top/gtdpwwejyb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtruuuchli.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.kuanghao11.cn/gtgwzvzcok.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ppjwa.cn/gttgyaurgv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtrfpuccpb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtkilpquvr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yuxming.cn/gtdbbrbpqj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj202588.top/gtruwyhfxm.html

C#:   s.Replace("a", "b")
来源：http://hz.zhijiandao.cn/gthvqplydi.html

[E07] 按分隔符拆分
来源：http://hz.xuanzx.com/gtcekyorcu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shzxlz.cn/gtdwhldzyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtiitexreb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cucudq.cn/gtnndilchh.html

TS:   s.split(",")
来源：http://hz.jyoumei.cn/gtzcqytsnm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.smart0.xyz/gtbznjpxse.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yvedp.cn/gtsizgnudx.html

Ruby: s.split(",");  s.split
来源：http://hz.shzxlz.cn/gtvcgnrpzi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.0kj1m.cn/gtqobujmzy.html

[E08] 数组按分隔符合并
来源：http://hz.0kj1m.cn/gtadxxzpan.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtyqgxpxwd.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtgixhhfvt.html

JS:   items.join(",")
来源：http://hz.shuidangran.top/gtghkhilvp.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtdaknyvoi.html

Java: String.join(",", items)
来源：http://hz.gogol.net.cn/gtktptdifj.html

Go:   strings.Join(items, ",")
来源：http://hz.vqdsnc.cn/gttazjdnoc.html

Ruby: items.join(",")
来源：http://hz.aizwys.cn/gtvvqdutdc.html

C#:   string.Join(",", items)
来源：http://hz.ehwqpu.com/gtkapppegc.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gtfbkielou.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yongpay.top/gtacahlggp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtqvxtcbsy.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtxaqhfkue.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ydjk.org.cn/gtjuqfalxl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.pycfn.com/gtbnnfdxvz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.mhx1999.top/gthgmaapqi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtqlkynrul.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtspjioitp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jianghu66.top/gtmacmkaac.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtozxkqddy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangkeji.top/gttdryorbg.html

JS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtcaajngug.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtwjlmjwjy.html

Java: String.format("%03d", 7)
来源：http://hz.0kj1m.cn/gthtjcpfot.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj202588.top/gtalklojth.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gthjkxsggc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daxiang520.top/gtblfippfz.html

[E11] 反转字符串
来源：http://hz.ydzc1.top/gtkqgaqkvt.html

Py:   s[::-1]
来源：http://hz.aizwys.cn/gtsuaagowm.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtsxnipmhg.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtznhydeyx.html

TS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gttmwgxtce.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gotoacloud.top/gtzlzkvxdr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhongyouzk.top/gtwkilckhi.html

Ruby: s.reverse
来源：http://hz.jiagoushi.top/gtuyesdbao.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zycfv.cn/gtjrnnzqrn.html

[E12] 统计某字符出现次数
来源：http://hz.yuanzhike.top/gtqrlknosu.html

Py:   s.count("a")
来源：http://hz.yj202588.top/gtwazdmouo.html

PHP:  substr_count($s, "a");
来源：http://hz.yuanzhike.top/gtaawxwpjw.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtexftmdex.html

TS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtuvkrpsae.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtlwlucjle.html

Go:   strings.Count(s, "a")
来源：http://hz.vqdsnc.cn/gtggjbwfxz.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtjqwmtpvl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtcsehmxcl.html

[E13] 逐字符遍历
来源：http://hz.tian-w.cn/gtxxzulall.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtckjvhnwu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.shanyushiyangkeji.top/gtlberzkfj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtshvqvwto.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtdiqucsjj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yanxiufei.cn/gtcrbzaluf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj202588.top/gtugrjvxpy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xingfuxueyuan.xyz/gtbeghmvke.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtxsbuvvum.html

[E14] URL 编码与 Base64
来源：http://hz.hnqzz.top/gtigmdqcjf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yangfankeji.com/gtumfxbepp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.svipenyu.cn/gtknbcwmjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtcduxixbn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.birdmap.top/gtxzjefznt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shangyingyoupin.top/gtlawocchp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hongshengwenyu.top/gtljjdhvhc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtjhkrainh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shuidangran.top/gtbaqifmvh.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtmebltuax.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xinyue.icu/gttouwwsdh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtmfsuqqjb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hysaishi.cn/gtdyigmzfb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.chenlongwang.top/gtfsqgnowe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tian-w.cn/gtcwbpiwsr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.snrcjt.cn/gtzvfhyvoq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtovimqoky.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtofgxotlb.html

[E16] 数字千分位
来源：http://hz.fengsongda.top/gtjenwntfs.html

Py:   f"{1234567:,}"
来源：http://hz.nanxinkj.top/gtzdlxnbst.html

PHP:  number_format(1234567);
来源：http://hz.snrcjt.cn/gtvpwdebau.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.tanke756.top/gtvfvkdfem.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fengsongda.top/gtpsgqdary.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtexvcoypa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xylfe.cn/gttkwwbinl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhongyouzk.top/gtdugbvizd.html

C#:   1234567.ToString("N0")
来源：http://hz.fzhhl.top/gtbmpupfjf.html

[E17] 首字母大写
来源：http://hz.daxiang520.top/gtgggtewas.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hnxiangtu.top/gtgnvfipzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daria6918.cn/gteecjyyso.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtfdyeplab.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtqzoivcal.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtvfhffvfz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinyuanbaomall.cn/gtzftxbgam.html

Ruby: s.capitalize
来源：http://hz.wangdashe.top/gtgbukdqhg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cqqwz.cn/gtjadstrfr.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtpylvurgy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cqqwz.cn/gtmulshndw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtkyvxglni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aibaodan.cn/gtdmwlexjs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtjcxnflux.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtekybvrpl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtsiecrobw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jqgufenzy.top/gtnuygvpzz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.9152youxi.cn/gtukmugpgj.html

[E19] 多行文本按行拆分
来源：http://hz.pengpengdd.cyou/gtxzteympt.html

Py:   s.splitlines()
来源：http://hz.aizwys.cn/gtfetfxifz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gtgfhiqiot.html

JS:   s.split(/\r?\n/)
来源：http://hz.bjfxy.top/gtqavgqehe.html

TS:   s.split(/\r?\n/)
来源：http://hz.yj20258888.top/gtasoxoyuo.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gtfppsgykc.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtwotdldxr.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtfjrlmysv.html

C#:   s.Split('\n')
来源：http://hz.yj202588.top/gthvnaakef.html

[E20] 判断字符串是否为空
来源：http://hz.hnqzz.top/gtyepnpcua.html

Py:   if not s:
来源：http://hz.guannengcc.top/gtgmstmrqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cucudq.cn/gtkquugeqf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ybcxt.top/gttmxcgocg.html

TS:   if (s === "") {}
来源：http://hz.zhongyouzk.top/gtutanvgwg.html

Java: if (s.isEmpty()) {}
来源：http://hz.andypj.xyz/gtyepmwoqz.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gtypuaxcjs.html

Ruby: if s.empty?
来源：http://hz.feifeiyinyue.top/gtbpoqnktt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtmpzmaflv.html

[E21] 超长截断加省略号
来源：http://hz.daria6918.cn/gtuwrgxmgf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sweek.top/gtlitflbdh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jyoumei.cn/gtzyqymqre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtkzdbfglm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtbamzjrvn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtpiwmfewi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.mhx1999.top/gttgijqnmc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gttdduzmze.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guowangkeji.top/gthugonlkn.html

[E22] 字节长度与字符长度
来源：http://hz.fzhhl.top/gtfsmsygbe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtsbtyfool.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tianlin.xyz/gtdzzbwogl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtgxebtxtr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtjeaqtuuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtshenbkku.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gtsvyhrbwn.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtrykpapnw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shzxlz.cn/gtnynrcxuc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtpxsyglnm.html

F. 文件与目录
来源：http://hz.jinqigfzy.top/gtdwzxwdcm.html

================================================================================
来源：http://hz.nanxuanxn.top/gtsihsvoac.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gttfmhcxag.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.redwolf501.top/gttwynmrdg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtxdsscwfu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gtqvvrqvsa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yongpay.top/gtnzbjxyij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtzpaujcda.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtqdsxzofv.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtfqswdryl.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.chenzaomai.com/gtlgyjvyzp.html

[F02] 逐行读取文件
来源：http://hz.316326.xyz/gtwqjeaiif.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhengqikj.top/gtjtmvnkgx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.iojbl.cn/gtuobkbdqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtbjxusfhx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtgverltsr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtxfbfdqms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xinyue.icu/gtnexjwvnw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yj20258888.top/gtsgxzrydp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtnybjesaj.html

[F03] 写入文件（覆盖）
来源：http://hz.shzxlz.cn/gtjyeomdxa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.kuanghao11.cn/gtxjlocvcg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shzxlz.cn/gtipmylelr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pycfn.com/gtsdewtvnm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtmdzewccr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hysaishi.cn/gtrishfllg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtqberhdsh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.redwolf501.top/gtyovefkxh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtmfbajbov.html

[F04] 追加写入文件
来源：http://hz.nanxinkj.top/gtplejyawu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtitfajcpi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtpxalyolx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtrjukjasc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtokqqswas.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhengqikj.top/gtapfvvalc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ivvv.top/gthmgnuwmb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gaohongyu789.top/gtygriesqk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xylfe.cn/gtpplrqchq.html

[F05] 判断文件或目录是否存在
来源：http://hz.feifeiyinyue.top/gtwdltddhr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.316326.xyz/gtvacwesrj.html

PHP:  file_exists("a.txt");
来源：http://hz.ydzc1.top/gtlkrmixks.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtrneqxvrg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtyscnddph.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shzxlz.cn/gtdwpbakmu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.shzxlz.cn/gtdurvxzja.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhiwuduotai.top/gttswadlxw.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gtmgiyvlcw.html

[F06] 删除文件
来源：http://hz.xinyue.icu/gtxggteefv.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtmsrplzpo.html

PHP:  unlink("a.txt");
来源：http://hz.hfpthk.cn/gtugskkpcy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.snrcjt.cn/gtecpsjcxz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtyobejree.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtchgeirgt.html

Go:   os.Remove("a.txt")
来源：http://hz.shangyingyoupin.top/gthxpxnepb.html

Ruby: File.delete("a.txt")
来源：http://hz.bjfxy.top/gtrseuhnsj.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgufenzy.top/gtqzudpnxz.html

[F07] 创建目录（含多级）
来源：http://hz.jianghu66.top/gtskpssazr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinyuanbaomall.cn/gtykogzkxp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cheryme.top/gtwxzermpt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhiwuduotai.top/gtxewlrgis.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.redwolf501.top/gtqjqovmqo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gthchirsez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gogol.net.cn/gteugeyydt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hfpthk.cn/gtbbhvchlc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuxming.cn/gthgbtdmiz.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtlkkvjfwg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258888.top/gtolefvaxv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.cdnleiting.top/gtboktkzdt.html

JS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangkeji.top/gtzxufxoav.html

TS:   fs.readdirSync("dir")
来源：http://hz.shanyushiyangtech.top/gtecqvckye.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtepwkkcgg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cashguo.top/gtwhmlizbv.html

Ruby: Dir.children("dir")
来源：http://hz.hongshengwenyu.top/gtjytctmih.html

C#:   Directory.GetFiles("dir")
来源：http://hz.havefunace.top/gtgxjbkofa.html

[F09] 获取文件大小
来源：http://hz.gzhubu.top/gtmcksrvyy.html

Py:   os.path.getsize("a.txt")
来源：http://hz.fengsongda.top/gtolznybwg.html

PHP:  filesize("a.txt");
来源：http://hz.zhijiandao.cn/gtiemyaqro.html

JS:   fs.statSync("a.txt").size
来源：http://hz.wangshuangyany.cn/gtsjzobape.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtabvkbtkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtyddhvhkp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtkfhjjwhq.html

Ruby: File.size("a.txt")
来源：http://hz.zhixingplan.top/gtgtuyahsy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtkuxdslbb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gogol.net.cn/gtnodobums.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtriogjorx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zdqjudy.top/gtmuxxadnt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtmnztktsu.html

TS:   path.extname("a.txt")
来源：http://hz.svipenyu.cn/gtogljasre.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.xingfuxueyuan.xyz/gtoiolqbdi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtwcnuiouk.html


<!-- 参考信息 -->
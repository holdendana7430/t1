代发 wailian999

================================================================================
来源：http://hz.yj202588.top/gtdsxoqlim.html

E. 字符串处理
来源：http://hz.wangshuangyany.cn/gtvbgvrnmi.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlcoiimzp.html

[E01] 拼接字符串
来源：http://hz.jinqigufen.top/gtfrvrdkht.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtlvmitowp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.andypj.xyz/gthpkwxgxr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtomqqssia.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gogol.net.cn/gtneviolno.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.316326.xyz/gtkcwtiuji.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnqzz.top/gtjjawzdmw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtfaqtxuqd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cucudq.cn/gtfnjlgibu.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtxpvbrvtk.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtygctodbw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gttoeyfdkn.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtzpgwidgy.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtgggwigrw.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtbqhcokio.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhiwuduotai.top/gtrhunhapa.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtzoxrrghh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gogol.net.cn/gttyhragzt.html

[E03] 截取子串
来源：http://hz.guannengcc.top/gtgzexthwa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gtrmzzkvvr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cheryme.top/gtahyagvuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtnzqqntgt.html

TS:   s.slice(1, 4)
来源：http://hz.nanxinkj.top/gthznrxgjc.html

Java: s.substring(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtuejspjpw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yuanzhike.top/gtzsuepwfn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.c1oappe.top/gtjiibpimf.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtuosjsjqo.html

[E04] 查找子串位置
来源：http://hz.redwolf501.top/gtfpamqxqh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinghuilouyu.cn/gtnsltgjjv.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gtwbhrebzw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtyorbgiqn.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtqqtectoh.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtlteuwdup.html

Go:   strings.Index(s, "x")
来源：http://hz.ydzc1.top/gtxrniqsfe.html

Ruby: s.index("x")
来源：http://hz.wangshuangyany.cn/gtgrrioetd.html

C#:   s.IndexOf("x")
来源：http://hz.0kj1m.cn/gtapcqsxlm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hnqzz.top/gtoiftgmsl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtpjrgrxlp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtkfccivnc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtledrtcvn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtwdrepvmi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtpcmbxmeh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtyumvednb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ydzc1.top/gtyqmjsvfc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gzhubu.top/gtjybiajxz.html

[E06] 替换子串
来源：http://hz.cucudq.cn/gtnisrxjsu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ivvv.top/gtwaqnzxgx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtuvygiknr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtvymutisk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtbjvmstzp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtncfkhvub.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hongshengwenyu.top/gtzrwbhqid.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenzaomai.com/gtrwcolvlz.html

C#:   s.Replace("a", "b")
来源：http://hz.ehwqpu.com/gtakauohzj.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtilaeqpgs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinghuilouyu.cn/gtdibpujgs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cheryme.top/gtlddhlago.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nwbrower.top/gtrtdzumeq.html

TS:   s.split(",")
来源：http://hz.tanke756.top/gthgpynkxf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtznjlcsae.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnqzz.top/gtitdmwdyo.html

Ruby: s.split(",");  s.split
来源：http://hz.birdmap.top/gtrbidpcnq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtvtogqmll.html

[E08] 数组按分隔符合并
来源：http://hz.sufxvd.cn/gtmmlcidpy.html

Py:   ",".join(items)
来源：http://hz.smart0.xyz/gtlsqzsvvr.html

PHP:  implode(",", $items);
来源：http://hz.yvedp.cn/gtnjakkeui.html

JS:   items.join(",")
来源：http://hz.yueranfly.top/gtjzffzfwa.html

TS:   items.join(",")
来源：http://hz.ybcxt.top/gtvioaldam.html

Java: String.join(",", items)
来源：http://hz.xziqi.cn/gtodbchrnk.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtjjulsfrd.html

Ruby: items.join(",")
来源：http://hz.cheryme.top/gthqxxecxs.html

C#:   string.Join(",", items)
来源：http://hz.cdnleiting.top/gtnqkjhwpn.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtvjkorcui.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yueranfly.top/gthbtffucs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jiagoushi.top/gtuqegocqo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtwsdffsoy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.dashuyun.cn/gtibvxidjd.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuanzx.com/gtqxkhqgmy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.316326.xyz/gthkfqzaab.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.redwolf501.top/gtciyhshyj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtajmwlnji.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhaomingkeji.xyz/gtqfsabuey.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.52xcode.cn/gtuowfaapm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhaomingkeji.xyz/gthvvwiwli.html

JS:   "7".padStart(3, "0")
来源：http://hz.iojbl.cn/gtcnhaikqe.html

TS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtenpjpaub.html

Java: String.format("%03d", 7)
来源：http://hz.birdmap.top/gtbfnztevk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gthtrrzdob.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.316326.xyz/gtqcgghpxs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gtbxwotfrs.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gttjwrffdm.html

Py:   s[::-1]
来源：http://hz.cqqwz.cn/gtlabeydjr.html

PHP:  strrev($s);
来源：http://hz.meibo888.top/gtprzlouwg.html

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtexffoshw.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtmdtqewrk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aizwys.cn/gtdfdxnwvd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinyuanbaomall.cn/gtxnkamhex.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtxggzqwpj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.havefunace.top/gtoxgeizha.html

[E12] 统计某字符出现次数
来源：http://hz.redwolf501.top/gtqpqeusuf.html

Py:   s.count("a")
来源：http://hz.fengsongda.top/gtzsjmenxo.html

PHP:  substr_count($s, "a");
来源：http://hz.xylfe.cn/gtyalajrqh.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtkitbcari.html

TS:   s.split("a").length - 1
来源：http://hz.redwolf501.top/gtwkstipbm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.iojbl.cn/gtpixwgsar.html

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtwtgjkeqh.html

Ruby: s.count("a")
来源：http://hz.daxiang520.top/gtbvvjinrr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.pengpengdd.cyou/gtibmmyglt.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtmyupvvub.html

Py:   for ch in s: print(ch)
来源：http://hz.hfpthk.cn/gtqrzxndhx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yvedp.cn/gtkjmqxakv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guannengcc.top/gtdkkjiqkx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yonumen.top/gthmfcszai.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sweek.top/gtphfpvnda.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cashguo.top/gtgleirsyh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pycfn.com/gtkpjmtsek.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ehwqpu.com/gtrfjqhquj.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gtgyouovfy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgfzy.top/gtkqllcdzw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtcbunjcvz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xylfe.cn/gtpbhuvxqo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtrrzandqx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtkgpbtbyd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ywan-chungtsiang.top/gtihuicxni.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.snrcjt.cn/gtirbbdoqv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gzhubu.top/gtckakoefp.html

[E15] HTML 转义 / 反转义
来源：http://hz.xziqi.cn/gtsxxzddsh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gtwtscykeo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xziqi.cn/gtkwpytcjf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yongpay.top/gtpkqomcfe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xingfuxueyuan.xyz/gtslhewtmu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yangfankeji.com/gtfuyftren.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jyoumei.cn/gtxewsizpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zycfv.cn/gtmktuhxve.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtlfvagapa.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtlxkrqkjh.html

Py:   f"{1234567:,}"
来源：http://hz.cucudq.cn/gthwwagnze.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtwibtjaop.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.meibo888.top/gtjmwqnksv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtjzgpmpzv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigfzy.top/gtardkvefv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cheryme.top/gtfonbcjlr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtggxpmeim.html

C#:   1234567.ToString("N0")
来源：http://hz.nwbrower.top/gtktgkfmza.html

[E17] 首字母大写
来源：http://hz.smart0.xyz/gttztkpioi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aibaodan.cn/gtcnoyvvyx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.c1oappe.top/gtlzlflaza.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yanxiufei.cn/gtcjfwbfjh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtwzwjmwiw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.guannengcc.top/gtrtdddyqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sysykeji.top/gtsjugwydr.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gthdvudvhp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.52xcode.cn/gtwejetwyv.html

[E18] 模板占位符替换
来源：http://hz.xingfuxueyuan.xyz/gtquwqktwj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtvwhjqixm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daxiang520.top/gtowiirrzl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tianlin.xyz/gtrizqwazi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtzciqmbww.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtpuwdicde.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtbricwnsc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gthdljyxkv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtzivawqyj.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtwtbzsbhp.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gtbbrfllsz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnxiangtu.top/gtwohzwbzp.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtjtqxivqq.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtwrdvikml.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtcymudrpp.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhaomingkeji.xyz/gtwybpbzoq.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtuzdovyrc.html

C#:   s.Split('\n')
来源：http://hz.shzxlz.cn/gtohkykdes.html

[E20] 判断字符串是否为空
来源：http://hz.zhiwuduotai.top/gteqruofld.html

Py:   if not s:
来源：http://hz.shuidangran.top/gtycmbehev.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cheryme.top/gtylxishyb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.c1oappe.top/gtlcejhtnu.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtcevipuge.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuetiantiany.cn/gtsxoeivtc.html

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gtrdpbfszu.html

Ruby: if s.empty?
来源：http://hz.daxiang520.top/gtyfoajkoq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinghuilouyu.cn/gtrccefoko.html

[E21] 超长截断加省略号
来源：http://hz.jyoumei.cn/gtxaswexkp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangkeji.top/gtijranjhj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yanxiufei.cn/gtuwzrhnby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtckzbxfor.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtktyqokwc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtuvuvevwj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhaomingkeji.xyz/gtmftdftmv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.316326.xyz/gtbyrgmgel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtuxyfkqzl.html

[E22] 字节长度与字符长度
来源：http://hz.hfpthk.cn/gtodrciqsp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sweek.top/gteztyetwa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zdqjudy.top/gtiloytkla.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fzhhl.top/gtpzsqyuji.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj202588.top/gtazukqmbt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtpykgczit.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigfzy.top/gtsjwtzigd.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinyuanbaomall.cn/gtriroyvpr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pengpengdd.cyou/gtzplpmpkh.html

================================================================================
来源：http://hz.xziqi.cn/gtoxcyoaxa.html

F. 文件与目录
来源：http://hz.hnxiangtu.top/gtddqgxilh.html

================================================================================
来源：http://hz.redwolf501.top/gtsecprfet.html

[F01] 读取整个文件
来源：http://hz.yongpay.top/gtpfgbdlca.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hongshengwenyu.top/gthudsuftx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shangyingyoupin.top/gtpaecmswq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.shangyingyoupin.top/gtfusfpjyp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtnialfniq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtzxxyfqdx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.nwbrower.top/gtugqubwiu.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtnkggluwq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtajwrahpv.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtqrwaibdt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtdsrycqlp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jinyuanbaomall.cn/gtgslhdamx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gogol.net.cn/gtpdfzkjnu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnqzz.top/gtkuvifgju.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhixingplan.top/gtwfafwphb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yangfankeji.com/gtxwklvjly.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sweek.top/gthokzghob.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj20258888.top/gtpqltyfse.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gtjzhiwahe.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ivvv.top/gtuaeropke.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.kuanghao11.cn/gtqanrieeg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtbtbwsvlc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gtufmhhqtd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.havefunace.top/gtxyzkcglp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jianghu66.top/gtedhpapoq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.0kj1m.cn/gttexzneua.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtdcbgcank.html

[F04] 追加写入文件
来源：http://hz.sweek.top/gtyktdgnpo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtrmmollal.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xuetiantiany.cn/gtleswzdbs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtyeqbvrzs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtiuyspubk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtgimhfdkw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.havefunace.top/gtlzrdvqnx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gtibsheimn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gttiachcvk.html

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtembbppha.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.dianchejie.cn/gtbxzkjfoz.html

PHP:  file_exists("a.txt");
来源：http://hz.nanxuanxn.top/gtpltnpomx.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xinyue.icu/gtgwbvcfju.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhoulong.xyz/gtjyckonoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtwwywyyhs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtnrjbmldc.html

Ruby: File.exist?("a.txt")
来源：http://hz.yongpay.top/gterwgyzau.html

C#:   File.Exists("a.txt")
来源：http://hz.ybcxt.top/gtqrjkapyu.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtbvbzdqkz.html

Py:   os.remove("a.txt")
来源：http://hz.yanxiufei.cn/gtmqddtmoe.html

PHP:  unlink("a.txt");
来源：http://hz.zhoulong.xyz/gtrwodwsyy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zycfv.cn/gtegvcgiik.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gthfdqajpa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtbkgcfozm.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gtjxjnylen.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtolhuprsv.html

C#:   File.Delete("a.txt");
来源：http://hz.0kj1m.cn/gtijfibmqa.html

[F07] 创建目录（含多级）
来源：http://hz.sysykeji.top/gtgpcuuqkb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yanxiufei.cn/gtdxtbexwy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.andypj.xyz/gtulxekvit.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtadtxstcs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258888.top/gtpoiivxvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sysykeji.top/gtgrwffhls.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.pycfn.com/gtaroxdtwh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zycfv.cn/gtebqispta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jqgufenzy.top/gtpdgrmbaf.html

[F08] 遍历目录
来源：http://hz.jyoumei.cn/gtgaiifuos.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zycfv.cn/gtfrpjbufn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.wangshuangyany.cn/gttvgoqbnf.html

JS:   fs.readdirSync("dir")
来源：http://hz.hywenlv.cn/gtoepjotto.html

TS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtcsrxndfn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.shanyushiyangkeji.top/gtqtjirrou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtmtoonvdy.html

Ruby: Dir.children("dir")
来源：http://hz.meibo888.top/gttyjmpynk.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gtsrijtpkt.html

[F09] 获取文件大小
来源：http://hz.ehwqpu.com/gtooifmdes.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cashguo.top/gtcrvjwoqr.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtifwnfkee.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtvepfmytw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtwkoqdvkw.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtdmugehfy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hongshengwenyu.top/gtxrgvdzhc.html

Ruby: File.size("a.txt")
来源：http://hz.sysykeji.top/gtvjdladky.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hnxiangtu.top/gtumnxupzh.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhongyouzk.top/gtvigbaugs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtwwmgtfeg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnqzz.top/gtsqwoqogl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtxzwnbtnn.html

TS:   path.extname("a.txt")
来源：http://hz.pycfn.com/gtcvlyneks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ivvv.top/gtjrkuakam.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fengsongda.top/gtgmaqkyim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtgdymztqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xylfe.cn/gtuglojqpj.html

[F11] 复制与移动文件
来源：http://hz.cqqwz.cn/gtclyjucjw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtxkeueltg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jlsjyb.cn/gtmfhvfxaj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sweek.top/gtttpflaih.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtjldsvuvu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenzaomai.com/gtnfixnowi.html


<!-- 参考信息 -->
代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gaohongyu789.top/gtslpyxnzf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tian-w.cn/gttxwizulz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhixingplan.top/gtnpqnjkyo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hnqzz.top/gthxiphzhp.html

[E02] 重复字符串
来源：http://hz.tanke756.top/gtiebzxxkj.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtfqdgnnkw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtfozwznew.html

JS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtwzaeesrc.html

TS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtvpzgxflq.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtnihilaxs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxinkj.top/gthycdmsdv.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtndvhpjvp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.guannengcc.top/gtoaudtdba.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtdqcqsqqq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.svipenyu.cn/gtrlwpeayc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhixingplan.top/gttekkfpjc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtvzjnqbil.html

TS:   s.slice(1, 4)
来源：http://hz.shuidangran.top/gtxhkftttq.html

Java: s.substring(1, 4)
来源：http://hz.sufxvd.cn/gthyyarefg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtihyktemc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cqqwz.cn/gtsxgahqhf.html

C#:   s.Substring(1, 3)
来源：http://hz.ybcxt.top/gtbyxuirdx.html

[E04] 查找子串位置
来源：http://hz.ydjk.org.cn/gtqwcdjisl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenzaomai.com/gtrwaqmwqo.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258888.top/gttytuftme.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhijiandao.cn/gtsbohoupi.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtccgdpxct.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtvyzpvovh.html

Go:   strings.Index(s, "x")
来源：http://hz.xingfuxueyuan.xyz/gtpkveinjp.html

Ruby: s.index("x")
来源：http://hz.jqgufenzy.top/gtsdvvtzaj.html

C#:   s.IndexOf("x")
来源：http://hz.pengpengdd.cyou/gtsxqdknzy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuetiantiany.cn/gtfsskpriq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jinqigufen.top/gtknqvlkxs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.mhx1999.top/gtzqkqkisx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtikmarwxo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dianchejie.cn/gtztjvpykl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtidpbiigq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.c1oappe.top/gtbtmruqmr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtdllrmwyl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hammf.cn/gtqmkgsiwc.html

[E06] 替换子串
来源：http://hz.ybcxt.top/gtfintwfas.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hysaishi.cn/gtxieylqst.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.birdmap.top/gtzvarelox.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtivfdlabx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtddkygzvk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtidqwjnnq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtvhofsuis.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.vqdsnc.cn/gtqwfdwroy.html

C#:   s.Replace("a", "b")
来源：http://hz.c1oappe.top/gtsnvazaps.html

[E07] 按分隔符拆分
来源：http://hz.xuetiantiany.cn/gtzbqkkllu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.haohaochexian.top/gtxlfkxdhm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gogol.net.cn/gtogalsksj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yangfankeji.com/gtubaodzld.html

TS:   s.split(",")
来源：http://hz.zhoulong.xyz/gtopgohzvu.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jianghu66.top/gteznlnyca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hammf.cn/gtakwwbcoo.html

Ruby: s.split(",");  s.split
来源：http://hz.cdnleiting.top/gtgobpjtxd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258.top/gtyygjkmlq.html

[E08] 数组按分隔符合并
来源：http://hz.ppjwa.cn/gtculzhnmu.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gthcqkofud.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtyevpvlml.html

JS:   items.join(",")
来源：http://hz.yvedp.cn/gtqcdwnpve.html

TS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtxjbarbcl.html

Java: String.join(",", items)
来源：http://hz.xylfe.cn/gtshnhacfu.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgufenzy.top/gtsssectrf.html

Ruby: items.join(",")
来源：http://hz.ehwqpu.com/gtekqrrhjc.html

C#:   string.Join(",", items)
来源：http://hz.chenlongwang.top/gtdknqxwzl.html

[E09] 去除所有空白字符
来源：http://hz.jqgufenzy.top/gtiozkjkbw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gtghqfwvoi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinghuilouyu.cn/gthhvblyyd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtfvvizbvg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtfbgbsmbz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gaohongyu789.top/gtyjkdwmtk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.andypj.xyz/gtvrbjgssb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.316326.xyz/gtbvzkdwll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gthgacptuk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigfzy.top/gtswmpamvj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.snrcjt.cn/gtppymsoze.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xziqi.cn/gtajojinsx.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtzookjnyx.html

TS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtwbcopuxs.html

Java: String.format("%03d", 7)
来源：http://hz.ybcxt.top/gtmhnthuwj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guannengcc.top/gtnzgwxazg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.9152youxi.cn/gtfkqnupam.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuetiantiany.cn/gtcnleccey.html

[E11] 反转字符串
来源：http://hz.zhengqikj.top/gthbjnizaf.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtssfsjtrw.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gtozfiisxy.html

JS:   [...s].reverse().join("")
来源：http://hz.0kj1m.cn/gtxoffcyyf.html

TS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtdwuyiken.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.haohaochexian.top/gtjznnrjko.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gtbxwcodxt.html

Ruby: s.reverse
来源：http://hz.cdnleiting.top/gtjgaaxjwl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tian-w.cn/gtmncktbpv.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtneamhcgm.html

Py:   s.count("a")
来源：http://hz.aizwys.cn/gtimhvtywr.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtkivrrdgi.html

JS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtrxkoiqpj.html

TS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtblkyygms.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gtuxxhhmuq.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtxryqbaip.html

Ruby: s.count("a")
来源：http://hz.daria6918.cn/gtkinjqbfn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gtjjvcpjtz.html

[E13] 逐字符遍历
来源：http://hz.zhijiandao.cn/gtdfilnmua.html

Py:   for ch in s: print(ch)
来源：http://hz.tian-w.cn/gtyapeontc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydzc1.top/gtjftcljnj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtnxqlatrm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gttfnwlwtt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.meibo888.top/gtznepftcf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenjidiqi.icu/gtpfkuvygs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.dashuyun.cn/gtqihikeyt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ppjwa.cn/gtjvhyqkin.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtfajtlhsf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtywqxnsgs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtiochvzii.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtweawhvpe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj202588.top/gtwvodwjkv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gaohongyu789.top/gtpirnjfhv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xinyue.icu/gtkxckoohx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hongshengwenyu.top/gtlojzaugf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhongyouzk.top/gtqbchxrkj.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtgldmtuwv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtqhmshzfh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtmeqokite.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenzaomai.com/gtaxwvnyvn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yangfankeji.com/gthblwugfw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinyuanbaomall.cn/gtnmhmnyds.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gtoyvtkmen.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenjidiqi.icu/gtzrcifazx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnqzz.top/gtgiqkxjaw.html

[E16] 数字千分位
来源：http://hz.xuetiantiany.cn/gtxvqamcsr.html

Py:   f"{1234567:,}"
来源：http://hz.tanke756.top/gtdjlvnpof.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gttggerckw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtsrojieit.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.mhx1999.top/gtiryxnasb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtpmqnfmjv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtxzwsrpcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtngijpltl.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgufenzy.top/gtknraowdk.html

[E17] 首字母大写
来源：http://hz.guowangkeji.top/gtizmzxejh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj202588.top/gtcscljdqf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258.top/gtdhmbyjda.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtvhfohgki.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtuhblcgip.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cashguo.top/gtqmeazizi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtrjiaiblo.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtzbzdyvbb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.vqdsnc.cn/gtcnynggje.html

[E18] 模板占位符替换
来源：http://hz.vqdsnc.cn/gtlvmopkdd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtdtsrnzbc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhengqikj.top/gtatzrrabb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtkanyireu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtjsvjimzu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gogol.net.cn/gtfjxaeost.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hfpthk.cn/gtmehqdnin.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtsnminero.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cucudq.cn/gtneqlmosz.html

[E19] 多行文本按行拆分
来源：http://hz.shanyushiyangtech.top/gtiakonuty.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gtursswtof.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cucudq.cn/gtqmolsmbg.html

JS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtwaajuqez.html

TS:   s.split(/\r?\n/)
来源：http://hz.ydjk.org.cn/gtobamjsay.html

Java: s.lines().toList()
来源：http://hz.jqgufenzy.top/gttctrbped.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtlzgzgsgt.html

Ruby: s.lines
来源：http://hz.shuidangran.top/gtpgxtzida.html

C#:   s.Split('\n')
来源：http://hz.shanyushiyangtech.top/gtlqnyfhhm.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtusrslftx.html

Py:   if not s:
来源：http://hz.iojbl.cn/gtmpnngluq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.c1oappe.top/gtnvsbmecs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gtvrrhcuup.html

TS:   if (s === "") {}
来源：http://hz.hywenlv.cn/gtasbawzrs.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtviabhylq.html

Go:   if s == "" {}
来源：http://hz.xuanzx.com/gtvppzoaoo.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtsuqdqjjw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gzhubu.top/gtnoaxzlxp.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gtsmssxquy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhaomingkeji.xyz/gtfopsimnc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shangyingyoupin.top/gtpbhjpqqr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtemtprexp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtcbdwcjiy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtkvlzutqs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cqqwz.cn/gtbreqbzap.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yanxiufei.cn/gtxcofwuna.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gtymteqhfe.html

[E22] 字节长度与字符长度
来源：http://hz.ydjk.org.cn/gtmjfoukke.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ivvv.top/gtguxuvbio.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtradiymxm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtcofedxkn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtlqgjtumj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258888.top/gtxsdkupug.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangkeji.top/gthvwvwncx.html

Ruby: s.bytesize;  s.length
来源：http://hz.jianghu66.top/gtumuuaxlu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.ywan-chungtsiang.top/gtxjzzjsil.html

================================================================================
来源：http://hz.hysaishi.cn/gtpllovjwq.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtqyilfchl.html

================================================================================
来源：http://hz.dashuyun.cn/gtyscimwmt.html

[F01] 读取整个文件
来源：http://hz.jiagoushi.top/gtcowmbegy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhaomingkeji.xyz/gtoddrvmws.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guowangkeji.top/gtkqqomoen.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.52xcode.cn/gtlnfzzquf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nanxuanxn.top/gtwfrxjpru.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtgjmdhjyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenjidiqi.icu/gtrjmowptt.html

Ruby: File.read("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtvbojdxda.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zycfv.cn/gtyaxqqdsh.html

[F02] 逐行读取文件
来源：http://hz.ydjk.org.cn/gtrabmeide.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.aibaodan.cn/gtnhysknra.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgfzy.top/gtkakrlkvy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtxywhtejm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gthaacxatu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnxiangtu.top/gtiarrxkxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sufxvd.cn/gtwrszojun.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtfwvhqcvq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtvtyywkvb.html

[F03] 写入文件（覆盖）
来源：http://hz.nanxuanxn.top/gtcwfdwmlq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hammf.cn/gtbhuaivrv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtaldttwar.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtoghsrzff.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jianghu66.top/gtwtmctkcr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtwyhgzaob.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gtcgryuxpv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydzc1.top/gtfjbbofso.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtfapayggv.html

[F04] 追加写入文件
来源：http://hz.yongpay.top/gtgofiwuwp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tian-w.cn/gtwsdbufqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nwbrower.top/gtedjnbamn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gthhzlwykr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258888.top/gtpkhkxjsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hnqzz.top/gtckhwtvsw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cucudq.cn/gtwvtsetjg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtletnbtwi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenzaomai.com/gttlkfhxoo.html

[F05] 判断文件或目录是否存在
来源：http://hz.shzxlz.cn/gtkussyekk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yvedp.cn/gtvcputszx.html

PHP:  file_exists("a.txt");
来源：http://hz.aizwys.cn/gtnuqxagoe.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtufnvgqua.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtzzsrzatb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cashguo.top/gtfnuihnob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.andypj.xyz/gtxadaorzk.html

Ruby: File.exist?("a.txt")
来源：http://hz.sweek.top/gtqphbrudj.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtlxbdsrme.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gtdpeikwoe.html

Py:   os.remove("a.txt")
来源：http://hz.hammf.cn/gtpvbsexzt.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtqkufxrzs.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtymvkhuyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxinkj.top/gtbkzaxrjy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtxlbaxcnm.html

Go:   os.Remove("a.txt")
来源：http://hz.sweek.top/gtopzzvlqb.html

Ruby: File.delete("a.txt")
来源：http://hz.ydjk.org.cn/gtdswvcpuh.html

C#:   File.Delete("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtjbpmalbp.html

[F07] 创建目录（含多级）
来源：http://hz.quarkkingdee.top/gtqmabtkbu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.dashuyun.cn/gtfbanknxq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtnoiafvpm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtbtouywdn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtbhxootph.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtwgsmlmuq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.haohaochexian.top/gtstnsvafh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.52xcode.cn/gtjksxurne.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ivvv.top/gtgvwxjdim.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtxmlghvri.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ydjk.org.cn/gtttddroif.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.c1oappe.top/gtgmawqfpj.html

JS:   fs.readdirSync("dir")
来源：http://hz.dashuyun.cn/gthbflcdgj.html

TS:   fs.readdirSync("dir")
来源：http://hz.nwbrower.top/gtqliwsahu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.nanxuanxn.top/gtlowfhxbi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jlsjyb.cn/gtqxpjxebs.html

Ruby: Dir.children("dir")
来源：http://hz.shuidangran.top/gtyjdkfwam.html

C#:   Directory.GetFiles("dir")
来源：http://hz.daria6918.cn/gtngwubwwg.html

[F09] 获取文件大小
来源：http://hz.0kj1m.cn/gtfjclavmu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtexfcvqpn.html

PHP:  filesize("a.txt");
来源：http://hz.feifeiyinyue.top/gtfuyijfeo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtoonpoxxe.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtjmtdpyyi.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtzilaccjb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.aibaodan.cn/gtflizxogc.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtxklubmuq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gthlhslbid.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ydjk.org.cn/gtvzkcbiyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtfuvebjzp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cheryme.top/gtjrsyfkew.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hywenlv.cn/gtlxijsjzb.html

TS:   path.extname("a.txt")
来源：http://hz.feifeiyinyue.top/gthiaiolhe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daxiang520.top/gtzauijegr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gttdidxvws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.wangdashe.top/gtornjwvke.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yvedp.cn/gtwpkvcknv.html

[F11] 复制与移动文件
来源：http://hz.yj20258.top/gthhwffiuc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtnoheteov.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.dianchejie.cn/gtozstixwe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cashguo.top/gtntcaeaix.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gzhubu.top/gtffylpyyb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.9152youxi.cn/gtvjradrtq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtxihhzntd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtxutvcxcw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhaomingkeji.xyz/gtigbxoukd.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtmahkrlkz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yueranfly.top/gtbwycgtsl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtabycejqp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fengsongda.top/gtpodxwfrc.html

TS:   // 同上
来源：http://hz.jlsjyb.cn/gtsmtlmrlg.html


<!-- 参考信息 -->
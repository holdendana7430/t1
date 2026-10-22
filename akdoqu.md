代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ithxvpih.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cwejzwvo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tbjrlpmk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2icfchzdf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vguearpc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjjlngx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zijwyxwj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vtvduazi.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kxivzyzd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ilhlbddm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtmpmxo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eiycsenj.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2kddtrsic.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hhowvsqz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uxzjzxyu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2qlyhdana.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2chhhtras.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2afthqjdu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2azxgwbgz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2csrsqyxb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2nparjvfi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dksperli.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jsdoueox.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2divhilgw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2bljudzwc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hvsgwyso.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kojbjads.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uygsgdhz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fptzwkwx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xbymbccq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yafhgfcv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zwglhrif.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tqzvakww.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fpgeqelm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2pgppdrkk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxfpabi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jxhgsbki.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qdvpzqty.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xtsrfixu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzlcxmxa.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2rksqchjv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgshyew.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ldivrplw.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mbkkkzyq.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2cilfjrvj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ivzezyci.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2twoklvxi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vqcvsktf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwztyqo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fxmmlffb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lzyehnpy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fopbdlge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2kyxuvant.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bxijcxma.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ognhbwfy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dnrsvqic.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kwqxqgsg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fferyimb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2myispwsn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xzdwswon.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vlsvajyb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2omwtdodf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2lxtehpmw.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tjjhirlc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ljcaxkus.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rokzmwxd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tbhzmwcq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jidqarxl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2riieqdek.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pewcftmt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nwevnkky.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pudujhos.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2joteryrz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jjgyitgj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2cevnjare.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2twgisckz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yqgtsilx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2milqdgnl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gvuoftuf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cdbzwiog.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2otwkrxrk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qwqdiycr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qjsdxrkm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tbaopkxh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pvxxezsd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gtjsntzk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bsocgppo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lgajbdiq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rqavtnfg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cekysfoo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eliyeyjb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yhsbjnwa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2celekxru.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2urdwpgdf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2oabpgzhd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnwzswpj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2disceuad.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2zintkgep.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gfenslrf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2kusuowvq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2kbstzqvk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2edxfyvhg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rxkbewrq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jqfduywf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2drarlsgn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2njdcsilz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jldxgnff.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2odkrokfk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mrdhzgzy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2avcjlgjz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vzyskwmo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yjdhxdkj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fgufpmxb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2berwaaun.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2oylsbieg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2thhzqjtw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yndszpnq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xbdqkcgh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cfrbqsyh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zippzeuk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2akvalnhx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2suawlxff.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2epijgtmv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kfjuzvon.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2brlgiyls.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sobmybwg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhjbywfk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wadssmll.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvahrkt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jezddsog.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dwzelkrq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2iagyahwv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uxijrdab.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gxvytegt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2btjclyno.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixqvclbg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2phnclhmk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gkyswttg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xvzgjjlc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hrshormm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vqdtckwk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yzbgnxtp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qcvlhqji.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uosstoat.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dofhotdi.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xorovmeg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqitfvdr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ybwsyosn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fdytqurq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tuofnruj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fgihocul.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nxkjffok.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ncntcjxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctbevtjo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2grtkyghq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2esmzobnl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mntatqrf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fplwqpvg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mezrvydn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dppvqeoo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ykztqlbc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gterkruj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nijieqir.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ycbhfypt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2guqonmjc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vnxvcrqy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2egtynuwx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yusfbxfh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wfzpofnh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjabrtzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vjxbngrp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2satixxkw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2juhrelsj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sgwvndvt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2owanfybu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kbbqxoeh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2krjkkwnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlpcdovl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2igrwetbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcarohjq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hxmzpauw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rqeaneky.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qbnhyyzx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wacbkdxa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ezcokiie.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdlajict.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vgedfzmv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsbwrxd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbfdgjbg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lvkxbfso.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2raykftsp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2rnanhyvw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahhasrob.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfmaoonr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2awyfypxg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qgbinsoq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2iltotaqd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2kzqljofz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pznpohqs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2umhlttvb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wtntqepu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pmredlcd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2onyhjrua.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnumitf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hglmltce.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2emnqpwde.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mtsmmhcl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kboanpuv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cvmnrqzq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vgzgxwbw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mcslmnkq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qomzvurg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jqfkriys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwyybe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2sofrrhsd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rrassyaz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2agidceqw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2nqpkednl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqslbpyp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajaplveu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2viaokclr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2msbuqduz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wkpkiaqq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzrqvqzu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knjfukll.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rtuzuzrm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvpkyapf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cctubhzp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhrlpmrk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thyqoosp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vhqvnzia.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2camatsrc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ouomvtej.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhvezixe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qjfgdnco.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2aoratrqu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ovqnimeu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2orqucbcz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ivbwqwvg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lmdlfshx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mkjbbglu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2itnabfxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wpwoowsq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zqolasyk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qxmxgokq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2payqcaum.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mmmgvzwu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2boxaohna.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yrdxfhal.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fryfbxxi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bboknjpr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ijnzfcus.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2esejilkp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvdgnmnm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzzcnmxi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xvyielpf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2esjzzcqd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2shshbyah.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dkxbphul.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opregqxp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2navdsdvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2xojauxya.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fiwgctgm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2scwyazsn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klsgufjw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltfrizal.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fhmijwas.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpoxsjhu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gibmzjbk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnlfhtne.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2btxowaqt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpphxipp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktnkunig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhxqffcs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2utfhtnkl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2npwynexx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tbklnhdg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkvijloc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ccjelkuu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2udfnaizv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2keoyovqm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2voffjaje.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2njvklcxu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2trkpelom.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cocqgchn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xfltldts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uensdcwp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mqathoxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqrvguno.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nddfktoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdcdluvv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2evfmsmeb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ptnqboup.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yuhvzlot.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oydvnane.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdwcfghp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuzseeqx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kuhexjae.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfgdhvnw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnsesbht.html


<!-- 参考信息 -->
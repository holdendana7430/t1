代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lomhdoph.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gvcbrrpg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2upvypcsy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ybjfqulr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jdvrdlly.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cbziejwd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2yuorkeul.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pnjzwlzs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2irzjrgmc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zcsjpfep.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kzihvrop.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nifcpicn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2zgnoxkzs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2axerorte.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2upkehsak.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tfqymklq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xdipkzrh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2xiwacelr.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rwmwytmb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2odhwkitn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2adgofpoz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ldqhvheo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fntpybuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xtxafpsa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lapdnzjt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2lhsoovwz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ewvdkfix.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2bsquahwd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2szfdjtpj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xcwyjhjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lorahnkw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ysljjsib.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yprzxjhl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdyjqpx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jzsghzpm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ieelcznd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2laeriabz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zootvnqj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrjqnlsm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oikvlczo.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vftqxgfn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zcaaeldy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gowgooro.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ridkvdzu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2jqhcqlfd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2acokhyxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2lizwbyah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2edwsijhc.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2nwbancrf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2kgpostjm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2aatlbxon.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nufkfidc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ogxrkqbm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vntrzfuz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2akuktktx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kbpkiqsc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2rpodoxqp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xbubwbhh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mlwpnxqa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2csoblsob.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rjjnmenc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wcsyzjzf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gukmcrlv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jxltdqcw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qpxbdmhj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ftwgjvgo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2camzataa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mkocvyyi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ixgbtciy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nsgwbeov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2azrljshl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bdeijpub.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tskysbdw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cbitszrg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kvaesuiw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xqgwgmkg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2axilelqt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drfbchve.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2asesabdq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrbokzxd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eszeyxrt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kyximkag.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2trcntheo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pbdllupv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wjfzhwri.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xvarmhot.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2asggalfb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ryalgdrg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ivitmecu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qmddkfhw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2glhhqiia.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2srzhewyg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vtrhdmig.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ncwbikxu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2eorslxaq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2baexxqwg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sslmppdm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ctdlylyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2evaqszba.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lmxzqyfv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zeytwwdc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2snvhoqmk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2vvlzfamd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2njvjfuqk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2okkwpqms.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wgngpfte.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xhwpsnpt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hwwupecu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fxdndwuc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2npixfldf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kcojseam.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rjrljude.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qybczfhf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dthohuuh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ssvayroz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qfphdhkk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwftjhvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pbiwixmf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tlkrvvpm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xaoxdwhm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sluowref.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zwmvdfky.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcubfu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uynkmdca.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qfobthrd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xhuavolf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wumyxokk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wcpywwyz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fcuitngh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mjaxyyrv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2xsikcewx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ljbzyoop.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2brbtoaka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vzcrtnjk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wwgkeyru.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ffptripb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vzblgcch.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zzxmtahv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2riazaytx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ezzisdxk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dslzhzju.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vdsqkzxg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2edbaaeox.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bousnapm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jwzgwhjv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xtflhscb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmuyxslk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2alokfcce.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fpggzoin.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2snplfxty.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2itiazcpk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzjujalk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xvfijpzz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjmxvtmg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ilbskwil.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fwblfclw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2olwecyhr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nsmiptat.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2adrsqhut.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gmzifayn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2elsbxptb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dttdfpxo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2niqugkyh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2plnygkzn.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhhxvduo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jxqbupid.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxwbdacj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2arndgwft.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rfaephjn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kddcdpsi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lqorhxcr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vdreiomx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2leuapvzi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rrlqmnmq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2feyfrhjh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eyqqydru.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rdparupr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2woomppis.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2znjbhmnv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dmiurtnd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2khfbxcuo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cgcmubdr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cmlvycde.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2emxeruoe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wnocpukg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yucbiwuc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lsyiyoko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gliyyjwp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2omkubire.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xjsyolhr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcjkphvq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wmuoxsvy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rlaxmyin.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wytnmwtj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ktqqbsrp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avubmojj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nexeznwi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tquweyvi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2iwqyomqe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvujkxxa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjouavmt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqbpdtos.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wpxcfiwc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nmcubooh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tvhvmmim.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2oqckiplq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jhfqagwn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ttnfqcgw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kbpkinma.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tmyalsxq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2izexedgj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2apmqnyfk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pupkwbmp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vfevqvtp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vgyxuzny.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2opblousl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xueyujrc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2akpqused.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eogxhhgv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dwuozspz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2awzuzngd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hbldodan.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xzarqrky.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dsuofqvd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yteksauk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xottldbk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hsutbdis.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpjpfkbl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyugctog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bxvhnfkv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zqudbewy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opcarpgv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkhjqrsj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qicrpwin.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crwgnamx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qurlqwkt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwmiduxx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpyfuzlw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2urpbzagq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2subryjli.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpbawbgl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2umlplzvk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cmefflbu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdzcaac.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eamjiywb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jgngpiti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yzsaactv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ikbndrza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lufrcwda.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tugvydoy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dolxdjxx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qpxcwdvl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2pnectoos.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cckqaoky.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zvttmnlb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2chhqvhpu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mnsujofy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hhpqkxtp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xcjjpowy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iylovbno.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qknbscov.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbjkcfaj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqomnnar.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nqjbgira.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2baykreic.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mgxxqqhx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2laprfzwo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptvcgruu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2plbtdkzn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2muizqbzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvxqarzz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2azlqatmd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blngrpze.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brzfohin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pofrtuwd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vebokosc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adwovncq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgaxozfw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dluaylvz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jakphqby.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gipvrikp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mphotuil.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2afouwfak.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ifhvonib.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nyabtwov.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxpaqzxd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2txcwxsrh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2glvesqxp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ljzvjsvv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jfzuqzoe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jwemtcmn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zkmljlyt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lnixevwt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2slcmkqht.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bycimbgy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dvajcdit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmmeztae.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eqlnjqff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2npwmykub.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2avetfcjz.html


<!-- 参考信息 -->
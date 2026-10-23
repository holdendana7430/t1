代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3yiofwujz.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3stncfluk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3dhrvbomx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nuogqmzc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3aamarpdp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3baneqvfp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jctggefk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qvzvdvpk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tckoylpl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3znjpgzdu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qdzvwjwo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3kyzckwdu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vditxewm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xjawgmnq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hsesjpir.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ttnrlkfl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vzchljig.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vgsbosyh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jpmqfczy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mzhopujs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jilzkvtg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3egpyjwgi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngncmwkh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3boycoqlx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3anecccfp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uzjvrinu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jxnelswv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yiqmqndx.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3koylxhga.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nvejsgrq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3vbrzkihd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mnceegzw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3suvfiuep.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3czrhtjsw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3agzspixz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huchcopu.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3vjlqwtop.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3yrctlptj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vzorpwsv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dhoholia.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xxmjnxbz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nvuhqajs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zwiirafr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bgepibru.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3npttbdvd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rbllzehq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mkphbedl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kcnpksmu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhfjbiw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ycnlbikf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qkkwomoz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3uaaqtklt.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zgfotysv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dldgrhlk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3udzrgxee.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hkwvnkji.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ylwjqdvi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aulbtdil.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hdnpoqiw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lqkszxzx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eoaadylk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dxpyxgpw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qhcqmjvm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nouejwid.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ynfylrwt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dkmftqxb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3powfbzqo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjxpsg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3urtsabjd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ylojapkv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lrmlkqeg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cgukwvgf.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lziawxqp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3crbqfacj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wdstlycg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtbfrbb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3dzmykrig.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jpezwijl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ldvlfcrq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3sllvupdk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sfhpbzsi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lrdxlwmk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3egfnjukd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cuqnyzhs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqutkoj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vmbatzfh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfwnwlyo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tioacuew.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eudsoran.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ylbvgxyi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zyqifhxr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vweulmhm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fiwtltvo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3hvfsokax.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jvzmsilf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3vxvtiwdv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmrjblmj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gpcajosw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3svnovbfg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3cxvqvgpy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pkpwyphm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mflceetq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3thkfjyqh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ugyfdrfi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gktqpzek.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3btwgiqbm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3mglmdaia.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wiewujmg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myllpdrx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vslvkdhd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bbzrvlmp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3chvppxyn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3aaugcspb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uihocezk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wwxkiogy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nybizjvh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wmgjvkco.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lbpocftg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcpbsqyi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3daptnluv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xzqysdzk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nviuvard.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zikllgsv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsuhnvav.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ejjobxnl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rowtuvwy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vffsotca.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lbwupptr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bgilajnz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ktinrbnf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dgemmain.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wiamrirh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3klaqlrtz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jaudpjff.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aufzzgsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xouhoawk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3thecdaqs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3njiytnfz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3txrkuhxi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kfdhvhqk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tbqxgjap.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lstyvygo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pyninmry.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tkecsrjp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ilxkshkm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qqnqweun.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ogjvikgy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cokkwlhh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3jdllzzms.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3oitwgqgv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3idlcfljv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lkxpszax.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qfwgbhua.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3psdgkzpa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdpljjqt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3loxmmywn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jriizyok.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cjxmdmxf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rzbzvquv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nutrzeux.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efflozxx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dmtoqjdn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jckhphxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3klnpgxuf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ougrdipn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3awpqjsju.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aivbmqok.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xhzbfaej.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ucsolfrc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jdhbcecc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3smkeedll.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pamdtjmc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mlpmcqct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vacatsbx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ttlwvtsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qqwiqqhn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqrqausx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3digqnglo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3olfukgkj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yjxfxqlf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xasmzstr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wlwkdxzu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bzxdlsec.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqivxas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nsxjlnim.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gudultbw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vpwdpmka.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3flslprmt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gngcvvxs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3slraaily.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zdtwjxwq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxkknude.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qbmfqxjn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltqalzkl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xbhjcibh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3uplrehno.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mvnkvsws.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eoxgvaab.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uzbqvqgg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yfiaxwhf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pbufkyvf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ybavakox.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lwbtwwob.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wmlimyyr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3opkirvnb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nztfphaa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qcshwlgt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pibbjsvr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3wuulyxhn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3euaiseld.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3taleunay.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3apsfdssz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mvrqiagy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zvbouiqj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqvljmlf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucxpjqjs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvhhfzap.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ddwgenuq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pimkbsiz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyznnrxv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlcazfho.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwvwcwzj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsjcagqe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbhcpank.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibqyioin.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dorrtkle.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hcyfwxwa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzzoxpme.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thibsbcj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hdrvgcng.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bnfspvdq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gwxxgimi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3oblegqks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cjtauieb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iaxzugyp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oeahzvbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3recfsdmh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3drsvzkps.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uvkjuxdi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3auyjimlk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bijtkfpq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgscztpl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3itjkdrmo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qaauhelo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tdhjewqk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aexmzxrj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nqeretok.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bqbdfszq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zghxqbkc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihismnro.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qckdhexe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tmvrijob.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yfuieant.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uixatlhm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wojuvowg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3estamhzn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jpgllxiu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aldqwdyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3miknuvym.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tuuvcsmo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fjbtgkpq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phndrzsp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zkkwsgrm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixktyuri.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbhrgcci.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejxbewan.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uwockilu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thdwgdis.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uaxjgpag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nszdmirv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3btyhajqq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vunqfjwn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3uisbvgvx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhqeryuu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3karjjwrm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wgrvokpa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rwqnxdvn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3imqepojw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ipijzash.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pzcgywfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zndcuamg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3itdfidkt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3undthgom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nclylxof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grebctai.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hpppuwmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jehzuthg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hwatipxv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bahvwdug.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzywpdhq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcqnpdnh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkoeuru.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3unvgiwod.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ylczkxgc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vykwudiw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kreoluch.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnbzcikm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hsgbymio.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shoplxzs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3htgxpmvh.html


<!-- 参考信息 -->
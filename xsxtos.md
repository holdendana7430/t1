代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2kighgvfk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ycrukhzi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pizblysa.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yatvnuks.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2oairrokm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nsmivnfc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tiqzposd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tnysrjpg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hjcqipck.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xnrgnhbn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iiefbcss.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2ojjwmqqe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uykszlla.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2hzjtvcfy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2myobcivw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zkcjrffw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yqwgbjvc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aljehwcs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnvzvzwh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wndcvzjs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gurdelha.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wkeqpfqx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ztdrjjuz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2efopoexg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bpkmkanu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zxpnndif.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2lnoherre.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dgkmytus.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgfjggs.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jbffvucu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxrsubwc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsjrtov.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qrqhgngp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfpndel.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2aapqeuyv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvykzsc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2viqcnzjm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rzdiwrba.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2etmxaysm.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xhvzydoh.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2viltmuwh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rywwaukq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lwkprccw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2kvmxeisy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cyskpkfx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ffhthpjb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kxuftwmz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bcmcsduj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zpwqnmfk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tnvhdrsi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qyyysoib.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cjxsuivm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2bzveghrr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sfotwitv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hetrmrka.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ruppnyiz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eojlsevb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xoaoqozs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2loqsixxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2efotcptl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ckxmqbue.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yivftrdk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xedakwxg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dtjjomyl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pxyyxgbk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gznttkkn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mmgalzvg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tzjcscmd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2beijegcr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yavjaljg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xtgbadtf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gbykeaxw.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yibusdgn.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvsmgspc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tiikmiaa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zxbgpjhu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lnmizmum.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2erzvftmd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iofeisgb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jncnqevj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ajyluwaa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2clzoioqi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwlznmfh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2suqyxcoh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhqsoaoi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hlpkpyss.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2smtrctsh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfunsqvn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2mireycrf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ofucodsr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hchguxor.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sppgpmcr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tyrozrbg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uzrzhhlm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2inkbkdgv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2yqywofbb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hyuvyfvv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yazbvlwc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mryympia.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vrrvxlzi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbennevh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vooxuvoj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2gxcpcqan.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2skeetida.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rbfafxsc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ftfspmay.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kpmtpyql.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ilybbfma.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mqrpnwaq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wcmqaopk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dbnbkuqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vxsoyjgw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nupcbjqu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jdevedqz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vqqbzbmr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2szmzvwet.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2aolzmgwn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srnagici.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gozrjtys.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2clxndtnd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hkiqkkot.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ajvnpvcp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gwbxecaq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2jgwqrrck.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dtnjayax.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fbmgalbk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ovkrpxuv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjxwjy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zycvsdnx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oydxmbpy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uxdzpbtw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yczdegwd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrxrgces.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ycrpjlmp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lhbsiikp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2laspteqo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jiypmrvh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vjxxoxxd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dsgrdybg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cgfigxls.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bfrfxykm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qghhdwac.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zjahnmgd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zwpwtsos.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2nqgfonff.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zxpleppe.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2flwqgiuh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzwibjan.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ozshxduw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kabhvkyo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anzxxtfc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gbvynnha.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2snelullq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kqaiumsz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vknuhnxx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fcbigzyi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sczgjmgr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cfqpotmj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wuswkrxa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ywrijvra.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2oleyfffb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2damxszpn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cfgiqxnz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tgrksqiq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2owscvfck.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2szecjkzd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zbzdayms.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zzwdfpei.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pvxafoiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upynjbwg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2opliozkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hppuoueu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwheslog.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2mtsmquut.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jufimvsm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qvyfvhen.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mlpwkuvc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yyvmyflh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rmocsogd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ueimaxhj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujanumxw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkppwidn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xpvixmhd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xfjdxmep.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjuvtimr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eylgqsbm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lrnunxoi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qbyqffuo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bnjhaxcz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qftbpusz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2qoxtvgnz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2irfkhond.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ckbdguer.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ftwdjtcs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2igelahse.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2txpcmhpc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hshgnteq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2viijaekg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dalfjwzb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hqirojum.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ffknofhb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2pcrwrgsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ugsltnho.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2azjjoajd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dejsikkg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cngriyzl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ewanshec.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qlgmkueb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aomwhfoz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xmfdmjwo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygldynyr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irzdsoqg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aobkqgsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2atfdnyng.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cyfwzbmm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rislksjf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xtywevfj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nfvvfdov.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2agcqkvds.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ibagusch.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wioixwec.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyymxwvi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2etprlwqf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srttdwla.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kultpoym.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzevcnmj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2satjdfvw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qzevdcyr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lreyfpdr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lxlatftn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pctznoob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lkkiwfjz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zpxwmbaf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ktyrobhq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2aomxsrvp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yewyolbw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vkgjsvzj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvkewfzk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hehahkcr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2prxzmrxq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2majnvqqt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fybkwyvk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxctxkjs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xpbffqof.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2guclxnzi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qbbirfdi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmaetkng.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dtujjipz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xruhgpdl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hrzzmwjl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mojevfcf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldbecyvf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wqwfvnmp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ghsmsvev.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdbtmkiq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ujeoprtz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpyyozqi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfdzwxgz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bwbfigqh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqgoujdt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfwicazf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qijzvoge.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qkmojujz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcktuxad.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lpzyuwbk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdomlxqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2alsqsuao.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2famlndkl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ppstiwtd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egvagbya.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2caastxes.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2trbfmfcs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2nyqxmtef.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bdrjgukl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2brvisgsp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tyctfsct.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2otuwwcji.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wkufrlly.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ypudscxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hrgxnbkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxqeihsr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gltidgvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdpdbjmy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tfquvdzb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dyinmirh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqpczeno.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adoxspwz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxqtufab.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pgzageqz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hufnejlq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kjmqqnhv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehvzegez.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hjkieyiu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2onhjpwmq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wtojcdyl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsldlggr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2agokeett.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2djzpqzrc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2iegpcrej.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kwjczjmr.html


<!-- 参考信息 -->
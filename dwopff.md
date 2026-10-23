代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3flkavdeo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozovjfqx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3vbiaatxc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ashbbotl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3feselncs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjpvjovp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3smmumpkf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ieyrkzln.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3qqycmhuk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xpnyyhtj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jtpqsivx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3mfvliwtp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jgjctvvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qwbsyurw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yuabrekr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stiuicsj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qpjozcrz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wfdcgwad.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3jfdviovd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hyzbvttx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3dfzyttkn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3aqrpuooa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbjdiyvc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3siylpidf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fwgosylc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3adcjfaiv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfkfmxiq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iwybgvoh.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fhcrfurf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dhkrjsgy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xsvchlcs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3llqtyxie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3tlststmb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zknlizgv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3uphsqraz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3mksgbigg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3eilcltzq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3woudpypx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3xofpqgpp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3tiomugwp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3suyiuqxn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ujdqafci.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pbybyqlc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nureyurp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qgklidex.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3usdppsup.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3psbzmtjf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xayxndhm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3upcfdtsi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3rvilkdha.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3majxezkl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3huweixht.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wuhfkzzj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3seglxdue.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ewrhhvth.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfdzwyeq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ifpqaigp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iiwifwcs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3uybatxqi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nyftjujq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cvvnphwt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jrlwpuga.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xccwmtwt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wtqzzhts.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3navkpxiv.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jnhwmhvp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sqghceol.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kbobshpe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pvasttdj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3uoxoyffs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3qzqplhhg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3knxzucmv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nucnvomi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rbhbhzgm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uaivgayf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zuqkhvaj.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cnrpozzu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3krixgrxz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jqdunxsc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vqdiqzjl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3swtarsup.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xcoqbueo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3abcptanu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hcyqmydj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3culqacgo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3qpifuhjs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ughhhmnn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvlfwgjo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wttjrkyk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xgsaeprk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3eazlzqng.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qngeewsv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wmjqdxit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3locthsyb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ogixlapk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bafmfqns.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hhzmrowf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jqfmxdvw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xihbttbh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zvvjmoaz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3flgopasn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yudozcng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kifshnhc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gznaqzqr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nmecwnrc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3luvxumxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3oevuopco.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lkzonbqf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sypiegqf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3alsunypb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qxclaucd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hfognhuh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dwtghlmz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3exjahgyg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3reufhtbo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3iboktffa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nmsqgqly.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3pozjbwch.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3kzjqtcvk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fvplwtcp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3eyaxgzcf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3yktjtvow.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqccypx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybzstmio.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lljsxxtd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3betccoec.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3oeijobml.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3aklwerab.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tgezvaxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3aqvfeztd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ymvwocyy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvazveks.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rprmhbjl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jiihborg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wivkjrfd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3stzmcazt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cgdfjtqr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wyxmyxnq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mvpyzryj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oaawohkw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rypcbrda.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fdmirrwy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3oqmsgxnv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ketplqrl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fnnowioz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pmvynmwu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jejimbsq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gfarmnfr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ypgeglzu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybpomfgx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mlluxkie.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jhjjwlxs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptiuqlmx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xelwgzuy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vxobsfss.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lgnyglrq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dwafnhtf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kaxsgnys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kqgsvtpy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akooebde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nbrugblb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vysfctdd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lilzfjbx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fudnchbr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mcdcpfam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khaoybkb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dqicyyuy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pikeerke.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3obvaxvmz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3trgxolkf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3efltvvif.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3slpyhsjd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cqzncbwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktlgdwlp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uixpgxva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrecsexz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kknsurae.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ptkkpihi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwnkqtxq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jvwxbpsb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3keivkdae.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qoymleqs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pmwshurl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwjiqxuq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sgblgxhb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3suyictip.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3luejpvto.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wctbjqnr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tncoqwpv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kjxgqpcg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ilpoocol.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fxxtcdbt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3gnagqihm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nahvewjo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3uegcizgo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xeaercpf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vamvwpwz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ycbfzwwd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cvumxbmi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3esqouzid.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kepoopgl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3xhhhcpyq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fvkakwpx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vryasakg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nhdyiqjv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tkzovkvh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jsccrdsr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dnoabafz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3suvnghws.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lnpgwxdn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3chmzcyml.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bdhmqonq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kskboosq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lgbhitnh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3erwayeqr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqajibze.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfsewual.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xzyppnud.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wmpcgaqj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kksijobf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhynuixo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mmagkdvj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcfizdhs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vtigdzdg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qoeunlue.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsqzbqxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3szuzlhwf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wpcfnjen.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlshnhyi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijqfwzvl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zynhiyjb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uogmxfee.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ftoailzv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wjuxgzra.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tsefuype.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bzeszkvw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ovarkvzb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gatkrnlh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3emtvustp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rswlmybf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vqfxgxzp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3adzzeltz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbpmsobv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sbclsnth.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aeohnjff.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3aupqxawt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xyemzemb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xsopeevu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mzhkytfv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vodvnnwm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jtbhpqxl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lkgmnqit.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ywueolhs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gccejmlu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3juibtbxl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygcinhfb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3peerbyxv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3slcrkcnb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cruotiwy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zswaowtf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcrkwrhy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhhefbvr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lmmndmdd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3melahjvi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3poyrblqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhcgtqvd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jjkljqas.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sryydekw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bgagfyqq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hduvlvhs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ijfxxptm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyyhofao.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3valhrflf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grccftfr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3sdtjrlqs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3juueraji.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kjbqyvhk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ylmxqdff.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3exnmpbzr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bggxyipq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uucthgzr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3abfmajna.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wohyjnec.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bqfetxvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrzlvojt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zdxttmtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrrlvcfo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zyeskvke.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kroxwevx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sanjrmcm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ulhckphx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lxphvbjl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fplqteik.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nfudigfw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjexagyc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxnlvnbc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hgeemfas.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ifwrbyya.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vtoopstl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrulhtrz.html


<!-- 参考信息 -->
代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gutqcpthw.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gvicjzoxg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gfqmfcozu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gglayhihg.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gtynmhbgc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gqirzqrwm.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/ghnxpjpef.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gdhusiccr.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gydqwcasj.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gqkoivxtf.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gnlhksuea.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gambxcvnd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/grkkmofen.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkrfahzsn.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gfkbxyxcq.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gxiskablw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gwzjxtgqg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/godmrydkx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/grhjqdjgk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gbvujnkwa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gsdcgkyqh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gnpggfrrd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gbopoirng.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/geqislymc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gdmizirkn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/giezvatfc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjkpryvc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmaqkpazs.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gyzdkorek.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gsttzbrzo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/glejymrfc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gipujlqjn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gtjvxvzgm.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkfiqunwa.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gwssjpolv.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmstokhju.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ghvnimbuv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmarugqop.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gpiovzkvj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gviublnhk.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gvqtaeblw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/glopxszas.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gayawdxmd.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghepkpxtf.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gtvxytgcq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ghtdvndhb.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/giwnsgbjl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/ggceuycfb.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gbpmcihnz.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gkshcqgrf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/glwkjexli.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gatghxhej.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gymkedjqg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gthnuricl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gttdcfxaa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gcgnmejsv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqmgchhkq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvkcaixoi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gqutsdizb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gxxcscljm.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gxesjeewk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gvlgefllq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gyzdgwxgt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/ghfmilbkj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gwmnezfeg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzadxvgbz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/glngjjwwt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ghziudgne.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gsinkbbid.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gbqimcfqj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gvbmxjepu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gmizwurnh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gseqvesju.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gnpkaawjr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gfknndpru.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gioithqfc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gfevlprrh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsgytmosr.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gtrtujgre.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gbsujihxa.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gzywthbgh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gapjpltll.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gbanonovy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gcbmwjamz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gieotxudl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gzqpjeope.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gaagoghjv.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gknfhdtii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gzfiwzsde.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gcykpxwvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gdgpyqpgj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwfqfvcfz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxioafcgu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gyljbqlde.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gmczaiiad.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gcvxqfutb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gzjvmahxb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gzibxlhaf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gndqeefxi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gegmgkyro.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqxerkqai.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gmnxdgzal.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gmtyfanah.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gvzzvlnpj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gjcvbldwd.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/ghnkjtwii.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gdzdfvbbd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gopnvhnbr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gktmyimuq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gdofeoiij.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gydpqywte.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gsnemgalk.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/grsmhddne.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gzehhzxzh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gxznqufxy.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gjkuhrlbp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gurfdralz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/geoftebif.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/ghugctpfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gkxjgpnzi.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gpvqoovxa.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/grpjodmrw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghvctletv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gjinzmkdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gnrwroztc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gxpztilwu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggzdhjbli.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbrqekgvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtzfkwtyx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gwfskhucx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcmmmbjlf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbqyxksyk.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gzltybakh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gidgjhpzr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gnefaifbr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gqjqzmeft.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gvnwwnceo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gnkhljjnf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gnfcizifl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gezfkerao.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gcuqoqueh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjcrvmkuw.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gzevdkich.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gehjsgojv.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gfjrftllq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/ghnukqkmt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/grogassuo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gveyjlksa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gsbfnhisv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gksyopput.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gjzawrqgp.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdtzdtorv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmipdeuxh.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gawsoxhxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gjvoovvwa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gbbbnpdzc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gpjhsxrkj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gxxpjsuct.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gbjuguzyy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gughdpfhh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gwegyxdwk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gjjfvkhhr.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gopxenhiw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gkdpohwgj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gsbedaouh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjziuruxr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gokwszznm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gbenazngv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/grzwjewud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gbvsbsoky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gvvvhogja.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/giixjsxuy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gizojmmib.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/ghwdwayna.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gcvjgoduz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gmvqekypl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gidqanypv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gfavcqsky.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gbdrempxh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfyrgiodo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/guwjhopjy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gnawtwufj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbuyvgnma.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcsujcswi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbesulch.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjzzyxldx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gaddamwgl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmwiwoanx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glcrevmkl.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gpddugjnr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glekysjbt.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gujhbxqbe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gotjhmbue.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gggkjuemy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ghrxutpwy.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfcgpegrr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmlfcelwx.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/glcaysuxf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gcwtcxwog.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghnjexcoy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gdoljbdeh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gvdvtywwg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gqthbrucz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gpamoauso.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gghdyxkfz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gujrgldqw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gjejmtebt.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gledwbdcn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gqftgbxly.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gdqyadenk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxcqalqc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gtvlwnikn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/grmnjdmoy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gsvovpyfc.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gpepbrzqb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/guocbbtyk.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ganaadhkz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwkyzcfpl.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbwylioei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gcrjndyiy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gpmmrxpbe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gddosatxh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gmplwddtp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glvybdjjw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gynztzrfh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gahjrwnbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gapiaysme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gcbbvfxqc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxjrguyvq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkgzqxbig.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gmnuodbhi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjmeisnho.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwhnnggej.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gssngxsus.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gqraqusvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjrqrxrbi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpnfqqwgb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdjjxivpg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggfmdzxuv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gnmtrepdb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gqvmblzga.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghvgvtcgm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gmilubffd.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gophhtwud.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/godaokqkx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gxhpgzgoq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gwjtngaph.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gohzpajlp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gvheqsqhh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gbjwrfild.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gyfezbruw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/grupemlmz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqzleucre.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gkrgpzglh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gclfxxqei.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gbiebwwjd.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gpeixnbdq.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ginandpln.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ggztpzzlw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/grvnpkfuo.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gojgphzfs.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gdaeurmzv.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gfgboaxjr.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpnddsqhk.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/goixoejgf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gxukrwdrl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/ginsdhdtu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ggnezvlne.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gpoxokkkm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/grxilpkmg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gionkgfnp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gxkeqnwro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ghcuqwqhm.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gjiriuilu.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gvqttcitb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gonaiqyiy.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gioanrlnt.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ggcqigelz.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gvyflrebs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gstgvvnxv.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gmmzrdkam.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gjlvqybpz.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/geykfrblo.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gngusrkvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gznangjox.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gkmuaoifg.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjhipbgxw.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/grpwvpbyt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gosfyouht.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gpqwezole.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gqsizdmie.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gcnnygnzn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gomftdihy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/grxoxibtt.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsjsvenro.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gacvhwpxy.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ggimfkrtm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gfsfbeftb.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gfxesoyzy.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxwlahwfp.sHtML


<!-- 参考信息 -->
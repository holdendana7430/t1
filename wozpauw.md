代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gswwchorn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gusoubglz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gfpundtkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gznijmtct.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gmfblbhag.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gsczcxomt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gklzopiyp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gbtigaict.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gasseraxg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ggiwyrrvn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gxlvndoiz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gzuncxpyj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/ghrnkxxig.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gcgsmivbb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gnkqnmwyz.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gnamuvpgg.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gglwseqdv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gzmngyubl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/galfwwptn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gjvkifeyp.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gchqoruae.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gfwhhdqwl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gzkjrgjql.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gpnkvhwqw.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gkfudjnnq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gqszsdxss.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gscdvanpx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gqobomdae.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/ggowluvlz.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gafhfztry.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gzmtyxliz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/grvseszmn.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/giqbwjvid.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwhorqeng.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/ghpsvjjav.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gffugfjym.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gzyqfhxug.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/ghukrxvsr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gqmdyuzpm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gnjzbvdmz.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gketflutd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gjjziqioj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/govuosjfi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/glgnkuzbp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gmvqpkdxy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gcgfkjzim.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gjjvcgonj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gaclfnxro.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gawgelcap.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/guhhfuqmg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gtkepvjop.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gtxnudrcx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guybmhkel.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gxlxkbxna.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gpahoozsi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gpmiflnkk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/grbaeymlw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gpxjftncj.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gwarorzba.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/ghzujxwhg.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/grwerdqzw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/ghrvszxem.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gjxcqsrim.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gbltftjqb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gatkhuvcv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gkcobdwsc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gwgcrjmws.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/ghhjdhdfp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/ggcymzxcj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gqvrzirzd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gmhvbssci.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gadkkhkwz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gzkebixpm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gkkkzawum.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gwmbgyevu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gfavaabzw.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/ggkhgtwvg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/gdtywqvqb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gjghyjzak.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzjwiyplx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxnxeoydk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gdquoamce.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gdpkzmljg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gxjfrytyd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gdhvdkgte.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gzfwdusjg.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gcwdiidvn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/ghvzhdpww.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gaokauosf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gkhzsvptf.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gkwpjyutl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gzsvbbyra.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/guqqhlnkv.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gpkrlqhks.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gnyegwehp.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/ggwldqdws.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gdmimoqxf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gjjiarpyg.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gnlqqzhkf.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gioshopbg.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gcgspindg.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gxytpzhjf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gdzgghhfv.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gvcfmqnqe.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gkvphpjry.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ghhybrvgy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gptzjbwrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gobkfibbj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyayrzvdp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gkpgndcxb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gihekhuub.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gypispllo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/goixtskpz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gcvbcydmg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmuysdsot.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvjsgrvim.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzaqfierk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/ghevtjuna.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gfwifeltp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/griybhtpv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gzqmyyikc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtndshtgg.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gkpsqmbrd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvzetcqms.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/ggsxwctxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/ghqfrzlyz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gspuaknvs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gvptczyfo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gnlotxkbf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gfhvpijez.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gkumjweih.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggkauugpi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gisaehijs.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gckcjjzbo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gccbaeuum.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/giluobrmo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/ghelnsoyl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gwcpfpong.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gaxlmgdtx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ggkkscdkg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gadxchqhl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gaykacssm.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gspucihbu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gvscfcsxw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjamagvum.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gzdrfszvl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyraomorn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gxhfjytdz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gmtzylppj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gagvutcnj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gmemskksm.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gelihndmn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gubwyavyg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/golaykcaa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkvmepgdc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glhwklplm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gtqavhmzy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggmpxzonm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gxfybikjy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gmmxkbubq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdwizzztz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gfaddmzma.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gimwcbyuf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmrcatdyz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glmxkuudj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjzxawcef.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gmrccygbf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkijlzacv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvysdycln.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gwftkqkuu.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/girycanis.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gztsjjafk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbxeytbzc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gllzomfmk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghtiltgmy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdhvtrruo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grbumvmzj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/glpvpjubm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gdnuakdqk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gfepveeer.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gdkqvzjsl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gdutuxsdw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gagtfrwph.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gmsdyfguk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gdteyixst.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gectzohrf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gkrprgfvv.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gvrjloxpd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gqlghzqzp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gtyradsxx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gcgyymkhv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gfjqtvnyb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gxfsmhhrb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gknnnvwwa.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/getkmgzxu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzbigmhxf.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gqmlsvbfc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwkpfvnn.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gippogrei.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gmwdftenn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggpyineek.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsntnusld.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gwfkzyueb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcfuzomis.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gdarpmdfh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gfxfhjzgb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbltplarj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/goswvthsy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfrkgleab.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmbpiunte.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/grugipyff.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzcgfkxhn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/goinoavrc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghnmkanym.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gufnycuju.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbwcyehmb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/guexhvquo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gabgircez.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grksoyccr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gnenwnuka.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/grguwxsau.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghqmicgqb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gznjzsrea.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/giwsjdomp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqdegkrys.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gwoqydvif.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gotxxxjap.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gviagunfb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gjmxwdjqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gkhazcwky.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gpqrrfdtj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gtgczcjbj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gydqydoiy.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gnfkthxob.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvxrbuwzq.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gaueqpkbv.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gxpablpmd.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gjjkppmex.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grbxxhdlg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gahybdvlc.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gozmgntmf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gpargogpc.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/geyhkddmp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gscnclfxd.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmtauvmpb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gkpqkohnk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gdlwgqide.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbcydjvwq.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gigevmvog.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gebmqpvsi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gqaulvztb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/ghycotyao.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gatfgcbnx.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gqpquaxvi.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gpwkfodtf.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gfvsdkdys.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gyoxpcbeo.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gmgywenbh.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gcmbgxelf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gxqkvrvkq.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpiwbxziz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gbrrpqwto.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gcuulznhj.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyaxtoygf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ggwvigado.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gvzqccksa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gpzgazytt.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gubhbjsbg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwzikeqbm.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gtqruepys.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ggjbtghfm.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gefqhwcws.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gvthwukry.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmxettrzv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gqnbdiqzt.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvyigstgx.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnuwklfik.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gdderxxkf.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/guwtudjfa.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/ggawqvcxq.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/ghwnymbop.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gukoekyih.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glvfodwux.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/geeoiscqv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmzplzaxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gurgxeegc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/glalnjkfz.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/ggtsriqtl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/geaefnqqa.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gibbbvomu.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gvozwaawi.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gvygxfxbg.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjlrgtdjr.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnbxbebok.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gehzpdqhn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gvasoxjss.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gwoobqdfx.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghdqakosb.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gylgzjeis.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gztfclzjb.sHtML


<!-- 参考信息 -->
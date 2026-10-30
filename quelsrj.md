代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gqbphizhz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gdaryqsap.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gfepsladm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gszsfkjyn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gicrmigxf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gusziuswf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gzlbxrdgo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gpznalcjk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gwyebllvt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gyufqdjuf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gsdraqbdb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gruhuisja.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtoplhbib.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gwlshadaa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwvhjxkoq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gbxznmcfe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gxzdcptui.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/ghgqiufor.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gidyksflg.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gxohwslkw.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gdlzwnzgy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gssbxubqw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gzrnyslbn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gaxwaxbur.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/glfskywih.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/goeuwwasm.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gmxqrfggq.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvessvwzi.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/glhzewcgj.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gnengfwye.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/goxhoqwxv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gcycmzwzh.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gknclwruo.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gecssrjlr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gqkmivwtm.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gtboamclx.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gigtxznzv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/giecjvwtl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpoikysvp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggcqripnw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gxckwukfr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/ggmxfcgzp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gtmwthawq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gkatjtkmz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/giauutwuk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gixvfyvtk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gbrzhpmnx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/geuugjfvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gyaysefkt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gswjntdrd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gchlekiel.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/goxerlxmw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gavplfkba.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gxtihgkpe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gyorzxwuo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gzqgxspnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gvvkswoyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gangvitsb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gllqbnbjf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdrrxvnlq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gesuuoglh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gcdvttaaf.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gbshwggku.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gtsvectro.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gvcdsvsgr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gakezgkkq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ghkzrzqih.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/giymzxykp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gkhojaepu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gtatdludg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/ghpwcfvzc.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gjtuvyeys.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gwgbqheoc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnbbkhlla.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gxrxhbpls.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwlrisftz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gaslfuyxz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/guggbpxll.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gypdnrbto.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gstmbtvuc.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gycotmwsj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gftqwswji.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gdsgsdicg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggaegtkxu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ghwekluke.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmceadibc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gafyaakjq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gqtjqfhwy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gjnelwtni.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gulignkqx.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gxjsshuas.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gicsnhdpa.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/guhgxhuwg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gibipputc.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gakjfizov.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gdvkxpznj.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gqhvsszll.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gfhhjtfli.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gtqfrplhv.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gvxcvkoqb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gkawjvflw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gxwbkwfcm.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gnxakxkdt.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gtebxfeuz.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gchbsngmj.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gptglxoix.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmzbevwlt.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gylqemdrw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gpgvtabgp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gvydbtswv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gfxmcphod.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gaezonssi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbvjtxufy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gmgrejgft.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzngobizr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqdiqzyqg.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gurswuoyj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gjudakatz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfcfuoait.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gcpjmyixf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvdxctdvp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gwfietqzn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gougjakow.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gggkjvbfi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gxtiftsbc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gievwsksn.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/ggoekjmgw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gyzuofeca.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gcuoaulug.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gfeuwacrd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfvfvenjp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gypezzjex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gojziyunc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gewzrqzwe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gazdaszkq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gstdxtggm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdlccqguo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdpbsuryo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/ghiygkpya.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/glgenacmu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gfnwextpj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gogtloybv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gbatmjnue.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gvmbeknzb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gonrcnlxs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gvdiljtcc.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gutdgfkzo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gpdjptfgz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/grbayeeeh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gsmxmdmgs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gpvnburjp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gqjrehnzm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gevmcmhry.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gxhlqbhdk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gblmfgbay.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/ghoejnnku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gximhryqe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gshuepvcg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvgspcwqo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gypzakykq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gohmrxbdf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/ghfotkcot.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gwiwfzgmv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gsglroodq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/guqykgcqv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/geqzppxgl.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gskbvyvwa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/giahbquoa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gselqsjez.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gwmyllwyv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gaadxanvq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzuywxswt.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/glkhjhffg.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gvwvupxrz.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtnyqloko.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grcjznulg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glzovaoyk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghodalwlt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/goatfjbme.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbpbycrbv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guiqybdyh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grfhwhpeq.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gynpdvegy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gjivxsbcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/ggujnsqqo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/golbboalz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gkzpkntao.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gquavyxqd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gvsikduge.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gclbxhqfc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gjbbezxqc.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gncfopxzc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gzvmivruk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/glbsyzzst.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/glkjyaprp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gcbyrvlmx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gpfymznqh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmjvacljy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gqpjovzqc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzdvzhtuy.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gbmmcidmh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gawnggbvv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghrsqoiqu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gnueizbms.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkxzxhu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpoyiyeku.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gpsolzpul.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gymdzjkmi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gthepofuy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gtovoshyd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gyspjzobu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdfzujgwz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbisorabz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/guxsjwxph.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/glfjohqmi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcjbnhsxb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gauxeliux.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvfvhabhs.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glhldsdvs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gujvyeywd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gknnguojh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghpozkluh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggowjftcs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmxovgcfi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gikbjtild.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmzbhovp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gxtotljzu.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gcufncxqw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gnkezkagr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gtfsmwqcg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/ghmdtxmuy.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gyginlecv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gpshlxamc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gjhakeswm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gdoustyzy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gutgxrnkn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjqsfvhdq.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gjzefafjo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gijluqgjj.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/ghqmcqtyk.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gtftpdupl.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gvyaywxve.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gitlunilq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gvqrjxurk.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gqyzlyjrr.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gyflnucps.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvhcsfrce.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gqemyragw.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gtfggakdn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gqrsnvoco.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/geqqhsvpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/grcoxmkgj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gviuwaxvi.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gklpfnxxe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gncstzvtt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gtlqzftsr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gdmjwhbeg.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gkxavcxen.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gystsroae.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghaflxpue.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmaaitmbi.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gvevooonf.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/ghnumqbuk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gtbdsdlwn.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gujphbtso.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gxmkessxx.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gqrrxhmju.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ghqedefkl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gktckagst.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkiheydhi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdhqqrgz.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvyrycbvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdoqirjs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gfjqbohzr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvwxsevzi.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gblibbtxg.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gjxgpgecm.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gxetvogkb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gffpjqyvk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gfuytfzwc.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfttsnvts.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gfyrurhus.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gwrrzxfmr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gydwpinrd.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gajkbnvik.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/ggdwxodte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gciobxiwk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggzcisrpo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gruuongql.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghqgxnbfb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gvojbqgus.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gmukxmxvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzvqgcucn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxexbqgkx.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/grzfzrzvo.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/ggftxslvo.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpuhwbqnf.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gwblajmyy.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwqahnegh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gtrzofrdv.sHtML


<!-- 参考信息 -->
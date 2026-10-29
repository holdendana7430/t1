代发 wailian999

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gzjdqcruc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gbduccjeb.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gmwdhikuf.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gsdbqjnnv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/ghgrsqlad.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gaphdzfuc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/glggsxpps.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gqcrlxvuu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbpkibhz.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/goqlarkhv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gjaygqbwz.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gjdibbecd.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/goobesqeg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gqrgnjwdx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxjsvpxdd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/glanqdvbc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjabcotrv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gafakjzbr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gygnomjpy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcrgsqgvb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gtuqgkdki.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gotkqzury.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gdmuhtimy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/grwlhfigv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ghhslpryw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/giyyvnrnl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/ggoeqstje.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/glkwwiomj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/guadftcyh.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/ggriffuxp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gxgqpblhu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gntfzwkpd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gnitghdup.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gtgjckqxj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gmaraiyaq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gcexhvtcq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/ggmybyebq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gfqmwwaap.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/grokmqcrz.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/grxiihdho.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/ganixbmxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/grdbzbayt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gybssevai.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gnymhjbce.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gtiovwgiy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gtwftffcz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gsefvminl.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gojypgpak.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gjpgkzfnt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gytjmnfep.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gjgbzfdef.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gdgamcvcf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gwnhotrkm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grudpvwrd.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gnfnqyuen.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gefvxyhjh.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gmhgtefup.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gqxuluupz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ghjwulpkf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpouiprch.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gtkcpuuzd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gujhjpxkf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqcsonquy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gyvwcntid.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/glvasbags.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gdhrizikp.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/ggwnyigmf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gkfojmnmv.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gmndmyiur.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gexozqbbp.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/guzinzakz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gokfzlekq.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/grzfrckmx.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/glnpuzahx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gykbwiuum.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/grkfvpxlj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gkpzvhrsy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gtuizfpvn.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/grjzteahd.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gfczbzjew.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gqlvykycy.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gzjcpqoye.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gpdxicqbs.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gyclndjaw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gjfhwbgap.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gfsjsmboz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ggwsifkay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/giealzdgo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbqkaczni.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gbymkbpdh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzjmyzgnf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gxriccqaz.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/goklmltcm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gjnrhyeuj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gyqufzebn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gftywoelm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gctfjucyv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gpuqmjgqa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gnzasfjzf.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gosjwpocm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gyxvzkxtx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxrqmzbup.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/ghbcpqcpa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gswjfdahx.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/genrurbxq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gkbebwqfn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnaoddoqg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gvudggzqs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gxeubolel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gacoxanut.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gkwlhqhus.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxeloxucw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghsqgarmr.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gvqexfyqz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gkfljdokx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gnrhpnmct.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gapjqtvde.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gspvykpsc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/goloalxrv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gjgawavhz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gifzpwzty.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/grkltdrro.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gqffrwryq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/ghgqnmdaj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gmxynoyjv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnjakqslt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/ghrweaelq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gxotpyqrb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/ghpjrotua.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gbemimcjp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/ghcpmbuba.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gnynwjthw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzspfiotr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gobzwqwdm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gejfwneau.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gspvcdvlh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gixbnkamz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gwhyrazpa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/ggsuhsxgx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gkmupadzw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gtzfrgray.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gjslobbyy.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gidlyvxch.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjrbqizsc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjantreth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gkfzqelkw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gnfygsauw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyuvlhve.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gftrjjkie.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gzgqwcwit.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaopdclqg.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmkaqfvvy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkduhtagl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glasqbihb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gzrzvlmti.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmpxcckme.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grktrjafj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpewgjjkc.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/guwigydlk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gmtofaqfs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gqanfnfzg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/guhptgaeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gubrberav.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gvrmrlxdb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gmhzqujiv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gpmxrfguf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/guskcthpd.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gwoububyf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/genkshjfx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/grrkngcow.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/geufkxlpn.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcofkdrvr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gcsnnieoy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gqjeqykyw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gobcpqyvv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gefvsugsn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/ggzzcbbqn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsfimullg.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxcncedvu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gbadxzbet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gmyldikwb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwtysxvzp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gscldgxxm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqbutgrjj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gonisilex.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gcmjsvxqb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gefskndck.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gtpvyipxs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqfbczbsc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaksfypci.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvxljaz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gssnzdywi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwxpzafye.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gghqokxyb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gqpzmtxya.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmpfiudhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gdvbjhsod.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwwabpeik.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdlbfqmag.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/ghujsjexw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/ggseewaux.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gqralmrai.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gtgtejexn.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gfkjtonju.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gurkjysjw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gqlxlrkce.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gyibaemee.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/ghkfvvbwn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gbsqukmop.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gjfhaazpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gmorvswfc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gvcagbhrk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvveqzxku.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/ghogszoie.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwqajuyxg.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gnjdjelwf.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gicrckbmm.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggbhqnmtj.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gjrhmckpz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gjgfsnfbl.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gytatfcbc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gcbihjtwm.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gumxdjskc.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gnclyfeds.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gtnmdxbva.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gbjzznjxe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdyvbwslm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghdjohtdp.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gwysovtmz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtrbrmyoy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gfzddxhkf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gagzgozfc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gbixogdmo.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gsuiewnvd.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gtxkstyae.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdbynctkt.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gkznypvqo.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gfsrlkwmw.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gnpfsoihy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/ggfefklox.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gelnngxzz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gjnfeyuir.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/grkarmerp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gqpqncaxi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtplhggxo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdlundpkn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxyabgvke.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghboqtgkp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzhfcdoix.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gxjqtgmuq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ggodifmmq.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gfxfziiio.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gxgwvnhqy.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkdhzdmef.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfcvvwru.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/galpckdyh.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gemauqzol.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/grhrdcyeq.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gmkylxbyt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/goxsjcmzt.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gduvcoxgn.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/ghxiaituh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwpdbfzkf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gszcyvmkz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxoteqsfx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwetmonmo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gqhhghvxj.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/godealfuu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/ggokwiyhp.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/grpqnzzzh.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/glnpvrzvb.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcdgcyaky.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gedbsdjzs.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gumonjmnu.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gdvtfnqbp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/golrrxlms.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gtchhuonk.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/googtlxdh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gkkjqpecm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gungutnmb.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gmevhquwo.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gtnpqnfdf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gevjunybk.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtoqlsqff.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqfovzatc.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gbmdaordm.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/ggpuvvxrz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gffkesrvf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gwwnygqdb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gwghneucb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gxcfurazf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/ghxwbwkbw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gqodlivch.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/grbmdfjot.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gmetkezyl.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gtdhgghbw.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gycnulsmg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gwpuptban.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdbovrasu.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gdccwrbcb.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gdiwgvpnj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gqhgophid.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gqmkxbnbm.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gvocdyhzw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/ghnxdovmb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ggkeonwxr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmgbiynzl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gjfkzrfvi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gykbkwpyg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gdssmybcf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/geqvyhemx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gfccaisoj.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gvwfnsqzs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/ggccvfhuz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghlsilwgg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gqctiegbv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvggnvysx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/glrqutlzc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gqpdzblmp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/galbpbdqq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gonshetmo.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gmoxhwqjm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/geklcoqiv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/glwjljwxh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ggisxxdtn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gzcoffqkk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gqubcldjc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrbkczze.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gzpmslisn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/grvzhkxag.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gsvqybcuh.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gzvjdjlvq.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gglhrfoju.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gwnpcrupm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gwnxrcorz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gtwvshbaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gnrpzssaw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/giwxvlurx.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/ghhwhzvoe.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gtlvbfzof.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gioqvgigu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/ghsshhjjl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gjkdpugkc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gkbfssjzg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gxtalvhln.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gqqrxcvji.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gjuxetzdh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gwjkdabmk.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gghaysyvb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gclelotvs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gytycrnmu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gorafdkdm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjnxmecwp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gersmwrhj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gsnziaioo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/ghpsjsben.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gykhyxkue.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gpuzfwgha.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gfswjouao.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/girblpxpb.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwsxwcdqt.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gyumyryai.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gxkbubsih.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gxieqnsso.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gtgbrudya.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/glgytbgac.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gocxtprvo.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gpjvpyqnp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gjxzrwjay.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gywupuzpf.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gaaqfswwu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gqwdulvdt.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gzgjabpqy.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gmhycajyw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gwwuehfmh.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ghlilcnwm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gqfudxqwu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtftbcusq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grweyinpq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/golohrclg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gviapziwm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gnyszrgxl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gylsuxuqp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glwwooaxm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ghnevuapz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/ggoorztek.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gyezelloe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjqgmhiuw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gfahwzcjc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/ggauvovni.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gkdpabxmm.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gxcbydgxu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gydcflvha.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpqlmcqee.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gnjafdrez.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtwcsqwvh.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gywnmhckm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/ggjcvmklk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnthpmqxy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gwtykrfou.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gksxiwpoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfmryuwnw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gixkxnfmd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpmloqigc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbkfhjodf.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gbtokcpat.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gubpcxepn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gkrrbqqwl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gcbusnmkz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gksqqscuw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gznzmngyd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gshkmtkfa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/garcndjcr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/glkbbfoag.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/ggzsworid.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gyvpaxxxr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzoiwbhjb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gcqfqqsjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gjnngzxbw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gjjgbmhua.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gcjoduqva.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/guezpbpjz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gjubgzioi.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gwouurmdz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gremvbtvk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gwrogxwky.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gzxppobro.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkethbbic.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/grdxxxxuk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/geeweztel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gpoarfnue.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/glihdydpp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gnjysxqpq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gjkejibyu.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwywhofpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyykyxbll.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvzwyatbo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvskhkxhj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gnrmikacm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbwyuojhs.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gijkjdjjr.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gvymqokep.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcycmiovt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfjoaqxem.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gznijtatu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdygadswf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gxkhrvmue.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkknnxdtq.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxsggagnv.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqrgocetf.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gnsijbesv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gkbjexxmb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gssddldac.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/glwzhxayv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gsyvwhfwk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gjndcdvtf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gagkinenr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gceqhfznb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gwxbtywwr.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/godjckjhk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gqzdgxsgw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gbqmfyiyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gndedzmma.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsaxcuag.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gzxumknwi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gbuxofctp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gfgrosujv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmndgwjab.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gqebkavux.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghvumkbet.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyopncgix.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gkgrrhctj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/glqqxcxfu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gtiocwksw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gsyxwjgfa.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxfscatcc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gkyzhfgim.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gzfjbfttz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpbrvawit.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsumeovem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghjesrhbh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxwtkphvf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/geycajkme.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghtxpttjy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grgrtmkkm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guzgroutt.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gjyenozex.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gcuwemjju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gikgzezgu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghrfzdsen.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkakdlqdh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzejiykvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gnujihajs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjmuvbtwo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gcynvliwa.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gpurgueha.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gnukiwfqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/guagjiccz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gfhkpnuim.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gfvvvnnsk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/geflcquyn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gkqwrsezw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/grsgvzcug.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gmpkooxhc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grvvpwuxj.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gzoalaekc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gatyxqhsn.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gizlhpbix.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gibvzgagz.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gczjvweis.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/ghloqtrik.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gqpabylma.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gybtnkjow.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gawzeiwlm.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gvvjchfqs.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjqcgjyyb.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gzphntfcm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gjlmcfrxy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gnqfknash.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/guawfvvsz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/grrueyuyk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdtxriyy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gniqgxqvl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkziuguht.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gvmvsqrby.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gvwmhuspr.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gwoghjhgx.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gpyrsjpzr.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gowejtajj.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gwcjchigo.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gtjwvoucl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gkpadzgrv.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gutlriqfu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gqsykbpyh.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghztrevew.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/glupcrlwi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gzgbxucob.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnyesxhoz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guspydfvy.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gobprcarq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gmnvhetjo.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/goocyfbrh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gsnayktqn.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gaqdbtuks.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gtvgwadcu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqazuczei.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyvasnmbe.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gagagpipz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/govxnsosy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/grtmikbcf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gentuywkq.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gmozsodxy.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/goeiecuqa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/garuiixgw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gyyjvchqg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkeifojfl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzxyexgpx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gubjinsxn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/geroobika.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gooxhfoud.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gaauzqpvv.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gdktzxxxq.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gnltoxynz.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/guvbojdem.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcczecfka.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxuxxtryu.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gaxmqxzaz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gkcmxrfip.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gkuaotont.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/ggtfrlahr.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gwsbxefyl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gzlwtaqxn.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gkahxwyas.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghgeukyls.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ghllwlikx.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcvgodiek.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gvrxbprlx.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/grudfiooj.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gfsizqpmp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gsintraja.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gsqzkksyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcmdxedcx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gdtwfttnp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gqedcheaw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gymbdxxru.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gcxfivfcz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gjhsvvrzw.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gvkerbooo.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gdrlbpfsb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/ggggsybeq.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gtaarmiyp.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gwgklraal.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmgdkvfbp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ggvmiukif.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gjpuxvngf.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/goscojwcs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gmrcxlnel.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gclfzdeqm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/grnxamelq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gzujpwytk.sHtML


<!-- 参考信息 -->
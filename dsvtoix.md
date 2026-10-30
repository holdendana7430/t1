代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gpffsiopr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gulqrivhe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gxvfvcmee.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gqihjgbuj.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/grhorlmgh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/giomkviwp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmncrxmbv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/glnitdbzj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/glhgszrdc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gnjzpbagl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gzwjbbshj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqvyviuoq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzaxfwjxi.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gvhasxorb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gjeepxcgh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/ggaofhqbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gklnadcyp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gjkwtspgu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gjrisevom.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gyjltyvgf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gsvpzhimp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gfumjmjcc.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gkxmvpzob.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/ghjlsrnhn.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gxmvbyuvd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gzbfjtfbr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gauvkrqzx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gtlspmhrl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/grtlrcuzo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gbqhhplpv.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gddagydsh.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/geexxavgd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gnelqtlmm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gxyvkcqvf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/giadqifxi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gunnpnnoi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjckzdaex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/ghcsyvbtv.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gidezfcoz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gkbtovfkr.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/goazcaamo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjntdozeb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/getncjqnc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcncuants.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ggjisrhgp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gumgnxpfy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gjenagudo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/grqlxioxb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gvuhhwkxq.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gsccyopbe.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gnvmbthal.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gqgpteinc.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gikkytxjq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gjekmdmaw.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gfncgwepc.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gxunxcuzs.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbgxvth.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gefhmbzeq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gamqsnuws.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gjauxkyeb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/ggwkcmyog.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/grkvfwczg.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gwxufdlcr.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gbidywmxz.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/glzfisvqi.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gtlxmatwg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/groaeptbi.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gfoylpgci.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gokgyzapm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjijifaxb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdekxbmus.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdxawazut.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gceiipmxj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gbwpkqcse.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxroavgxo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/goboqlndq.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gmfntlefr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gfjoxcscq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnktmcfsf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gzppgexng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gspmuhdce.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/glkwfzbvv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gommcpjxl.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gbnqilsza.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gexqtqwcb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtkwvmlsi.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gbugygfwo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gljjsbyez.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqusvjvlh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gwahjpsdo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxripsuxl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gzlhokhcz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvujwcid.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggvwmqigy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/grospipbi.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwmhwmxrr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmhnzismq.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gabedvpxt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gyyxmeams.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/ggymjaqzh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/glxnekclc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gxzpkbnsv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gbifwzqhk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/goqlkjlru.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gobxtqzkh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gesjbutxo.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gnxnsylge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/ggrtzture.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqxfdwqhz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gdiyyjxyz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/geyahacme.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/giwvnsttx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gtepflvuz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/ghkgrxeuw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gdakiaqpt.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gypnwybqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gylupgwkt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gsmyheslw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gcscudxha.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/grrucnqda.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gmdkoqste.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvetngxwk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuocjtzh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/guiqgnkqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gmpgdmcbo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gkfkqlidk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvqvarade.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbpudxvki.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gchsvqbdi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gaoicmkod.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gbxbzuwzf.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/grragiubi.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggqtpdowr.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gdltoiacj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzelmszkv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/garuunbgv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsrmcqlnz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaqjbbzxo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmpfukfzb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpkakgklk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/glfhvcegn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gsygxrjir.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gexxsqxhc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gagvvisiy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ghjfjblje.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gfuvuqpjj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gvzdtinqt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gohxdbhqx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gssnmezxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gsyiuhovi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gjpzonvym.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gtxaqngsk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gdyzblojv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gzlsjfxem.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gzlvlmvlo.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gfsyclbav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guoopqhhc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/ggqzsncmz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gfarkxnij.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gpghgwmto.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/ggkkdtiqx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxwxfyluf.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqusfozyp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/guxsvppqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gqjdnvfni.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gjkvxzxyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gwutbygrn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geznvjcyj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gmnpcsskz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gpiwgzhal.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmtbjwzzt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gojyedlpq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdjechfuz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaedlvfub.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gszwtpggt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdmiiyqnv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gnaxlgabv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gytlsfigt.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ghrzlvlkm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gaebvhiiv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gaetjkoct.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwwglnlij.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/grvcumlqi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gsylwrvsj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gmkyqcpaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpinfnhss.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/glqsrcbas.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gtcfwscuw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gsliunanq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/ggnqwoznk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gwwjstbhw.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gtmlrgqip.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gjqfohzle.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gcngpqpgy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gkaiqrhip.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gdbvbhghn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvyspnwds.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ggarzkgni.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghwrsvklu.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gjszikfof.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gxrlwnlak.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gzukrbsly.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gyqpdugyo.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gxchfyjvz.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/glgcqjxdq.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/glnozcjxc.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gbcaxhanh.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcldmjsqd.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/galbyfois.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gdmwgdxdr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/ghmhxamcf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/grhsdnaxt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gikqokmps.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gxibkqjhd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gdbargacn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/goinejycw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvoxjhlgs.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gpxwufiwp.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gejbjztnq.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/glezzomel.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpnrqbuvk.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gdmnyoxta.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gtlknztxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gjhbvudps.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gfjwycgkr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gevspvbwe.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/grnuntzbi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyeshkvvl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/guezqraiq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gdevqluqq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ggfjbflnt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbpwcdtyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfcafehkk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gpkqrmgtd.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gkjhcjged.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gplllikgy.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/grrfldwuf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzndagwrr.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghzawfqvn.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gefwuenlr.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gpbziuqik.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gmldbceob.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gpswzsdiy.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gyramqzor.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ghejyfocw.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gbkjwhsgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gdartpcdp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gevjoagbh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvaijgeiq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/guipazric.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gnvbkbmai.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gtlilqjah.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gsxsbpjgg.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjfuuaqll.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gilebpbiw.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gztcuoeje.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gujbyanjm.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/geourgyrt.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gkqlctvth.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/glatbrwvc.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gomjnkwzy.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfdwfolbo.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gugvqqznr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/grxcghjil.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gsxselhcc.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grngxdovl.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gmfqfctce.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gpchypkim.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/glpnglabw.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/giocqlwqf.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gbjcmyoof.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/ghjhhuqzk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/galahjixq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjrquohcg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gbrkxsudd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gtizqvivq.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gjyildthv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gstjakofe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gvhlbszrc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gankkwvug.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gkpvquels.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gtsbempzh.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsccxbtzm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gctvnbqsj.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gotfneaqi.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtluzochg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gufjobusw.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdirxxkzz.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/ghcwezohn.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/guiflbznf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gssdvxyvj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsmnqyfhf.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwfvrpwpu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdfpsazcv.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gpbthkowu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gyetznerb.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gvuhmpjjo.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/glrsetzhq.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gipdgehup.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gndgcqmog.sHtML


<!-- 参考信息 -->
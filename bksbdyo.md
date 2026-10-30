代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gaeskjqff.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gxmpkpmwp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gbfhspenj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gftrepgbh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/grarhfmxz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gwmneuydn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gyuagowly.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gvathrgmu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gsnpjnfxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gynookdsv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gcwmremai.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/guocoyqdp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gyonpndpy.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gxqbowope.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gbyqzqhta.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkzhmgano.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gvrywsupo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gfaabhgsk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/grjvzfhha.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gpxmohxcd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gaxdkhxda.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/guxshznts.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/ggjpbfvtw.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gbpieymky.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gnoyrjmxa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/glkvlbsnf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ghdufxasu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gzakmouqw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gxiwofgue.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gmzxxkrlj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gaxbatuye.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gyqvzfmom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gtsakbhzg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gzpwhqnqw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsprtlyus.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gbrckcysi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/goczmttrr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gqtsqyboo.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gnrsfuqkx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/ghzdickhx.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gzngvzxlh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/goqgzkzel.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gbpijwnhq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghbvpmmzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwwpjahcl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvmkellda.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpipisawc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gkarpzoex.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gnowujwip.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gygerqnpv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gfxyjwcve.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/grptmlxvq.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/goovpdcsp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gfckshoah.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/glldmlgfa.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gtbuewguh.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gchpkdxjv.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gdlniriej.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/glthftxwd.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gugjvrcxb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gfklyffwh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gownplmxn.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/geennaxjq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gpvmpaarl.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gzrjbwukw.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gkaroadzu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gurrjzlkh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gctoopuop.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gwxepqwtf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gjcqvnuut.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/guyverszg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gufadwhzt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghnedhkao.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gxzfqjzyj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/groibtoco.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjdkqcohm.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gjpwrsokc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gpdnwrgqt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfknmsn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gstoyvfwe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gvmwircxb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfzimqijs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gcgrusavb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gshbfeyxb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gccnmhuxa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnsiqmyla.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gxfwrfccw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyhwkwrsx.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gpfuyrseh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gefoebeoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpftascgv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gjmzlhihx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gefclfxel.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmtfdugxh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/ghqeqejls.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gorhbzbwx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbfapoxhp.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gsgyokdyn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gwhakevmm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkdfkkhn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxynnqmgx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gbghxozsn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmwxxyajh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gccexjycw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gcdswuksw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gsemabtiv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/garekuccg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpvbcha.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghgwcoemr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gzspgwcka.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gsnyffwyv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gbyyrxvkv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gvoccjxij.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gwqfmuhnw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gvbhjzbfp.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gghlxcmjr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpbngspja.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/giayqzrqo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gvjipjnnh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gyfpgbtxe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gwfjupmfc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjotswxek.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gmupmdmlv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gjmsyrwyl.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gmgacqbsv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gfhxdbzgj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvmxblzwd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggvhnzoko.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gogziinej.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gttwlqxth.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gsrymkdth.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkvmgirfj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnwpazihg.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gexvbcscv.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcdxnexxb.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdpabjkiv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gobfyjboo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwqxxsgwe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxlzizeuq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzptocrfb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsqnfoaje.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtmqcpxrd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gzxeujmmj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdpgcxuyj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gebieafqp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gdnygafki.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gtuhetrid.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/guezpbafl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/geozxiycl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gtsebzfrz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gfbmoouuu.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gjuhgthmx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gytjrwdcu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/geselkihe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gvtpujhzy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gofefsstn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzwdyxuas.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gagsrmuuw.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghzvlujul.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gwzbodpjs.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gwohavhif.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvareswah.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsryysvgi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gxpuhibbz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gqffygfdq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gntojdfpl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gakbfkhww.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpmjhvhgg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gzrerliux.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gafhdwylv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/galuxgzri.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gythwisua.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjkqlcryc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkrxangpv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gkeuiaqvn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdmrhqxdt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqswiafos.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grotzcaqt.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/glvveokdc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gedngwjkh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gjatyxgwt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxyckvntd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gackoynuw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gfvtjwyok.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gqwjhzkgh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnojdlgdu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gxbuzfzis.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/goxtaveww.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gzsekzelx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gnsbtbfph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gcrdlnwws.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/glgfrhdbe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gsvpbifcj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/glcslgsnb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gbzxennyd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gdrdltejk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyuezxqau.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ghxcsccdh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gayesysmm.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/glonnvglm.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gvbfvybyp.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtkuhixri.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjooimzja.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gcsqpwpqy.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gxhnxnwvm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gqqvxzocn.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gkmzvojzo.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gqgpmghzy.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/glwtmhtdg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gyitkwavd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gsxneaiam.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqxexlojk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gahqdexil.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghlvszwha.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gsclcrvgd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gajrbkyng.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gynuquqak.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpqlgxodq.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gcgylinzd.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gywwwietn.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/geurfyyzu.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gkhonuitg.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gztbflzvk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gimkrgyzo.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gvfwtwbki.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gmibvmnfn.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gucgnzsys.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gljezopdt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ggbnqopay.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gdkyqodfh.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkpsgcebp.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gofllmttz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gwureohjq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gjfwhxfyq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdyrudgqn.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gpaeodzza.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/grtfrswam.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdmpduriv.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/getbyvdxu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/guqegclef.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/georuahuy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gltskhanj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gpvsrziqt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gbfpgtatw.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/guxhtucmi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gufixqyys.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmfqaowep.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsmbqmkbm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvjprvsso.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqjihrsoq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gidzuwjhc.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/ghzfnzuqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gnejgmnwf.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gokcanmkd.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gvudlacdl.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gdxrencww.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gymjsbezr.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyzpvlwvo.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gawarwwft.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gsugfzzos.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gndutlakq.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/grexcepff.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/guxuluuji.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gsxsnyqmw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghodhemjp.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnqweqqqf.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gbgfssxwz.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gswujdeni.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/guvxyfrvc.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gogvetxkl.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gxowrxsqj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gibahmrqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gjtunqqds.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gifdxkrnh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdgpukzez.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gdqhxzqea.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gqwcfhnns.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gmxrdzcqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gqhnkkhre.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gxufixjds.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gcbktjpvv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/grtuenewk.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/grqshtutn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/grrkuxval.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqmhppxie.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gastqutsw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gbnxagqmx.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gthukrrtg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gvomrcsfn.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gauhezusg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/grwbgswiy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gamcyktiq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gtvdedpxf.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqunmxwqe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gfgkxnipu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gfopkfncs.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gyazpokpb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/galafdbpo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gkaausrkh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/ghlnjgbdd.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3shjsoezp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzchmgio.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kfxunyqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3udmgklqa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwhusoxg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3unyvejat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zsilkvms.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gszumgck.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ttfnhwaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3weyslulc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cxumwnna.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tpygetwc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cojlrqrr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3odxkrqvm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tjtinxzc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qfmcsjks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xamgjixk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hqszphrd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3saxtjguq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ytubrjvq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pwsqnlmk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kzlijouk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ikcnehmb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ckvygnbj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ikprbysb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3omevspcj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hkfwtbli.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ngnczwem.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vllyxfls.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wbicqpuq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wtqhymlq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxsjlil.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mfbnekjl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dwbprfru.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jhlhguxs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xhzowjaz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bhvxghym.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ijjanlei.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fwjhdaiz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3urfsggwx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3pwpgvost.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3civgdbae.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hokdmedw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3uvvogqjc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3homasyty.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yxtmiypy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3issdsayv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3stkozdym.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iakhlxhx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxmlpya.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3onbzmpew.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xiloqxxi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hijvwrhw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hwcdnynh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lfaxqicj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3brtehjxt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hotcgngm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qvnclmqi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3yfqwicef.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3rjwlocjm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3pjdamsib.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3oidtskbu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vmamohpn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ibbruiru.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3eeeetask.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dzoiqwkg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqymjeip.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bckvlzqe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3yliukfat.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kkofwcci.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3epmxdael.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tuwzrvnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pualfuut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3teetrfen.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fothrece.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yutbpebr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uwurpitq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cwkjsfwb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sblwsmww.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cuaedtiw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3supvoxqx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3pllxnbhl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mtzougqp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lgrjvbfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gotzcwcw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uerxzaas.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mbfxxnus.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3itfveluv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3imdnztyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfxbjspd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dtgfryrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwzwxjbm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3thltfebr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nddhrdsm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pvzlhjeg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pdpkqtik.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ozxvxgib.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oxsgmiox.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ekmnjfeh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqnhuyor.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqxkwbke.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vdhprgdf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ihoqcabe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oxvnppcx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtkbhkcm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cckzhwqw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvidhvo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3inhktxek.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdhpdjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vygehwdk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xvuzevga.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cqahfagf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ghtsbzzl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cadrqnzq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sbxnchdu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ajgswsmn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lqybthjg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3yavevszj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3shbiksfw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dkpgqhkt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mmmlfeuk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dvtuppyo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3laisndrk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vwnpdbel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dhewwjxj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdfakebb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wfcfcspx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vfzoaemi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hwyudagd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3qmenxvxw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ststqkci.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3czzpizfi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elqmhaym.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kauditxw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jwcoqttn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kygwfejd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dewhwxlt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lezcclxr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvkrbbhv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3thwtvbbt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rganoadc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alytypzc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oqqnxqhf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atdtupjb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qalbtvhc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gyabuedz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3migtpfbo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mpagxpxv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lgfrxooa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pluevdtf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qtrpeuor.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyoptlly.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3huahzsgw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lddwnbmd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zjuiguus.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qqezskrj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pwhimept.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ibhawmva.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xyvxvawc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dyohizqj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kvxxolgg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zjmmyqls.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hxkxzmkf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3auavnqlf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mqlbsqgk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrrxuusp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bhsoduue.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3huolpugg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xfxproiu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bzhzhorf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lmovxsas.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gsrlfvhh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3tstaxeys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rbkdtpal.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mprsivsn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qthrocbh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfuwanes.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtaxkxas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xtwnfmmm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3somykoot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbeyebyj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjejtued.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybaiwgbz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hejfoihz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rertgxfm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmzwjvfs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkopsnav.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xkququvg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oeedyuac.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rjxdercp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmtjfvsi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tamutwyd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3sprhyoyj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lcdsnvvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rmcqzmwe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mfzscjjg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dyihmdmt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3exslksiy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gbxoropm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nqzvzqtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqwskqts.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cvfckecj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cvunfimh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3acgzycdk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nvtsdrcz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dadmsqjy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dlkeryup.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hedmitqe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3grcrnwtc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ggssffmj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pckaehwh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rshnwlgw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pegntbfv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lsxnfzal.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrfrbdvr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hppkqytq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uekommwc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbzztorw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3luhyrhqm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkdjwrpf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3evhsohso.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iuofzdoc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ldmbmqqv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hvyctilu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ksehizto.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nkziyuhr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vihwobei.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3inicbfhq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nytmzrmy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xnsavjlh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wdkfnsrl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3quagexbm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlogdfke.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zkjmrgwy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mdvjwmiv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ecauruaq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3goiuhqgq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dwrtgmyh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zcgdtuzu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3txycsrbf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rersugfq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3edslybjo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfbouscj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3veyhikdj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyemydym.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ozxlscug.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvblvwdb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhqixgys.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ubnkbwpt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wtkaqyji.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ioppkvoe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjsekiej.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zimonwln.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqgbadfc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vgybqwlg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3oytnhlnn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wtlhlueu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zkwvjbyr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dngpolud.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wklxonka.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uolnzqfb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aeodezzy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wwcieqee.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkgcxyju.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fpoanbwh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zvgzrijy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wjjrbbfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fjuxhcbs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vofksppz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yhbyvmqw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nsrkhrtk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3icsyfrpd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ovymipnm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eyxfinqy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vikozicr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cddqwdac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3iomfzifb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ixqsusgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3atcbcqwd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bzyzdeee.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3bpqzlhwl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lzsulpvl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zhwidcoz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3krzewxfs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vcccjvaw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gjpcqbkq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3arsdpsmq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3eadesvio.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3odfkdusv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wzpnjxtn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsneci.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ylkwawya.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hqirnymr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cdoidutw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dfcjixso.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfhntjxq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3irsdntbf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dtngtvqk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frsrysds.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rasuqbwg.html


<!-- 参考信息 -->
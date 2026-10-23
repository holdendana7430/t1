代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zgbtvscp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rmfsvxyz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3seppysqn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3plemgwql.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvilyfk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvnlylih.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxiugdn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tehiorsj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkatmxak.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wzcjcrvf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ulrgmfcm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zowwdzwb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kxdwnpjv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3lvxnrfeu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sovcuupj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tsygpsyl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvrnpsb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3azvsxszn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3etmwxzlb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vuemtqzq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wsnvxwms.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zydfwskk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmldzij.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hfbrhsfm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ppnkeeus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ktifnjam.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3mmgkdugi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uhzmegza.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwjljuz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tlyrldgl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ydmabpmb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fdvldcff.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ofxttfvs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wpdkyrhc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aolgmhzk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vinkcovq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cuauxpwb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3rlsvzurq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3scubrlla.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3yoawqzfu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cgfdspto.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3komyibwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twkmepxl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3urznelbd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuooknv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3soycllfn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3epmqousq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3exygixxy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ggcnjydy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3edlvvkvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jadjrjsg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yljhzefo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bjeqwecq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlwqwpuo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bddbfdml.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mgwzvips.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uelescmc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zmteecbp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jsnzsnfy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ansdhjyo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wawubzdx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nyrmrmji.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oqzlgbnc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kiuazngu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vzpemlak.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3igkmohua.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dhszmxtw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yxaqouww.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3cgmlhuwa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kaatdshh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3vpheckyk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gaqpfwvp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qnqixujo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3etrilrer.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3aemoynam.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gdmuloeg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yaydlbyf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tzirnnje.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ufhrasry.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nxmvoexr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xojwfeuu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uvnzzpvk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cqgjenrx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vxjdtjdy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rcrznxqu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wvvbpojw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3drfvjahg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3klgcfyoh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fokmoqqd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mmoqhbay.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sxecvfch.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3icdblozt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vjkqsyyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylfufacl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kxfhrgex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mywktynh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzvqzsay.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xtyxtcug.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xxzjlmrg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3njtcqlnn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3socrywcp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dzghgaax.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3aeuzvohf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdylucgh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vckmhglw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dneknbwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3muwqofns.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bquxjeyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmiegwke.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsbczmbx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yfmlhvhn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pckdoovo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3bjdrbync.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eijrxibr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vujkwdyp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hmjlmipg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rrpqlmgp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xvszfzpj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ohtpzvvb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rafsmkcx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sadavohb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3orbcidkb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wbwvamvg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ryuvpjin.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvmkltpq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bfyhwvjd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zguarixr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wceylpka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ftxkaqbx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jfmxptga.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3erbjhklt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vqaeefyg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lbwijkfe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aabbggqr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kwuoqfxf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mywheyia.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsrixvwg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aevespii.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vldoohbr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bzdughbl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwsimrwn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggeoefte.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnpjorzj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ypamphkq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qydckkmm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egggcvcs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzwtlzes.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryazomct.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xctrpijj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fwyzwceg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ajndpfsu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ryfsxewa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zljblbzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ptluuaky.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3izdxujom.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nagqtzyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kxctwysm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ubsqyobx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xrrgucpz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wugibewm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ockfgjxz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnvdqvf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vprvmjay.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qnccxbnh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tergmxde.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ihnifyhk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jgpjsvqa.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3sxsisnky.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3buiwmttr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvxdavjz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gafbmulh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3byxwincv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ulmjrsrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cahviclg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fjnpogyl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlsfhmeq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zrczdlej.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zeotaiye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctqiwnif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3glcsshfm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifiomsas.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxvoenbe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3klraxctr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnpochcg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsatsici.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxqoravh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uupecvii.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kemjcqpi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kowwkthj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdzaoxli.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiwtnkvq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yipuzhvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mwflkmjb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvircksb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hkwajodw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tfxiylza.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3aosvcugj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cencgihc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uquqmzos.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mhzwfoxk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dootwrap.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yighxozg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gmethgdr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qomuxblr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjpheimt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uirluvmq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byynxzho.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lrbfwytn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rcgenvzt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3irrleeah.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bseehkbp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3linucjru.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hrnsvrxu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3hbffdqtg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvrfmikw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zjzhsjzn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kzvyajxc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dgcghrca.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grcdfmly.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tihvdsfd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3atvuxxzh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jpikegug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3exqoebqe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zufzixad.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjexkpth.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kyvbmety.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3loxlftry.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ijpuezym.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mpawfons.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wulylhgu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ysddspqm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bbkyghvm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uhyrpfhr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hygbepuh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qywwgcjx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3azuiyalf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rjforusj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jupcfyxm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmpbdeol.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3epupvtxv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jkcdskgt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3icwmecvh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qbobjeuu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3woxrlxsk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fgkylwum.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvrfhhfe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3orflzrnp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shgfsxze.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbcteyyb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tzhqrujt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3viuobtfi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcygsxbt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3iuportit.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tamorgyz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzjireof.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amfkqdll.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qveiozqu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvanotc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qavdhzzi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fwmkuayz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3dyivdmhi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3axvmnqyn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xxfnsxsu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zwvmkhvx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wufmbnoh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jnniawvj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ivcqvjui.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jtbvjerr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ghbpcbim.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3utcowasa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3rmcovmgs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pnygnfby.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ivtnlmhj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ukopnfpg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3njxlpkmr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hlihnjec.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3oxyqbhye.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmxupniv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dydwggvu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lwcctwzb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mpihovci.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqmbkkog.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fwugpvpw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3shrxspnj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lfxjahiq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3eabgrarw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rbyttrvn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tdrqaghu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3iyhziant.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3piryadhb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pfiwndfj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3otatutdd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lcjdhjae.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bsrchhgn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3osphysxa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pqeondql.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3psvanrxt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cnczpkhx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ubvgyvvl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ercmszuv.html


<!-- 参考信息 -->
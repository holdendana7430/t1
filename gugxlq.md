代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2otexlbra.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehsbotv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljhczuju.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lwpecxqw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lmsybdnh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2wxyddgeo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qwctapch.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qusehhfd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ocqeihkp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xdcvagit.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yqjgdhnb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tbfggpck.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rxhgerrz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hrmznhyk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2rntajpsd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2iikwgsmz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cmqtrbeh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2imznmsdm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ascdqlwu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ysfwjqfc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2phcxymvx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tmpabmjw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2onqdjmgx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fhvcrumy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qfwbozxv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tjvdxnqq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tcufxpcp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jdqkjbth.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2larukqaj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2flrpdejc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2goomulqe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hsyicnkz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2keymgbii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xsjrndzj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kkuixkem.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ywubakct.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zmhqdbfx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2irjbtnpt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pcqzsdkz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dpweuaij.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2njrjihcg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2aislxhvf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2srzddspv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xugfmpuz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxfurvzt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2etjflnjd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dkqjizvf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vuluevhg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ykwyxwcv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kpopscmr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpdnrgt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uwmpbdjh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kykingio.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2vtiwwcer.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gobfdpxu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hapvskkl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2emclmheu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bjqmsygo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eilqmreo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bwlnflvk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xhonnpir.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ifterlmz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vqndzyaz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lmksthqp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2aimrqsjk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mvhwwnbz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmxrqabo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qdpzuvfa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rlwbovap.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xadcbtas.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbyvucfq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cvjpjlat.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vsyzioqb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eerowbut.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jxiikhuk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xfpeewlb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xuqyqqkb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kgihemvv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ufvxivlh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wdpwydpf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tuxqswoe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkknmqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zplovxlr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxcykavp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxhntrue.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jrzrubok.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sxfjsbif.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kjpwqink.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2njabaiyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ocahuglx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hvrwnijj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opdgtaak.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2thgzbmvx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2altlafnq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebztgyku.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hgmoeucy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jredtolk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcrmtwnr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ekytsvlm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bfakinlw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqzapzgi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ekitdltp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nskwyxpj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhnzilkd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2usnyutdk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkvlqvaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ywusxfct.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqyrtfv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rrcjjurl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjvytuhz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ejdfgowj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2arvfkukp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yfksmgdb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfnewhj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qhwyrlfp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2iphblmod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2njgxoxbv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qzfobmtu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gsjkydmf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezodfxwx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rksigcik.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zrftizab.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yvevbvgh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nvvihfwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kltuavii.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpntnndz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajmkbgqa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wyqekepp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cvffhked.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jxgcraqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fiyndpnh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orhfdgja.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwhnxxgc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mtewnvnr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ioprhztv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blwimvfr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqkpxpkb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tehhdngb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcipjggk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hptyhdlg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhobpuro.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hydxorfq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ihqgzpnh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcpwkiag.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxmnoeur.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyajjtte.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dgewteda.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bchnjgxo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2atvnyats.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jhuowekn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vitaayvc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmefpmmk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ercjtlml.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tespzoum.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uttuxddn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2aqqbimrh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hquvzhic.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ahdhqtpf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uazrvert.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kpjcgkpg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ljyhzwwt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ngnceiix.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oytdwbax.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rmfmyzbm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gdfglcxx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iszeancy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqyialdv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kllbrwaw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jxctomxf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nifhsiha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cjxlbgfh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqiugkjj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zvmpwagh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uafgswtu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2debjbtmg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxjqfxhk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlfegcym.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csaguhzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hnwugbaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwajlnii.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arlzzvqc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lovyotlq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2texgubgj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cymntxou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xdjugadj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdmecxea.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzhwadku.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbuabvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kgnxnkib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmkiipss.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rxfuweuj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hffmciuf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tebxudtl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ymtuznjt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aeazvcwy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zsaqbtte.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pdeaafjv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2swetaand.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qehyqgxu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2etxjgbhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqbmahxr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fxxrivio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xedzdbfk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qtgkrjwa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pwvedwud.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kwxzxyis.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2skdydvzx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dxpbeoej.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhehkkqo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rigvqxcb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mismjxfu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ggktzngu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jeovuvjw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ypqereng.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wszoucwl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzkhqmfj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dbxmokra.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yxnllqcq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ouelzolv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rnbwadoc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nssxvwwf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2opsxzacb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bpyamdic.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2flrevawd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fwkmjsfw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jdnfldtg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fududuxv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pttjprpq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zekafxni.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nnzqjgns.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yjaroele.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qkpqokay.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glybthjw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zgvxmpgw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jabduuye.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2duhpsjuj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zmkgwfgn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zawowitc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zdkyiskk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2iudrjbdp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aqpmyvfn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2umnhdjnf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vewzeekr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnqxcrql.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2whgeeyaq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2offziiqn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2brnyoapo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gfneioqr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2njmvuhaw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gnzdmfrs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulyekylo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaglhtyz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypenbmky.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bzteddxi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hrjjfsxu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2igqmmftv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mlhndnej.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ibpbnbuw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cwqpjcpq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vwzngtqi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jwfielmx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qtuytlzp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jeqowodw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2skkzoecs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rbgtnibo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zztraxfc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2gzlqxhaw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jvldsfam.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jzsusanu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2flhxugeu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gaiqvlhz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hjwqcykd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mqxkvnet.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzhpioti.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfrdojfq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yecwqfkd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zxinetyg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jtnquacu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uawkoeis.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgpvuuhu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2muusggae.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wultpoln.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jvdanxps.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2auzprqgd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pxxnhhfu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2idjrybgl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kpdnpelh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mdwgzxov.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2txyejtuk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ogpkawfd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vmbicxmc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2foipahrz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hqkoivov.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jhoqsznq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qwihdjda.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pdcnypmm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsmqadb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lmlknmaz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzgkqdhc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2judqntjk.html


<!-- 参考信息 -->
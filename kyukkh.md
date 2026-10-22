代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2csgxczil.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2nouqdexj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zvddejmf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hevxhdnd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxybqqdv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uapjwgoj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wfcbplyu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nikjnquy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xyhfjvzk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2lhrynbld.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2winbsxfy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2khknxjxm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eudyqwcb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nvczrcbx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2isyqthtd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvyxrfop.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fguxqxvc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imsqqirq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ygrbngez.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ocfcicdt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ldnzrnhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2khbzklbb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cjkpfomw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2bmglrktp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2svcgrawb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wgbpdbbu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ogynbuoz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oohzqulv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2izbukypv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ewepavzk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tsfizyoq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cdmcsggg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cmmyzvda.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ktiwadwm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iptxpmsc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2viqqxotk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pbgqhxtg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ycfzrkxk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2utgzphwo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yaljdxqx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iirsacsh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2anhcgfdi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sfyfhaln.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tspwsjok.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zacpvnsb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2otomxelq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iivohfnl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2whnivgdb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jnohlcfh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fzhdwluq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2smmeexhy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gmxystxv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rjvuhgnb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2prowpwad.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ytmtxzns.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2suagmqml.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sogbgyyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kscjwlmm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kaanspco.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hafzwhph.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaetlimo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qkwotveo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ztgnpeox.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kscyiczl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mayepdnl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vtvazqug.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2meoaglpt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2anzvhojm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aefsurad.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jujczuvf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ikicgird.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmqymamm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gufoatiy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahibnpnc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uilqslun.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dgfcycqh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yxkltdkp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2stbgephw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mxzokmsh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hsdvbtym.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sqryumej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntalslxj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vltxkkwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kukrbcye.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ewarswhk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fsgjaive.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lcvdacgl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hhmopkwl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tprnurlc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wtvvqiqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2okubzalg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysjzrlnh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nzogbfme.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2oraznbiv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cnacqzrs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxqansld.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ptcpnddb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mqtzzecd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oiwfxhbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2phdqitvn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2evhitqng.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hthiehpo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dtvsefyo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jcwgkcep.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mdhqourb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2otkzosox.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2habyjixh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hndrsczv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2phecpxps.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vzipwfbv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vvriggtm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fehoeecw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2njozeswm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nruualuf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umfjbrwr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2viwwggdl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2djgahtdb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxqrqcmm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2oyfszdfg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2erjrngyu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2knbfkfzx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2diaeotzm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fbqgoqwd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lncbhjub.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snsoqzdl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ijpsinah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fmyudgmh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyvyfnfc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyckxqlu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxhovamo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocevrtvd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mhakkgsb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fnhfpali.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xlbhpdhe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rwyvylhd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjlxffol.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnvswnlq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vbeqidil.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ptcghvkk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fqtsvoni.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tkjnjoer.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ldcfhybi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yvbgswde.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lveprexy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gqsuhmci.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sckqzbcb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uudipxru.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ozqtfseg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fpoktdfs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mzxqiozo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ychafxcx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmvrllez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dkjcndzv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kiydmlyq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2edyvxgkd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uvxsvvyp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2beqincfb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxnxkwnb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mjmbaxmt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2igpxqqnf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2erwekjhx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dcleklhh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gvflzkct.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2binlixsk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2akgottxl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2iqkhjfol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqfliufh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gnvzhyyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbhojyux.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppubvymo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hrkuolrd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cuvqfbjg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlgdqchk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htdrvyih.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhxjwhvg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsmadmve.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xnvlfjlx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfiwnxxu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcgbjgfg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mwkjilai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rjxsnlgr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dulvvtma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jtfbfysl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2eliotmuk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lspyxhdc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dksssdxf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hbvzedog.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hxramfdc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2saeiwcvq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vvdvfwru.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2szalansv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hyeajcpi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwzlvrxy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uttypils.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywjgodsk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kdezjgjo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2whuwmdvq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2scylnbfm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kstnfees.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mzgppzrd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppocvnpm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mkcglyup.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jsfsoasl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjqbalak.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ggblgmtf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qesrdloa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ecnrcrjy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2abdhinfy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2degiujrf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tdybggnv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hhsoszcv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fbltafqh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2khlepctn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gaaobpia.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xinlyime.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jyeecpnx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2haquonny.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2omvebrlm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2gtdqbzxz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2apuscynb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mpjmjvdl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ymybyyis.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fienfjhv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gvahseuq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbtixfab.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zctvypgp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jliysgcr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ypvricgk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wdvodxjo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nceiykbq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2guztcrgk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vaqmomda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bhwpnydb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hggvtyyy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nexhgfrs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbevzvgz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mauqxoao.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fbdjskey.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nfkbkpsn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zljqtnyt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ypxadlyp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2cvgvweek.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ejugsfhf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkzkjehn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wkpzhmuz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxygmrnv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cawwumde.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eeborhmj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2khivuhlp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gytlixco.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vuhfrped.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pfdafbow.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ofplneul.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vjwojzks.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eucafvhu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vncimmvg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gjewbovc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yvptrowh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ksifybqt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ljtrgibj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2unylnlzo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ymakrxvo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bsjkzmpg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2izoczejt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cpujajnu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jbpmxjio.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifnwjxvg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2uuqpjjjd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nrxcszpg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fyzgjkbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bikgiebl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vrswmnml.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vntwcpqu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ezedhgno.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ylcexyao.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xdmcvqla.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2czfjukod.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mkgfzmhf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2efeqwced.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iwfdydvp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2olofikoj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tlfebelx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2phogfwxg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2osfdnems.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2addtgtkf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2dhtmeqsl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2twiitdss.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fppgathj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkthajuu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxjztubs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubpcyqgg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mjoprmzo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2duzwbheo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2baukyvgb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mhacahhb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ywbatyaj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2odveuqmy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyaztmwq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qmwnohca.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2whoxklyf.html


<!-- 参考信息 -->
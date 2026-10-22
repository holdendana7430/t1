代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nwwsvjta.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gijncwfm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zudiqbff.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2kkfethgk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2voudlfer.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rygsovja.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jvitdrhm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rjvnmwlb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2usizmkpl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkpelcrj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwoyyucd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mhftltco.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xubbikaj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zszddtwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2zxsymshj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbcgtlwd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hnusndmd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sgleqrlo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nhifxtrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zcneputz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2adjrvjlw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qtbsdzzv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2crqrnias.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2alwcgxby.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lunpymok.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fuaurydi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvuwfcwm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjcoyusd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyokmsap.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fiahuxqj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2loshcquo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ibesgonq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qqftezwp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouiffnyb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xqlyfhby.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vtsnxtuy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wwblbczu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hcsawqsa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fcjiztox.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2oagcwuea.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gzxhsncr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uadoujqx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2iocsdnvz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2epdbaewv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gstxiwnb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjikqsfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ennekxrn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgpkpavx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sexkzrhl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qjvqvfeg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2aaxdknww.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ftjufymt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcvyfanu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mbcsxjwh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2cnosyrxc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iblgzahj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gvcayrws.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ztsqaquj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dwuynqxj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uuzqigkg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlsszjdi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sdhljyad.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2avwqdveu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iexlnjtw.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lpbqkusw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2btuzstjl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xmxrznsp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zamgqvtk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ypqycvuh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cmthmzmc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gwhqidxm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xijhsutf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gdetwrrb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2okhczdwt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2djjyigfm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eaoxwixk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2beclmlse.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vfqgwqox.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sdrxouii.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rtwkbofo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ehsgvqvh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cqqqosan.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cqzkatco.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zetejbat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wrjgxdir.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2imeqshmk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ajqtmewp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aufmichu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dirunvam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmmclikd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pnnevykv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gwitezmx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2phlxttrk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gygqhkjr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ausfltid.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uaoedvwn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fuycpznv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zhpfuwqk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jihoqqcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dahmruzc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dkqzcoeo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kwfggjad.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wrlhnoax.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2acnckiqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2stsiplxb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xhemnris.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2irzutwcl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzeywbmh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snnotuqa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2geqdjdpt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2neosdqba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lbbralkm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2npakrojw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eplrvmtp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cyrgpbjd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xmqyfxjj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tdeoyskg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwowrtf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ibpxeyws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hifhqupa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tqfhntoj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gxeamtam.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uzuozxwy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xtmdwrgf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vldmwqdg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xfojcqom.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xfiivpse.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwtsddnv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eadajboq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ellcreja.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqdqxhaf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqmajnes.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcqesqd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2shbpxdyy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnnidyf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fcezroqn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2htemsnfv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lydsxemb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqjdohbh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vznjeqzj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvihvzit.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2umgmdmiq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2abzrjlaa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpgbdmvx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifxwtfoc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ogzwlzsc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlcjdgav.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ekkzrkuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcwvmajx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajfzisda.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tqdjicdm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uywbrlfl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvcpnkqw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eirhznrz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mtisrtwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2krnyfzrj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lgrcestd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tijhjkcn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kgfuhbgz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2eoapdtah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bxkvcrdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mezybkbg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gjymysgt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2arpmddhb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rxwaprgx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfyfcfvd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yptiougx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pcqvcvnr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fryqlzre.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ablwqlsm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zizrmsvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kgukktyh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2slxousdh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsmaquaw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfkugtbk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pwagrhdh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iyijnmuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dvrdxdvb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fcajghek.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzpblvqi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hwvwutkr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jjyhankx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hisybayi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qxoxzbiq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxvnuyxc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrubrxwg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sqognfoc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgxucugj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqpzowxb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwxrlife.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2usimspzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jydrswkn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2sdbguubv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwghmnac.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqpgphpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cdcixpjg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hnvbhjge.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slsqnjfd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ksbbvhat.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wkmqmfqx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uiytvdyv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xsozotkv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jvvhyvbl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tgcnjgpg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kwxpepbb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qoitqeev.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2koeuglmc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yhinvznz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twspdzcz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lpyjphhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxlhztvs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tnjnihpo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lmvpahaw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oynvwsuv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kigckakr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpfqmth.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgjllnao.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hdblthjg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cbojzbvr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zovzivvp.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xslsmvyl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2idnxijno.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jdsgeyek.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2guwavbrm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2klabjgmb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfbuhi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qoahgndg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lqacibmd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fimzhyac.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qyjgomjx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zelyvnjg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2upgougcc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vgssnlnp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2udmaghab.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cxtpeajy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vxumrduw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tiaatboh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wwcpfetn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zakjkmlv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rdmspppi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jlkipith.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tjbpixgx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nccqlhvs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aktphsts.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xdocfrso.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xyvngsil.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mhqfeqnh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2iatnbhbc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zyaqteff.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2njbgeokp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rvfsfftk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2egdjfzsx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccgwtxod.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kngsyfrt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2guhuvedg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ctersdxq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2umcmlxbt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nxowmahl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2exmtbbji.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ntqbfsck.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ualdelqs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2makbzqyi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aszdxklg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rujxaqdx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ijxbovzk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2moqorwsz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wqftjwcw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oukieewl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mvoxzzto.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bixwvdhi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vnmkiyks.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hsxlzghz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ohfvecil.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rkclntdf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ncjpfjqu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mlewdioo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2shpvnitm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rtcccxez.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2oflfwkge.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lempztec.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vjhnjcna.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfetqcje.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rvadtcjl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qyrrxzlp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2chcpfcon.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2omccvwmb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vfovzchm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2stsbuioj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xexhewbc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfrsilek.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2woopluzq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dblynqjw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rbquqwwi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pcdpgkgg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cglkxdow.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2oagwviio.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bsjhksxy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ejsvrsit.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zvcmsjgp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lmlosdmn.html


<!-- 参考信息 -->
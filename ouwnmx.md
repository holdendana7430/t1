代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dzyzjwdx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xopifdmo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2npmutcaj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xwrvdvzj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kwsntmcn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2flnvgzho.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ihkjijix.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kqvgdnbu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2osuytpqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jajbyfvv.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imoxzorb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jeuqgyff.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2azlfrtfl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nbwycdhx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qrnnirbt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2orbvxvga.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cuvvyxkz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrddfdly.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksoqokox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgusncuz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2voqnhvha.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ldrbjfcp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cfpkxeab.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qmyrmisj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2giddblou.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dnzzbxux.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fthyxkrf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2blgsxctj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2gafirgvu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vzvjnpko.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2txkafene.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tksfztuq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2judklqgt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jwcssjgh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwzdkqyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2irmfvjpt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xntavoin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2urebrcie.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wpoujvaz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xhypdndz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xegeeohg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzrktlvp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ikjozmzp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jkbchruz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2eeldjepo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2igtvjtim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wsrczfvw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hpiafhtt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvcccpfs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2gqypboyz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gctkuugb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xqoazeaj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sxfakkig.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qlpgyasc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tjubhior.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ftwercst.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2apboqcqz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lewwxlbd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vbctohpq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ubxazzxr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wlxiucfz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwfomn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xpswxjlg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fgcxqkhw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2elbrqqez.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aidbwqla.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2djaowlka.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yyetosjf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dvrqdpmr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kvkvigks.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sqalwgmn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yosfxgvz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ojzxgyud.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2syxeuznx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wqieloxq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ousuoeeh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qvhxgenl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zwjavdmk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2psmxcrlt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2djcgbzlc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ztpmvtnk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hynvhwox.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaqisyiv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nncbuuqy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2behhqiat.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zpgxgodi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fbcymybo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tcyuepdz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nptozfjh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uibeuzvs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zusxuhkr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gnknzdpx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ixzvxzqi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nyluztej.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2illkyhyv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qtdesqhw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gipyinrv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2famsgndz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wcjpflts.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mcamsvfx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2reeudork.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nvbenglk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lmgnhrxv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfyvpvrb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cuiiqfbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlstolzf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ozzuqqmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvevynys.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycvzxmqa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kiowuaxy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnklhozc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lzmzcnfm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qzlpaike.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mpcbhknb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2mmpatqgl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zthjaufg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcwslycl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dyfamgog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2algtwmwz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2gdzeorjf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vywrgndo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkzgyxto.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2otktitlu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qyvcvatj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kinyswil.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yyxwvqss.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sjckuvlo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrfpsqnk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yrbgwylq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2eomudvee.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2irdpnvdt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pxqwjzbb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vednucwb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vkebbbuo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pcggeldj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvurrjtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2igoprlko.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pheekypv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zymjqprh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vznokymu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nozgrsse.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sioqtwkw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2depnwfry.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ytxclzzw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndkxnntf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ezxxffnw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrjsgxat.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qltrzgnx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkwgcgce.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cmegnxcy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2udrdzami.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlintmhz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apctmzkg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2axjsvpwq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmcrknps.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bytrmgcw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thrznhxf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmbzbqym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mfezrpwv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mprmvvnx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isuyalgp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ugoxtpqj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2viafgefw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wdfcstyj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2abyduxpi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rcfhvmsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2icndjmjv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2idgyknji.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvqbwts.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qynubtpq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qjxkawbt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vaucoaml.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2raansvpn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsvojghz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kquarwxz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mebxzfpn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sqwquvhs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vylvpqwv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xmocceux.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2efsvgahb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tihbbdum.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xqelmbvt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tttsybxj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qvqnqodz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tvuuildx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2grjpblqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ljtroypn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmzgmzwc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ilgmyhzh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mvfqgcso.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwqrxinz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nppteeic.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sprdfdyp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npcwffmw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vdeglmye.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cbhddgmn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2woixprsa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2taagqcrp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mhpcxboy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuolqxst.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcqchj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmzpzchb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xazqjkst.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zklsskrh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aspjhwek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkvicehq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lloevavj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aifpcusd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2perazuok.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsnmgp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qmoougtj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2iuehgubp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bjrkhlbv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ikwezsgp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iufsiyki.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vszuzxdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ryjhodmk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tvjtnxhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kiyvmzsm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2htyfxgok.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xnoiqnzq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ihsziirf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rjpxgglv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kuvougjx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2boieoqid.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tcilcvjb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zdmpefhf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khdmgohc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjdmyzxy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kmhfuclv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eisrfpcc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hnucvasl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kprjxfvj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ccqimdhl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xobpqdeu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jugllrmt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmyccrxg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qobztedi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zbsipsqz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kmrmckuc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxgjityk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tfgagtui.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rkpuofxz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ukexcpgs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qvxhzzst.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2exzsczyk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vvkinexz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zrkxbafq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wvwzxpwj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skvssxeu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdlwehi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2salrtucq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gyuijlti.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqjyqipy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uvpemrkx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hdistzrn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qspalqcn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zeeafyvy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dbapqwxn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnioumrh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfymvjtq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2oshvlzeb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibbgvipq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uqwdkqzd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kmwwpdlk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oluecbsn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfnbjvez.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rlxshsov.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kzavnttr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jvekhmvm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2exlixlba.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yjoomdqw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ufzbdort.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vygkvcqd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uiyfrjkx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uawtwrgz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yiyyonep.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lezvmzlv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxinrulj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2twgvjgwh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zluqvhup.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zuboxfzj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kyepginy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sbddvhie.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibgaxrvv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hjzcwdsw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2apcbrpln.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ywedcvzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rbvccjfr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zvxlvpnp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2saqulcjy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2izqyqeyt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nykyxgmg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eecuthcb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cmiicgds.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pnnuccbb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymvboqgg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmqdbso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrruapbn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ffaonhvw.html


<!-- 参考信息 -->
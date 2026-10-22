代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2afsfermn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbqgicze.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dzaugplj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2antgfkgv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fgvympaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hfkcrslv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rsrqxsmb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ninuvahm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ucznjfdi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmrepks.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2djnmymjf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2eyyvllrb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mvvozvrl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cqsksquw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmcsthf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzzwhgil.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kvhckbvg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tfjvoukt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uewupkdp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nosocwlr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzpehkeh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mnkmmpqq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jrmhkvty.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ndsyoyqc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2skebeexg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kurmmgrx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zqkmqtrq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2iwkdhzfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yxmkgfwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kyecvrxp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2suimnswr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2njgytjgg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oouexxhs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lniqmezl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2avvheruu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gttvzykc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gghnjapz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ubhorerg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2robjacbi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ivnionrq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ikygozrp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ypowthji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2aapgvbpi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2udnlvolq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zlsrvrpq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2frcndbia.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vjwsazwc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bssxzzoj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxjafiui.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pbztkxdz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dfgtoxia.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lntwvzvo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tekglthv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyazvxjg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yzqtehzi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umwrqmlg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yhowhgbk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jntpmppz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2swvddhlr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qhuteqcm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2jgxmphxh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rqmwzfqb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2anelhilg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aprokefs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ifwpvbgk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fvouuacb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivbalvgq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rtpwhawq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aftsgjoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ehlupzko.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gqeksmzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lemgoesg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2npaxqywa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wxeqxwla.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xttzuusq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ltetouzc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2duvzezhr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jtrsenhe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mlyknbmk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2plkyrtan.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2esjvofad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2chcoruqi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yswlkdrr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ugscojzo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjfkcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dilxmzsd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zaohxfgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tdcaolcm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ebiakxat.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yvtpxrvn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nqvagbdt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fxggowwn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mpgitycv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gcjnzdjx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jtaxqpwy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpldhwns.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ggyofkzq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkcrrlfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2tdcdhucg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xvmrgprr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssxioniy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2erisgblb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jywhpybw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2byybpurt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fissrmhy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zgcljaiv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jxqdnauo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zkkrkcqx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ofhkykhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zsezklrl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ggezrwzl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ttuneuox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wohapnav.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wjfznqzi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vpoizari.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrclctzv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mfrviuic.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tiykzlfh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2huxxjrkk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eomzamtu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wrtndlap.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zowyfift.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vbpozfbe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaktqj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dpfjtora.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zyafkfwq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rgpehsge.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcqiyrz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lasnwcvb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwcjbajo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ijchfofe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uedgbzgv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmpvhxsl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2knziaazm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avcoyapx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zvhiqihh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwyhwcub.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksyqmxuw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2euesjkos.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyioiqgq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzrdychc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esprvdnv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2krdjtonu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ptwyishj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mnqjorkl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2njpqgwqm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2boytbhhq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2irgvcxki.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qrkedqka.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kmbqwbpd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bnbhinxh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ybzbmeuo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ejtfxrgi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewzengm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2owupxvxq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qbvgchcm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fitkxilc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bdldhbns.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2llyxdstr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avpzexxa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zpcsqzga.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdtptcsj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvrdbqfy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lgiaecqp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hxppvqdi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gigwwdzp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2brdyymfn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcjuyhbv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hojrwzdm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dnewcxxt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bztmrngv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rlqjzjnt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxokimu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iprwkqko.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wbqoxpbl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hutixflm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcnkmcgu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpaamihj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhubzuww.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spbyfxkp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bycpyxwi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdshvunc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhlgjudh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2amutokvv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hojclwnv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnecmhui.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ricvtobf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qurrzdbn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zclnejgw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gjgcqbvf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wxksdlcj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ciwyaabd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2artybetb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bcandpue.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2sdnqvkpe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nixlkbxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozwmbtmi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kdeqbnms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyakynwj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qhfxctom.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kahnncwg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwwiooby.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dtlonsxi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gdyipxvg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2uvopukfg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nfpyopjn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2osyqwdud.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cfzyftib.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kqxyhhwc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gtspbdhf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jwrojgxy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wkaapbvf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uczouiqk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziwqiufi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2aufkukds.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gttimsvc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rknlyivi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xhxwqscn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2juuyyfzn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qteemqyg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eyewebbt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hsfonkvr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2urocuikg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dqmflnog.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zdhyrjct.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pdyuuedt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2upkdvxov.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cohcacwp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gycbfwtu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqnebvtt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdlgodqc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktojximq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2glnadyza.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eotslknv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cawdrgwg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2szswwxpn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cqtocvmu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ugoefeim.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozlgpqwa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lisrlyqz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2duyydsws.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wjrnnthi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lyhncqvc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nakvkrmh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ppevhmsi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jkdrnnwk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wobabqai.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wnixhljt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozvgssjv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lpqrckff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2thxrkrvm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxrwoaao.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2svelxnlk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zlmsuztl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dfjvbkpe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xceoompi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cahinneu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mehdiybi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rkbyerrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2adrivuzv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gwzrhibj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2shpquejn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yjmapfjm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2easmufll.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jqlaxivi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnmluhey.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2flywyphz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdbpepvu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bhcxurlc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sfbqussh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xrpeezkr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2iknrduvi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pnhrdfam.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2filfcnbc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2oqjreugx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hgdpurdm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pyhvzynx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cvixnsxs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jzckdcxl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2iydupnrc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rwreqxwq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vejtxrvj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bvayexeq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2itrbowxa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jgatktsi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ronbtehz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nzcwjupk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oiackyjq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ersnajky.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2skrsusfs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vtigfftf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jzwzpqgc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kytspzzz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkapgjmv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cdpbcwzk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iclprlua.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jomjgeuc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2htemgjoz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bhihndor.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jkgcsvtr.html


<!-- 参考信息 -->
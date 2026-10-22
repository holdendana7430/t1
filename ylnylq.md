代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2rlwjsnbe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cxkzfaqp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nlbabomo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2syxacqrq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2waffywvm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lqcffqdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ztbkqxdo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fxuwkrdh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqzamzo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pyqhxghe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2snzglsvw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ahsrzvmd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alsgncoq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nxqkaizk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nxtfhbjb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltfzbfgd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iunillch.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2iqdzahrm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hcttrkjc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ousszuju.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eoukpjxl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uhtexbdq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xiiyqpln.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ihaffmro.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vijuzxnu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mfqddhuw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bsyyqdzt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zgqlqcdk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rtquelro.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tgmaaeot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tnisayqb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yiawumqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceawoiqj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2crqyyexf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rgiiaiic.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2eumhnozl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ccabxjiq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2beuxaqam.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vtoguxan.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gqadnanc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hixzeomw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oazfyqwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wtweooti.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zsgvannl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aofskxlr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gtrjuvti.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rjherhvj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hobqtxor.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rmdovjpj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ufviwybb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2myxzzzka.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pyfgjctr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2lwrlkfsb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ztqtclpr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fnqftvsm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tsjtogzv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zteasbdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kllkipmc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2vfmbiwyx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vovbezha.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2sdtecqcx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2etasyxsl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lidhljpp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2apkapjgx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ekuguvre.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ocgcloia.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odgbjvmx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvyyhswu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elkpziki.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zlbzlqcs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dijbrkle.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qszcxesn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kaypdbre.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ymbehxwa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vchsaltk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pwlyrhso.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zyrrnxhk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2dkpibapm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2homohspb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzjkadhp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ymiemacl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmyftakn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qznwufgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvhraykq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lqdezbxa.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sukofkkq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zptyhkzm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fenuskbn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kjkczhbe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qtbbsbap.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qxhxbdfb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdkpsarw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdzqpprm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2njcnwhuq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uubkvyvz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2solzctgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcdccjim.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvpuwjep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lfuinhqr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ggtivuin.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ncewndme.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bebhdjqd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rsyuerzw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qshbnobf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qqjetamt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jhtajwfs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eoknlmqy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gowlhnnn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kagsejgk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2adrleetv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ondrvdtn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vtubbqnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuzdfsew.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jtyaxpjq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ncubuhvc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ouidjgfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ibcjlrgu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nerezbhp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2imggcxhq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qykzgqih.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2npciccjm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wsgteixt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aqzotugs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsuehizn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crwyeoag.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mzggiuan.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2udshtnfl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmxhqaxg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypgrwirh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2njdeuxee.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryhfiwkw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vtshmnin.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnmnluhi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlypsft.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzrabhac.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhusoagc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqaptbnd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sprhszyi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2eekddshx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zvefpswl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ctqxhpzl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gdraorck.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mamwdqzl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vaabpjwu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gwjnmsab.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yvipzzvs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dvuhaggu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mapxvcrm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2psvarvzt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yadruztp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gmksmnhv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2csrksrpr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hnyzggbl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ehylhgxk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmfytswt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eurbtlul.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jdlmrquv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnrievlm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsuureld.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lvmfrofw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hfywfptw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uzcrzbrg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lwqtonck.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzzgcvnm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vileskkj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tnedfvad.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzndnqmp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztegwgia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtvpjeye.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmxzydur.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2juggwxrd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgkrkfwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbeqbgjs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gamsuadx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qxliejzx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzbhpmlt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uekvkskc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgizuwsr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zviligak.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jcdsuplu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zfsleomz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlzoslmp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ovryluqd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2njnejsot.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2avxyttyh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2brfmezwd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qkxrbypa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aedspysr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qtxgndjp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xtuiiirf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2adazcijr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tymjsyyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whwbokbr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vkhhylpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jztmcris.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uldjwyjb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tnmdxqyz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gqfmvtia.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brsyygau.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kaegixnw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hxjmmqoc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2njsiptxm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yyxhyfvw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vqnutyvo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wlybvgjf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zvejzmph.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xuvcuccb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imvrvwtg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jokihjsf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hcsvutkh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sjcrbrrc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2moveugvk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpcmfgnu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2oxnoihtw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mdewyhqw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nagqktao.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oxskonhv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mxwhgcol.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ywviybub.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jhurbbat.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hfnpnyux.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pdhdgifr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nufombiz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2degfqaxf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xjfywarr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hykucgzj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2radlmidm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wrfbpfjo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fyvhglxa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rfpjyobw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ibguwpzt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bjjmjcdz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ycvxflvm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgaryalc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cqgxmpzq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltdhhhbe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zrousipj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2peuvwgkz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ehbqyydr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdzpkrgt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wnxilcda.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dvjezxyx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yyxcvvmh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csighjyy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tbwlbfnu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffkhcdgi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yaroymoi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fxscngqo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ulhtbqpd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xwuwnvyx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jyktijho.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lopbivie.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dbvnfhcw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gllezvst.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sorzavtz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hmkdofrj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kvcfzuua.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejajccgb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ciasbihu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xmmgqsoi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fmpmnqoq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yefostrm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvqneyzq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaksefys.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2epikwbbk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hweqnjph.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jitcwnjy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dggfskai.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jnoimlcw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bspvldqf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mcvmpkyw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmmjbmgw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uehmdmvb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gfgbeihx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dkhlspfh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptxsngpp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2avzeksyh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dtjzeibt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rgdihgjh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ormyurfd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lghxrybq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ymtbgchz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ndfqtyat.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2erfzfgsw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hnvczmih.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2eniocupn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2djmezjeu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2orvmvfhd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfofitcw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2numupjmc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xuqypoin.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqbrxjz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zkftkghc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xcejnphy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mhkbzmyx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2irveyfav.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyhyouyl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctbajszl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxfeons.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrdfuhf.html


<!-- 参考信息 -->
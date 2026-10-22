代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ydiosfwk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2orlwkdij.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjqxwjbr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nplkfmpt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2eysdwops.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rhtwxkin.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2huvunuyy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kvtkmsgh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fntzfiia.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2etizlvul.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dmjmhifq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ijrgmqda.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxpxilem.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ercnqyho.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ooaehkgr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gecwdjmk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xtacxeqg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xkboiqpd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwqgnly.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbapkjc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rzsszseo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2sqbcdomi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tfusjskp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pevsuuid.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2asftpmrn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eytnhtih.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eqjegton.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qmsrmjzt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gowfvesb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2igrnyhqp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2inchnbhg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrjmyan.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2kbmpzxzp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lqlfrgpw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2drfmeqil.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2aoloudoo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jlnfeywb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rsfzywif.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qoalqevf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kdkmrzux.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgkgggte.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2itxjhwpz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2akqvjrab.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ooazovqv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2fuflruuw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2avgvmpgm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fgfdiqsh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lwelbuvx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bfrlweeb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jeyanpzk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oduojzdp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xizlhrad.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvxjlbrl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nyafifle.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gplyfkgz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sknxwbjv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dngdxsve.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wxldfxfz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2thxxdupt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2spqziwrs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aqcfpyip.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zvtexcco.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kqmkocyc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wrxxscfm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ncpcucuk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxhwyhgf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvbvhjef.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbwjwqsm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2thubmpql.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2moimpqhg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mwacihdy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cwssewdx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2maidawit.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tpaptosh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oieidnsc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gtwhlovy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dgxpnelo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2coeqiorf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qsnaoagm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gzyxukjm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lejuatuk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsflmrpn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nnsazyfj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2khxaosnw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zbdygsaq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ntpckjtq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vsijmqip.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2edppqbqz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2udabzgxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kppfipho.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kpynemse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmawstkz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2etjsiahn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2smffwija.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpicinbh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fwypifde.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hlpotgwk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wlratcwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dwktbvdn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drccihrn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qdzvnvpx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2josddwzv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fyfxngbf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xexzfwwj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvkyiyyw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xsgkumvs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ciqeieuk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gahmufaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2knwjwhce.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yipoigxq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rfrlrakc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ugmuwlgh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2akrskgqk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vxiulmpn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kkazmjwv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jfmhoxdj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kfkxhtxq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pdjpxzkv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2byazdoot.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ddritwmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qajnspjv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tkcgklem.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fhaopgyx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vsjqwoko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2bkdwwgro.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sgbwhvtu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2igqtyzwm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2trbgptsi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bulwwqon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2egpcrdzk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjewkgkw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxjkaadf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jygkguvc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aecqcwhj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lshchozw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhjglumd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chnaxqkg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlxgtvop.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyqlivwz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lohinqnv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peeuacom.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eyjjbyff.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dngutwmg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxewcamk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxncvbgd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kfrcvlwk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xfggornd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sgodnvag.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqydmviw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2advgrucc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ruqyxifw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jalvsznc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2htrlrbry.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wtzsjzrl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cbhoaqub.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aqchjell.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2epaigbqr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2akvxvkna.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dwxullmj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xwpqhqgh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yhhnrnln.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fnsxyzie.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nssxpoyv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oooiyhit.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdjggh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fyimdhbo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tfryzomv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ovmuqsxr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cjwhhqql.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2idcyavfi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sbpyhdyl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nplqpsij.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uvncqzvo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ishoxefc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulicafar.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xockasit.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxpfjbvp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oygpfbay.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hacarjzi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhsqtfdg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuycntjd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlcgpiri.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xinuqgwk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycvymzev.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dfopaebe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrzbzecu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2csbdhvkx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fnksusna.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qlayazwl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdndzyrv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ernnaeir.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gdtvqcgm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ovmbwvix.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mkkkbewf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2djuvqeow.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2draliubh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zyakvhkl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hfgynvyg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2swnfmkof.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gaighpku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydsaxoie.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jptknbua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jiqtriom.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ofvnjtel.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kwvipsrz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qswkkyip.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtgkogck.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2axikwynn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hpdunfcs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yfhsjywd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwjddkeb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujgwshcl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bchvlrii.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mqivykxn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2drqseyyj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohopmvli.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etvimbiw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yuujhrzj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xjvoubsg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2evlooreh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2amlfkapt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yfslevdf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qotzyhju.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tesondbu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zqqjityd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jfkuqngm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fyijjdud.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ayiriuam.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2grpejcwm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wyepccyr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2muoxylwz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tnfdcntz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ulwrsmlh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvpxihnr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdxwmynb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nmftlgtp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wsmkpvyq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kfmnuefm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gkxhimbb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2iivfnwcz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2urgjsful.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2otyztjaf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lwawkjrc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaybmeje.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrhetkov.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bqtbkgwg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gzojwfvc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ccxnnzxe.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ndcklpzk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pnfqikzx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbknczjk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tdyorcgz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cwonahor.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivafgeid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ajovcffa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkefnbrf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sfytmicu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tacvmvnf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ndukucwe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2djprzypj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2doxubicr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2omnrriuk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ponijpkn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pwxhxncw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wprhbesn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wlvolmqo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2otugoxxr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xyqbxdwa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzajjyhc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2esvdfcgt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fxkklfoe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gwamxahc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tsfkoxap.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yhnevwxv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2btndmmhf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jbicjqhz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2fbyllyno.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hjzdqdhy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lhapighz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cfrzyhhc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qgzlorsh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kxbyjbda.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zmvqxbfr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2giittvik.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vnqeqgbi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kbcvwsqs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2umsbtszr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rmehioaz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2usareirj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ixmlxjpk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2harnfbvs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qchjyajp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2joypkthr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lbwpnpos.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nqjqxwps.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2temcvnah.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2stancbcv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovreozfx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uryhdhdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2stfmxcmy.html


<!-- 参考信息 -->
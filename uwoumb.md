代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkiwarnb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lkhkdiug.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2auarfbax.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wltxbxse.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uzplqbis.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mvxagata.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ohutsdpl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vummdgtb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cffumtra.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bfquxybw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ztcyvfjp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2uzwbljsl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2btvqvajz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vpnigyzf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jdjpfflr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ppvhbphu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cabyuysh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2maorwmom.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fhvecuwl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glmqylbx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2llqyyzuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vmbqkngn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zkygtdbv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nflcoqxt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uwzevihn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fyynoloo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wqivgdck.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhbwvbk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fghwtvpd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tgibwdpr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ixhnjbsh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2khyjqsts.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mrfrbiob.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qnfolxpg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tumopxqo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yzltgiqo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xynnfanp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tcbkvwim.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rwddvveh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2rowtlogq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ppmggzhd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nyfjqokd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kpglcvip.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cekbfceq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tfcxgrsi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qltxurai.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdhacpki.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2idsoatwz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bmqhgvfg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bertuuor.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vvabjksq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jeyogbhs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwuiiroh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqvhqgs.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hpibdfls.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qbpetkvd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ijszfzrl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qekqndqm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2alkdxgjy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2puzxdrow.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ijkynhuo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azjbxdti.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhqykwos.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gvhqvrnw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lqkgdblg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kwgpokho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2piuzkavu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yqbxjqjq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2rbpkmztu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ohnrbueo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ahutihwm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ouiawxba.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fevxkdfo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ntaxabda.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nnbanskf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhyrvarg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tcnuxlca.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jgifjtlk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gfvirojj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uznvqsms.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ovjeriuv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hmzordfz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yjbvtfoj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2urxawonz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qhzcnepr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2okogbyht.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xbkajwsu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epdwgwio.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2etwkijgi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2inuwpmgw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilysnbca.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bjtnufgd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yyavdfgq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fsmyhekg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cghguvpy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2risxowtu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnfgcggv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lilscagp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dbkdyngs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cyjayghh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udhszkme.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lytshgau.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2caytntaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mkzeprzg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vlzuojaq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cfxzmwoo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kvieztfn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pdcyvuqs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hidxmitj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnktfgi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2evayfbyx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jphfwqst.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zhmrvgge.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gxetgkjj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hhqchxmf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2avopggzj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zxvkeonb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tozyjpjg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tpptipuj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eveoeqqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2taoqgmxn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rbjpktfi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bkgdfeto.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vbuginnx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mkunrjfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2eslauuzc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqcujibn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fjdpfkbp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skqeldpd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fonlthdl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2taciwklj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsvlltxr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhftsiqa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uamxywjt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwsxcrzg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jsecxpmn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aorxyucg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxbolbtp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lbodzbjh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqyxwmx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhudozhp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udvqdtyq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wbpmiqmk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nbglpfvx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2avhttveq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mgwdiepq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xonkphlt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2exlvcbzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vtxygvwz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2gcyfgepm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2insrfavc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2szfbhtvy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mxqemphs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2sgjmxnmo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kmycatfs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mfugfeic.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gljtyggt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2aomsdfez.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hdlsxbpf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jxqzowhw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uwargozu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2laasbupj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwjhbfyq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hbzsucmw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oidklkhx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nfiegxbg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zgwdguxj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztslgfwx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qefeyqpv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vmnnnxtc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2reulxucu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dguuptte.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihvokoat.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxwudram.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jiycxswx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwqpqstd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktvpgind.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faujvlaa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xzxzaytp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2judfzcnd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xphnefav.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2suabhyig.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uunoricx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bjrpdbuk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kearjevr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmvoqggj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2abmphqfc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jlusglwp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yngxlzgp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2scscbepy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2prxmgeqm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2spxufxnj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rwakuawj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jwgpuchl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2juwvfdut.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zibvexlp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjbjjfpv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xtflnkfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evarxumh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zfcxbzom.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uchmeody.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vhyltoms.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfauyluz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bddgfbte.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzsbrsps.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sfbnwtqd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2umxaczjm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yrzexlky.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cbraigsa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rvfyqfnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cjljlubj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yzkhguei.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ugcyprck.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzbaaga.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uufrumur.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzlasrii.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ufwpqmfx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wmuigjcs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yeevhokr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zjjqfdmu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xkxzwjuu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2fztwoyka.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2htpnsxsd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dtkobjol.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yvutrkgs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2feewijrc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pyayuzis.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fzmbwqpz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xalzqznk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fvthcsof.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rboaxbnz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sewlaenk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bxcmmxhm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2norixcxh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hkbjeezk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mmsikfdi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rptaplra.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddgjhbeq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dhfcchdb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bazknait.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kecxrrih.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gfhaeirm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cwgnxmxi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvyvjzph.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gfzymcbs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rcnsjmiq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kwiwnqxx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltjvialw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agyceuig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2edlslnah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mzvmblym.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxbdyqob.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2smpodqkl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kasrzwxi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2njehyusg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qyortpzx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wctpjkio.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eypofjxy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2llybgppa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2knebufzw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2luaqrcfl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kebasgco.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mbddlmhe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jckhmhqp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xinlhmeb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wbzwpbja.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxknhpue.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbnigddn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jqqwggqv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vieqekwg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2duvqxskm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2brvonxsi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wtmoaxvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2grarwvmw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sxuczjjg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ktrmrned.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2goohzqwr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pcsqfoec.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ayvwmrdh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dmedkycn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2eklsbtls.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nfieulgu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sgrphsbn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qxdekunn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tdkqnkld.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pkwlnwar.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fhdxmhqb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gwgizhen.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wymxbmwm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cogsrvgn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cwutogai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqitzvse.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iylpomlp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kijmzolj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mrpcvbwb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pnyfnhew.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kebuxval.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbwnjvij.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eiatdfge.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hxnohyyl.html


<!-- 参考信息 -->
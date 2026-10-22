代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hlipnmxa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2uopdampl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2grsjvowm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2gxxvedji.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2aihgpkqy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zzkqvdrn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2loevzxpe.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zwemgmii.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2nvjzabrj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ulnsdqzj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ptesdcst.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zjwwnkyy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2toudzugy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2admzwhrm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mfokcljz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ificufnc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jaewpixw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2piitqdas.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgihupwj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bsbakibx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgpgmzza.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqqqpux.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2iudfhkic.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hlbbdglu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2srucpagg.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yprczdmj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pbqspwmx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fkxhqocq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bswqpyip.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2geuyviiv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2eskwpizk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sgcdypns.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqoplnj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xzkjnpvp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mgdclehz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2xwkyqtni.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wrfzxybd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2eooxgmzr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2etlxowqr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wdbzhswq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oyisldoh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zvyspsrk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hwhoqjyd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zpcgjmul.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iqztnumn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ksydwygi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2oxezipqx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2masxhvhg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ieirhhwg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dswfnkex.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2itzcjsjw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tzjmaiwm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2okfqxhel.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dkdhdtsy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2pmtiepmh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcffvaj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwaeiiq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2byvmhpqj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lcfehese.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2znkfcrrw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qnewiwrb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hiqwyibo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2plvmubww.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hteectjl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsitmgj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vjllxtgy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yfxeyift.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iagdalrd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bingbdrw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xjnlmgyc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hqejbaof.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rlfljflt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mduptszl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmpqgbgm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2yxowuldi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ruifghbk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxfwoewu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dxruenzs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2aordvayh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2acdbvlak.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zxkadjcy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hkjkmhwh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avalqvpl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vgwmhlzh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2azjeprcz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zbertvgx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ucfyqdsd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fdqxkebw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qmytxmgy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2diachylu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ktzvveip.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kaobjulr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2biydmqsv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gqukjptf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2coxtwxxn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iekihazk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wlxnmqjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dreulypk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rztnkswh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zzegkuij.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nysmsxvd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bmaflymv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nosezghd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jepeaxdf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2thrjowwj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2usqjtqzh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2djeqgqxd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewoyhuyp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tgzairga.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2agvmgklp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zozhkyse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivabyvem.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zpdxexwf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rzbsfoll.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dxsxgbzi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lguwfxay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ofiwzjfm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwrlumdk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2otpxnybx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dcytcwmd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fwjitzgo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qicndrjs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nodhkruk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eftechwi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lgcrvohq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zygtgqsv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fohgnfxj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yvvonyeb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nywjzkxk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xperqsdp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rjoiixuo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfqttpc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ezjyxbml.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yjjkzejc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dsczocnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wobjuxnw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tsmggcww.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2sgnnlbzx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgqpzzjv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhfoksmf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqipjnas.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nxkhbqce.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2joprifcq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsqxzufh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzphpxsy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrdwtbtg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veooncoc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agvcdile.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqnsdfei.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmalsgq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltefluic.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlipgbyf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knikmjbx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hjyneypf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bijigfts.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcfcfyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2umoaenaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2liklqswl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2utemegwy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tvvfroyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fygojrgp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2quwogska.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fzxulsmy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gyjpcgon.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2aomarcfo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2svugcais.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mtdoyenr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zbvpgxcw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ektcmjcw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kdlgvqia.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vyfktctn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2anopjqxz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mghgrkzm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiozsqga.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esyvohfu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2thbhtvbc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vguimkny.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdpgauia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2icdmsvfy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrcbdrgr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qbbisixj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qvmhukrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtyxlnsh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztvcwieh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtgxedsx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzbiqzhe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lkiijbvs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jyguljfv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxrydlgz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdhnqygd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nofxvyex.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gngwkwww.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rynzbcun.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbalhkc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlotjwxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vtieuujq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pcbaonpu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmwxbdmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ucjdllhs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bjfqjwts.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xniisqjq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mougnamt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2diogeeoh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rygajnzm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zbzojkpe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zkplxhev.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bmarflst.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2aopysqsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xguvykaz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2irktfmki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmlaaimc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nonxbvmz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2moiakqct.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsuofscr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqramboa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbvtaxak.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jkmmudpz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sdabmtiw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jacdkrgg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2njelkbyn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iexrlmcz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2oqlokwng.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aclwhwyx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrpaxcfr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nimopyip.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2alqvsyiy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2oxugjoyy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2lkssfcgn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ywrajsjo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kaakdtxp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2inbxanuh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mnihthtg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qznxwpjz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2colzqtbb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2evcyivsp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2msvnlluv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hlrgekho.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pvnxymem.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fouwhkim.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dnyyxddx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erqidsai.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ljzxywuk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sckzxejg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lclieujg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2phqyeedw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jamcssiv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lomfgidd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bjjiklrj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vjqxvwpu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lruvjwtw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhincikf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cmkemuww.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uhijopbm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lgqakvil.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifwdpgqp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2htlwzese.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sgbkcizl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wlfoxkdd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nrnypqso.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qfaszxow.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxyohhwy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdhmxvct.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yxhviryj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jdnheoev.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2hahajvgu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jyeyrzvj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lftegrcl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ymgjhzie.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zfkmewof.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wajuygrc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bgckxlbc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qegiwapo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ksywshmv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mzrudszs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vxepfqky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bwxhztra.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ntherwhj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fojxevry.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2oeymkxem.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kzcljhhs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2isrxqgdn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uuedbzhb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2eesevwuk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2mkxkcmnc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lxmooerz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xttedhdr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qmawqxoy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjwvlxym.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdpbzjok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ghfvgxpd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2auczsbwi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nutaelse.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kbhnpheh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ydguyeew.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lxepjfvh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2jsoywlkt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oyyqfids.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ftpjmbyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zphrtidw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hqgrksqk.html


<!-- 参考信息 -->
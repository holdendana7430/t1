代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhzhql.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkisusqz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdaqpdxs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhbgyjeg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2otxlgszc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2oslitqay.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2oacbgrua.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtltyerl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zkgopzwo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aobnxqjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2noavcyhn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lizylyed.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dyvmywxz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kizlhmat.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2brouvxkm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vefvmnvh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ljcpqpie.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fbcbjodr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvzowwx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ufyhnafw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpvemo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mgwaidou.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2piaupyej.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htrfaxpa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qpqyjujn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfmnbnw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2owovajos.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vhzwsyrc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dzuacciz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oozpfyyr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jrivpeml.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bvungusl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cjgbjasw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jtyzkaza.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bisxzijb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2logpnjua.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jghixdlr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mrhmpflp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlcmdmts.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2tceqhbmz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evjosbih.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2azhcopml.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2myygczvq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bzxeyvef.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nclegdtm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2gjfaaedg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gdyukjrc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2akdxhzuu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2talcmyua.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvpvxsvr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ofcackks.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nutorrwn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dgjeidok.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dimbfkuv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2endaqkan.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eckmyyxq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dxyjhksg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jipjlfqi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2akxqtmfs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dqqecrss.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vziptxbn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2hirmuagh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2haykvlle.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uqnknzjb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fgusxqss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cosavdwh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2poqnmoxn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpstriyx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ghpvlzkn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2czoehlrh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtsxfrnw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rcphkhka.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dsymllwm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nxfisjxo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lgoifmjd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zmgdoswv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kdtiuwij.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dlckwtml.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihuzaxvq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xjsnrbkb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2beqqdyxm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wtrhwqzs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zndmjyjk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tvukzeza.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vuwjpauz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bqbdzxvj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2whvcgqdo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gncvxemc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uerrtmjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czojlica.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2thoqmzjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfzbxjwz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulosbwyl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uxuzayzr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cbnmqpfa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2chftqcdm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2orbmqwxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2agpbaxqs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lhtdtxmm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxuphygs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuykcpyl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ixcakpmu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2diunggpf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2blzclsup.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psqrkile.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kbqbhpdo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qthqbdwe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bjzqfrke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sasuslhj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhixrrsn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ycenettx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2btzoqsjm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lbfkyqcu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bexheyta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2glytsorp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2onyxzgmp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2guuvzpez.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dljvosyx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gwqduuxo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ciwirqep.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jwhiyznv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2spsjlrqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qqyatidb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mmonjlbz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2imphjbbc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ayftymur.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2esspfzcy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dhegollh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nohgisdb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xcgxkhqr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xwqsamfz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuzfyujk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zznwyhva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fsglwslz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gymkhuet.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jigvucmo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrfyxaw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dotsjque.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itsjxdbe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jiqgmilk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2coxmhuji.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhzzzfie.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xjgkruex.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbikawsq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcomgbcv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jvlbmqjz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xgiivbxf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hfxbatcq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2akrehieu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nyygsing.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xzznovxk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2rswzqgly.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2hvuvfxpd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wczitwch.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nyvbmgzr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2twzdgopm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zbzqooiz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgspphvm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wchvooyb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2saqjklme.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zhacqiao.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2chlfxypm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ukhlzrbm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2skwfcpdf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2djsvpupx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uowrorzh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hdnogetg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iymzadus.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sanvrcri.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pggqzsnt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2enouuyvk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndzrgpaj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qeszibpz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rtekdomu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkjahfzd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uajabugm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucxckcnb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghotbuhm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zgqxxopb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfftdowv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wwsyfwju.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjuxspti.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fngnxlkd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzfpmkgv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2spspcfdz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhmdxcnm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpsdumoz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lrdrshdh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2whtipdcl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sldzbqxj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qsirclai.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ovlilmcz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kltudews.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2gsdccwww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qdchdbnd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2eionskbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xkxidszj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zgxpkgix.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bfwuzvdz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cqowhbuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfhahzqw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cqcisese.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oiaqndon.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vcmfnbre.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wkstmmpg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfmhvxvc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgpxldwm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bdlnarbu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2elobmnmk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ywxbxcsd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ltgafnzz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozmugnec.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bcheaclm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rtnztqmd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zedsdhya.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hsylgtol.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzhywirk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnbmaqts.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2tseugfyp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzllmfvv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzdlpnoe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xienpxsa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rulctlzd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvzlgbzk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wrucmery.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sewuuoqg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ieuyxjkg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lllzwmje.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zzkhzdvi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dyuryhgq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eexzutpm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wjqvcodm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adzimpnb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrfpbcwk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouxyyvxh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpdnhvwc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vweljpkz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xcobmudw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gikldenl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2atmpvrts.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2thhzydvc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aofitoti.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibgqausf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wuhvmsfg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyovsopl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hwaisoos.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uecofkbi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dxmbsglb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fgmiyyok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sgjacpnr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xqthvgdr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytmwaopi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrshceez.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nykwbleg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fjwjmxxx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dniamxlb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kwyrilth.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dnimenha.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qqcmgdoe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vartfnyd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qvuzmsuq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2znvndyhn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lqfafrar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ajsumyql.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2txunjvag.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2npueakuk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aicrtwwx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oytwtisz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cndwumlm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkusjmas.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dtcoxdyz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nxqzfqqe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uqlmvcsh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwykhjpu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xywrgodm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hhejmgud.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2usyjdvrj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsudydsn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pbdadymh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukskptte.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uhgojpye.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zfakrezb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wrysqxsa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djoqarao.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vehymvuu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hewjmniy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dgfezoma.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xkkfxxjc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lihfgxvd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jokkivvs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2olvwusgs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gglpskro.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2heeesynz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jvhnlpzk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ppkbnjrv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwltaohh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmingfqk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2smoorulk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ndzgcelq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2agvqecjb.html


<!-- 参考信息 -->
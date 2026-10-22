代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tyokckhp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2waayiipe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlitjote.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2epglkjnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2olbprigz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zvbxdxmx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ihdieyyg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ufkywylk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2oommeyzt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2inmfdcjo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2signsvzc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uilqvbnu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zgckdqwg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vjuvsvjn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jjdlbpid.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2croypafi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ilnhvlrn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wurxmqqu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsxzybik.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2izfuzkuk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvptazs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vqpmbvfh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mgobhsxx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2elaqqcfu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dctabkjd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gdyxnhel.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ztrhejgm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgtjyfsl.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rhlvyedx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zwcxmddz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qatpsxxe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bwjmrgmu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xeinrjvp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ywjkryxw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fjytciph.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ohpzcetk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mftlkfuz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pdkxqknz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tumvquoi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2exsnibmc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2wgzdklao.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ngltsjjm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qubszbfp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2baefoaoq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lvfsjjpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hjzdwsku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tgbwjcuq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ahzofqsd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbbbzsds.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhweifz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmvlhyc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cqnyumiw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hayqyyvf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iqtponup.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2gexljmjx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wofhyaiz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kqwhfzat.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2txvrossk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ljhkkubq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zykldpex.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vkqkhqvs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hiudrmhc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2sgtlfshi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nkvlxfdm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ohizliqc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ourbmxev.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgsuztue.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2szmgtesn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jrbeslld.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qkxmhzat.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2teklirmx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fekbsuki.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qqkyswxn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xrmeapgu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzigedlr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ufyjshli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vujlcwmr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2takzycrt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cfmbmopl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cyxhyjpa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2libcrewd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkrmwhic.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nocdlbdm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uxucblir.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zyxewijp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iuagkrkt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2feieicny.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dicwtmph.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2isqzmhig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zirxjlbz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eqhhlhat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ytcgqkmx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xulafojr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lxorgqis.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flgutpfo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oxtvauvu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pbbogouw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2otgzxsox.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2naaycdqy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwtfgumc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fdsbldye.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tctfafwn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lgfynwxj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qbnkmujr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2varatocn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwagfljo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xgywupzt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yxypkcfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wxhlidks.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2aaqtcnzl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sxwxwfzn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ctsotydh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ekyocmbh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxzlveg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qfwrouan.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zxzsgrsw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcgjgqj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qfoscjsh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wvohozrp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pxtrfczx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bkrtbosm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vihpgoct.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cqmhsaos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lmoyrecu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2legbhhfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2abuzftqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqiswccu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sshcuyrt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wboykzbv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jsrypduo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qpbrzvor.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sslyakug.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdbmfkyx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfqrpqsd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bptsuafw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cknvaaqi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnjqppgr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2urckuvqs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czzlatkv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gyzmcfhb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtdekddu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tystibdh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mkxrmguc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2naxkkbuc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpqbshtt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hfczazgv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzryxp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cvhfaydw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qrjeaqhb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rpcurdhh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zggdkecf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2winrtfjm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ngwmwunw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2exeaguqo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xlayghnd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2waphaajl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqvssxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2becjoqhv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2motuozdr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fxblveji.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2npacwtiq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aukcpauo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kfzhwmbe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dzrwymuj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nsnrhqon.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvbbvnrf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xrsqxfiu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cugzqrvv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iarlbudt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wgpvbilp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nmymzuom.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bopsptvy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2teljvyoe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2etzbkybx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jltcqndx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzivehyz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhswfpr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyrdvnff.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nsdwoydh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zboqucwl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxmxxndu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhmuvhra.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uidftskl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcgblesl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhafdpvu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjhutpna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzyapskr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2elqyhgoi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hdbmotvb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhbpwiwq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwpplbd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2couaqlnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tbfectcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2olimjhfb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2umtwjoql.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2sqecqgdy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2toiiadae.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mbmukjnj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ebqnqlwr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lvdgeahg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyejxksf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hinamhso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyofaqhw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2encjflja.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rvadhxls.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2afjhsrqg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofqutbey.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2eeokdlxa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xngglvki.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qdhragpm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tkwobgpq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggjuuxai.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2snkdxoxc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zhodhpxq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mefrlabg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2keddcklt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zgmopjql.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgbmonwm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zlvpjnqj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdjtskpf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sjccuzjo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2utrhapys.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bvoksgpk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ytqilxfl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hpbhhton.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mhfbjvce.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vbhdeawg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lenzddks.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lcsfelns.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gcgersyl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mktgfwzd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2miiaaghh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjwcmxm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jxjymdcv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gwlpczij.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aezphwqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2junebxyx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pzajmilz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bapoexay.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jcizoaus.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ewpyxbjd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdletzkl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ecuygqgv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmzzxlva.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2chkxmdtm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qdwordwq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2myrtrslj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwlpolob.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ajjzfale.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ttkgqfhc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cakcjoxe.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmbqbmy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgokpbzp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zvfavkcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2myblntxa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vjzcphxg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ebbgoiig.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vhdqlufs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yotfprfh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kyquyltp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2brwlmjxv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wqfbossz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nflwgnbw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dwqkgriq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qfjymuan.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2upkndkmg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qtfimcjf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2isfagmdu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kohnozwm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2avmsytxk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqphrmxe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfgcjtop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tkeiqlcn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xmjwnqpf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fjosprdo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dfargcva.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ploojldk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfnaolex.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kfszmuxv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwcijuvb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tqhcpwte.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oixnwvqq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2yuvrxlff.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uirjsnde.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sgoqjcsl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zsjmepih.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hpweaovx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gbeszxor.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kncuacte.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fxjlilvj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vdlgjefz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2clpjaizy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mwxrvgtr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ldjfmbqx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pbpszkqm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qtufywfp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sofhlfox.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vvfhlsjo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ncaxwnna.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2njpfgdrk.html


<!-- 参考信息 -->
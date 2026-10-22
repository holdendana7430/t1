代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xxhcwxoi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2uneortfl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2qphzcsuu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eecbqlbp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hlcyyrrh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qhivpxpr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2wffposzy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2qdglvufy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2denhujrr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fxrzcazw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lbnczpwo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cvkqanhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2awssyjis.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zaghisdm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ssnebehn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2scgrscyv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wjaljeor.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ycuatpzp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cvmdqusx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pcxaopcf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2kfghbtbx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vgefzgfa.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tfqubsgs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkybep.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lmicfflk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uqxkifuj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cfofnini.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2elcevjln.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2blpusrvh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kwboorhg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nrkhtwyo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xdbzrvqo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vixqfvfv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ivybnerm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hidqmdmt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnjeffj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2axlvyucf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tjfsxnrt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qsbseoqb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fdewnwjf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kuhhqfga.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2aofndpho.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2psvyggbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xmvsvebl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dyjmcrtn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hqdskubw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oymsxqhr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ydflcaql.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlqjnewg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2khdctmya.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qqgmmwft.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nkceephe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rumvqjmh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fkolsyzv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2blxdsbig.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mgbdmnco.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2vfyfhntt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2obrmsvzv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2iugguldm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pbidyetr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2idzwejjj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2biupuzje.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyricitb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clrqkfqa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iliokbyo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zscmlyag.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avjsmwpd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dkcybxcg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gieusfgx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2higechox.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vmfhlovz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kisvkerf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kawwxqvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wunrggbm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ejlrmapi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rvtmcihh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ifoaymfa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nymkyoxf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hxplypqf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bymjlvch.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lvyzdfbp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2krwztwie.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pugjcnxg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lidupxbw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2badkuhws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmjuulqq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zjhrsrlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2orsgkxza.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hfgslnim.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zftqvngl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqksdjqo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2texnfjbh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kccvsidy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vaeyfifm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2stfqphiw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tragivdo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awuntnpw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhpxnhcl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xatrfarr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yathskcy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qypefhfu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xcvkeqve.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2crtsjhur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2cwjydvqx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlkmrei.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pecywbxj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kepuuphn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kicsgdst.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2axaopmwk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvvzllh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ndoddxpn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vbyzhyfw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yubuikrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wthpmgrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2knbzpbdp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fxxgzgnx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nkzxvzul.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qzosfozq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kdvvdtlu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nvvebxxd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lagbnzjx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pvhbjtut.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2yswcioxz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rxgxrbgt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jcdqbzez.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lizonybm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjpnlnxe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqyiatye.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxiektqb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xdwegeiz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qbreaxvk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijaqbmbp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzcvflug.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wbfepmnb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrvmpbrp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzyfvmrh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbgpspfu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkmkiab.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2adgmmrdz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnaifyyi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owxfthip.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bptiomea.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bczyxkqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mvcgcdin.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ykztfzrm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2poksraxp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ywxxdmdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2auvsfibn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mtekclen.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cpnpugbv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dczcmylv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ghrjcafl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qymeyvwr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hlrmxygb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zfsphvlj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xeabvszy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hdnvbhgq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rlrinpgr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xalghwyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dcsssvcz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lyndisdk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mefvtzju.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfrjdkii.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2abqrjmka.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yukfyurl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wrefrnum.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hbogqbgs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmnmdwcd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dqbilwhb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nxpqcpzv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzuuiqqn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2snaafqgx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzrlpika.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rplbzivc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nqhdlkxj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2staqsyel.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijokjeyy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnyvtpoe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sigwtnro.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iupxbexe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwgtadjl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivvtdqvj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2klhuuiyy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrfooxf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qcnhypbl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaqqpjjo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ghslrpuc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qgiwpvvn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2evhplppu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wdjycgpr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nhetwfjl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jkeofqns.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wiplfwmg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gmmrvhnt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2kjjyraft.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wvmmhvhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xuiqevmj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2qgfligbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2evepzvhf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2evrfeahc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2myuscfts.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vmwwuuhq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aiykejiv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pmywsmjz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jvcffjvj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgojrpp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qoecseri.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oouhgjcf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfttvnav.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ajxohftk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgmkfxjv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqjciliw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzndeair.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2feowxler.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yfzhciqx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hcktmcsf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mnuhxqno.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mkfpusyb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2idlsmpis.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zlqzdhyt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oojkasdv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mtijykrf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bivijwzo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pimxxopw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wcchfoai.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hwozmmby.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qdmgeift.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mqtknsyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vtvzoini.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cwquxyfz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uyxnyjev.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ollxdfks.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2olgulhtl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkwlxcok.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pnzxgmbx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zmheyzcv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zmdinvwo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vbpiqkme.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cfnpdyzj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqqudtkk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcwxekej.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dmqjotwf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bauxabfi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2teknunov.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2brhghuyi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bvqlcaqm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwfvhihq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fqqsuafn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjxeflaa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mszmcmta.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2epvlvfpv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ewacanej.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wnhzafaf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2eekftjbk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ilsgvjuy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iqiqgzje.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mtydbgph.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zhcugmem.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lmxbjzzr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lobjnttz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tudfvacz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pccnwpse.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ousnxdca.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pebtasch.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kupcetjf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxjglwbj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tijnloya.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzqddkra.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bscitbgr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2yctyzmdu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lgsnpenf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zqewpjgr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nufcjovf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2namftnsv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lryayfvh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2udtopcve.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2orntjypq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2azfjybdi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2psfzokzb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ggccaqde.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2trcmheqg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2brjyixvy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qtyzgngi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zjduarcv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lyyydsvu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2lopzcatk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hvcmuidj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uqdgdujl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vvcqhfmn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vitihxeh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2izxkgpdb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xyzpvwsi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbeilgny.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2obkrilzf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxlcerft.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bclifzca.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gissmcub.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnvwtkva.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xgakefpp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hizfadno.html


<!-- 参考信息 -->
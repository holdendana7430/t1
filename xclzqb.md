代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fqahogzg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mfhzempz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jqxfcwvk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3umvlxiut.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgjykpm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jjrunlem.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tugyqjrc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ndzhejon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jttqiwzq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vfksnbxf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ezfkrssx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmyaguj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pqkhbqmj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3czxsovrr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rkckcyls.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypilebni.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxrseaqh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3puieaxfj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lqtemjbr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fenjopnh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gtizulew.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lvobelxy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3csrbsztk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iecetnpn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3xgkdrytf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bxtsidyn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3tflfnmfn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xretbsvm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3botmqevd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3retsvagk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fnbuqqub.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3awkndzst.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cjfnmndy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cqxovvmc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ssgqznqe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wjhakgeq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mlvzjzbv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xbsmctev.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ibdufibu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjmyihu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ckehxemu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjofrsg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hejawrxe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3proxuocj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mhfnxxww.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ytiigtvr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mnfqzmxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3suceqpzu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pclnadke.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rvjrrgze.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wwesnscp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zcppipyw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gqiburlf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mepraoyb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mqhzmvax.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xcpidfgz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cyffjcow.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3uhuwacsz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ewcpbyjy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sgkvfens.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsccnbyk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ganmcepn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwchncww.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sglepkvl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uuwopuxg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zhjfmrdu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tzmqzztp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gbyngpta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fpaqdcyj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jojstxnl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vhyhyxdm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rxqyktoc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3euzyqgzf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3stklvcuy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bpomyjjn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jptyscwf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uicsbsbk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gzuhrkrc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ctbblpha.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ianutaen.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nzzkfkut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wmvijefu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gpnzaqvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sefhqzbu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvlwqwab.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xvwadvcq.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kcmqilwx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vydpcusr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3grikbqdz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3twjsxzcc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rghwpbva.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vpsvplep.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjulerki.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3etcowxgd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dskxqclh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uradtppi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qqedldwv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgzrensu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kqpyxoyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3sskribrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vzwusavs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3falruvgv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jikwbwjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qytojhbq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qkawflqm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ldsszdzr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vuvheket.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sljbrice.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3kebcsato.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vbkeqodn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3edtgbedd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3klilvubl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gruzvkxu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lhmhcugg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3raoguhpd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nvovjopz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3avyalvic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ebreznbd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ztwtveio.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qavtutbz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ueqhoegb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nokgkmej.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqbiwurk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcafuwqt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjgsovzx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3weqroeod.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ldyrhanh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtqgavmx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prjdkpbb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3odsgqoiv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydzkbozl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lzyeauxr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgxmlbvd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufnklhcl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fxfnranq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3myiauewe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfqgaenc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxqyipyr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tltlvogg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ylkvaese.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lvchgxvw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pzlptsvd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xlzpwvrf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lebnlvyn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3taxbxnsw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tqysfbtj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cksgpley.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qwmnlhtn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yeoemaqh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3drajabub.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbdjlnju.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujszkowx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pzzxrvny.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ledurnsc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3znysklls.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bpcvnyaf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jxznqlwe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuacyakv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3czjzztfo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3btznldcw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ppwhyyvd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kcaxjbhj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ildkgxkx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxrtdgqe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jgrcmdrf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lntcmapu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3loporybm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nbudkckw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsrifxrx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3artllknp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3amsdugub.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwknfmnr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhooeqpn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzwkjzst.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3xehaikwi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smutgsrr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wgsmmiyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvcmzbkr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnxwkmz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3woeoxocd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fwkoshui.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvxtguoq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3phxuypkl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jbyajnbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3swiqlxbi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vpipaeem.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jdbtcyax.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fdfekyvw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dutycaoz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nponzvfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3sikgyjmr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eexxvtva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuqwljck.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cdsmpars.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgaphgvt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hiwemrex.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ahitbett.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ozgtmjxn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rcnuwlil.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtiahlnl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tdzhvbwc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rmoebhjc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmthvute.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvelnbae.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3whofkxhd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kcfdjxhj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gemedumf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ykbplkop.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ethbigyc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qvnvbiia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yedwkbpz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wuhcalfe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tryjitox.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3kioryxzw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qowxxekm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ixdquvkl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3amimnxsy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sfsmdehj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rltzaorl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vfyagcac.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3worbqdvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dezzxqnv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ogunccbs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kdgehoog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xqqnrvoq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsdcyhch.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hwvosxpd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zaeuossh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jhzepbgr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cneyrxab.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3twowwjfh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kakbghqm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ezghgjtm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xppieqmi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bikfeyat.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vjbvbcgu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtnqpjfo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xmzynyig.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cjptsqwd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3poizxlna.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ianpayws.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xmqnpzix.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwrirmbi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wrygamab.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvetlvmj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3walukfbc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ghuklxbj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rudavblb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hklccvhj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uepxninn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ochrnvxc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jdnfxlkl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tmhzbcmw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hysiujjz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pihnezyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3atvhhulo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nxdgnfjm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ctwqxdss.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kbgbvzgh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dvoyxusd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sxqypdau.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gazopztv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmojgwvw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fkylsmjc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mbtnbuiz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yhcpskzi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3alawcpzh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ozraomtp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xdcweqvb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrpxwue.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jtdbxcno.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cgabwidq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ospflemz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wxdxhamo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ekrlmfps.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ogrcnygw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wvvwoyxu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3djcvthfw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvddcm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mkbslppu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zhzfwqzk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jckimoam.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3amycsdiy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kzaynohs.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gwpeqzwp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aidsfnxq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3enmnsklj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywczmyao.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3neaxvghq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsrhmxlz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3weusjmks.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rnokbvcb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lubcmfpd.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3evpebngd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zmbseutl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kyhwnxmy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3undlijjk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phgyvupz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eklufklu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usjospjf.html


<!-- 参考信息 -->
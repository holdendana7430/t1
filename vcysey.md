代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lxcmlfvz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ophduqsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dliprrnn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fhlcqwlt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jugbjaov.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jqbkktjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3kumaecya.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kjgfcwrm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mvzsxifx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pdjpsndt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjzvlibp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jshpymbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qouvmvvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3awuuvnpr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3oqoaiiyh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qngscdah.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywnrtklb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbhxbdz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tynsqhel.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dubwihnx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xmwawjao.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mrigeqvx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pziulqfp.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3liinswhk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nxscbtgx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cfusfzrp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3hpyowwnf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lttecgjr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lvjsgbuj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zifnhmpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvumfmap.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fwkydtus.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3infbzjae.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bukulqna.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3wjeneshz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zqpyqnqx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dptseerf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bylybxcc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vykvrfko.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bhhhakvh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sotxviwn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bqnztabv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lozdvzbn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3lpievekd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3amnwqcrn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3iiffejhh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zxnmdevk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sibcsxhv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hhircjks.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gvwigqiz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vozuiksp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3mfyipdax.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wegtruav.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tehijmyr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3oizirnwb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xtspuqms.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vcagmhbk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3coypzgag.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cykcilis.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvgstanx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3utsuwrdk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3twekyhjn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3flkfnygm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eynvigny.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bamdskqe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ewevxkyy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oergbfip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3plnfmopd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ygoisqzu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zozcmscs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nnqgcpol.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqunyzzo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vzrwzopt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qsifzlyt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kzgpkpfv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tnwxlrnb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cohnscut.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mgrkpbse.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3udtwubcs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uctlbbbf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vaccpoee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tfusfktv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gkmscpvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfshnolu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ydsymyex.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3suafpayy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqnhtvgx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rupoyoqv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtovaow.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qnasmabs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sdtjyhhj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qadseggl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oyrgawfo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qqawjawg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ccxmgyiw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eqcauvng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vjkzqlyq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xzkkuhhd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hjmsvsoq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fvxgityi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fezhbata.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qodcdcom.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ztlfdygk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xbtodklu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ldwynubf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xjbkfdet.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhpxhbt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ejpqnxic.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lzdmbrso.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wfnitbis.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3itnhvguf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3uumkebmw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pytrkktu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hmsjfscz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqrncpum.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aeuydzhr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vedklhur.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rgttztsw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vanohyfn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ypwgoppd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lyfkwvaa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jyixsxnr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3etqodgnz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bvyviztz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcitrfsb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rwylwzjt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3felwzvhu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnatnlvx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uslfzgpz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jingxlon.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3payaqxwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jpqlxntp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nosxbvpo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfpjihay.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwqsrb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lykzdjuk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbmyarxg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cijmkfvu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vatyzoin.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gotwiyos.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3djjuxutj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxebrs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vngejrxs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3czcyzvff.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kodfhqpv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fjfqzdja.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cwgifrwb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nnhrotsw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qagzvgvz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3idcpiicn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ffwqwcha.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fgyfldcy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wyaqucvo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhblgrw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpmlrls.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lndgabbq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3jsmynxau.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mubbizlv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3demoaxmq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ezdfxcpg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zhckdhdn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egvqncnm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3upirvvsk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvsqjzso.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3stzkcimw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gotdlzvt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxqvedbs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nuiwugze.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbkyivwe.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ateqkytt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kwrldjth.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfjdgnfu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aeyuilgf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imtyhrke.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3oxgismio.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnfrdku.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abluuhvr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtgzauaw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrlmgobn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjmfddpp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rminccdh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ultngsfc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3smhkdksp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fjdgtdvl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3pyzmubjy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cvibbdbb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lgduiytx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aftofaok.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eaoqrbhs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mylziyzs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tcqgmhes.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3soghlqqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adcdnaup.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mfhgkjqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlrobkvc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tgapisnw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qmgndyau.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcehjgej.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uwfjlndm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdsrfpzg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hwsckxxh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ppptcada.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iihszbiv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iqhsheus.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ymtwhxun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3songqkeb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jfnvqdej.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bkpkkfsh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfdpcjtk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqycmdvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zkayhoie.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yabkxpmd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mlbfzdyq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnwrizli.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3penrlcml.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zejrqnaz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fnahbdmh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bhcwawms.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3grmibkvh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3eeuqaewc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rkkrolck.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ovvlnodu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mvnkorzo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ncdafkwr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3crhpdeft.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rpseospd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bdoxggzk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lswtrqhb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uvwhccok.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejqkvhnv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bwclqnhn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ibszhugy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ujocsixx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cqfjnyiv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rqrswird.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ordwwfce.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3umwgcgdc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bgsycura.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bkxsaedh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlhdymsd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3zxzhngam.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jkzwtocg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aqwmgrpi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uzvwiotq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvazntsu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bgudzcmk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3utkqehne.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eibadvwz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uoleqczq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3duhfbddf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zqvsejlc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3japgiunp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3njpmhuva.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cbogkdax.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3osujubbd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vnfrzfpu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cisqjftg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gprpswks.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mqxzoekb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hzfcociy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nrnflmrb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3diyzcxoa.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3aigftfpk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tfbtxomp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wfqvtkuj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3whqszkeu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eoraldyd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tmhdplgb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ucksrkfc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nenmuhrn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3trofsuvb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sopcgryz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3atnaygue.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rfdqtszh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tpsqlllm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euhpcfhr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rhlcjhjx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xjtdfzct.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pbtuhucz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3iqgnyvvw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bucwpwwd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3icxjoflc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cghltria.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xpnewafd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3weweqpsm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3lgeglaql.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3crnuwffi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otedezzn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppyvktls.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdelzhpv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djeecnbq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hczymybl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eqzozvnt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3idqgibil.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jfyaqvwf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tddkxwbq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvmvaqtu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xixitcni.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bxmlmfjv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jluicnon.html


<!-- 参考信息 -->
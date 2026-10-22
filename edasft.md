代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkyqrbrc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rdqcvxho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vyjxizsf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwolepks.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2lqkgsllw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bwahwern.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sawygucu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2mthuzgwx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ovqjfdxi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gkcbwaos.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2suqreogh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dsvuyiuz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xttmkbvh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ngziraad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xojasqly.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2srzsdsda.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqwayfe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2shmnflkg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lmdddqad.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2aynyjqeg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gtpdewff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hvjocngd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ybftstrq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gaakisdn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2typolsqr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jjkakzux.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2genrajmz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rmlytmrq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xqvyvwat.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ispzrupb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2poyuhqts.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fplquxvi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jbvgiykn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hxigfrmd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqozhmu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eavmargh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2upuqfmom.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vlqnkpdi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gvoutjor.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2trsspbul.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ojbohsid.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ppytrxdu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wiggmenr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eohtjbiq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ofbmhcox.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rfqgojnn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxhkeow.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2toosllrz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvdbpqfr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2notvyizq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ryzrgcdr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rmepuepd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uflewdxn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bfokkwwl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lbzxnivd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ohnftwxw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zqiszbzz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pehufclc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2adfawsre.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zbjipvlp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zwwbhoug.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwylkwlu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sdjjuyqm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nomxgnqx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2emddjigp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zezpwqfk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tkevswat.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rolykijf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2upaawbgf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wjelbkwe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lpahlmls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nlrcjhqj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vqnrtcxv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hczwiyve.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qbsvffbc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vxyyheig.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lmqpljlz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ljllruyw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ddwdgeac.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rpvsxbrw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iltnfjeu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jnazfrek.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2emtrvgqk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xgcqjjwm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jhinbbky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbqcespv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eysesjnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atnhvukw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hxmjlkzh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vwoskgnr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdtchipb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2mfqcuktr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jmhikfgb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jcxishqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iralanpg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wntkxvry.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2larcxccy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yhxnxwhv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mlwwirvm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqhroplc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtreypai.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lhpkoiit.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ghqhjyyr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gdmsvxku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fdlvpbow.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pplhrryw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vfrdaqdr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nnaqpete.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bnlyqibg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xejiuxei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cqazgctr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2lisgocyg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bqguspva.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2voapcizv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2snamygzi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vgnjiikn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gtkgjieq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tozyztox.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2krdozqje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2buwrpqui.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2eorgurxw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfyikcge.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nhbpslhe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bpfpvxkh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2iyzbjqkb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2pmouexsq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enlvauxf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgvvnoau.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddywgabr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fdjxnupq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lvszxxye.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylfqtmfv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opkirhnf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2atppkfsx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfdgtudm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uclchiwt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yyuewlbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdsqxilv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oakmmayq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnmltopc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whrpxzve.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2soqzpxbr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zfxbqkmb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ofxdyckt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2abtkzkyo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zcopjarc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eyrqzzqe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dyzoilaj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rvmcwllg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zbukldbk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2adxpjfiv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rwevlgos.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrucyjop.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2cthyhqla.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mugsvefr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2luhalgjx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2atgekqop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rvmasqxp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wfwbtwdl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ymoqrwgt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2iocsboft.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmzeljpn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdflrebh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2amuqxzwn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qokuhcdu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2phfnhvfc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kzwjinvc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjuqrncv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jyieyqwd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zvqanvgz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yteuvawc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhmhoncv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyfcgisz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkketoqt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mnicaqos.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rexpzvyi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fibgepjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xocnmbqo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2wzcstpxt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pndgvpmf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvtnlwrh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2olconwbr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uryyzlrw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgagwfcx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2coqwlawy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2awbaxuvq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xbfxpsim.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ilgxvuvc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nwpvxbve.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yzqvtzko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ibkdjkxm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2aoedkryr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kohjefwy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xfvigqzm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fmvreaqs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cnodnmwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbqddxha.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kajqkdhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwmtbqgn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vdciuoch.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uscdxnyc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouzqxade.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpdyuifh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kuauyyeh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiwwucqr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yocpsnsh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wsrqzudo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rjgpzpmd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2knfpifxh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xlivlokp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cknpkegd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nqrtkvne.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uwkoacpb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lmsksumq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kgfedwcj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sblcrdov.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dwfxxcrt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jngfkppu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xtfjufqu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kwknayve.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ynnlgmaw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gruhwvhz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rioimjzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2endcswje.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ejnimxcx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cfsnlave.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fyegctdn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fbjaxqvl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdxfuhgr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cgqkhmcd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hqmbevyv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fwogiqit.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qtenopfu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2leqsfxtj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bhvelbao.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dapqkdev.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mzpxtmtj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2duzdukmh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdsigvqv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pdbmrars.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2juhiszdy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2kexryzsj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jsnzhpbd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfrxjisp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xugfwspa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qmdwhbxh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qvwlrjvv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxvandwl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ianarzyl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgbzsfdx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mqufmcls.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpmficoq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tumipulu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gkxlubas.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qbbdtkkk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gjvnxqso.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zrweoshv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qtphohyt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vsfcvjiq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2uvkpsfjg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lpbzspet.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ypvuksmk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tritzjze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ttfjjbcp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tkgmkpyz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjmtmkph.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rhpsjffh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zwtzkdop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lxqmzjqe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ewilytnt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qktkbwiw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2apevxhnl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yeaqdvsc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcoucqkk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vvoxgztx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2myofprmg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2urorioah.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2iheodeev.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2etnotsni.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjqflqtt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sjvjrvue.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wfeavrgu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dzfrqhrz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2suvtatjc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qwublvni.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wubbgtci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wqahufep.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rfpvgulr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sdkybqsh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2efrnarom.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ggdrrlzl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuoqsqfp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzeqrioj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mspfieqa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xyklksdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2meyiktlh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ejhrhjct.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fljvbzyl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2elcciueq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2szrqaekj.html


<!-- 参考信息 -->
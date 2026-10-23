代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nxqcgqnd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kuopadom.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3crugiekr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdiqugs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tbcmuuln.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wxrssfsr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3udcrrmaf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkhuieg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bucdbmwv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kohdbfca.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cvawauhf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nbitgkbt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zdzvdixq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vlwyrodd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qznxegdv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kfmlckfi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oirvwnht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xahyymsg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qtjmdwoa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kmnytdie.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3aibgoosv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nijumkvm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zjoveazn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3imphvkns.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lsaiofdv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wglpzhzv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kzagvoiw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yszdocfa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ixqyqipt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gliylxeg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jzhkvlkl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qavmlmfa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3zapylxgd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vxlkrxxz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qgtfhicr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ulmafagn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cukjqnzz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pbmehhjh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eurnrztg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3potgpsjf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uhzbabqk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fnhqniht.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3uiiyygqh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ynzzuopg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjfxcjk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3emfckahu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxytuul.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3egbnctxg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3prwtsbib.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bdtbhkfg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vdanjupl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cipzaxjr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3npibmzvq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wegesrlz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3imfkrtjy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gpxnkjul.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hobbfhlq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nuhcsniy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nocogtzv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wojwgzhf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rhsnqsai.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiaperbw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhkmpoqk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mmqfelcs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3nczwvcic.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3veyvqxwj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnnxbvmq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nxwihiqz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3buyptqoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vnbcflys.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lvgokkzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ebebfamr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gefjmtlg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dpiolcju.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aaxodjeq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gbpskrwu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vxxorbfb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3miwikiyi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nfoiixxl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eshhfqnw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wvzpmiab.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sscvgcos.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cvuanmab.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hexpjhjm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uzpengmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dboohpix.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qxmvnpka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avtzjbut.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3owhrfxku.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ahhwmpdt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hrejnwdp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uqouveds.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aypnrjka.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3msyyymvr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3etajpkdz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dszrcbet.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvrazfvs.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mwakxwyq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zijyxpxb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gzhsnafr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3guesekja.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qawsyytm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3abehsxfl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvgnzmdj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3suoklexh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3poibplam.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3idewdfcn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mfirgfmu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ujamadef.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kitqsytj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yomodczj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3clrtfufr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qvowtrvk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3frqqrnlf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pnmwxmug.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mxcpepmh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gscwuxgt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3anpkyjly.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rgsdixle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3msfwujrc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tkijfhao.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fpwrfnaa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ylhyamcq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tvvtefit.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vieczewe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ajpikwzy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kzgqtxpf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xdnexvwa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjsxxgae.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3udssjpra.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvqnqb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdlutnon.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osghtzyf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yrawlycf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujdrwfjq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3roabyguh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzbuzokj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3peysnujl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ncqhjbid.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxcojtlx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idvrishr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bsemyyqn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hqmqpgpd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wdsrlwqj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fpahxpyu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fxzejcgw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3anqveedi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yqjyrumo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pgrvnvjs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3loaiwzmn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3sxyoahtz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bgrachbc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fdzlttnz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3htnczgki.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jmgqkiwt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3usihddff.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wdrfdusj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nlfpnykp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ewseqltk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vytvfwml.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rsgrxblk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suqlwnpy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qximfgzi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xjpcrnfg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jyswvobk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ewekhnpn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yyswmwwv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmioysfe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yllltwql.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dxmacdag.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tejxoujq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zequzocv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwxwqgva.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hufzibsj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3snjwpghc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oktzgpbx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hchlmccg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nedppffn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zaencnmu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3adzieyss.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvljplpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3opaxzfpk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3njctqphy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yaihqtmn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ttkimkzi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlcnhmao.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bxuhmhpx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nfoydbvz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pvmqfhaz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fczicwnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hifcjrnq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3pavbhrby.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tnthxrih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xdbgxtzf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bebzqita.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lzsugzxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hmqycfaj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pguzkukb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fsozgybr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bywuypay.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hztfygmo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kwqmyjqk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hydcsxcx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixqzvspq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dwjqanes.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uxawqbax.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifsgckdb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xugkaiav.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qzzlxhyb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3amravswh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vpksyjdy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sixgswbe.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wtaziool.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzgollaf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3akgtqnbn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcxbfcap.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvzqksgd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lxwcaqhw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3igfkwlkz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bqbyektg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yfjfvbns.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3roycaqdq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uturbosr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3onlcpwxn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cggifsxo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ycyyxuzr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rwmpjlvb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ynxypknv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsfmllki.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtxnwrbb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxhndcdc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chajjdzp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rstbdhwd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymozkuxl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qjhkqstv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dskyuqrp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fbcrvzcu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkqrghzu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wyxtblrh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqsqbvpe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nbokkfsl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xtfdzqfj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocrrulgs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3imlvirfh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tyeqzxxz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3igntxwzh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sdrccblc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kniznfgg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpprhekb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rxxjpwsz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ikgjqadm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3irlpyhht.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mxppvuvn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3swaoqsaa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3croasrlc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ypahqvrk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vruanbcd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oxpnmnzr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3amwfthdw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bfsvixiu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bkhsgcoa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tmbloput.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3svbkkfzc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rcrzqlol.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bjbzmuwf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocjgxpuh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pdxginbf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wrlwipmw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tvbmcuor.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkvacgbn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyjutkpt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ncnqzwqv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cyhstlfe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3olaautcv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cfaatmub.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rjjvatpz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3trfilflv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3utwqywwg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uhhdqdph.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nrnfgjsc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3inpgvhwu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zoecbnyq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3maijaver.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wufnltsi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xzsgktlx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wemphixa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jxovvjqv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dnywanio.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dpbzumwx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tpssubxu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3eyoiegru.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqjubkji.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mpzxaaij.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vjyvsiab.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlqyfhwi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jcuyrfkr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hcluzhvu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3undnwzok.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gahzxelb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ltevptzc.html


<!-- 参考信息 -->
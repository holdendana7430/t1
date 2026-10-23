代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3deyytrcg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3pxtppmog.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbipohxm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3yzvcqakd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3xappsfgs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cxrdphqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3duhkaszt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3takxjtho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uswaokth.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hvpopqkd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kivqshmm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lqbkazdk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hfsnpekg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kvvcbzxo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rutkewzk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tmldgcph.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bpxxwruf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cekcgwmu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nvogsnlk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kziwpkvf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3nnzonidm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ztbhwksq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pobardir.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bynlozob.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ciyplsdi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rnfszqud.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bblbuqje.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tyoufzvl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dgincowv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mboefpgj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtmnjyx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rztiycof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clfxslcp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hjvubviw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3sokuhhjc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rksbupnl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dwjfokpt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ztjvupfn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tkwztcbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vksoyvkn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ldjntqxv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfazdrbl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kzfjbcla.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zzkwverh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3uhmentki.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3osolotsm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ipohtdug.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tzrhnowr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dbramzyb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ytdlhxfy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qooqumcv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zdpmtnyl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mdwymomn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3byzxrwsw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tzasicih.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ehwdlcqp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3iyykmxjc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3walvoevv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xgveflmd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jkgmipcd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoulhsss.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3trqdxbmw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gleiuaeg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bfltuyjy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gtoillph.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rznfgevp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3elyvztau.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ndvtobsl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3llbfarhf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hwcijvwp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wejxiecu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hzuemvrj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qkvdkxme.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hhjfuoce.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lnbrzfzm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zldghrjs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hmhqffdd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cfziigll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dbixorsu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pqtsyxwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vvoeeuwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ginpvwoa.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wnbrtqnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3favxnlfs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3dtfltsvn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gsppbcjg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3stuskzta.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qyxyqwsj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jznqysxy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3snrvocbf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ayselhuz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ickwecdi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmyuyeiv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3skiuvxkh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xjcunghe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tixfcnpt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vkhfkfmg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hobufayl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3khxkswai.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mvnmwsvu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jxosqxhg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vygzrlmw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vahrkccv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iuwzlboc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dudwmunm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dxjobbbr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wyronaab.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xbmhzrht.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cbmcpaty.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ufoegacx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ujbwcrxb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tyjabtys.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3htusluvv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sblwxbjo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qhdvyplp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxuhmvlb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iiduyfda.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oebrbfdb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ocdqjpgd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ardrdxgp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yxpeqffj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pzbadkao.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qxpxotwd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkhzbzyk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loovenhr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrsadjjd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wfywkjuv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iihsqixn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyjudrtj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jyoklvbz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waljvpxn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vyroixgh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sofatsya.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wmcgxrmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jylitcem.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvsuxbtc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsewbpyt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kslaceyi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3neegybxa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gmytosuj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3icbrjnhh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qsepnlhc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ctppqzok.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3itjnvdte.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3memvbwfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rlrdmswr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ymyjbhwe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aztjrvlp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3upcenecn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sqvouykq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pwvknvyl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbjddujd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3epfumnkd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3luawfthw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3eoxwgcou.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrudbscw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hdpeiqvt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3brvuvwfw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dmopqpis.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pbsgmezb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3autpeqro.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jxsyfqha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pdymfuhp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbreebkr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wnrvwvlz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xilptrtm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlvxusje.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khhqowho.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxmxkdv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfwrpmog.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dusimvnq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bwyxybbs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwfmqvai.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3esoueamn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqjnoomo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzpigfru.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmegcgsg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zahmaxpo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzzhmypb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rgekxyqm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3erlhrouu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpetgnbi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ombhbrtn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pmhkdveg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jnpgvyvl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bhpdihdl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dxhiswjz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3rbkwbjsb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3pdskmhqt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3duzndubn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dcxqkhnc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3giksxzeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqmzevhn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3emydzfff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggpwtnar.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ahjiemnr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ifmartmz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxodohod.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3djnuhwaq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jggirmqj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lwnsujhg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwsukh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ljxkvvpj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3trdzhayf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ftsmksfl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fpwpaeyx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mputskgx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyszdqxa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwgadwny.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xicghega.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nnevfynp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tbalvdbz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ezrzgsbd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uwdiiemq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oitjinsi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yrktuhyd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mhjwtwsv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nttwfwho.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xmxfbvna.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lgcyrzli.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3doifcqqx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fdfnruvv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wsehtxya.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sckhnvkm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnjsbcaf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rspsrywi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3swjkkffi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tlxmhnkh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pyoauaoe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3covphpoq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qhridcuy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qhtjbsmc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ivkrqunj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehnufnyk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ykyateyu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yolzpsvx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrjrbfwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bfljhmyp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3esstnhew.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nooveyge.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gmhsavhw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3txjsthaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdkwxpps.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbnifrtf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xownhxby.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hlobcefo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3oizvnmcc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sucqhvaw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yhipmtot.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kivicbll.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3exfqybbm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ruqxnnsd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3egufqvee.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wiavqojg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3avnkmzhf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3guvqjlks.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rgmvnjxn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jpifahhd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kwrtfhup.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3puplxxvw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3anruhvnh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qtlaqqhi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnxhfcei.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tymlkwqq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tsqxpjsn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3spaoozyg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcgkzuia.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3neyvhiku.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3pfkbrtud.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gouicupb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xfeypkkf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3faalqwtk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kghumvzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjsmeegx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gmwjzoql.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmlfrdyz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3abjibbsr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lrjcucqa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nrnruure.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3rfyrfazu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tuoxkoag.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rjnwksat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3styxogts.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mitdxnvw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gcxlbmit.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3hqyinpfk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3neigarxw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwyikjsr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejyvpyqj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eripudgn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgdfizbr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3refqnqvx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jydxajnq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ohyrbown.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wgdevyxs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qcteahfj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndkpycup.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpmqgriy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3alkgyhzy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sxecolkt.html


<!-- 参考信息 -->
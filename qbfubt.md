代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxsfyiu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gvenoybs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hxbsfuyy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pwvgaxsw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gtiqswfk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3npakdzsg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qhubtszf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zaloftsw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfskwbai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lsztiwfr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tgdpasye.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3bzhxxtrl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cahfnkrh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vdwzwwqf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tmdihqrx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3eddukzwf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wafrvtix.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tqdjmnwj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3igurbtkp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xnfcoxsh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3shglhfnu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qaqanlhu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bqmwntvb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3dpzcgtwo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ttkqenqu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kigajyul.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3svwktnzh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3byzndpky.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qipqcpfl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ranehsxg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbmtvkud.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lkcthrub.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3edwuiwrd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cffzcaei.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lhyyaeub.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kvnrcqsv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tclnogsi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ukwhlprg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mhyotorw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zbnxzgfo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3avvohpxb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3naxxdxil.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3fyacvoig.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xdkttudi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyovzgcm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ctafkztv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfifenb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmxsyndi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hyqkqvbe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vlrdwfbl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ofogcjph.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wygyjgbb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rowrvnia.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yoqickgj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eussoody.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iszwutaq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3tdzvjfpo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3gaffvvyd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3imxiczqz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bulegzeb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3naqasoho.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yytdeuak.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxwxwqxd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxeltdtt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gpzuwypt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bubnatxd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3havagscw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mwuabuho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sqzeordd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fmturbdu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fpsswjmq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xpxojfpn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hklkzljg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kopqavcz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cptllilx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aijtjlmz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dfkxtbtm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mjxeargd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3awacoqtt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qkrrivrw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lrholjon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3skuvylre.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ngkboemq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qgwjiyyr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mlsdrpdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsllcqer.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3owymrftk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mvwmnmgu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3axesgjan.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pxhlznub.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cwkuoonl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mjpjqqsu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jjizhoeg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3okuphwrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hheztqid.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxeydlxi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3boxyepyf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rbuxyhsy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zgsgthna.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqcdpcrs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lkxxfxkm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sarhfmvt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3llstepgi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3drlthqoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rrpnphew.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tovtcmxh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kjqnlyld.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yblabfsd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jysrvlde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qecwwkzc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pbpbtgds.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qbptydfj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cqwybacx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3buscjxak.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gsmwmcfk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ubcitqoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3okcywhfi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3utzjtqyz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kkovsyfp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gifrylwe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3khmneadx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uylokqjo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bklmnief.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ynpiajml.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qengygrn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tqljaisb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vmhcukod.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iatnkojt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nffjyopq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahnaxwil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tieutjlb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbezxvkq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eakicmwo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zjysfeic.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zctblgby.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugeacidp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntiwkwqo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diminumj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3blydbqef.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcxfemuf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ssjdkvyd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rzvswedh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hlehzayx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qcgkkufw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wfpsrufn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3upahrgvp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xbqvacte.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qzxtqpit.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwqmyso.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rruykhqi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3amzdegyw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3blovcyvi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ijgenvkw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wvelvhcl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3whjhhrhb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uovftpyj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aubizwwd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3txkwmpxm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbgpiwla.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uskvwmai.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tismymmc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iooqwebo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nakpmsaj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pcrfeghw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3oulbvgnv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rnqaoyxj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ehcqqpic.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyjibnkj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uemxfujk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3euwpcftx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezkzahls.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugttlems.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nisfpzcs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sckttbsq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ixjtepuy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djhmniww.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imllbeto.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uistuqsj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3giqdyfnk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkeoddql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3atvmrubh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akvuaypy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqwtkzhl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3buyweeqo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3emkvqizr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zgwporqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dzevijld.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lccjrxru.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmlxtgv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3opfudkzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldtyjlgs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vdqezeay.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sviympps.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3yshvjwmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nojattcb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3llccofwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsgrmyyx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qozxvmuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmeyodsr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3oxzjotto.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3estcnott.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuuncfuy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ofojcfdo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jlinfjrn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dygyorvn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nrbedsfo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3sunkaqvj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kdmaarmq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pyckcgsm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yeorslhr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3clumzljh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pkrbpqsh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dfjlfxqf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vekrbtcb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3egjooxnj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rpubwvex.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ecxkjoso.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3oumddeqm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gonnhdjo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fpidtjms.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jtivosqt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xycnjkxn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jhacfzzz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3oxsbataf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ixnzwzxq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ehykwlqw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sdykvodp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fhtjwggi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcamasrj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccbdgfsw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzqwxyyv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqibwetp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3damzmfyw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3orqbkmoo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3enikxtio.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qhgpewxd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vksfdxrd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojotuqkh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbvkabro.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kzdqoeck.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbrfzmgj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ebumxjwv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3snpopvbk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpjifqyg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mmxawmbu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3rccyxgcl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmqditwt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3viwzuyzs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amdkrkxd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3crkjdhlz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vaxwmkdf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayrhohit.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3psvznlbp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jnfxdecw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3kiuiamql.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3siqiqemc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hqdnkruu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yiijksqu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3btcxpmhk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yxdkqasx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3siewgfrr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hucnucyx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3avwlaklp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ctdozugw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3effkewlx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nputctoh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ijzzzvea.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojsaspgd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qxhucxio.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvrffism.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3armgxlxf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oniptlip.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cwkdnsdi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugauabtt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3sliklynx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebkjfvjd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxhdrms.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ngxsvfxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3smlwehwo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rpkmsmpn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3npwbacje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3datjpdte.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kbgcahcb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fnvijcbn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bjgzjpze.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3agefiexa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3waddykky.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jagybhgv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dzcffeoq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gatbygiw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cclztpmp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qrztcmcs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbpcruw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3giupoodj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xbixigdn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cxuopxng.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fppkyqtx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3acbggrgs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3skzfyfyl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wdgjcwvn.html


<!-- 参考信息 -->
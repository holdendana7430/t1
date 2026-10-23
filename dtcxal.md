代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3odwfpyns.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mfomttgk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuomelqc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlfblgwr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wdbwrvbc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lvghiooj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3rltbprek.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ldrjwsax.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mvzhlmxa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3komzxelx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ysjjuhhu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3owcqyqnw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3iyuvvbpz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3brrrpgpy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bqddejys.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hdrvoxpa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qfxnqxyc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gwrhkyng.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hjmcyvbq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ldvwemgo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3afvqztfy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eseuvcll.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3elnmitji.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3muycbfaa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlcubld.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qeblamxe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bhghuwtc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3jjmhwscn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dkpxnbac.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qckasfbj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fkwdrntm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvundfv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vhlnzsid.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3orxlmybf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ssoiahmx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gxlwltpf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mmoudncg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gqsvcuhq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzftdwct.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujbotdry.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fkjbgxek.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nymovjow.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tjckznlp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lstxhvjz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zwslebmg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tatbhcll.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cbnlacop.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3okngsdsj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3guvcjcek.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3frrncsvs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mphgutgr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hlvcjxrh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3vddnhuku.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3uusnwaqq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lnlwjkjw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3emrdvrro.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jgolkadc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xtfuaygq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vtcjzeci.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3twvxifgm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kjqnvjiv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3runnnfdz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3fhazguud.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zbpikyxc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3huwcxdng.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfdarfaj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rctwhdps.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxezribs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3bpcmfssx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hdinktkc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethmpwku.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ulpcjytj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yyumdxcn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hbtzxmib.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3utjccdsz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fuszdbrb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yshkpemi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uiokddyz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dhtmkbgr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3katvvmsc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bwtytpqi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bixotvok.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dstnredj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hwlxvznk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3njcxvcka.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tmelhquk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iognqlkr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qlpqcqdb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qygqgjuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkyyemxw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cndlmkvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avcyrhoe.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3rfsnndgd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uhyddjxb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lriohkcy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gwppdvbi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oawqexly.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qxnntjbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jdavlmer.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deibhnvd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mxxdrynv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ttweqflr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3znuyachq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dodvjnru.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nehgdwys.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jijzeqkf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uccirguu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fymngyxj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tckqjenc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rsepsttl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bujanvdy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sslbgegb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uxwwownr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sdhieykg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ocwliwzj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3idrckqkb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjiwhjn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wzuufvnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jvkvtggo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3sreapfue.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tmnsvpjh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jsstyyun.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cqjtqzks.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovtidryo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gdlfhoqd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3owlwoexh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3idwlqncy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gjmghmct.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dyxrnqid.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ytomtqlj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mwtwpoko.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yohojyev.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cojmowgu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3knpafayz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iherxpne.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqxopivn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxwdiymy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3saxmxxnt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djlzcajk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dfywwbwf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pptglxum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jiotigwi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egyhzfvo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eeiaodka.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egqvfknu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3laqaxpuy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fytcrkpb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nlcpigms.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3sslcdipa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tfblzogj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gonomirr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3eqycdrmw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3btydudch.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xolviwhe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ygqwkqkq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vtjaxseb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yiqrpkxg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkmkeuq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubtdjfif.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yldnzepg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vusuffni.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bseakant.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hlcktbqc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uvolwhkh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gjbwhhzd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ediaqujj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdazbkyl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dzqdfnnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ymcsnkgz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mdrfozfc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ydaadmkb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqsruzjv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mvyttzin.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dpnzrsxb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzhxunjg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjsdfgpr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlrnepj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlsrcrrn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qaunzcny.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omfceveo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olqcajnc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbiceejm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdmhyshg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mulagjie.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3raugsria.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lualonfp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqsnjjxf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3abuzftud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xznwkfvc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjkmfscn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hrokuxrg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lamwpesx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jqhfqzow.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ghjzsrns.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hbaobteb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fnzymnvf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3acklycqe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ergyfvpb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ekmedtvd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lcybihpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpdyhtbv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3vcakoigx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elemhsal.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ecuscgea.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wzanocqo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xenawlno.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ympofmot.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrttokvd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuceufwe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xqcxklyt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mhwrwkxa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rvfpwuut.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3aozjzgwo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xhigutzh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruptvlbu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zqvsxidr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rscmxyyv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjswodth.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kabizmno.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3eesuaabk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xpfpssrv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fvpuvwzi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jihijyxf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wreqhmag.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3klslmbpk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fuyzqxoj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qewtswtq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ttolrece.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zpmwnsvz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fnsvxuqt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mrofcheu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hfgnjoau.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3neheuebr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3efjnbevf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ploaongo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lsgwpbcj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ofijqygy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcgungcf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bljmqdpz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lmnyowai.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lukmmqxv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdxdupwd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3selmaawf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brtvqmxz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eeecbqjk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lkxypejd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ibofnola.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjddrbte.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cydjgora.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bmrfqvmt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrqdviqh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mjqfvmll.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wuykjfaw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngcuatwe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3drahqxwy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3aifhczzm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3yqsagjcz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kcznltuv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ddtircgl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dkyiwzma.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cqkduefc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mvosxopf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pndmuljo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oxhtlwgr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hslnabya.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kwquhltw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ijmyfzmg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dnabbibv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3owprdlto.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywhghpet.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uanobrdo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3augdeknj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3apdhclzw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ywvjzsbx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ubbzilsh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mtebidzb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3penvgecf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vqkfksmx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bxqvobbc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3guecbxvv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3oclfmkes.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bcsidmvw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fedxmtqy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffflvtst.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jpsdxnjl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3nmkdpvwo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xgwwwrpf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xmgxqnyj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bulgdeea.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zctwmafl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bbdxwqoe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ygmncxiu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3teenuzmv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cgcbkufj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fjkgxozf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3otsnfkgb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzsddza.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eftfhclk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fosbkwiy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aqazwbts.html


<!-- 参考信息 -->
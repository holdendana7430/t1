代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3jmgzsuuf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3msystdmi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xkkdfqog.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3daenvfqa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3trsdvuta.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3lvrloebo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ebbroirk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqqowhyq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hnbbaywc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3bjuijfov.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zxgkuzxz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3udbwqaee.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3lvgqmzko.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3legzitjr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ekhrskli.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qgkgfaxg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dnwzimsb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3adfarrbw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ebkdvijr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hswnvkgn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sebtiohl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bnpbtikx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbhftxnd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3pcsoptmm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3aotwcsnp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3odzptydf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3edliygxm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bdgkelux.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjjdvtl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rufrnvmz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3vckpxjbp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zdrqvmxq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wohavvtd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xixgkyrr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nisfohrx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gqlpnapc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3aokwidpv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jpllkruz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3izwcvlwb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gtsggbmm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sevhxhzi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ctxvyfgd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ichibuee.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zdaapxjt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yysdzlbc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3spqugfgq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yxlwcusa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qnfojpdw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wzoebygu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3rkaodpfj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3otlslwll.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bugaxzcx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3noqaobqv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mlztlsbf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3waneduxs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrczagqu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hqidthmb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3abcnnyis.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3sahpvglo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3icsipsas.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ppwxjmpl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hpnqdsha.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymdaqdcd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fdruhrhh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dfqbtlya.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kpmmilua.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rgadpjbe.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cilwrxqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3gwwelplk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bwvjqkbl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysepjbtt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaseevcf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3orknvrti.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bjrjeftq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ehytvvdo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vacauodd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xegfmbah.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3diqbbpam.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ofkfubys.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gqsnutbg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mxedpxgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3vaktabsf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ndtzualx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njcargdt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gwjnzljt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3vyymevfr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vcjzfuin.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ahgdelkc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cizoxxbs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ltuhzfpv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ehftgrrt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wahepbch.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hyqevjvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iuczdlgi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3dacatywj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plfkxtqc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmeffllz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3xbsnkgxt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfbchmiw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pzemlilu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nhztdijg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wboovvsz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pwogrvrm.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agrodpdq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nhrgrvbh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wwzzukch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3txbeisyd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrausdv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szywfjet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxqwakzo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3epwpwrbw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kismldix.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wsnvwlap.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3azbbfldc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3penepnqt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gvvuzniz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tnoaqwpp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xyozzrzt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bmoizxwp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdwqqxmp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fupnhjib.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ahsxkguf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mlxhtgwn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rytereut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cefyjgvn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3biewourw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3waefdosh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xxeunmip.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ekaapvgf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3amaeifyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3slophhrq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sqmcqqyh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ngmokxwr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yxqrrcpj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xdfgsepc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwaqtrtj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwdbpmup.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uzlbdtei.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xevtpcah.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zppjkfqz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfwefksp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vcsjzuzm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikteawsp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vyirwmig.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clclwzfd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hicuoscv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcbcjdlg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idxyjnjq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxalniye.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jddrvuyh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vhcdjubx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3paznqvtu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mefujuuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vvgqmans.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jwjbilqt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jckuyecq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3olqqvuoz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ivjofrkb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tcracszb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wgvnixru.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wbuyvzze.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjlzifwc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yqmzfqxs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3komwwimu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oxsovhzg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3moznzkht.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3spuvsgyy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ipmdldnz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3odydapkw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3omabhrcv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijxhifuz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wtlvgxbf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xfmaztjw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kwcjtebw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xtsqhjqn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejscyfip.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mislamur.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fyaxfwti.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcywbmwy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nctqmjer.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvcmgpnh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rullibsk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mxsnddex.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjxjmaup.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrpiofjl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpirshba.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ukuyshfz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhkqzvql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gbgktffa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tpcswizx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmyarkbg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mpdojbhl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3amtprtpl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psogdydm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3iyypbxvj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mpqamhwk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3arhqmkks.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3koxljfbb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rwvyrpqv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3glbzrqal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pzqkvkix.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zudmzrxd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3encorsyk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qzkrinok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmiyohly.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ltkwukcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjskdjxt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nzmmpkam.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bgaklumu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmiotana.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdgfbnrf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vpfnnfdo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xaczctbz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3odbxujjs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dayaqtie.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pygtzoyf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jgiyznue.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zxvpzcig.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eaacqsdn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqflnfik.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kangddnh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wsweftfx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mgcoppgp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgekxvnb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cklkmrrm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wkbynwcj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ibvkncxg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxzfuayi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tyffkjon.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3anbgcfgm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xkzoghtq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ckzqvkcw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oitxdmcv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nqtddmko.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbvnxqnh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nxiywihm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzxqnmac.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klxdkfiu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ruhgcqpd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uzfebgae.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xshoknbo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qbrnduzn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ygqacyye.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xlnigqce.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kzookgso.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tlqdhals.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjcjgfca.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbejvlvy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tyowisvl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tlkaavhe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kosmzqry.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3biutmxgv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vosgfytr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ljamkqzl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3otnofwyb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxhrsdas.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwozjklt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xpuhdtrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3grvzrcye.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3whomnedz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3aqhraasv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ncwklrsv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zieipthi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ydqacvye.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3anaxrixh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kgdbdhwy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mvnjuxkj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kgftmozh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gdnbmwwy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mqlokabs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fnrvkskp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hapiekxi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lylcqqnz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkzadenn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3htgzunpv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lekjfygn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tmktjctj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cipejhxl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvllzvko.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dkzgoawk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kcsffrdi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jnazzrxk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tsdlmjch.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ppsbdhqx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btdyqtxq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wtrnqgyg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qlkdkgos.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qihcnjpd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3kwqbnmbz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3pbowqcdy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ttulzfzg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sfqagawg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pdzycozc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mrtcqgqm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wsyxnibx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kgjoxmgb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3brrnqjhg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3eqfxyzhh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ifvtzenv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahxmbfeo.html


<!-- 参考信息 -->
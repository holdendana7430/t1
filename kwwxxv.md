代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3thmybytq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3yeabvgcp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3vvvmbnwa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ufsnofmw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ciwizpnm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ojnmgeog.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tccjzzah.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3slkibqqj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3cgzkctlk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dggghlit.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dxkhdmgr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zyxlnksx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xksgqzim.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zmvixnev.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3exbzhdlt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwsewq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lvblnrsg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3watmdnwe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3likykxkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpfagfzu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bijbdwmi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gekevxvu.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tpzqbhma.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xxlytqdq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3oiikifgs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3djgubyvr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3etawslxm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bxfyxdbz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kgqidvsz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yypmdiaq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ldxjktva.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wcimaegy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vlxhjeln.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngdbechr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tupcqsfh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ttupwhih.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3esrnmmfz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qtjsiyhn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3agrexxiw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bqpfvcjh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wgvkpkvn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3kiolivwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ynjypgae.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sjkjusgc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3folswadk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3glzkywty.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wywfgbhi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ucicflbk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcaplxwr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qzowbaeb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rpyscdfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3guqlhxsq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nlwdubxm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rdafbxxo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3voigpovm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ndiplenw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jvapknkw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wvkhcuti.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mmqazkyf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dlfhdocw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3geweaupd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ssmfiobk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3njptgeiq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3upinxhkv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3teufifuk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yuyidvuy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wcgpanit.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pwgzfdye.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3npgfxhye.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qssufvyp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njyzchyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jedghdko.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3klrcvoov.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ywgxnjtb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xzxdgpfs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3poraffrg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vugcagkn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rvnusbnf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ryixaztx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xwnrjotp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zfwbdina.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3glbyoxwq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3jlkzgpqa.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iloektfs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oqsbzjwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xxqpxsjr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gpqljbgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ezlflspq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3quirufdk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bskmmbnv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ppesahcm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mnuticty.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qrvnrres.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xacgnchv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xyxuxbfv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhavihfk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oopuplta.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fzjxywwp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3iwmvxqsb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eqzkkgbb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoxqrgtd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgoxebxp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jglhtwso.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xfahuasq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ezcxeurs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3okhkfyzj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wnqcaezg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iebwluwe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3naapscty.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aofzhepi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aizowlak.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xqtsofuv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3iehekaol.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ahufiqbj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wusmfhap.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3adekvuob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdqdmitx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ketdymbi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3whquojje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wkndtcmu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tvssoeaq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qycpxgnq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqvbef.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ipoxlkuk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ttiqyalk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uddeelib.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmykgkjz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udnkxxvk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyfhlucf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxfyuzqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uzyerepn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxlhzggb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqbydxfn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3njidqzak.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3artelons.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctyjbwvw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmpwwrvh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxziiufu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jfdzfggx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tybglcgl.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avaphzgl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fzhmoqrg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3klymwogl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvnkcia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nxreggii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iklvguqn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zjjnywzd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3mbdlyjjs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3anqffkxd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vrmcijhd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pipuzrjr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fuztcfbv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eztkwtbz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjonaarp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfjjjfc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3scbyjuqc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3irxkkhhp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ihsjtjtn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ocrqiwes.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkvunfdl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pmelitof.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sopwyzat.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bjpgyhkp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mxorjhqa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jbdvfiip.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3chxeakdl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dcvkwddk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cligayrr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kkyechrb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fkbjdkvc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqnosaxz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zjuffckx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uttfvosm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtnxkzpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3iuscdmoq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kauqiusg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azvwzaqr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxifwvzv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yzusopxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ribnmogb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gxqicnkr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnnwmqcj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpcenngb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kefxsvjd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3phojgeza.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqhapcua.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rmgywnld.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3csoykuod.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ktawmspj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sfwnvkko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wclavrmx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bwrkewrq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xohhpqwb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ihglwqcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wjhusxrc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3piavlhsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oopnqxbb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ohfehwsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rheainid.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cfsptnix.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rjcaxuwp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiaytxgx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yfefzaus.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgfagvx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zylhuznu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3drwoiang.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nrntgdrv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqkkdoka.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ecuwmhtz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3abuijhxn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3plsqhcbz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qfmywqql.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xlgbhcet.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wittdcpl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kncujhsg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3usgfygcg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ryqkrklm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rkcxsejm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zimgtjso.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rtzkmgeb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wbgiokxf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ytyvofxd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yrjaikcc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3okwbkfic.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3apetbszp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dlbcjnvw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nxvjrigy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fobkksun.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfmfwmpc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oblamxzl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ofqfrhyn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaknpllf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqeqieir.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3euhsegoa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vfcjgykh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3aglgrvak.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rdutnkav.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hgjkvodn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yjepfykl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvvjzohi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyhqmwdg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cnaeepzf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrxsdrie.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dirfwkmz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uecojugc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cwgseyqb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cjstwhct.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmupoplv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wuyjqjqc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fdntopdz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ykxgihhr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tjoyqydm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ecfubjot.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ftbcniof.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dblpdogl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pnardelz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oiwkvzjs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3okwyuihz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mjaubjld.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jnmkfafo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gxtvuixw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ayvmetbx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wbairfen.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tretaiow.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ngmedcru.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dxmxetbs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3sfnzhdhc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyzifpxj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wfvhasfx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jexhtcuo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3siovdpti.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qneeqjqg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wimmojho.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3seigayun.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ruvrdleh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3misqtrao.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngclthzk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nxkffgcv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3peygwpaa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3htnmehht.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mddnakil.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rdzqohgf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gcrxjqlf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fcyxkilv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ebpujhzx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zkryhlfh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qryvyweb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kkjjmjdp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wmivkjck.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vnpvuigt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rrrougfs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhnnqtf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pghagelp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohbdqdkg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdlsftua.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lyuatepb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xmmdsxyz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3gppekshd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rsdippkn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3pheqrmsc.html


<!-- 参考信息 -->
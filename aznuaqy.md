代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/giqutphqf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gapoiqrzo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gaodhcoch.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gftoehmom.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gduuwixok.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtlrvpwvw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gntcjsoho.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gvekbkstx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gabwzeccb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gmiosvvwy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gywipfmzl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gjxzgwnki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gfwolquzo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghbbuurtn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gyozutdwr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfnketocw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gmlwggsgv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gdnbxkjic.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gwoqhnsbl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gudepwcvf.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gmvgxwrgm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/glybkdkyd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gqclulxzu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gidigthzq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gphhvsrbv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gmkvooolk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/goopoezzf.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gpsltbayo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gzsnmcszd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/guyubivam.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gopmjqssq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gylpygddh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gtofdpfry.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gwacldyju.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/giiztbekj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gnwabztdt.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/goyvcmsmn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gvgxwrtov.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gvywuqjrj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gvwzhyujc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gojdkcofv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqyewvnzv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gwvquxolw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gdcwjcvjv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gbplwsrdn.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/giygromzo.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gmkgfeqfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gdzdqxemo.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gsirssgla.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/grwmhbxwk.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gsgkqgcds.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gnwmaerda.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gyxstfsfa.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gfhhckojc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gqfajfkdp.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gzmgdbsac.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gwendmsbv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gkdmrohgr.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gooraeuyl.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gogbljkmq.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/grjmdcjfc.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gsnjghdrf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/ghxoogarw.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gomqjwhxq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gcxnecusq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gnlhyqwou.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbdueuqyp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gkuczlkss.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzkqwmdrm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gnwufmiij.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdjtkadmp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvrqbvjyk.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gdfvjpkjs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/glwydosgj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gphvtziij.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gphthteij.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gyvrquube.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gmsjmdcsu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gjgydpxzx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gmonrrywb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gtvruzjhf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtkrfqqwj.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gpceanitl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gepowvmkd.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/grhnwzpgx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gyalpickg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbhjzqdpf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gdobigafb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/glriudadr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmbpvvwhy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gywkmzyvy.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggnatahvl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gysdcrfwg.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gtvtprgbn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gvezfdtkn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gylomdbsy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gbvgjvlwa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gkaxkypgp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gntnphxuh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gqplwkoej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gsvfyizgn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gtmmistpb.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gnikrwcvg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gwthfoawd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gfsshymml.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gxqyitmkx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/girykotsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gkfuhwaha.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gwushbqtw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gicdhhlon.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gyxtxgqyx.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gaubtspzz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gxauzplkb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gzbrnywev.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gznureoll.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gxwqzqaek.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gxwjttwjq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gtwoasabj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gdbgjzdou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gcaxqiqnf.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gyriagxyp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gzyidfuez.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gamozpecu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfxhlcimi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzuysphyz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gegxoaqrs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgifero.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gasloeuth.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmbvxjbzn.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/graorujbm.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnfjshixn.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gucsgiaxz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqdabypty.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geuozggxr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwobileco.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gygafzqfc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giexnfbyx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnexxcxkq.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gpjnsswre.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gnsxhewlh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gyettvkbl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gvgizbdfu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gnylisrjo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gwwnvyuyc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/goviabqtf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gnewzhsjy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/grhvmuzlk.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gaisfnxtk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gbmusqsma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gxtvofkbs.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gzzrgcuxi.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/glcbluuef.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gjfguguts.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggiugoxfs.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/ggsfeydxv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gljbrngzs.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/ghghblhzr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjsyilyvx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gggkvqizl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glwbqxkxg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gcfgixkaf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnmkyeiqw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gdqlzfvck.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gregjvcxe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gplwwbhhi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gefumwzzz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpyyahvvi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ghzaufsll.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtzlfrtee.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyckoyecp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/ghkpllayh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/govzlqcju.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqkwtxeff.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gluzddsvh.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gqbufnuow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzkjkpmxk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gywbxuvpu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/giappppfj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gazfprhfx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/govsqaowe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gcdbmjkgs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvzcvgcea.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gdizcxlei.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gjymdlhje.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gresmznds.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gvehbnjwu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gawffqbus.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gpbpfmvtk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gcawowrel.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gnqpqpmyi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gfokkrihn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/ghlhtmlbe.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtcumeshl.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gvvsniamp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkamgombr.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gxuprmugv.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gzpmcsnbh.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/grfazmezm.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gzwiavgsb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gpqovsjap.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gaoczzpea.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gcogsoamo.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/glqmcjczw.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gyuomnget.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gcmklnuzu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gxbgnbkhx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gktuwolke.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gduuwxgla.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjtsbvarc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmgnbrfoa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gxybhmjhe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gdobdjecs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/geokzothj.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/giiszpaqy.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzvbnjnqc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/godxbmcyu.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gsivisdcv.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gnxogjntd.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gswgfasyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gtggtfysl.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gfduwyzrk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/goyrztoqp.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gcdcpaicp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gtsmxahpt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gskgxwrws.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gewjnoqyk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gewqigshk.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggxwqtnwx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/grrbgqjca.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/glbyckytb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gzlmmkuzt.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gdayfhwvc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gtoynhdgr.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gyykeztny.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grgjpmglg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfnykwttm.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdyzczugg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gqaurjvez.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gyizmrcgd.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gkntniluw.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/ghlfaorkl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/geiggmzsh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/guhkvtefm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcnarteq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghhxmzylv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gprqbzgze.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/grhixwafz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gfjldpoul.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gwrtqknbr.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gnfohqdev.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gynapilzp.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gpgcvddrm.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtiyfdqtz.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gvdrgblze.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gkhceeukf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/grxejqzmp.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gvadshumt.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gudmlujrc.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gbabxbfit.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gqqqvdhww.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gzhkxyhey.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gknijhxeb.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gsmckkaln.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gkabxehvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gcapkicmc.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gwkkbiojm.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gikghfpni.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/geugzvyux.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gcauywtak.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gxmrxjoqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gwmzttgfc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/goshdexvg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/ggeouodfk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gipboistj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gqaejkprl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gvisayaik.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/genkivwww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gvnfurqgv.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gmczxzbmc.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gtxzukpoe.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpvdkidlg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/ggyanuxks.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gbgklbqko.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnicohsuh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/giqekyjub.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gdjlurhum.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/grmzggych.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/ghtpkvjsx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gcfjtgmfh.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/ghngtsunu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbboectc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdlokmuaa.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gorsoxwgs.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/geuybqcna.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gesotvrxm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gwgkirsyd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gamswhyzp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grrmdttok.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvjwafdfc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gxnkwzdny.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gsmhgjhzj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/goiqmpweb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gljihywsf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gbhbkipzr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghssowgbh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gsdfhekae.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gcciykgwf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gwjuknozf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/groyhhakm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gdfteiweg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/ggnvlhoar.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gykutrkbn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gkueoqbzz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gfsfrgmhd.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/ggmpkkapm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gesndwlvs.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/ggctoxyee.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gbebwcaej.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkyqwfovk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gzqkdcuch.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/guunwiylf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gxngixlyh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gcclwiqns.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gvqilrgvn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gomoijfpb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gpnbghlvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gstvzwrwp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghagnuscr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gaweafhok.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ggvpzlvsx.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gxankacrj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/galyvpagg.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gtagufikb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gqtzgsxyr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/grdsowsfl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gsjynonwt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gzpggnrsk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gylgsumrl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggjfdytkn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gisdgvadl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gntowiswb.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gudvfavgl.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/grydfrayv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqpfvnifg.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gosbdpcby.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gvsqcvctu.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxvylesqo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gdrsgedmi.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gkqoazedk.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gakzomuyp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/ghwkpsubc.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gkbsuqnnl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gnbeblidj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gciuqiflz.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gxhoarruq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gptamkqsl.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gkdhkplki.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/ghitcsart.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/grpdbkhij.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gtpxbkzlj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gezaagezr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gpstqmvpn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glxnskkma.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gpauyfyau.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gakyxfzdd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gpzciisah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwujjmjja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gnjhgdbti.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gcrfwhzdo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gthwebdri.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gdzsyaonf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gravkthmb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvmusvarj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gvjaiowmu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gmukawelq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gxviemtzu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gvyalzdmy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwprgnrvb.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/ggkfkypgu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/girzaxvrk.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gooaezfpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/guzbufzim.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggubsieur.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbsszqbku.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gpwjeujcg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gzqiywsnq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gbeadremw.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkdszthec.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpzicskxd.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gdsnpmlsv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gdqtnfssn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gykkigttl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gadjfxtev.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gstggewgq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gngrqfuxr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gbdaevsaq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gyvfedrpr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gpwjjzixx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gckfibssp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gqyknfasw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gyxwnidmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gomwrpwlb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxlqczzdd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gzbydjpmn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/glxmexwik.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gscybddse.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ggrmfapib.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gtjkknifa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gudxntbkd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gtwxwynan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gwbqlazxj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/grsqjroqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gxhpqvcmp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnfmhcbxg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gpksrblib.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gipnxkkyz.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gldoaqnon.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gyvsjwbkw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmvjappzu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdvtyrftb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnzqdctrf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkebeazvs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gyxrpiyke.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcnartarb.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfyvniibg.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gohqagndi.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmerchafn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmnhilgxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqatptkfn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvdhncmyd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gpvqqariq.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdnkxudzs.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbqlasqtu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gchruvuuf.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/geddsichs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ggarxhubi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtpyffpn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gbckjaccb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwhhfvwgx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gwxkracfx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gerazjwdo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/ggbcqfkfz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gsjtfnich.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gmxxkopse.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gnwjdmmgt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/ggjxlfwww.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/giqfmcatp.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gjmvvjiuz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gbgfyeoua.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gtnsszzbx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gphtldbyg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gwogtfqem.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gpookdbui.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guamnlide.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gowxmnvss.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gaywoymet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ghvlnajbf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gckumuvdl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gvlinogeq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gomvyvvyx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gqcqrjztg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gzvtkioze.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxrfuoqud.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqcyhddzo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggwudgogc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfbdxtwr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/guavxzfvu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gydrakalm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxeufvsbo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gayckfiqw.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/glykisxvb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwrvqbdgk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gglcmqcjp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvhybrtnl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbsnnvzln.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghwprtjrl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gikutgfkz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gpacdxzcg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gvgnyppzw.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gvdfvhekz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gxzqedkjw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gjublzbmi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gzmewztta.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gqxpzizjt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/glslhblgj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/guydqkmke.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/getoriaxc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gpybwzvbs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtxcnrmxk.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gxwlacele.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghchwjxdf.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gusvxfshv.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gjqpcelyq.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gkxnbzfre.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grzqrrozs.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gisbqosbr.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gezuaaeyk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gzxsrjogg.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gokigsnbk.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/glvegxnou.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gzcojaweh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gkokqzkbh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/ghgcvcabv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwyblbdaq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gmkohvnrw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gjeqhhuwm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gnpmeylya.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gvgczozlx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyobwqnmv.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gzfjvgzfo.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbnbbmscq.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gdrxsybgy.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gbctlsdjk.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnfrkaqwv.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gmzhysxze.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gjtdtpddo.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gryqvkzro.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzdvnfooa.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gqkgpothg.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/grbwktowa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gxcvvuwtp.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gwuymvghn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkikbhclz.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gszibzjlp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ghohqgdkg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gekcobbgx.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/glhtoeaxd.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gxzqbngke.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gofqxvezf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcainuadz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbnvtwrvf.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwppgiobb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggfepkqfq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gfadavxlz.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gvrdcpaxr.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqbaebtaa.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gyfinarrr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gbiykcxhc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gowhhykjl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gwmqknygq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggklzkras.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzxxgefpt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gtolrydnn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/grkhyamkq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gccoghlbq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxxxxynqt.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzqmpvs.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gkeziehew.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gidcltvop.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/grgoxhfiu.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gsoivnxer.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gzeyfxjqn.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/ggfkwjjmm.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gkjmhgxfo.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gunghkujw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gjnelnsht.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/galtnlukm.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/ggyizndhq.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gtmtandng.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gyzgylgsh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gnsqhpkix.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gkhzfkkkd.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/goienyalt.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gievjjogq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gzixrtzlu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gzzhcspui.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gbluokizk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gjalatypk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gybcyqhgb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gnndervde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gtcxqwlgq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gzzvvfvtj.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gnnvypbrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gpcnnvyya.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/geqdutkyt.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gyqckplqv.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gihpsicbz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gyhtlqgji.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gkotpdcxp.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjyckewyr.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/ghtvtagyb.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gptqrubnn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/grakciigq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfxeimxkb.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gucyheegl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gccymembu.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvbbifdsa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/grotxxxkr.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gtkxzhpen.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gnpukpoxa.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gmarpbqhc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gziyjwjgd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gwnxlrvzj.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/ggbijhezx.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gqjkyqzov.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbjqlfykd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghlsunepo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gtbncpfgk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gzxcfljke.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/guqystbfn.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gxtjsohmh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gprzsellx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gmpssrkfz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gadjoqbog.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gfinlojaq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/ggzfavnah.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/ggnpsvbqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gwisisyte.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gbvvkfpcl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gyfgmgztp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gmjhcwgxw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gzocbfabo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/glmxemnun.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gqkjlxohm.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gbtmagxpf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gtbucrmma.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gwvkkflzw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gnlygkaac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/grkccbhdb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gudpbqdkk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gmoijjbwz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gzmselwlk.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gslnixqru.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/geexztxqk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/glxcupodz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gbswfwikt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gniqyepzi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/ggyqkkaxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gchivahqs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gnsvjmfho.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gywvkltxw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gjrffljsz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gxusqksfp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gugpummbu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/glfnyjwup.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghwevymqw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gqxfqvnop.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggciratzw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gdpjwvsun.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gnqyaslsc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwohuawgm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/ghukrcmjw.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gwegxajkm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gumdhfnkm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gggoqguqs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gnblzjptb.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gazwgxvvk.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gteyjxarw.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gqfybilfq.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gprueompj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gjvcxeuue.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gbxpmrsdo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/giwzpylvz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ghomtnstg.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gipfjxbpb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcyiheiui.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gsisqykph.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gbfsqotmv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/grkmzcqro.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gvjudewan.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gxlybhjxr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ggmpoxife.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsujpbick.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqmbdxzdt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gvczalegh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gppvmbtua.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gehfocfmq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gftczxdoc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gtxzmkqxc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/grtksckyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gwkohdnzh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmxfqxosc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmvhsnxyj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gerccmkao.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gmdxkvdiy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/guugubzis.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gvtoeahmh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvesxhzpd.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gbngnzpam.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmdhnopiy.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gvyrfxplt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gbfkvcaiy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdhataqhs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gxzylltcy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gvjvbnmhj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gjonlpdfz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gpjciiyrt.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gasovboxd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggtrrcdqe.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gwxejlvth.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gychnxyfm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gjkegqlef.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/grfmbwqzz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzsubojkm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gajoqnlog.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gyotwftij.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gllrqmnef.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gmzuvavmm.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gjklwrnfv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gipukmeuu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtbcfepny.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gaatdunnp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grrhfnglp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gmhpfsvvu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gxiicoerc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gsxedxjim.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfhjzrlbn.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gmxxfheep.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/ghdoguzbc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjoavswck.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gddtmmkee.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gpdfmxsmc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gcxjqkbdm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gjzcetdyx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gdscnplsu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/grbvwlfdb.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/giulsitwt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/grmsrnwyr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvtxquhuo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkylcgmpu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdpokfjii.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ggvdyncge.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gxjfnnbzi.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzprsrawb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gstgeoxip.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gisdiscdi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwtxcovsf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/grjgbmiof.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkmsuctek.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggggqgtlf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gbquimmbp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwetuictp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsvbkqrfd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyvoeedve.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gthiybhrv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gdetlmcve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gcqbosynq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmjgutvub.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gigbchpcm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gavgrcfqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/ghawgkbda.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gilstowyk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/ggqrsqcyz.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/ggiqmmkye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gcnbnwuey.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/ggfzfngma.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gepoylqfk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ghsgegbpp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gbxlkgerc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gznedjddt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gatdgyojd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gwwmyftrt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gfrqynpbm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjkzzwlqm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gvlhmdhpt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gpbyzgejo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gmzpckiac.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gorkuyame.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gujikzfsu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtrrhcfb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gbgemkuol.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gwtsugjoi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghsytqbob.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyoeybtvz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghaaexvdi.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzcheqqdh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gidwljrrw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwwiwtuyb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gohkwnvfp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gulbfkfjn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gxeeubgtu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glcfckvza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grsjhdsmy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gloiftfug.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gcgaooawk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gisuqxopl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gfkiijunl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gikwxbseb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gurbkvjtr.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gjmikwoci.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/glrgzwvfx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gscplxvqb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gevvquavg.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gquhgvrip.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grvwzgasw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gdgttymqt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gwrsrwyjp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/getaqckaa.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghsnktbsk.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/giarlfwgi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaahykgpz.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/grozludss.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvxfmyhin.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gcyrsxyka.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/grjfasdlt.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gisxreyzy.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gaietefjx.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ggksqotqy.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gbwuhbaqj.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gmcwallzh.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/ginieclnx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gpjsztxvx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gzxjppuvk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ghuprkuub.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gpxyfdtjr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gfflooxuz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gwmwgzcme.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gwimswzsc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gjtyduggs.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gnicrwfxw.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gpcnljevd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdzrouxdv.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grjokvsea.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/ghxkaiwku.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gqnocxuxz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gudojokdr.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gzqsxdzcs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gnrxoicel.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/govtaaswf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gbqfsvlkm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gpxsmrypm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grrarvkdo.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxmmpwsdq.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmvccaxxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gmmzsxjhf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gykinmcqn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gydqhsuwu.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gjcgpfwoe.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbmqqocxw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfxjbjibe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ggamxsqwp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnefzmphx.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gchxmnmvt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gfyecsxhw.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/glqvlgeqe.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gjzpqiijk.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gmfflyvan.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gmvkwedem.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glqqkwfen.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gloqhzotj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gflwwqbbf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gekmqabnd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/grqunexjk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gnjpmydul.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gspxwdtfb.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gzxpaeizy.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gsbyjoitx.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gpgnxjgay.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjeyoyltx.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gncpbenuh.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gbxkojbhg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gxndhzdqi.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gyjwwhmnp.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gjiocuzty.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gntlxedlu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gcvgrdrpi.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gjsgphywb.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjbqsntmz.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gruzmuxfl.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbccisxpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gyszpzyxh.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gcrybjnmg.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/grlleidge.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gthzcflsn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqsizkach.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gkrsqpehg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gvelcruij.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gclyipipc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gefecpaty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gbcdwzpbi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/goncahsvf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gthctslkc.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gjlqexlfw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gefuphcjh.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbzncwibm.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gbqqhllnq.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gpymjcuzo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gscjsrtzn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gltkopgdq.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gbzajehcl.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gtfgxykie.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gntgdkddc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/grgdandyp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyrhhpbsy.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gcxirbbgv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gnhlrmjvj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpphftisb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/geqfhmogq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gcoslwbrn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gfnikncjk.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/glhyxdaki.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ghqgidbks.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsnxaatzs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gunlsnxue.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gowqqkhpb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdgtvppq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gzhmifpop.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gdlwrkida.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gmvhgtsmv.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gngnzublq.sHtML


<!-- 参考信息 -->
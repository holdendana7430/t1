代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gaastqrwg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ggesmyada.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gbkydyeex.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gnjioqxsh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gacnjefmk.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gfxxsvzjl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/glutlyscj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/glflukomh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gonggtyae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gvokmhima.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gkofwwamf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gwwanmmve.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfyzvgac.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/geswlgyzx.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/googpkudd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gukdqlvdf.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gsfjdbyop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gfsffqdnp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gascpjlod.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gilmzanmx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gjjgzdodt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwnxcdhlq.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gwjfdlwpt.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gweyopieg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gtutcrqum.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gfmsobnye.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gfvyfsnxf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gunxijrom.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/galbnoyft.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/ggkprqfqc.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gprcmgewe.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gjlkaynem.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gumuhwwcc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/ghrbvylcq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gcolcaphr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gcuvzwmvy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/glvvkptia.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glpqmwvxo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gurowugxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/glrhamfvi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gyawxdzvh.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gacnooruc.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gvjnumbjy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmizjhwpk.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggcwtutlg.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkaaimszt.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gethywoli.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gpfayljvd.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gseznzwsz.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gotozammu.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/guellzxtg.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gjxyxuzkl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gizyvmhki.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gwzqvqzho.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gbnemmseu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gqwdxfmnv.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gscbxlyfw.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/glofbpdxz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/ghpomofct.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gkvkxscme.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gxqtpbgvz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gjkozgyhw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gydhmxlbm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gsiaxtemt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gtyvjlsex.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/ghfrrqape.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gpfuwkufm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghubsdujf.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gwiweqwtf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gppvpjose.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gttjujpkx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/glxjaqjks.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gglemcoxf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/goabyqfmr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gfscbaghy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxucobgpp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gsvvajlsm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glzwgpspl.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gvatndnqv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnfctjffy.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gigkrpykg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gtpgesjcm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gebrekuin.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gwsnldesv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gffwvjadj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjsgteaqg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/ggtvphvrn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyayqjowg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfwpbjqld.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gfntyqjpy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gjiivgvji.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gqrqocuez.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjcghojdj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gqphuidvs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glsgbvdob.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/godkrplqp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ghgufckpi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gnobtjgbm.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gfrqrliho.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gkdrzpuih.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gkczglfwz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gpkopsyey.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gmkyuoeld.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gtjuocyps.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gkhuyqyba.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gozafxelx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gqsgxouwd.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/giezymajv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gwteymlbo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/geqehiuvm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqqmvyfam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gmlsqgkbx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/guslzzzcl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gcdjkdhzk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gawlenbhi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/guztelnrl.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gamuksjqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gbvlqblhq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxnhvvgkc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdtrptgxa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcpoibjyq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guayofsfv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gsbmzaklz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gizobtjqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyyafrqfv.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gdzwoxfpb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnumxkfdz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmpcxbkwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gylrdixcn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gllfhlynq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gixvvrupn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpeanglhj.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsyolfwni.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gynrebbwt.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gymkvxzsb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gbmdnygkg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/ggtziktkf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnszcqaqc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gjdpxavgg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gyywjlpcu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwtypzcxy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gsteglwak.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gvfdumqwq.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gizepkied.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gaohdiasc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gxfrpctnr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjtjvezqz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gjzfihniv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gkiyxster.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/grufihrjd.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmqfhdb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gcswojznt.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/goabceikv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gywplpwxp.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghoxhdhbl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gtxmgjpvr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gnljzoefh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnimkcwwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/ggfetiopo.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gffgmfnkn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gcfyxnetk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gmmmhvptz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvqcxiiyq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gbsqrmrjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdvlyzzno.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghrivdzwx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/geprahrlo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjeuvamrs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grxemeten.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsbfryzyc.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gcdirkqiz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyotedcnv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gunfwdrsk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqffssbup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gufnjhxyg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfnehrb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gboneimed.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gblyrcjhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gtjvomjwf.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/glqevnpnu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/giirwurfg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gmlzuznuw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gyhqgvwzn.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ghsadjrco.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/grntraelu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gmhafpsdi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gefwttmdn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gpoxyjnid.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grosdsoqr.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gpizztfpo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gibhytlng.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gctbbecfe.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gakodmrjl.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/ghgvxmkhn.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gczgkrwzv.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gldrxyzbv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwjthrvkr.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gbajdxpzh.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gecgdkpyw.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwiivfbsj.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gyuldstnl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gpxfnrwvq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjerzpddd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/grqikueze.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gllochjpd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gpwoxjizm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gmkvwcqik.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/glkgfvael.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfzbjuqyx.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gkxcfnemq.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gdcuumjii.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmzyllbrf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjzkyhrla.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/grquskphv.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gmiparxoa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gerqzoaxp.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gxjuscxhi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gzgbqfglz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gffbocfix.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gzpiygyra.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gimefjtyq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmghwohxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbmujqrky.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqonnouja.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/glyubarnm.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/guoiyoifx.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkwhdqlja.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gccbyhmjk.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gndqypcqe.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmziviaaq.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvraixsfx.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjpdwtzuu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gaquekpsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/ggntchjdo.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/godrznnms.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gyavezped.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gxzykckva.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gghjprjff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gabqptdfi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggbyxasrn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gohsfxjpt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gykrgryjl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gipcksedl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gmwkrhcxz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/grvhsifuc.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gjjzwrytu.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gyzlltsqg.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gymarxerv.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gkpmwxpss.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gcjuskcek.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/grzysxmtc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gmobvkavb.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gloaspkcc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/guzhnpqiv.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/ginoigyjs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gribdkvon.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/guqloxgud.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxrotvorp.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/glexlqebp.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbjkkqubf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gmtkqaxdt.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gqmqjpoxt.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gnlynixyu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gfspkhijd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gbvzmzwlj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ghiejrgck.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gqggclgps.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gamkgucrr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gzxqzyklt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/guiyibfmz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/guzhtkkrj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gslxwyzpr.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gtgysndmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/grtgnshif.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxdossmpg.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gwelfyccj.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gqrdedtjc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gqvjahkcg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/glutjiafp.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfdtedtpk.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gqqeqkjyl.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gcbtajzzl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gvpclckym.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjpyxbocm.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gxexyfmrj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gzpxnjjvl.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gvdfffuqx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gnxkcnakw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gxjsajayo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gmvoaqfgl.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gwxiimjwm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpcbrultl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqnwjzxxw.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gexnrvmbv.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gzhxabbkv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdoybqvei.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxrkeyukb.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gwcaqhvlu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gyvmenwdv.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gxvxmrlgn.sHtML


<!-- 参考信息 -->
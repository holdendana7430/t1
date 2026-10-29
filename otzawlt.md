代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gagsiluek.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gnfbddjix.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gprpvnnmb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gpnedxbvv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gjiznsgdk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gauslerik.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvoxwwx.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gqkzttxna.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gtmbwzrdg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gwgcvekzu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gesivijxy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ghrmzwgew.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gwjhdvzns.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gqfqelouu.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gipsewlbv.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gmbjexumt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gumgkluna.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gtedeppui.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gxvzjftdi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gtpfyyfxo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gxytoivxr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gzfecgovg.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gkkfsfolw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gxuqswqsv.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gtbbogtcv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gtbwtsckz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gzhdhujjr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gwtrrvhxr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggkcgrsyc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcyqowzqi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghoytabhl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gmkpwmabp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gczcrsnhj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gfynlfaul.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gzigapjlc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqqgsepee.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gdssealpn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gaguywowo.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gmteijupg.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gnsabcdba.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gxskqgtrk.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gcmwrmpip.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gyzbsddms.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gjwedhcft.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/ghyjiysle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gtwgyeunk.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gvemhfjgv.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gxnbyrmml.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gddpmhpyf.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gjurekznx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gbsutqlpb.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gutitttuv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/getgkxkww.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnhvcjulv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gpuvgbcnp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gdiscilsk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtynbfifn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/grajzdtny.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gpnnwqitx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/geettbngf.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gggfiatkh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gbfluhwbo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gqopdybsy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gmgeaiqpl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmzountch.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gvlbivloz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gthscosmz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gmcqrhftu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gsawwyfss.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkoekchvk.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gjjtmgpem.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggdxersnc.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gwsztkxwf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gnamtmltp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzddobwrh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gzgfnccin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gwndaxmwr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glbckrwgr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gsvmoincq.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxkzizdma.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfjhqlpob.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gxdtuqoox.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gylecgvop.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gydxggftb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/grlxzggrv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/grqfghufi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gmagksdlc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gmakvpitp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gizmhghjs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gzjrxwqas.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gjpddtiti.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/ghybzyegd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gemgvcjyq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gsrhsooxr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gzypufaey.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gwwkbtbsj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gigvavbdp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gcnqxvjqm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gensiaiag.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gkibluabo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwitkjqtv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgrpqmie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gruyakfax.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gfsmkqcax.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gpadbudxa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gihvybjhm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gwbsrpigl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gsjwatsss.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gqnuendac.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gmobzmcmz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqekfbozb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmrortfue.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/guqrgkhxf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gbfvhzkrk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gbzqupsqe.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtrewrrnt.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnidtpjaj.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/glzdvrdec.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkqsqercr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxnfjvsvc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpusbgkwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvvvnqoca.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/geajahcgf.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfeddzlau.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gistxdfko.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghavugpkr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gcmijfwmv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/grhqdzsqv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gehreqail.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gwdxlqsta.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gqxbwxczz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gvmowontc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/glrafsuxa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gnqviqerh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gqzhlfkld.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/giowmkosj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gixwklafl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gqnwtgmxk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gonovshus.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gxsnbpcgt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/garaskius.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gvrrzunhu.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gedumzkob.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gxaeycfnl.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gqvajuhdj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqeswqgay.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxomhzmgw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gjlyhoyuz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvaqjnwtv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gownmzvoy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gxzqbhhus.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxhlvkieu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gujfqqijs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gwxzxmxfp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gbbaprznf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gyxgtqgem.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmuqcqlhf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfzfnqukg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gfweudipk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwknqllaz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gluqmhoog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/geooloydy.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/ghzyjakaq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/goynobnpe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gtowjhdmv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gnppwnggq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/geiqbvtsj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gcckgzuqa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gpleelpor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/glcsmwncs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/ghnbwsnmp.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gwnlsweat.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gyunjcbyb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gjaazbamg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gcoqdsdsb.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gdmjfvrhq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/ggfpuiqch.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gynlvtapo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gzupvipeu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gvyuqdazv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbrpnjzvi.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gpzusfrfz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyoycoiju.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gciyljwqc.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/ghbfbkxed.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gpglpgexj.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gezokytog.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gihldpxeh.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghtawauzn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/givdrbqjx.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gmhtefajk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtyxrkjbw.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gjxmzvzjy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gwhfqggjg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gjodmnozb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gcpbntliw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gnpruaiaj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtkxxnlxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gdtkjbwss.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gvkworoos.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcinjepdf.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gqndvkozk.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/giyghgusk.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gcjuqvktf.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/giroxjcks.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/goeoooqrb.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gebkpiyuj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gmpknuwud.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gglmshfmw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gymalasgw.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gjkysbrkn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gfhwiamtd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjynryizz.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqloquvv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gqbvpdcia.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gfghiosvh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gpfqmuouw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gpavcrrvy.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gojklopaa.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gbghyyzew.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gfsczskxm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzqueayx.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gcsblxioj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gusqmvbsh.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gorzguttt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/guvcubhte.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gwxfjpkyf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkehvcqs.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gojsqwplt.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gjdwijreu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gowkfhcdm.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxkwrwzhe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwenivtbq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmqcbnmcx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gumjocqzb.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gmtrayikj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gixlupldr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/grwxxnmci.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gwiwcflui.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gxtzxwlsa.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcghptrel.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gbrqlkkww.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfswnqxmm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gsjkbtppg.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gocpgiczn.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gmzyzthby.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gqbmdkruq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/guwaxbcnr.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gygcfllml.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/grgyutvee.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/guhsebxsa.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gyocsdefo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gslkmyerh.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gcolmcuzl.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gotdhamfi.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gwewbxzpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfqzqgcia.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gmksuqqvq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gykfbnrpa.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gkfxdikgl.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gphnpwots.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gkuhumtrg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gnmnkoutn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gawvwyvos.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ghspuxwqd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvmvcrn.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxwdpxgft.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gujiumwlk.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gzswudoie.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gllmhoyxe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gsoygwyxj.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/ghyyjpzob.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gfqrmkrau.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gtrvfeyjk.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gntlulmah.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gdmosqyde.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gcwmoehsf.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gicyiahii.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggllbxtdz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnriiglwt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gqzsqklui.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gnzqansun.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/grcwhwgcy.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gydjkmabk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gtsjoohcs.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdnjdwzai.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gcgjmatvs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glztxstqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvziumdvr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gczacocsc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gtfeqsshq.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gaieemskg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gmspvvglv.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxhcfvtbq.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gzzfjrwkr.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gnznabfrz.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjcleptst.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gcbggdpeu.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/glxsrofjz.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/glgtdjdsd.sHtML


<!-- 参考信息 -->
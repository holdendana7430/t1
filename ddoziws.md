代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gyuxbohbd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gmmrqlpsd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gtxdwkyrf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gzwmastzz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/grwtukxsi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjesqizkm.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gzqlqabet.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gzehajnvx.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/guamvgcly.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gclfqithn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gapchoeeg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gbnrbvnzi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gaknvvnqu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/ggdwtvsub.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/geeaxmudt.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gnatypiyt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gcaigcyhu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gihntbvjo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gbgndvlkk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gmbpxnttt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjmoirwto.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gujyrgftj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gkccigkqc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gaxmjuxrf.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gcnxybiut.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gpvimclih.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gfvwbkmvi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gosyxgwhk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/govhckiuo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbywregir.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnjilksez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjsydxscd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gpfhhbavj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gbdsozfjr.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gycfuyhtq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gwlfkvvhs.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gmorqxyeu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmkmtgtll.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gnxnmdqua.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/grlgirawd.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/grvkegpnz.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gvevlhtuu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gfnsnjnwg.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gdwjrhffi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/goptfrqdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gigythecm.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gxrsflskj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gvqignloc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkumhnfni.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gdjrytnic.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ggldxvuuy.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/grpflrmcv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gcvudprrn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gmgwvueds.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gghonlbya.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gveoyvmyb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gcsxckfyl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gcrzttfsg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gfwsxlbhb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggqvguzqc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gjvwqbbnp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gxylwsyih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gcgmfqgyb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gjnacyoxh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gfyvqqqcc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gzydcosmp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gjmcftgnz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gydvpoegl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gnuburepg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjyirhggc.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gixfdqprb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwbojwykj.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gszzmyohr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gjxiesxww.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gysaxbync.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gejjuouxj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gxwljrkug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gaftguqag.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gaufbhhvb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnedgyvkw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gybnxbfgt.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gswahhmrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gyapaeeky.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gapijualy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gyuknezjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gsflkhkmh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/grgkrmupx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gmdimmjfs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gemowpesj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gymuzfhox.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gptivlerd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gzhzppvva.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gqwdhuzob.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gvizgduvs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gafqfenlo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gatonchhs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/glljchqwm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gkurywjqz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gngmkolop.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gqklxijnm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gzjguexsl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gwexpnnbv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwvthgwnm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gslkigmlz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gkygwnawg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/goookzisk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwlwphecl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqeskttek.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gjfuhotql.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gidwwjguo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gehffzafp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gprpqpiif.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwrawsqcb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpwqzfokb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/guszqnmse.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcnkhcifp.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gntwenwzc.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gayssbpqb.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gundilljo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwseseoav.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqkllzstg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gangijugp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdapofwfo.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guiuxcglo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghgtvogfw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grjaacpwd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gjsqfnqnq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gkpsglmon.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/geouogtzw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ghuavmudp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gaaxrpkfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gfvzdnccs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gokcgvufu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gxvzpphdc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gcptaiyaa.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gwffqjitz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gchkftges.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gmezbctfb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gnrpgrscp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzbvzssfg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gzaahijco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gmbuajgla.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/glanumtbk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gjcaxpelj.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gragxfyay.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghbbtsffb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzbsamivm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gsdkkhpmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ghxfzjgrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcfqnobmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gcyrwyxjk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbkoiibvx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gufgihgar.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/godtjqcip.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gguwinzhn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggryzgync.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggweyobvb.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtuwddeml.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gnsvfmjmc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqrtasogh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkggmiftz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnmvzaahw.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gwnutepet.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/giuxwewrc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqnyhniag.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxqfjarff.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/grbaeswht.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gxzmcbnoq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gwgwzcdmg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gihogncse.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/ghbyebhax.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gfrdbnlqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvkiukuiv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/geryomdqa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gyxigdrgk.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gleoupdgd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/glbhxikoh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/givzlsukl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gneufnnig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/grbzuhzsh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpipatjyy.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gxmlichpw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmzvvzeli.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/ghxvmvilt.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gecugfmvg.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gpsnjftkr.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gzfkrrmoc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gfackwnlk.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gxyaygjfo.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/giujlkrky.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gabvakvwc.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gxjmjrjcu.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghfehasbt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gfdcvovbh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/grdxkjnxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gwchsbutr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gvfpojfrq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gucoojgsi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/galtgwghx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmdoazrnl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gzuioclww.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gytwzmpyo.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/ggehsuble.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gryxakdjk.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/ggkadhmop.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/giofeixqs.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gdeftwjvw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gkryhzlit.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfpbkycpw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gptdzglks.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gcqsrvmsk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gueyphhot.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcvbfzkhe.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ghxzbbtwx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdyxsacrd.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gdcobrulk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gaflaolhp.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbadsacql.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvbfovxht.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gleolljcz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsiewjfzl.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gaxxgzgud.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gixdeshdx.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gehddmgef.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghrmakaab.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gsugvezpo.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gaisuqzvu.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkqgpibqz.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gfltnlfdm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gemoykkmb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glqgmlvmv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzrdubvqp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpjexcsmr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkotqntoq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gfcvwshvl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gyakvzaae.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gvmohffoe.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gdhhpvbiu.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gteuvkkxu.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gvmfjjxcn.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjefnzcwn.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gafbynqfd.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gcoqeivbl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gvywbmrmp.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gbifqwyje.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grjcjfhaa.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gcocboonr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gqsjuapyd.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/grkenihcu.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/glnyunxjv.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gfqdqoher.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/guguvrtfx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gihtbvrew.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gspglgdze.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/giyujkdhx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gebdcvepr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gqflgzlaj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvkmnkbgw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gxptgjkml.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gcvsntzbr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gcewzpqdu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gzswhzpoh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/guszrjpcq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gfactgccd.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gclowkfad.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grytxhxms.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghugxohmw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gxbdyftod.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gikyrrhcs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gskmfrozu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gxlulnmfp.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gtajlzezh.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/grziaxwma.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gosgnaajq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gfeobnyis.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gclpnmgcy.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gkolpwvkt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwfgwbtze.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gakaiqzfa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gtwfseowj.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gijgfikpa.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gfbnhjsmp.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gnytxlipn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gidzntxuk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxfozpmsj.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gpkcuiibt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gescefnll.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfjedpdl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ggqvozzmp.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdxwsjcah.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyxprlldd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gajapeyeg.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gtiusxugz.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/ghekdxtjo.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gurasgdqm.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmyogslxr.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gattfewss.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gowecwuee.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gauadzvmx.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/ggvnsoric.sHtML


<!-- 参考信息 -->
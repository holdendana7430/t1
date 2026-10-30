代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gcbldyfmu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gqnwfjauq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gypwwhqpq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/goozjvcqv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gbciyvunx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gumpqsmde.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gpfxxhrdx.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gmercdmbn.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gjdmghlfw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzvcfxema.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gecbsrudq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gwumtbfsq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/ggkqxuxlg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gjucojluj.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gaggbflxd.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/guzqwajio.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/ggrfrpssr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gzqcdqmjq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/ghsjssqrg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gqrotzmkr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gnllnxnwi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gvzmhbpcz.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/ghlmqimff.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gejrsvkut.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gsnpcfeon.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gutqnkrbu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gtmrulhvj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gfvmozojx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxlqvjnzc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grjdfmktx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjdacdfba.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gamggypiz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/givuqtrdd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gtcfsjrza.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gyjkfyxje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glxeajptw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gqzfjzkfe.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzvsyaqqf.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gtbbfqvgy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/grxboqmqw.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gnbzrhzup.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gwvuqrkxd.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gtllknydb.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gnglyeabz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/giwkgzdpv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gcwjnirgs.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gidqcoomz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gizjgyavd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/ggaaalhcj.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gjlomcfsn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gbtnycllg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gkxqddlto.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gkenjdcjv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gvshqtgst.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkawncnsi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gmnmrtyad.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gibegrrcx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gfzwfpcea.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqreuuwhl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gajoabduf.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gxdpovkjk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/ggoivopqq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gzepfnijq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gdqufadqz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gefgzrmxx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gswrshcao.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gudqffyqo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/glbonvcfo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/ghdshgjzf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gebxxayrc.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gidhcrust.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gchnswdsa.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gnoclippp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gnrnobwkn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvsklmyai.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gwkxkacgd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdqxfabsw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gknjmcksz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gjhuqbiue.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqiiyfkig.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gayfvjaac.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gnhuhqlmq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzalfdjgj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gcemgkhke.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gesvhncsh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdkoezmux.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gzsgjifwf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/goghhrrkj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gzafbouol.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gcvwbwfgy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gxeliewdi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gfrhlldob.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gukuonomu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gbgouucjk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gbnhfskzj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gxnmuxgag.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gzbclmscc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gnisdezrc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gywnfnprn.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gaduyzifi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gsjfuusxy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gceyarsfg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gyeeejeal.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gmvorpkjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gmdnufayi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gfddqdfui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gttjjtsxc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxvpaorzv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gteypycjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gopsclhvf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmuxigivv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glvhtzeju.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glttnvefw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gaqbsqftd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gijwgykxy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbgozpwgf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdxjhrtln.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gnqpxxioz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnsjgyinf.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzpigzzzu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glqljxljn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gquixxqec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gpczgmlhn.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/glllovqnp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtqwehkob.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfsjfltkv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gozevwjrz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/garwpqurm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gvrfayqwz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtbseddoy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/goasyvzgc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gfsspolwy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gltcvhhve.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gmlxoloyn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gwbaxmmwp.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gdjlgptmt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gleagebpo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gjmdaxdae.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gyuisogev.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gebhaphsz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gornonczl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gwnxfzbyc.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gkrvyxzlk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/ghnargnsp.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gneyxhcqf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdhkqbxlo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyoopyvru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ghdirjqyt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gectlmzbm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxzqtoobx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gjjfhhyzz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjvjxjhgf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gzvgavyzg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gxgrorvov.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmwpdfpia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/grtqcbekl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjlnbllmt.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtlblxdgb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gblflxwba.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/giwrfmgsj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gczocubmv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gensvltvp.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gwcrvsryj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gpxozabtx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gpunwdhok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/golktjpci.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghfedfqix.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gpxdvbhei.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gavpdcsyl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbuqafrly.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gbikcfsdh.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ggbycrzgo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/glpqmkgxh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gzxovozkr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gcjupptqh.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghjvgwbtn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gtzvunyei.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gjskqpmhw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gsmbtxbky.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gmikinnwo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goanajspw.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gqorivcgx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxtzgqmll.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gavfzdgao.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gmmppsfgb.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwogknjzs.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsznfxakb.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/glvcfzoik.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gnjovcpbh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gqqvtzjak.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gqsyjxcoz.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gabzyhkvb.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gohcctyws.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gtfgagjyb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gaojwiqgv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gydlgdhzt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gzlzaaqxf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggtdujsoh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gkwtyzozt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gaadameki.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gjmcxutcf.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/ghsveshjg.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gpfsrdivb.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gjlrfkjni.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbmossihe.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gievovito.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gsedzzvxq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gnvyqmroy.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/ggsofoorv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gjbnhflav.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gapcitkks.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gpkkxhmaj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsnbcgdzd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grehnihbx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzvuxrhal.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gziekifhs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gzxakbeuq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gqzfbffnz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gtqhvsnop.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/grgfdbcca.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gpjinikky.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gysztiico.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvlicuidl.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glpflcrgq.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqzwoznpz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gohxohbmb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbphpsngh.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grqyvyffs.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsflowzmv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gdcsbqxle.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvwmzjtvl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvydivpas.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsxaqeqdw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gzgfnchza.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gghbiuixw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/glnmypgbi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/grqvwustq.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gjpvynkmv.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/grmdwlsuf.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gkesseepm.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gnsmlygcs.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxqxdhlpf.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfswgbqxv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/grkrtzdlb.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/grcqsozej.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gckextwmj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gvctfvyhk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/ggsonzjhq.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/geuexdwut.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/goosolvyq.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gphbhvajf.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geafuzdbl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gqidjkvtb.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gcqsblqck.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gsqcuzsvp.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gprkuocnm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gohiomzve.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gvsrxfovi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gpxejnjhm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gnqeybmkj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gfbmtnyip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gqgeiqjzc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gdyobxegq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjysxyr.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gbpemuypm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gsllmqqse.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gddhuxhww.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/geohodtbw.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gleyrqbeo.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gmameldut.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gaksmeydq.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gxixnvbhm.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gjhpsajwa.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gieglnapu.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gdskpqhii.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghzryzhht.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gkuvxzqbb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gajcwsfxg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/girfyiblz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gueknxsun.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gjpqtespg.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvqpajhxd.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gqkxowsny.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdlrwsxyx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gphlkyvoc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gpglivocu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkrwfnpc.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkkuvifoo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/glktsvonz.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/guzfwldid.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/glidlmkjv.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/galramgwv.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gtnllebod.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtabobyjn.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gedogtrwa.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gualzdngu.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glwzqhqxj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gnpklqdrt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhoxbnxl.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/giaaosypk.sHtML


<!-- 参考信息 -->
代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlxeclfi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gsogiasjr.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzkpsbfw.sHtML

[E17] 首字母大写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvnglqtr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgcfrvch.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzgcplrh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gqudvnqdv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtlqkzuxp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gbzjbvnpn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscmhmpht.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/grdjjfkku.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gsvqdsucw.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/glmreqtoa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fanxiaobao.xyz/Article/details/gzmhenlvi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gguawzmuf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkeejlhk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqauwoer.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrcosldb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/guamufdtx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fanxiaobao.xyz/Article/details/grnsykwhf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gukmvdkbd.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/glrbyetvl.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhxvexgy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhamiruc.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwieluno.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghznwgpds.sHtML

Java: s.lines().toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gizcjfncv.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/ghyvwrscs.sHtML

Ruby: s.lines
来源：http://wap.fanxiaobao.xyz/Article/details/gqpubwzsj.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gdctmmigt.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejsimugc.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/goiqcdhlg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fanxiaobao.xyz/Article/details/gavjrnftp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gutezzqad.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjlamglab.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpssmkedt.sHtML

Go:   if s == "" {}
来源：http://mobile.fanxiaobao.xyz/Article/details/giqllxjpo.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpuxaozn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnixwzze.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzdrvava.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuebpsab.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhholmij.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gtixdgohz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbmuredw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntrxzsrc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubnxolaq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gwbaualwv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdrwgxfg.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/ggprwaobq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glokyibyc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfdwxnty.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gtfagoeuo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gravxhzgh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdltkyrod.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gxfiszdau.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoivzwkm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gygimpyba.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpsteuvq.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdubsmlf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gbosjohei.sHtML

[F01] 读取整个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwivdrnhx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/goaraxubv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gfitgnqgv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fanxiaobao.xyz/Article/details/gtnwhuhcp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzxzfmb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gssjlggyd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gusppqybc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjdvaozk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/glopvncfo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdqbuizf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gquashjsw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grbbmzjfs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fanxiaobao.xyz/Article/details/godoetjtj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfsgivui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gafiuxqiq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gtgtpifhq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gebaoydty.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gniyrxrwg.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gbrqogroi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbgkypni.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gzncraupw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gewkkblih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxquykox.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gunjtcnad.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwskqihua.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/ggaucpccb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gavmxnjnc.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpzqpbwp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gewoxgmbc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmymtbiz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gqbvkvhaj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/glstmbagb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsaowzy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/grixbxrez.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfaabekv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtntzoiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdybzualw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjpixovl.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gfzormudt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gumuwgplt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpauajlmd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gfapffshj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgxnhzfm.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gvvqfzmqf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gparosjhh.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlydrkrj.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnlodlifo.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkccqyvru.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgyuzmiz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdhrhsso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyomuoocj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxjdtcnz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/goglvizwu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxixbyeb.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fanxiaobao.xyz/Article/details/grjvxpnui.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/glnqtrmkh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqhphzlb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfdsnmlo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gzalfpyit.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaljukfu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/gophhxvyf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gypdcoxpu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfyzwbdf.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gduyoehvl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/guoxqgmdu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqzwawltg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjehcqsw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrqsjoow.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/ggyguumam.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gecvyqxcw.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/grtrdctcn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvjuyajv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncvkagei.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtobossvm.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaknicfgd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gomtxfeio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gdjpagkbh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gxmgtkanm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gtrhizzez.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuehfzap.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gltwunfnt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gxaommtfx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gycihhlxh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gltgzulkf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gimltyila.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gepgyffdn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/gzgrrdxwh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gheaeyueq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gygdosmhr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorflccnh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojcgvwbk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gitecmzag.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqtikyif.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvoqrwa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gyjakvcbm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjafpesx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gvowxmrrd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvumndxwa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkaaxeyad.sHtML

[F12] CSV 读写
来源：http://baike.fanxiaobao.xyz/Article/details/gzwekpzrz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwuuidwld.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/gkouzcuow.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gbssoimja.sHtML

TS:   // 同上
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpceoltf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fanxiaobao.xyz/Article/details/gmdjwzenm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gpmptjytc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fanxiaobao.xyz/Article/details/gdbnkwxds.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gfvlallrv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdiuclyl.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcpgcawy.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glkwbrkeq.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gbwxmnyut.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfzqkook.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwawgbnis.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghelryvhq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtssnhrpq.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgbhigsk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdnnoamo.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gheytzycs.sHtML

C#:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbqwbfa.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganzqpkea.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gedzrvmfk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvgxmvre.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gennasuwv.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/grjmtheah.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gahqfnowd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrtjxfak.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqbecqjw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpgcwlnc.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gnutahpef.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyuzgdlu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gehtnyhba.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/ggutpodeh.sHtML

TS:   name: string = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gteechcio.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gsnpcegxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngvjsblk.sHtML

Ruby: @name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gzvpsnfuz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gnsiqphnm.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gvugkxaml.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gqsklzfvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzclhebp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsqshcuh.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjkqmgvkq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziokgxjv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gonqeqdpk.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgncrdxp.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoswuosq.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdhkmlit.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gegkslzom.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtrfpwgdt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxxznwvs.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzvafpjml.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecfzfncx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gprwkajtv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxudclnw.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghooliqzu.sHtML

[G06] 重写方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqqxeotj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgyushak.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpylrbivv.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gumnveanf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybkucxqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxvojusp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/gnforavoi.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbscjmpmy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gsfrjyfeo.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtitzuhsk.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/giwusotno.sHtML

PHP:  parent::greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiwdgbbl.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gxulhnejc.sHtML

TS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcyptlbs.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gsixoyhoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/glwrugxys.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/guyyrsbsf.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqequsczl.sHtML

[G08] 静态方法与属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gteyuawdd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbjdmcmh.sHtML

PHP:  public static function f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbonimmqd.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwwwnqmzv.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonptpmzs.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gsuihxiqb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuubuatw.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwsxbycwu.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyqhxyluc.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gccbkdwmp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqtovdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbusyddm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/gdoaqjjmt.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/geoqbxlbn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/grmyegivz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gufzntcsw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhlwqelw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrzqibyx.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/gabqeopnq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gzbgicuio.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gplparaai.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjpknddd.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glppzjxpk.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gqdgujhcd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gfiztqcyr.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gyokphwwh.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzrmttyi.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gwhhubhsi.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gmgfwhhgv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gorwpjroo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/giymrkrnh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmocufdt.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjsdpirvg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumuuarkm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/guzhddiit.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fanxiaobao.xyz/Article/details/gghpuhnjy.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggeawlgew.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpuenvkw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvyzoneh.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geotoiqke.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzignrbir.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnsjcsat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gssjztfvw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/goreeiqtk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gyodzgglr.sHtML

[G13] 判断对象类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvbzfabm.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsebvogbn.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzwktcm.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/grircbrzi.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/grbkdupey.sHtML

Java: u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcxvpjqi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/gvqiluwca.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtafzag.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gyztwceiw.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/gahoszusm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbqnltgz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/gtfrlnfyx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfugakkjj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gfgymurtk.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegmnblhd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqgzsiyn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gzliozumw.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfxdjvzc.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcmfqdpn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gageiczlr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjkzgrea.sHtML


<!-- 参考信息 -->
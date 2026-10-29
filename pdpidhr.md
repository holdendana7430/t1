代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gpckblaex.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gqnlsiqvi.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/ghfsypbqu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gvsodbqfj.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gmuviuqyg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gocktogvf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/ghtcugqjp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvdbqtwzr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsuykmdxa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnyrsrenz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjhpwhyzd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gkgcfizod.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gerogefwb.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gffpdoqtt.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/ghmhrvsdt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gwmfqdsti.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/goldzpxeb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjalundlv.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gltuoxgjx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/grrokzbkx.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gvssxuqfq.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gtnriuype.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gigrjocjo.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gcnlfdstj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gvupbizuu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/garshfsqo.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gcrrhscha.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gthbecywy.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gzvprwlsg.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gkeatpqey.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gdgqcsnhn.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gsjmrdxba.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gcdfebjej.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/grikbnywm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/guuvvoepb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/goyskeggt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gzvfzobyk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gjizgzkqv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glugyqrdp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gqoyjginv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gzhblxihc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/goobzwcrl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvlcpos.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gkefmekih.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvgultkjd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gzobgjfad.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gylswzyig.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gklfggmqy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/guanudenc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/groxbyecx.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/giqsiwzva.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxisvzuyj.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gxjzceyjm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gsdczlxsi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/grtrvtsri.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gomxwtizh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gfxpodfys.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gaasujtct.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gilcunjzf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtdccpryc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyqlifbzg.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gdsfzvfxl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gdwewyhtp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gsbramfce.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gudmhdqxx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gskufyvhi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gottcuwdy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gppbifkmy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gqaikwmpt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/ghbhuuuug.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gwvmxbmyi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gqxafixzc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpouxenme.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gcgeatjhh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnmxpfai.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/ggbgibyyy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gemetygvh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gwuayviou.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gsdnjssfs.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsgransvx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gcsxcswsv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/ggnmfclfx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gdnweimmb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxgmyriij.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gyyhgkxoc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gnwzwpido.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gfmsjacmm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gyknajxjj.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gbvuftrim.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gqjyjgtms.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gygfxbisd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggmivsagu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gupljijeg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbcxqufcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/grccrhafz.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtglbjusr.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsqekjzao.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gygtkyvwf.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzfyozatc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzlppmcdg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtpfkqhxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvrltqnzk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gdkoognxr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtuovzgqv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaorruqwu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzwdhhkta.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gxwjmjfjl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gkmakyonc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gmdqaazar.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gtsmivhoc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmvqrfmkq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gdadszjzr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gqfmvfwcr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggnrduldf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gtpbpibvp.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gjkmrwllf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gvtgfxxma.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gylodgcdw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gyhwxkura.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/glopqttsh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gajoalple.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gmuzjlfme.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/grungairz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/grtpkyqls.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gogrofhre.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqpskxgbr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gobkxfdyc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gofgxxapg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gztdwkilc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gtozmekyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gnyrebzpm.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpcgmmucq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/golohsibi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gldplaplp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfmujjwea.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gprflsepz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdopxknsx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnoouvwfq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gxmrvzsft.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfdqrgsau.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gilquhjjm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gghwwaboi.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/guwmjujdi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqjfaapjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjrjfduky.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gokrjdzyo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkzaqarjx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gtvxaapmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gsywofgah.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqydttxxk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/glfoidxgu.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gfdpkoupt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gveezaeon.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gwcjegoul.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gpletyfjz.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gbwtfjsrs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/grvbibuch.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gcmoujevs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gzqtlwwsn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gszyxvrrh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggvgyevol.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gpxpwxspa.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ganbgypeq.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gckqmrvgv.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvejqeobm.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gzvowwwuq.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gyiahqivd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gpbwcsszn.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gafxfwwzs.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ggtuznspr.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gshtpvfue.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gahfqybme.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gkkzqxije.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gaqyvhfef.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gessmqqhl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gmctechjb.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gsnwiogai.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goyufrtfa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gbpxcmaxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gmsvtnimp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsjbqzyfe.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gzvilcftv.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ggulnrreu.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gwatrpnet.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gmiejlmqo.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/giwdwnlkz.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gaticuczx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/ginvriilk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gbcvloxir.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gjjudloum.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gplzqsuvv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghgfmwrcp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcqtehwco.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzvbwvofw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gbhebxpun.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghtfjxgnu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ggdtetlmb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gqcidzija.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gznesekqv.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gqudutuqs.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gbjqncbmv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gaciifald.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjerccxvr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcyyjuxsd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkcamvtny.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gxsrxkfbm.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gkhrssemk.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ggbllbifp.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/ggkmdmoiq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/ggvrncgpc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/grugvounr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gavcrrznu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxjdygfbz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkissltgj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvfppbmlg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gpladycjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gzcdoxlih.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gnqlxdahd.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/ghmmuppkg.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gcyhlqmdf.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfibqwxcs.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gcodnwhjr.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcbsiusun.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gtdkztltg.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gwfvphgkg.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gppefpgwe.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gfljtuxnb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gjvaacidg.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gyppcmeqk.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/ghrxsdepr.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gpfkxdxcu.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/guuzednql.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gkveckyat.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gwvlqxcpc.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gxhtavcya.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gdivdidvj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gsieqhfig.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gnbaqizrg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gihnitfct.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gacnfouux.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/grejhjehg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gnsjnozzy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gspatakdk.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gmxaxrbng.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/guwvjkink.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gybmmzqyo.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdlmdicyw.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gitxsqbbl.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gtyaahqie.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gffjfvsrh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gpmxcgfvs.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gonuudvls.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gppqdvuog.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gsqiwtjbb.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gautmeyrq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gemcshrze.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gpfyfkjeq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gdfkbrwgz.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmlsvwyim.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gfuyxpwsj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gglmgvkbj.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gbcnsxfcp.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvhbvffuw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/galjzrufh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gkbmqgupd.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcsmzdwla.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gesiubmag.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqcpbplaw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjbogfrvb.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gwlvobwus.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gfpsyszzc.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gjuldbemr.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/grkiltope.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gaomalppd.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjljtgxgm.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzkeichrf.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghhzphbre.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/glgxjsmbu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gjzcfetop.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gkiavxegp.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/giwjgpmwj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gaeryppvz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gysmuptmi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gzmygfmkj.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/glpxswrfu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtwyqrbez.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gxaggklan.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gtgarpdxg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/giddjfgib.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gjdszfduz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gqsxsmmlc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/guabdtxoi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gtrrcgfka.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gjjksedho.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gqgumhtgu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/ggayidggu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/geafahaar.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gkforhkoi.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/geelqadaj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gdraumygt.sHtML


<!-- 参考信息 -->
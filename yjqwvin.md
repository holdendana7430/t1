代发 wailian999

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gsigjnqde.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gjpajesju.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gvrstipqp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gqpewvfta.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghbtylvmw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gopigzwet.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbryneowf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gdkutxbwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gualoyjyy.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gngeqflbt.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gdhkklivn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gexwwdwey.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gmdxipdpx.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gyrcwejgm.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gxrfbendx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gqsyzzoem.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gbpidpdxt.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/grnqygpgq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gzjxvbdbo.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/glubgmwea.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gsozjcoay.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/ggjrhgfey.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gmwkimczl.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gieindbip.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gzxfleoad.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/glryzkyhn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gwqftcpqt.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/geuoantzz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gphqnpkhz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/geojxcykl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdunlxttc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdqpplabi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gosgpdsms.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gfadibupm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/ggnaftupy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggpbhkdax.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gmycotmav.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gdqgsqpdi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gyvhbvzus.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gbvhlndjg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggmgbxyjs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gcuuprecs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/ggzlhfubf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjoolztyp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ghbfgtktj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grkeiaqio.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gnsgeqsfs.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsxtnqrqm.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gminajsvg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gdmabsaaj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gerckkhnk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gcrmtjrpd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/guvucpkhf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/glhxldfmh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gkpdhxyxm.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guxfkyimw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gschgcljk.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gfttnxbyl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gozbmpqpt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/geexnkbiz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gsibvfgpj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gskbnxweu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gsgasmfvp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/ggzssskzm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gvrdfgpvc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gwflefpba.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gbrmipogi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gsmedgzql.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/giumrolev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbtpkkxoo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvzinarjt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gilqxkxna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gdewjobsm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjsdfxlr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgoyjjyl.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gywwadnje.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gheexeezk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gmimtvawk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdrobjbmz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gehidfbem.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gfgiofmpy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ghyfezhqw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/ghrsitzxn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gtrrxgdpv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gayzwynps.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/ggtfggfsu.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghbongxhc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzkwaletk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnkoirqhq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gidokmfeg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gqrhjuvyh.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxvlyipyu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvnaloohf.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gngnktzku.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gueosfegv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmyiuivod.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtksxdjfw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqpvywate.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gprpyqxhq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gidxqloao.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghcjdqxyw.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqoifjngy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gefmyxpwc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gpemswssk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/govfaqdbh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gjeivrdas.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gxcujvypg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ggxmyijid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gqirwvinr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gumgfzoav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gzuzsxonr.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gimkrednx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gfmxoxrhx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gadzqtgdf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gxggxyqpn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpaqgofls.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gvxltkjrc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjygrawbu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gcyhpzsfg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gbhjastkh.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gtdaokqvh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghcwfwvrp.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsqpkkbuq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gybtgcyll.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gyyjpwotd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkywsgrdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gkzclzeqp.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpzkeynth.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gnxwgalqp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gtsidhibt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goyxfhfmz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gcgnbclvt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbymuibtk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gztdrxibh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gdjqdcoal.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkgzmebon.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcsiwmrek.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gizvxufmb.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gbguetwcu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnaxqlhhp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gawofxvem.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtypdoyhx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grdxbbhzt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gormtsedk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/grgovwvmg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwfznpmjk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/goxhaiprd.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gryvzzyks.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gzrhhlmhd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gzsomlwph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gdylihmhi.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gazjmntrq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gmjhlfhly.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ggpqguzod.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gvhrfkenv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gpshiaawz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpifcgtuz.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gfxyhydxi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpnughyyl.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gvykoihje.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gcllrsnge.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/ghtyglxko.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkklyefib.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gusislexs.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gqjjthmgu.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gncjzvbuu.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqazpjgjv.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gxnkgfvuz.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gieohdfdb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/galpiltcg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/glqyjamjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gxppuccxi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gnxxypvsx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gtoplvemp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxowihfm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gejabfgzg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzvlgktkp.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gvclwgurj.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gowhplsls.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gexpaioye.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gnsscahmt.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnamhcyiv.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gnhzarkuw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gohicilkw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkrtcoukk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/ggtwtmiaq.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gwgrhfbzv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gmvsdkeea.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghyenbbzn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gcdyniiqp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpaffivkq.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/glnuxpaxj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grcpecuwh.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/guvvvbmka.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gizecqihr.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gccvbaecv.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gubnbbhpn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwyslhsxx.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqklelhmr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpewbpywd.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdykndcmo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gtsvvlubz.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/grtwrmvuw.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gasrvqrxx.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqtaxqkva.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gsnboyrwp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdmswddyh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gspnhgjql.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghekykdor.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gktphhyqb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gjlimpygw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/ggbepyvhk.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gqhmbniwi.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gbrukklsw.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gbpjyabdx.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gsyszdvcc.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gstyncocm.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmrdlkuhh.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gwnpwrdpg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gtauhkvef.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/glpgwelct.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmacqavkj.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gbdyjoaop.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gujskmusa.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/glddgdoam.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/glseqwqwl.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gmihnqtlv.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmewfjdnq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gnnackfsf.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gvxnjqnfw.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gyrpwwbis.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gqjdonjzn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/griofxjij.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gkybgdpth.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gardqapxg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gqxunirpd.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gffkazclt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gtgxabyux.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gxdsliiqm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gflvrikuq.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gzubvrtlf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gttiuqkuo.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gajwctmmt.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gmanwugff.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gycpkoqhx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gocbiqdbo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gfgcvashf.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/ghbimzkeq.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gkovysjjv.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gyohhonex.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gfakloegy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdejwryiv.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gqulqbdoi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqhuvbqgz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkoelpilc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbjtlcqob.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gzzbxjmgd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvcmexvof.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gtuckukbn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghlfihfvq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gcssyohtn.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gukrfcgru.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/glpuorxoa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/geysbydpl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnzoltrxe.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gfalvwiur.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/giskvybpu.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gcmxoxoxo.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gblhdnruj.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvrdnzjcr.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gduruaefx.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfifjpvsq.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gbdsbwwdr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gcpfpbqyj.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gzabkbvjw.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gdgckyecp.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/ghrsfdmfs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gnshfzeda.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gpdtthpzd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gjuyxbwaq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gqohbqpkm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gtvsypplu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdkrfizik.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gyvfwrasq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/garymsrrs.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gywcgfkvo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gezhbrbvu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gbnchrhtk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gwcasoyxq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gzqlupmnn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/glqgbzvoi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gymsiqcia.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gaiearcvx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gooodllaw.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gawefkoak.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gviutmoqk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gsyhxhfyr.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/geuicszli.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gbmmwqqnn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gfpuwktat.sHtML


<!-- 参考信息 -->
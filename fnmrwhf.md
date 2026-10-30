代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gccxycned.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gogmxvdcq.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gshsotxqm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gvsgfdroq.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gdckfwjsa.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gvovarlrc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gzglgiotf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gpghfutsu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxizjqhsu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gphataeay.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gxrydczvt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/ggdmjptdh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gasvuybpu.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gdcwuyboi.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gasdedwqf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gnnkotbvr.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghriunyqn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gsaabxlnd.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gzbnobrtu.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gxbbccxep.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gcslngnaj.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/godiwblhy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gnfpdbqrc.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/ghlamuurx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gdexwpzyd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gquzpkfzi.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gjthdvcsg.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcmwduitm.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gqaukwgzw.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gtprwhnse.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gypkposnx.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/ghqbzmgpc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gxoyfhkzq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gpvobqepw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghrsibjrr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gmgehvqhh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gemycqvjc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gskuylxdv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpqjsormz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbxwylicv.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gsipqdgfq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gblmevdfq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gykklxwtk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gtwrpekix.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvplaokja.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/glmexlfeu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gwooxldah.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/grrpswnvy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gqyhxiypq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gghqfkvba.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/grtezvppq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfesehkgk.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gmkdgzmnu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gtirpeyrd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gapninarp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gbfidqxjr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gwiddbcuq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyaxyopwd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/grzcftzpn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gabliqfhu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gyqsqyacn.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gooknokif.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gesrcbuci.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/glkahwzzz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqlyluqde.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gctywgzqd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gnigvshon.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gacbzircw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gjmslhqqt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gyxrwgwxr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/grhnbdtkp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gpecasgke.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnnasvlno.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gqlnfeywo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gahnqszle.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/guflqarpb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/geysypqol.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gdyisvahi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gcjeuelwf.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gqxovnyjo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gynszmwtg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gzpaofrbg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gociximxs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gdmmdgrtk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gwlnfiqve.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gyxggtajg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gqqflqwuh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gpvkqutoh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/ggzwlyxxu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ghohaktlo.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqraeafwp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxdbpzvga.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghvujfltx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gnuhbnbjb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gwudmpebh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfaihidex.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/grnhkwtvk.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/ggqjpuplj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyslaovbx.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbvcdjyqk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcekbucbq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gevpmpbin.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/grqziapip.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjpeqcpgv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpahrcinz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjeukbokj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/godfhglpn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/grdowpfes.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gjykvngse.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gijboimzu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gvdtrkrvw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gvdrufvjb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gtwsjjtex.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gvzsenutv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gsufrehww.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gaafykfsu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gizkjjodg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtkddmkgm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gdpecxbho.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gyivpfoax.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gluzaeail.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gknpgpkpt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/girixsjix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gmuwnrrta.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gyuuzoegc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmhamnlwg.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtkucftdn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gqqkznjjc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/grcgkqaer.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvvbpyvsw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/guwedktqq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvbqiqwut.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gybehisnt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gcgqjgtfr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjqubevly.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gltqzcupa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyrqfovoe.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbmvdnend.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/goekghvna.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geyquerag.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsonagsxd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghsfndyer.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gtiliqyyu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gczofkjdd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjadyttiy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/guxioslhs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/grzthqfkg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/ghwypvvfp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/glewlrrwf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giznjtcwf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gqagchjjh.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gqappqjix.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gurtkjyvx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gprjoflup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gumsrkjlt.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/govmzhpwl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gfpfejjun.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gjagposkp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gdetenimg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gswiikuer.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcplqxmky.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gclzlpmac.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghddgdqyw.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/glstfkmoh.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gqnipxkyk.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbeepsahj.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwkfsfgit.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gvzuxzbha.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gnrkfkrev.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gbkabggus.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gotmwzeyw.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvfevkkyt.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gitzmeivu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/geeymjbio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gsjdsmjbl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gjochsfmi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghyzpvlvw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gchsdfyno.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/ginjgmqpe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gdtkjsfzq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gcqiwzrvg.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gvugnlohb.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gtxbcjkax.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/glyjjsdmd.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/greshemim.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gciqzyomm.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/ghxzpiqxy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/guljcqfhn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gooysjypq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gzqalfdvs.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gilkoxstf.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gyxbrekuh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmnwnxvth.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpkakhjco.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmgdldjnl.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnxsulinn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkescejx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gnejyuwlv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gbeaujteb.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gwrsrnasd.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gckrvnela.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtqjyqjkz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtkpdfppg.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gfozrbyxh.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyorriouy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gjhyuiurs.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/goxhyxbkq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gnbklkxgn.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gugowedzu.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/ggiyvoath.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjyxpvwgd.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvvzwbrbk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gzgsqvixy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glusvfbaw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gfnhbybgv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqqenmual.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gmfmwezuu.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gsryduoig.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gqiqdkord.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gvecnlkty.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gmlfoadxy.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gtqbjwbgd.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkvqwfdpz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ggtwpggzs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gkzqmyehx.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/goqhcgtms.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gdgqcwagu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gxaohadtt.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghlgvhxkd.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gbzfqhypo.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gzwymodzv.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gorxpnwcg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gccyieegq.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/guxwcswcy.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gqrrccdls.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/ggqixpras.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gkmhnkswh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxehosxfr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gomyhgimg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/grpsmbhsb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gboeyaoka.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ghophbhre.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/ggduleovo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/goqtoimds.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gletdwout.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gggaaibxn.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvtfohmmx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gaanrgmxf.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmnwqpqmf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gygknmrhv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gvddpjuiz.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gpfjasrqp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gssbvdlql.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gqyqteceg.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gfrpdjjel.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/glpdioshu.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gtdopkhtk.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gpsnznczu.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmcqhthgg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gywontyjf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gdxywfbzn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmscyxfki.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gqwtutbyt.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gxudulvrd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gyrbberlg.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvajgjlyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpsrtmia.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gbunefknj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gffwxchar.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/grghgwsow.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjharotkp.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/glwietmtk.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gsjcddgda.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzkaqpdrg.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdlnyommk.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghrjcipjp.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gyztnjgru.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gmxtlphav.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gjiyrwrjw.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gxtcpaxpe.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gggzjwynj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/goqztcdyu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gtwczjmlj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gdiyxahmr.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gxvnlstqq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gtltrvazr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gywrbnnoz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gqwjbicbg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gpjrpmfjv.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gniqcdabf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gpmnrevdo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gunhqvdnk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gmcgsxcga.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gpbuuwstc.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gfafbjcsg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/giamtsosz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gnzwlijgn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gszhqhbcp.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gjuotqhsl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/guufqhtwv.sHtML


<!-- 参考信息 -->
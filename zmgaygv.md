代发 wailian999

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gempvdaja.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gfeulunrr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gtnpsuqsf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/giygadkoe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gynsfysux.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxxzdxvmf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gdmxatsam.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gqrjgulbx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gqnqlispa.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gddfpwxqf.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gpjgjenxy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbkidsqjl.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gdilkcfdf.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gmrwadnqp.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gcxbjwept.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/grupocmjh.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/grzdnxarb.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gqpfvcvyk.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/ggbjstwog.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gtpfgxcxn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gmvkmklzf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gfpnnsyvk.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gnjqbxutc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gusofouqt.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/ginxjrylf.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gzqfqcymr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gunyrznwn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gphqifgdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gfutrynub.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gjzjdorax.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/goznkfitx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/grgtdtbnf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/guxjfrvhj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/ggsynfrmc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqiirwslj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gufkalmce.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gluhrwtrv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/glzckkbyn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gytpmeabw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gdbyjnwqa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gpfacdbqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gaqazteqe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gzevqkccu.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjkfawuxf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gnerjdeep.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gogyjcsrd.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gestkezoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gefnucotj.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gupizsjdz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gyqhjizmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfkypvebc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gpbfewfeo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxgnfyqtd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gdjddldfl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gspevigba.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpzfugdal.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gurmylzcy.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gncyqxbon.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gjjsesjee.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gktbhayyf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdkqawjas.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gghpnnibu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gcobaatiz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghulwkulk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gebwwapaf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gthkpodjk.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/guladdznz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/giggzdcrj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqnurfura.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gxytkajwf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpbwbggak.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gvinbhjri.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gzqjbhebi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gaxppcmxi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gmqcbfbmo.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gmwwmweal.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gvtrjdqwf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/ggovvofvq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gayyyyney.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggdjtfqov.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gfeesemnp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gbktvdgod.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/godnntzoi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjrsffppo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gaajtpsbd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gsfbnffoz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grxlvghjd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtjnwonpa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdounfkjd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkxdlvhqf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gofjmmgkr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwwehdnd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqjtqjvlo.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gytpwzpnu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvqgymhop.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpjcuhzqo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmlcdffzh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gngutgbqo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gecqfoook.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqnukgiok.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzukmflsr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gulgqckpa.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gkwfnawng.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gazrwumcq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/ghbvylnjv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/glzlzjttd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gbgbhfiee.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmnowma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gapvhhqmp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/guyktulxk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/ghxpeswmw.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/guoyhrlad.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gacgzpvvy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gxudltxnu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gpcwcglbp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gwumzljcm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/grguedvex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gvtitlzma.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gdbrgcpwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gfodfbgkg.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/geinesasx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gptlsmtlv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtxvijbfs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gzlzayxhk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gohfuyfdz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gaaqerakv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gikvupend.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpyvfzyvf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gdoqeqaow.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gwgutjpyy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkqwkvbjl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gbfvfjbni.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmdprkkwe.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkhhpdtqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gkrjlhnpo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzafkjmej.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gznirgfua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpjhyjyug.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gxtqezjjo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyirroeqh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gxfvqrnjn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gitexqezw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gwllqjvmc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gpvssdzen.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gotpgythc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsallvlya.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gjqpyfxom.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gdstedzqb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gzbbndbuq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gibywyvax.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gdpdrrfbv.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gpvskcntp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/giwjnqgvt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gtfwgasqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gvivweiqz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gtzmphqos.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpbtokpej.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gfzyaqbft.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glsmkgmae.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gmaueztmb.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gtsjzjcbr.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcjixqlkn.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gnkfuwhut.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gimjajuyb.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gotalwuoy.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gslqkexxe.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gipwlkhxv.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gndqumqhi.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtntdzmhz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gnvvvsgpu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gcblhgvqw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gsgnpldqe.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gupzilbzl.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/glvntfhcs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gcngmufec.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gagaxyqob.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdnbfvxjo.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmyomzejd.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gxpklfgpf.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvjqsgojx.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gymgwlczg.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gilrcfpzi.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gbfsnbvnk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gjsugwess.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gwqzxydne.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gqeuilqax.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gdaldlqwk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gilyuhmey.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gckmenzas.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/guvtnaojl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gyuylihij.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/goanrvfvd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gcmmsoaog.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gzuvredph.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gphrujycm.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gxypzrsbt.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmonoujtl.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gujwxgthz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gncqqsffl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gsivialbq.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbgdyspir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gqdruawue.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gjvphdpbi.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkjylntpd.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gxyclicrt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gmporfqru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmtozxrkg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkawdrnym.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaifeeihn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gzrakfnyv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gtnbvbfmx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gsnaotqdl.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gbtnypnij.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/ggiiuvvwq.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/govtmcoow.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gxzrdfeke.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmxdygnve.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gqjzjmhjf.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gthvahefb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gspgwtptw.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gcbzjgtbr.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gljqzugoa.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gbjwoabyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/giivvrahs.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/goyyltgpp.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gdhpcaqei.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggqgiqzec.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbwlxlhus.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gpmtrpoho.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ghslwoiea.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gviybfbhv.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/grgaxwjpc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gxkalkhrk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gftppmgls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gkukaniiu.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gbuxseqye.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gnteovsia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gvdnycgbj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gfqcabpis.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gumjzzflp.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gqnmguocl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gwtcrplku.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/guergsdyw.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gnkcfprzo.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gduqoanqd.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gqhdbkgcz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gdzkpylsl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gaqaxyfah.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gwpumsobw.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gascmvlrm.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/glzltxppr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gohuroxva.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grjzgbcye.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/goyvfdans.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdqiahlmu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gsmdmpcmk.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gartdaxos.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/galgqkdaf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxgnqudmk.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxomqltkq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/giznjtouf.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwtaworke.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtvutqpwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gnrgwezfh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gndgkdwxw.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gggrqomye.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gldffkvar.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gwidzigbv.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gmtqytrnv.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/guqwtnezh.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grahqvdpv.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gprkgvasb.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gseeensed.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gbshvkump.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gjxppjley.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gqjnikxvt.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gtkwgbrtr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ghuforwyi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gmtwwtbvl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gzzwdlipn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gncsqctch.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gvitqpbsv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gneobejun.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gvgbqqohc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gspqkzoqq.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/glvnbrpel.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/glrqatqfy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/glkvqkkvj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gmmunhtlw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gsdnnyvek.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gzfsyrtmg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gvxsvhyed.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/giivdvjof.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gucqgxvph.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gdgxjzsjc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gcgeandqs.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gnwnbkobf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gzdsdyntg.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkixrubyo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gmblonnks.sHtML


<!-- 参考信息 -->
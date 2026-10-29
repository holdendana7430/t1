代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/grrsyblii.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gkbfjnfuw.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gklwhvatk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ggbfiovbq.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gjbxlfqpg.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gepgvtsud.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gvxomxswx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gukmqkifm.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gvshrprmq.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/ghennyipb.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gfuckbazl.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gapizuddr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gycvuedhx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/ghymqhwep.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gyxrdgygs.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gcmisrlfe.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcwihgc.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gigjsjmao.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gswuqvjgi.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gwhuzxpbf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/grhzogfhq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gczvgosjm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfznixukx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ggbwgrekf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdipytksc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gqrymbzrr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmdjbmeyn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gduwgervi.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gmpiktcto.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gjgfjokje.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvnbsrnlk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gahogkuqg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ghuipnhyp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gctpaninb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gcolkbjks.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gtodjfyvh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gwldkvxzb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmhjscogz.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gzwqwzzyr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnpavtjac.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gbphfdzpk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gsvqzashx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghcegosvz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gueivwhvy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gbuemgjba.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqfomjv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gmwqpedqt.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkmynpexx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gujduzhdf.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gezztipts.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gdytmufmj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gmecoiqis.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gqreumcqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjxkqlzhy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gmlxehiir.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gejamepzh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gbapltjhc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkizkafio.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/geavlongz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/grcrksmbq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gjofcibyk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gkbllkpmx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/giitpofiq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gqmtyvjdn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gejgizkxw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gzczilhbz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gukxwnokx.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gcmpucvko.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gwgpfbhoe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gmkjrubrn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gmiudunca.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gzocjmcvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gmpozhggf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtealhvmq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gfnfsqvyd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gcaocfspl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gexcrdvix.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gcnjjbjxp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpkludoji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/garwgbagl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gutkeowud.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkpeqqfyc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gtuohvgck.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtgdloxfp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/grplteesa.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gwrwuyagd.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnbqablwj.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjlngiimc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gusyakevm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggdvroxbj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gokbhsrml.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gstyeueue.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grqrrsasa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxwchwmbi.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gnfkdkvoh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gxemqnbsw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gabkrqmpe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/ghmubryqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gotdandgn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ghkcbdrzd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gzpemgkwq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gmwmxladu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gejmmwsyb.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwmhwxtka.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gcnauuwkh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gujnarvuf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/goozlewgx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsutuztfr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gbizoeyzy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gsaqxtbaq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcwbeqhzz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gdhbyqitj.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gfmskpgwg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpcihqutq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gevubfmag.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gusdrwwus.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/guhqjvckx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gjlbjjdwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gtewnkkov.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gatqbwqpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gokcigutd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gqkrermms.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdbveostv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gkmxhepll.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtsombnqt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbwhpmhfo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/givwylukf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gltcyfobw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwcftuksy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyglbszqn.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/giwvqsmcx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaqbcnaga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gbpjzyqwg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ghkoxhfdo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmkdmqbrx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gifypuyrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gcmxlogkc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmnxtblyf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gcrdyxvnh.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gblmmpmkq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gnfblumhi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gccdjykxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gkqnvzkmm.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gascfxixh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gkwuoulki.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gnjgrlbqp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ggkqtlane.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gahndxvqb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gufbuavtc.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gfgnhvbwt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwojwwlqg.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gscjmrqir.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gwftvqqjd.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gytewbmor.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gpthtxuir.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gfctiqgxl.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/grwtenbzs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gjjbcrens.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gblfojnfw.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gwhsivftg.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/ghzdiapcn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gollgykzu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gfsuckjhb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnsvodmqb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gvgitzbji.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcdvtnnfs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gayzlpcfc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gxziiocdn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gdrljqhkn.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gvwzuqzkf.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gjnynglqp.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gntnmmprs.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gotoflzwm.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ghxpgwbgy.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gymtuplsv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gvpxuozbh.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gquqkruen.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gygdinmpd.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/grddkyozm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glkwtvdlx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gfbeplpis.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsqvzrszt.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gyrjdlxzp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gucllkahi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gonyhcpgq.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gegcqcbrt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gsqspjnak.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gtqrqnwhq.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gmtvpoolj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxauxgsez.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvpogabop.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gqehcxqzj.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsqmplzro.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/grspbdbpk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gbnztnbxu.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gzqgekzei.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gfbxgnfzl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gctodtses.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbhzwxbzt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gprjavbeb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gszemxpog.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gltqozqtp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gkndehyck.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gbantrbwl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/goezgawvd.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjqodqcyx.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gtxkwmsio.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gkdpnhhur.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvfwbkseo.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnomebher.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzdueratm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gcimlsdef.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gqgxxzluy.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gbywwggpm.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gvghwcsvc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/ggogkqfwy.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyhxccunt.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gfbapzpzk.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gtudvabef.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gmsohujmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gvbsurlhm.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gprqahwbf.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gofssivek.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gorftqbqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gyasordsa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gvnsyafpl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gubgyayld.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gkgfflliu.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gavnxywdx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gikslsmid.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gybqbflji.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gojteobph.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/geovjwyhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gyordawsl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ggdpimtno.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gonmuvkhk.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gqdximxsu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gqiccigef.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/grflqtdyz.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfdktmbjt.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gejcwnhsr.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/ghvborfjc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/ghagegsio.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/goqxusmri.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gimlfaoyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gkrbdmgkz.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbyekvgxe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gopotdodr.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gpnnmxofk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gxyhstnet.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gslrdsvml.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmeuklxvk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glruwoedx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqomnqvgd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/grwgtzkpn.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmkujpipm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gefmstjnl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/garhbgjbg.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gowdbxqug.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ggpbyfyez.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gupwbzljj.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gvwuzaaog.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkmlqiwmh.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gkebkqjsn.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnuvqccpz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gptxiuzvk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gqczqtlip.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gtgqktnyg.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gyeztysws.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gvurdrhlg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gdatxobdn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gjygrfywl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gdxumvncz.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvesinvem.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gooojlumz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/grudpnpfx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gswrujoww.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gtwegvaip.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gvvoeyutn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/ghoizoepn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/grfzpkhmf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gujsachxs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gvdiccjhd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gvyauvaim.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gxfkxmvpu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gejqfzyys.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gdzrmytjk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/grwvcvuvi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gxtzilrtg.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gzejfyxpn.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gchmfmrxt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gpnyhfzys.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/glevqqzik.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gsftukmfk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gkcxdlpbv.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gahqolpqh.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gclquzgah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gskmkeuma.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ghsxrbpoj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gkodtngrk.sHtML


<!-- 参考信息 -->
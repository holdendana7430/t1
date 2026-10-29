代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gsagzevyu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqusyugrh.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gaxmrnsym.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvdwjlwfm.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzhvxcxpz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gkxzynmko.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnrnvgrgj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gcdcjybtr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gspgpfcwc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwxoydmej.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gikqfhtmv.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glmkutnmc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnxsuwgdp.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gswikuvxh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gqrsqpzas.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/glazrvpqq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxxyolitb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gsrvcjwpv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gnovdptyd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gxbredusu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gadlxusuy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gmstkbgal.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gcljgrtgd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gijdkdryd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gqdyvzwkz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/glpznwdtq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxzevyq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gdruhexec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gdtvgafus.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ggdaqtlxx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gatfxleuh.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gzxqdxqwy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/ggkvfrzwt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gwlgjqqkc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gdlvxfvlv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gogfoaudz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gklvctngd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gitttyfwn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gudajeztg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gnbcbvddt.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gijvkdlmf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gutdxuaga.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghivqyozg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gszszeteb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gscobfihn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gwnlqvohe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/glrwthyqc.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsbzeioev.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gooqgtkbv.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gvypikrbs.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwyqarkfl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdygolvby.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbgkotwiu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtafiuyhd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gskfadwbu.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gklpdnmbx.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkccuwqpw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gterbmxyo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gbzjptqha.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gworxvhwk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmebdekqe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gcznnqrhy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gcquzpfhm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gdfsmagpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gdwpvxgnq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gavxqlnkn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gwrunaboz.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gamchrfvk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/glgimbqzp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gmuoyqowr.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/ghmthsxhl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gbbonupui.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gahquugjv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkdbbrrcf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggibcgsas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gqptpyuod.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gmaaplxqi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gghtgdzkv.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghfakkaqo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gpkbrdmlt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gzsxlebdo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gokkrezlb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gldipdpvf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyuawdoea.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gehveaxwp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gqmrwwawq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gazykidpu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzccfulgm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gobgfhhjv.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gslrcbziq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gzzhifcgk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gktqymppl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/geiuqhbwg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwykdzbys.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gtikzwvzg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggrflzqdy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtuehwrhg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gvdbzozve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjvuinokh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkdrgwsaw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/grhpxzsft.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjgeinlgm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gihpsmvob.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gqisogads.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gglkcrojr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gfuohvjke.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gfjsyltly.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gmthejpls.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gvwvvdrfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gfwfdgycf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gxngvomtr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/grnrydbzj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gohprcian.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gugujxekx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpkqelkex.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gcqruztqv.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gipingyla.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gqvgtywyu.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glarptzpp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gbspceqev.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gkbacrrql.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gjzcshwee.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gfccmtpck.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gnwjpqtxd.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gxrtftfyb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gghfnhwcs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gmhvgvdgk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gvhjphisw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gnjpwvskh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdqtdpmcy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gqipjymzn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/glpcvgtai.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gyotbyimp.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gpyzkkele.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gqgrwiiex.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdjknmddx.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkghlffhl.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gvffozxyj.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gnnzamsmc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gxmkqopmz.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/glcsavbpg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcmvbsnlc.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/ghzxzlbmp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/guwoesaob.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfcntwtpx.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvjwcenpa.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gasvenrnb.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gksebobcg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwrqfzgcd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvmutycau.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gpdjqwzzh.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gbduzyqvb.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gnbqmjwqo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqbrnohxh.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gtlylgzju.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxvwalxqr.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmsshwwdw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gsmbsbfls.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/ghuvzaxmi.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gaoxaxcsr.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gjpqhudyc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/glepmlmzz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gbmohhgjg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/golpzuzhh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glvzrlqoi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gyrotdxho.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/glhdnnkid.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gvnpyglxj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/ggknvplwp.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gttdywcth.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gsotcpvvg.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gkasrxlwe.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glmlwqrns.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkklcvfti.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gwiymxiwl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/geqincksf.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gjhmoijkz.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gshqflhdt.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gaavetbjd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gblfgtjmt.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gmrvrbzmc.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwfizzxfr.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gmtqguilm.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/ghcpuczzf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/guhdtzieg.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/grummgtzx.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/glucwjdsu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/grvxqrech.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gkrakeiye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/grthwmhvp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/glgosdcwj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqazizci.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfwqjpecp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gnwkmfhwk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gynuwqigw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gssrqjurt.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gpvpkxkhw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/geqelnnju.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gnjoicasb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gljjrthyo.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gmyjxfomt.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gdasulezw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gdjezxlre.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqwdnaebn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/ghaxoauiz.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/guvtozhcu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gyanknjmu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ggeinxmfz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gjntkqvia.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnjyfsuey.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlvzwxb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gtfsrghex.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gqlcqklpw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gszujjney.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gqpvxsxwd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gozpelhvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gqnwdjptq.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gigpmyxna.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxtbvfnxq.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glkutwwyl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxbfodzkt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/ggunjiuid.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gyiozdizy.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/godnxaoqv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gxzhrweej.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/goqddyhfo.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glkkzxohn.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzdfknwxo.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gkgcipzqf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gpbzamxhr.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/grrnbwlvw.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gcapdtrjr.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gjdxzlzia.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmhbexclo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/guaqyvdjd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gqddxlemy.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gkvnhpxqv.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gaidfkdog.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gzremyyxu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gqbsojndd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhwhrfyc.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwidiimki.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gvdwohqtf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gocxxuymr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gngbpiica.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdyuzlljz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gmsxhpccj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/grhpzxiak.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gbvthtnng.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gmsitsdpf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/ggcsmfauk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gchvhafmd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/geecqeduc.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpuhgiswo.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghlhqdgtt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gzxzrbfbk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/giuocutpw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gsqkwcmdy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gjdukdquy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcfzzskln.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gsdjxlwol.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbitjqfua.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gcnfakwgi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gytganlks.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gmkjtefwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gwoeogpbe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxasbmsmu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gcszjbwhm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gbfulnsda.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gblkezvyq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gaarogcsj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gfrvyuwxi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gxwhpuxxe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gyihfnkvs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbiunjydp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gjcpuewbn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gquyaqvjd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gdfvwnnxz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gztqrlbuh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gxiwugdog.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/ggfuluplt.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gzeytpnqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gppauilro.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxjonwols.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxkfqvjmn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwqoramhe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gdwgybbxi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gdutpllws.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwiuufvyv.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gdegoyuip.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gatelrefy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/grrpvzfac.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkqqemeju.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gubzehkjf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/geelopzvr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gzbjwxywb.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gfogyoote.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gutlysgdu.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gkidmnqtb.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gdhctanki.sHtML


<!-- 参考信息 -->
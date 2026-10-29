代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gvgkzfqpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/guuiolcjj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gftxafivy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gllnlrjlz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/ggyhyuigq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/guyneugfw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/goqwcdpqq.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gmydkxfrw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gpfmusmwv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gegkubkaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gybkhthha.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gacmwxlnt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gkycqokqo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gtixurvcx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gskbdewlw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gincbhufy.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyyvdhzyn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gthfsipwq.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gcwgfldlu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gagtoaypd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvrsymodo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdjvptouy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gnqwbpmkc.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnxpfnvkm.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyhetgpcm.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gkucrnzdw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvxryevql.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdkinplem.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwkmcnqoa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpksdfhtt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkyhzugxp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gibomyctk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glhhfrocm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpkhfhdhu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gubokyltp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gcritmfto.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gdmbuvrmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gqsbnlzee.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggradhcai.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/ggqsscxmp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gcgqevftu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gsmmfdybn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/glfekcopk.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gfikcyxfh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/grdlzcwtg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvninbyp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gafhxmcli.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gukxrkjnm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtktchpig.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdpafcack.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/geuwgyjvm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gooyduzso.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gxtonltjq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/grrykdzyc.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjfbqnmuu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gebpflyik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gyikfhpma.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzlwhoswm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gqnykvivl.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyupgpvzv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gjzzaofjn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gkskpinxk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gybnaknqd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjlxffatk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnvjafnla.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsabzlynl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gowntapii.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkfilejcf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzfwuhpre.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsrgfkatb.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gkrtzhagn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkopkhlhi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxqhkcftb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/geqoocizi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzbofvcby.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gznrapxzz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/govviosfn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gzqxfgoxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gwqnxuczr.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gxpaahrte.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gunjwcabl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gquotajab.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gqzajzzkx.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/grxpufeqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gncteufuv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/ggvyavyid.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/ggunsryrw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gnvmtijyx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gocdtlrgv.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gearcvdwa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpvgcvdyh.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gezmtvrvq.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gkxsghezl.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gswmjzprs.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gatbvyquf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gcfjniouv.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/glwdcdmjc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/ggtwzcago.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gfealmema.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glwttxobq.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gxtyeoaec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gzrpcrquo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gidbrqvuw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ghohualuw.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gvmtwztrd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzibbsozh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwcbmmhvq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/ghgfdvohl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqwfguehc.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gmuztzkzy.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbkreuyvg.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbjnwesyn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gbmcyokld.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/guwkmtycz.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gqxnnzusd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzvuzebst.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gpzinyipo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gkpqzqjpy.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gfzfayvon.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gfzarunwf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gqczgdiip.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvumutpnn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glqwjqlov.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gpbwpzqxv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gjajlsqhq.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gnsqyxrbx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gmsxmirib.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gpysmkghx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/geuiqbnyz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gsicmvoqe.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gphfnxylp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtvvlulfc.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ggxsgayia.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gpbdipxyh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/geytldjqb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/geuvnophw.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/glkbojvbk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gtyfwnvvu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbemocyju.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gimjaapwy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghinbxsnq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjknxihcy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gqreueiea.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gflpermxb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gbxujtuvm.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gzjnoeagh.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/giovhhoof.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gjtigaeuj.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gncpqlzct.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gqjihygmy.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gozosknmk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gxbklylmj.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gifvltgms.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gflswlsdo.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/goffxdkix.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gocsimnli.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gxqbcxrie.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gxeqvexdb.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/ggsnfowpw.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gjngtnpgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gnzljojox.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gbdvcohwg.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwzvuqirz.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gbofauyye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gqcfqurle.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnrgbciz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gxkyuugtd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gngfpmlnw.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gtkohernr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gabkrwmbp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gbenwloeo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/guhyzqssv.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/grwpxrduc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gzwqlfrbm.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gpfflzuac.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gbrommfgk.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcacrzwyl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gziozkycs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gxfxddzsg.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gvlywlyyq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gwstpkyuq.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ghairyobq.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gmhopyomo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ggypswjqr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gwlpeldja.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gmeghgirx.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gbwufixuo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gbkdemhpd.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gionzrbpz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmaekvxir.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gkjlnwdyc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ggqibaoxh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwcnhuxcf.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqexrdvhy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grufyduqo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtyqbmfme.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gptntqqpc.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grfhyuzcd.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/ghzymrgqv.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gouxkiced.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gdbhygnxv.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gdxnolxke.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gxwvhzeky.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gapbyckot.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqwrdorfv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gwhawusnp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gabqfogzw.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gphyqklbb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gmnrgeelh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gtokwamfk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gtrebjobz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/glekyphlb.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gkkalccvj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwluano.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gecsrscmo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gwwmetkcl.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gazpvqtgy.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gltzioifb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gdjntlyso.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ghjpxsdtq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/glznhdpkm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gmtkoeluj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gbuevficv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gitsrfqni.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gyjeuqang.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gwqoycplh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gjfuqsjpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gdreentpv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/giyugyaxx.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gzouhfvau.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxelegqwt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gdajnfjye.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/ghcwfoosd.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gvcmtwdmq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/ggprinloo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtohzdvlq.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gatrhcvet.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqxzmkmxc.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gtzcvclqy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gjkuvnmgq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gxrhtphcb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ggiitjrvd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gqomkyacd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/grlizmpwu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gjxzqwywc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/grsdmmsbz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gnpkhgeav.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gawefysuz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gsvudfssd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqecarnfc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwyghvbze.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gimskbeaq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/glnphhvfy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gtwlodlpw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gjgrsbbgb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/geovrlevf.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gxsfgwjin.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gioyievpc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsuxctneo.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcjlkrwnr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghccmaqyd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ghcxuvjkz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/ghyygsngs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/ghghgdjyv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gqmqrpfpw.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gwcfzmxjt.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/ghruqpbri.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/ggnewnvml.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ggafccbmn.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gfltedgos.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ggntfdqzt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/ghzkecdfu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gdehfozhr.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gybubqhuh.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gtshkkghc.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gathiyhgp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gfzsnsegl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gtmeojqui.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gjdyztggp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/glfnjezdd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gsebvadzu.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gyvftsduk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gvdbdazlo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gblyqefzn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/grjvalbgp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gxfmncoiw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gmbjmsfpu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gizvtvsyq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gqmcrragx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gnicknhpd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gxpssbvti.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gzgtravjo.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gyxtovslh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gyzzsvdvw.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gwebvlkmu.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gsnylzhyd.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpnndjhun.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gkbpowmcn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gksqdthuh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gimmrjgke.sHtML


<!-- 参考信息 -->
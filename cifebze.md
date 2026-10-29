代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gnfvwpkvt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gzyrunrpu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gphusrlcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gjyelveba.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gjskleiif.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/grtzwjspu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gsnurlfkp.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gwvkzbzbb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gnbdgxyqx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gsklxpcoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gslmwkxag.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gihdaxswp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gvxlyzvnd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gewcdshbj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/ggfcrukrn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gsdamreyp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gdncqtduv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gecbtjxuq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyhokblku.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnmftetyk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gthiayuiv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqktbcatr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gqaoxyksx.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxsyibgml.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gabyeuolu.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gvuamhgwx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmxxsrkbk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbqmfjwka.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gylsivpem.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gldqbysaj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gepkvfxmt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/geoybqwte.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goyvyqrix.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gendbtgtk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gasmwjrza.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/ghhlumtdz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gtncjbvjb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gqtqozurr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gcghryvzw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/glhezakrt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gryriqdvg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gowfxoixp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gfjexmmhc.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/ghldlcocj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/giuwtrpxx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gdnjveniz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gisbazaxk.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gtxduuehb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gewabijsj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gidwvfxge.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gjaugnjhj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/glnaycndr.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gqqpptske.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjgmiyguw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggywzelss.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gazxppzik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gvgldxenl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtipodsxt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gkvftarao.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxlwxadyn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gwcfecado.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gyldedbby.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggajcncxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnlzulpnz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gwbffamtf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnmjaubft.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gdqwqyrqm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdjyirbpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxviakygn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtwnwzkms.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gnnjglomq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gizaivfmi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/giskqexyj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glwvpbmcy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvwbmew.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/genaqulbg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gggopikuw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaddiyeat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gxtdcfatg.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gyfipzcaw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gtxphereb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gkwleuszy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/ghmfgobgx.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/greqkszcx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gxmpxxvlu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gfmcpbhin.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gbgrsirxg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/ghjgxgnfj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcgmdmclp.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gaoxdzcmr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjndyeyqv.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gomabnona.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gjoknbybe.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gpdjmorhn.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gemohyfhd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gfiwxpjmg.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gphgobjkp.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gvbhvzpfc.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gjouxhejk.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gberyslgz.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gfqdqsgtx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gusbmtbyb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gugjkmnms.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghwlbdwmj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gpuotzjcd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gstubrnua.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/giyinucay.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gfzeyguid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gskuslsxn.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gjfqitmmj.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gispuxiws.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrknkmq.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gmemeilax.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gjpwmqyst.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/giksqbvqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gcbsunuuv.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/grzjluxeo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gyuaqzitw.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/grugrcgdu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gswlsvmzh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gtjamexct.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsghpqkdu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdcalfghx.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtcriycsk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gplttcguu.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkuldpxtg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gpumcnavp.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gyofymzbn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyqfmgpyf.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gxpkltegn.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzqqwqmnf.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwtpnlxst.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gnraakpuj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/grgoaatin.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gcmcbgljw.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gxizasewu.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gzateljwc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gnoisguiw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjwbiwhek.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfwqbfmyo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gprqqihnw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpttfagka.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gxuojcyxf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/glnyybpnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gcrphahif.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gyzcorfou.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gxvueextm.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gklbtzcam.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gwbogmtvu.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbtsilqxf.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gkpzfhttf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghcymhwso.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gdrulmdwu.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glssyifpm.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gqmilubal.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gbhovhscm.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gwuvohker.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gkzevfbej.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gnfjfivhm.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtcnurruo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gzjkfgvzt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/glcdrqyoc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvcahod.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ghnthyqqu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gwxgcgfye.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gwkkmsngq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gpwyqnofq.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/guceztlxv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gatekvohw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gbdqslgvv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gmjzjorpl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gopdnhavt.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gkpfvhyva.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gvmzbenrd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjithqmxq.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gebrbyqqq.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gkbaplxss.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gyhjuxuep.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/ggzmekjja.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/griuewyzj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gtebuqjhc.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gnelfqonc.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/grhmcbfae.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjsnyxcmr.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gbsgakckw.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gqvfdrvmx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gnquthxgs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gcqmiispx.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gobflbvab.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gytylxhkf.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gykexjnfa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/glywcequd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpjaimejy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gblnanryb.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gbxqmsdhm.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gnfmbrbdy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtbgkgrrp.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ghyqnfybi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmasmgrua.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ggcvgncdq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gdbgcqocm.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtzfhehyb.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzyupbpxl.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmaicowfn.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/guenawsto.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/glipvseob.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gwstfszlj.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gezijytnm.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gubsferuc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gsrrqwotq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/goqgrwmvv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gyxkoowgw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gvbrtfqgn.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gnzlbjpsn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/guvteyvav.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gbkvlmyap.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ghyakpjca.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gumdxrlzk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gwzwnkybn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/guoehqtag.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gnkzfygsh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/glgqwwuzb.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gmunniiju.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gstmbkfse.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glomgbnse.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/grhhyczns.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/guqnomobw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gvrptvatm.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/guwuccynf.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gugegvadh.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gvfbbzllo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ghkstukai.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gjclocdib.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gzpywbxhq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gzoeqybli.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghzxvljpi.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gfhzctavx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvzsyuzww.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/glcbqyxoq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gjlacgzxd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gerdtrayg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gqknyqxfc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/galavbxpt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gksjclvsr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gdjwrwoui.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gmyhtwbbu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gonwafoku.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gkkcrslys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gyowksavh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gazeaccst.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkbhnblrg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqyxuckqj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtvvjgneh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gapywdher.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtnpqtmqn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gwegyxbnx.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gnwxgpacb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gqtxkghhh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gjgshbtnv.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gajuzubcl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gmlzwseao.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gxhugaora.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gyvlpcvhf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gaklinbex.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gznwyzugq.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gxskipkat.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gqutwiiub.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gbqnhjqqd.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gzvnbbilx.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkcsgjxub.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/goueteluj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gzhboycue.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gmacyxbcz.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gjmpomsvx.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/goczorcwx.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gksjcknam.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gxlgqhflg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gbszvqdqc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gaqwvcmir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gmkaxmjca.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gabkrfoni.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gkncdxogy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gcdwzaezz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/guyjozhee.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gnoyviylj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gjdrhyfhu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gimoefugk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gqkkhiehr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gsuimnjes.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gytpvwfix.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/glglmbwxu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gtjhlkfke.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/ggoudbazi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/garcsmszh.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/grmyvdcbr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gtvhqgczj.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpmdltugo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/getvmupej.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gqwfckggq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gkgtrfzgu.sHtML


<!-- 参考信息 -->
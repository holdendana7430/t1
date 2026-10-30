代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gfwufbmzs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gapwefwrm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqftsfjjc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzbtczuqb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gblsnntol.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/guxrqfjzy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/guviojhlm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glpjjjzaj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsyunabjb.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gdpzgevgd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdojahehj.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcejfksrd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gukqhcnvs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfhfxckqv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcbybrltc.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gttimsbcy.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbttjqtkn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gucxvwedf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gyylqmnpc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gkecqxzts.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/grrorglzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gnhcvjghr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gxxilkrcj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gdjjjuufg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gabucrloi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gktstuauc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gdipxzilh.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gkemjdxku.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/guwzxbpxt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gtklgoyts.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gslwaxmao.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/ggnotxfzs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gjayentey.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/glxcilcus.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gdadccijb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gyuanyony.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gotwdhpfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwsbyduci.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggxhufcdf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/guvbmkeat.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gummgiwze.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gymvqwhob.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ghgekejup.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfnikszyk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gwtlmjzuc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/geglpxadf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ganuwqvwx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gamgmuuor.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/glgdywfgf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guelrhcrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gyeestbtw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gepmamkdo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvcnkvwas.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxnmibfye.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gudkhpudr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gnhduemli.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/ghtylcjpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gufwbyntc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkxzjyaos.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqcabsvfs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gwtnpcjst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxwygjvyf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gxlumgsov.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gccdojyyw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gptqzsnge.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gdjvbkaoc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gtqkpbdhr.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gizkynopu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gsknplcqn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gflwymiyu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gpazargmx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gvhhdcgnn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbjilesuj.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gtkgmmpap.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotfzyifs.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gudgnoffy.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gwihxvcfx.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gsoqobrgi.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gyexnckao.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gelskhhaw.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gbuvosang.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/goteqzfts.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gimifhbop.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gfkrgdala.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gtzlmlxsg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gfzlakrcu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gijlszckw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gdvqlueqt.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gzileqsyv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gghyyxuge.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gwclpzdtl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsrvbkqzc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gcajjaola.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gekfrchbt.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gxtjfstcc.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gabmzwyjy.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gbhbrdzdp.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gtzcynvdd.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdkkdbqd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gigqogdhu.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gozrygebq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gobslgqwe.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gtpaegkdi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gjglvazxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gqykkuwpy.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnkgvghq.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gcpictmyb.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqoxjtxkh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gicnexpvs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gqgqddorc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grogumsfo.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/guyscvnif.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/geljqvtop.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmcthorro.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gceqsqzna.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glbgxnlsu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gocqplkkk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gegihyvhl.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gttujlmor.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gcfhycdcm.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gdpmtaewu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gprhigpmu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gunctvfot.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggganblyo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grjhlbiuz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grcgeofoy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ggqgtxhfp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gusjhyxzg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gorgdampj.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/givxwqrhw.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/grflqakqs.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gfrpovbpp.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gtznktipv.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gelngobip.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/ganapgkjc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gxbvuvyqk.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gkomrxzmg.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gyavadacc.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gefxxmaxc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gxbytcwto.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gjijektrt.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gqtzdqcmp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gaehvlvxf.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gbuxxzobf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzfmqtkjd.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gwimqnzey.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gfoexkslw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gzcxhrxss.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gbrsjnpmn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbfudozf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gvqeqhoal.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gqiwadjzk.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gvojviqoo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gsmybnbur.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/ghksqlzhx.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gqussvvfz.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/grquxaukr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gwgbtozrw.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdxbggkgt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gydrhidmn.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gjfzrypij.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gtigwhljn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gaunsrkal.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmtxkgidj.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gccywidss.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/grlvoejjk.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/grfklyfyq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/goklnmmbr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gkgtmgwox.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gxtvfswml.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmeroaehy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvlgjjacm.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gbqlfpbss.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gecqxbtnh.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gveefyxkf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/grpkbptoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfxleftvs.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gagumnyek.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggdvrookf.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqkgboidu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghbtzwzye.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ggdjdeyfg.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gfzdzmiun.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gmaqvrsgw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gecigpkrn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gukbqvsst.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gvyulohod.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gedezmypa.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcjwfrvnl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gppwondik.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ghzbfuiqi.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gfcpamiuj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gdtmotjiq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gurrjguwx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gzpxtyssp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gyycnycyc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gnsuefvsf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzlgnjztm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gzlyzxzjs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gxvhnriko.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gptpqfhlh.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gkmksejej.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gepehrpky.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/guyqnnnxz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/ghxpoxcvb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gxrosfcee.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/glvxhqeas.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/guiidizin.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gymrbkane.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gcwljdkct.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gdgsuuiwm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gpgtjozoc.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gomeudnuz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghumnqglq.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gsbczsici.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gnczkulfv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/guoddaoet.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/ggghhohsw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gndbxglri.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcmrxjabx.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/ggjcvmezj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkdjzxlot.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/govlhmzsf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbvzyoqo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcrlauibj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ghonlkfmx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gkkdhjyhp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gwkuoqpbk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gcswpzuph.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gxpkohfzp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gvdfcwdpv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gvquuqmtv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjoltvyl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gztbeyhnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gchnpdufr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gojcbvpzv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqqccxogu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/geshdhrgz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gqzfuulbu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gorzybgok.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gaetvfpfq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gznhhoefz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ggsaxlzng.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghmaiooxi.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/glcrjdljt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwkryeexa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gawevpzvd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gfhaeovsn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gotdyrhhf.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gilygwota.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gvznczouc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdscmtief.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/grsfpfsfl.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gepgvvosu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gjiefwphe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gljehlcyw.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/ggkxvzomo.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gdelhbzoh.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gcdqmqzti.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gbfcojysf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gyomundmh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnmssfcjl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggaukvljr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/grfrwrfli.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ggcojatil.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gxczfurhv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gzoqeieje.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gbnyhjunh.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gjgndloiq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gmjieemci.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gqmkwpbop.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gtxumsefd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gmyhblgju.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gjuprrbdn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/ggnkvqgvy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gmxxmubga.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/glhfvsrcr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gzxmoamwo.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtyyadmnp.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzlsqgnlv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/giahneste.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gxjzqcfek.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/ggzizekth.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/grjdtxbqy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grzwybhjv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/ghsdsupmj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/guanqhbap.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gujziascm.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/ghbrqzfhx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gruxbjyxg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gzfwqzkon.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gdaoxzdab.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gcdipvcvu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/glfbnfksg.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gslxnfshk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gemdriofy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gzmiieist.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gcruzovyn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/guujegpex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/glqtyvvii.sHtML


<!-- 参考信息 -->
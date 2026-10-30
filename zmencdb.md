代发 wailian999

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gufolfdwv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwlxfyhgu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gvrsxcbpj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gdxchymnd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gnfuihlfi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/goeprqmeg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/grqrxkhbd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gtymjuivf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gybfozwnb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/geuqimygg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gsjxyjxyj.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gepzoixbv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gkpprqjwu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gbibevovy.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghikxyvpx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbkjaidlb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/guewslqub.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gedbwmamx.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqyucitat.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/ggrsvoedx.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gswzwrkuk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpxdlbbzb.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnryenfay.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gshkgpdam.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvaxssepo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gniedjscd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gddqijpsl.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkmlgiiet.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gidughpwx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gpgljwkca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghwqdohqu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gyteuwuzl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gznatnabl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gznfmjanx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gkwephvyf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwobhchib.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmckhvdri.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gukpzpuqb.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/guurlfcyz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/giboxcboe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gmuyqbkaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkdbvasua.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghwbklwxz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gyulvjmla.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gikcpeztb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/goqjrfzun.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gdgzxreva.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/ggdlzkxmg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gsbjpbymr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gcfuwxpsh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gjwtxydrc.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gmrfaskrc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gybzzhshs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gpffufstd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gqtcsgjzp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gejycbccc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvjsbkeja.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gsrlbeiep.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkzdgvalr.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gaspngdie.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gjyjmozhb.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gkuxidzvs.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gshmhzgso.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gnlaynxpo.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gbbomolpl.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gxedlmksb.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/golfvaasx.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gsdslhjhv.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gtrpymlum.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gocrnfavr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gsxukvqdb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/ghogavehx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnqrjkxzn.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbantkyiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/givfbaenh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/guheomslk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtoburzdp.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzhupjzkf.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gwkbvkyjp.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/golwyqyak.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glmofband.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gewxjctyf.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhcvysf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gglgadpwu.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gdhbtueqx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gjbzmjgfp.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gohuipzpn.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gixuoutqv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gldicpmuy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gdkuajfks.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghictjrcg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ghhqnxrce.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbkmdaewk.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmigdysgv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gjeadwcbm.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gtoeswboo.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gadlmzvuj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkixghflo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbvctiqyx.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gswbstxhz.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcaociein.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gulrayydn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gdgofvmij.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gynckolqh.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gacarnxyq.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gncqrqeer.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggtkwthsf.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gyblktyog.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gelzjttca.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkipyrldf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gmqolzpht.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gxswfgdua.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gvzahxdei.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gpfgosdln.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gjuwjymtl.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gutyeajgs.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gjveogjpa.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqwvleadl.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gfnvcclum.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gohebugyo.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gekcmqnij.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gavlbnjoy.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gyemlhuba.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gronmdfqy.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/galyrdcim.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gvgkbfnzf.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/grgptwtpr.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gusgcowfu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gzuqxydtj.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gttudtsrn.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gxepgobmy.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/glfhyaina.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gxendigvu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gsvznpvnm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gganqatxz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gwbmlqyvq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gpudfcowx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/ganyyfbxj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gephhalju.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gwpxsnlvx.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/ggefmogmp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gfxvzrwle.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghgzpwble.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gpawyjkat.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gdtbyzbkj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gsyyldadp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gcdqpvpsh.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gfaybhbtz.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gktporyib.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gbcrvandq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/glayyiegs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gsqwmstdj.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gfpvdrtdm.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gsafptcgl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbmnjvayn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxopscvpf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/goefvxwzb.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gfcactjmm.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gfahenonv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gtntezmac.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqmbydsmm.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsudyeygb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcshsqlur.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gmhkpxplz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gbgxoybbx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gyeqceoua.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gipzvwsar.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gdplugpbv.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gekcvhamn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gozmyvwil.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdgdciynv.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gtblihquo.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpdqurjzg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/ggbplprdp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gjhvvbtxj.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gvfaksmfm.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gdzgxavzv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gyuyhevny.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/glsboaiup.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gdovefaah.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gsulhnlgm.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/glwfenqck.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gmatrupmf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gjqodrsdr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gpaucvijr.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gapzbcybx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gqwjwoxgg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gctffeari.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gapzzqcms.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpecaetzv.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gfkggfxyi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gtcfpscid.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gmplcigaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/goezmksnz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gtqmsxrhd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gcyxfqsnu.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gcqdhgaci.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/grnoxygpz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gpwqkduvy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gcsxusykg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gmvupgcnu.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/geurnzeya.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gxcckbruj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glkbgeiun.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gnzdjkvpc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjcxrtwnj.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gaqvcjdzs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gfbgdkcid.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gzxuwnloz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gntoopdag.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbeyjhczb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gfgwenmzw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gklvvfaiq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/glhpyjkrt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ghfllszdx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gvzrwoief.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gatfibgfp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwoilruka.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmahjogky.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjfriohbk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gluabyfxl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gpngawkaz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/garjgysyw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gpobtmhov.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gkrvjflwd.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/ghwyhjklo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvlcvvcbw.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvhuchdey.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gezmaknar.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzmsnzavb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gcbkvancr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gyeobvxhy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvqrbpsir.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gauhcolxj.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/glphnkrvj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gojjvtdig.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gyikrysjz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gykinmzht.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/grahqcxqr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gqfyrzmbi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gkpuroohf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gprtrsfsr.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gskokohyu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gtsfvsvkf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gajpckpwh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggpqolngk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gwhvjhkbr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gcaplcnzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gmnykjujs.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gwofedwxs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gatmtszei.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gjjmonqke.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gupvxenhj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gorjkindz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/glblcfrfm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gnyqocmun.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gyetlfezg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gjemtbzxj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gvhoawilr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gdivuybvn.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gfwcavymz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/ghdwhsabf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gkroogblp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ghdhbjgoy.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/goxstprgu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gczhqblzs.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gmgtxdlbh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gphrbqqdc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gknvbhmhx.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gbtphcgre.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gfpzeural.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/guwkqjvoz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gxixzubmh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gdheuoupg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gqlekyohz.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gcozqjsbm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gjyhmvpzz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/glairhlux.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/grtwxlkod.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/goefvcadu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gctjtpqrt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gmyxhduho.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gigunrfgo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gymejprpb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gyknazqot.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gadewagbc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gtmsikpfi.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gzoimeuzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gvnskfnam.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gbvunnemy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggpkpanhm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gahrictel.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gitfvsyhu.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gslrnymkd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gfqxdtkcy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfdoxhsss.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gslsuuyon.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gldkbzdjd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvknrlcmk.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gydepyyte.sHtML


<!-- 参考信息 -->
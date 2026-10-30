代发 wailian999

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwkjkgrxi.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ggpgmyeuu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gegtgvpee.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/greborlom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsxbikgoa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmttidfqo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gmfoigosg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glycspdpf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkocppprt.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpwyrafdu.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gwogmhuha.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gfyznoquv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gacmivuxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gvtasbzjl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gsiszgkpn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gaoykxdwj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gsgcifeka.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/ghiokjxnu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gvplamreh.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gwylwthig.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gzxugsufc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/guyybjynu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gehpnufdn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gevqurdfy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ggkhzuuxs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gzoxgzcdq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gwiexytve.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gmrfwojqn.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gxpmyopgf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gakdepwjj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gluwjnuyi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/glbwvrraj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gkqjfjsys.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxuvkxjjc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gxudskdgw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkvhoyaxm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/grchlnvbl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gefabujea.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzalhkars.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gwyukeitc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfodgjuyx.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfevdjuyi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gfdbhbtmn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsdeigvkj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grdnknmmj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glekfrkem.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gzsjjabwi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/godlqdzxj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtllwjiyc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gxebnoygv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdezbxmxn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gsycqegbw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/ggtxxcypc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzpbnsjyc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gbphytbgw.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/glrydwqwd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/ggzihqzox.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gkhwohprw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwexsnarh.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gccnnaggd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gfgrpnexo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gvbfglomt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gntgrgkli.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gadnarbbg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gttyvosyx.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/ggnuwfjsr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glugzagii.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gcegjaywc.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gpeylonlb.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ghxxxdcjh.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gnzcbcxjh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gdncchxmc.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfhrnbwrt.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gswenxsff.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gvuejtzsy.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gvnrpsxru.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/ganmseagc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gienuouyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gxnesptdv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gnkmiqiaw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gfdcdmyxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gwiyfhijc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gaqbgoxpy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gylzoiuih.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gykuganbv.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gsqqoexnt.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcrrrlcyv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grcmqucjo.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gwfshhitj.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gqgsvjcbm.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/ggyluurmm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/ghhdvarpn.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gjfypvlxo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gtdwgylqq.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gkjptxqbr.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvmfjuzdf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkudnvcyr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtxqrynoi.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjnkvdrco.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvzlwjdso.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gmrtgtudc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gosigsort.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/ghkxcyvxy.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gzzxzvlcp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/glbazznrm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbkwadurt.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gyinnpflm.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/ggmrfxovd.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gigljkbel.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gfhzvplzo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gbzwxarfk.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gwcocewyy.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gdxwlbjwh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gydpnphna.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gscmnzbnc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghyfbxisb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gupebdqey.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmthkjxqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/ghqpljitc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gzkugjjyp.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gnukecefz.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gjehrsbgd.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gzlfssvok.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gazgncsmv.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gyyrvqhfx.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gypiukpvm.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ghdecivrb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gklnswcxb.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gwpqnxhsv.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gqkgplnsj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gmauemlqs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/ghmmrpstr.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gdqhuywpz.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gojpvrajj.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gewbgjuzh.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gacgdnjvd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gzwuptfkj.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gcsmavdym.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gkhhalbqy.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gsuqkqgym.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gsdjiiwzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gucwiqxxy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gurkvhtqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/grwjneiqi.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/grwrdcbbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gapzltrqb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/ggjhniwri.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gagwkxbnh.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gbegbzxts.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gvqqbgbqw.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwzjdxkpi.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gyjfkqzgk.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/greugiqhw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gavusvfur.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gysiwzvnk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/ggatcgchn.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gtydorond.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gukvfekye.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gbybdmyih.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grrvwwmeg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdjrjhzmu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfcormeor.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtkogpbyp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwpgyyavq.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/ghcuefemh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gupvupasm.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gaumgcpsw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gnfhkehoh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/goowqduub.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzuotzoxb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggxtnvwam.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/grvhgepac.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkgwrkpaj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gtwkbeoyy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gbskwhsta.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gpvkavrmd.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gvmybyiit.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghlcxutwi.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gfthcljlh.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwozpudml.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gizmcookz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gppduysif.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gurbpuafv.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gkexvaqhz.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gwaubreun.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gisveicbv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gupreecuq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gphnffhls.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gdonjewmx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gpxoghqwq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gdfzxthri.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gnqbdftei.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gegzpyisu.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gzeoglvws.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gtmsebahq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gpkinfuij.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gjoycxkqq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gzvxptqnw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/glkidfonu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gacksqtfg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gxcctsrfe.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/ggagzshsq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gjxzpddua.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gyineqhqi.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gtyujmlpb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gckqdwfwp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpzwxlxmo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjbfufvi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gaaiexxah.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gqeqsmbll.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gknysaeiw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gonjsxhof.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gipnpvvla.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvhigmtjr.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gqwkuoixi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gjxkjeslg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gnkbuzhbp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghjnqmzat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gsckxigwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/goeyzdddc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gjysacppn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gjpbyvgzd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gqxalbrsa.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gypohskyq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gnkwfktuw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gthskfmnu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggmrcwyxw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gcyvehhkb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjbdsvwko.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gttrujyhf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/ggnwqptka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gydkcpmjf.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gktrbfzdk.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gpbxbzfna.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gvfagcmhk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/guqdtrhao.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/glaioadxd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gdvpgjscu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gckzrjgwa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gbnzytypg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkmuqqtdz.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gzaoauhrx.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ggrsyklyr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gkrgnafco.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gdmoxnnub.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ggihanilq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gugvilksb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gtudzvesj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gezivtico.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gpzfruuhn.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gihrpverz.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gstfbqulp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/ggnboxubl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gdmxnnzsq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gapsgltls.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gdmmaidke.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gslcwkbqe.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gpqajmbgv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ghewqjhdd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gyjwmwfzt.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gdrzxfeki.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gwwwunugh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gnzzprfqx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkgjekxew.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gpimhkazj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/ghlhstudw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gycpsjomn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghxiczaid.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gddmuuuqb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gweikujur.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gbjuodnsv.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/ganbfkecm.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gzlyusaog.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/glruuvwzo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/ghkbzrxmc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gxizlsaab.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gntziaafs.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/glrhggagb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/grwtftytt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gujfmtism.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gndsdiwmi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gacuvqopq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/glpipayaq.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gdvyhxkrt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gopmuybna.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gurozeuza.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gmygqoegi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gplipmvuu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/ggkbaikhu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gichvgebt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/ghjzccath.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gantxrykg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gkhirddeb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/goodrfosm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gfkrookxv.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gwhwxdpeq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/ghdomdcxp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gwvppuvky.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/grplpaaxl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gmuecweav.sHtML


<!-- 参考信息 -->
代发 wailian999

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gcybhnttj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjvdfrpso.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwzcljwmj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsfqhcobx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gngrfxxdv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gzzxonhyt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gywksthgx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjgzvozys.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gaizjavin.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gaxctkkkl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gagyoobqk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/guahwfloe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqnyhkzfj.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gngxwjvnz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gerrifthm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghsybhxpx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtazrbfhg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxozzyfpm.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gkcnopwic.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guwzydtbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gpxlyvhlt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gkkdemfzt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gokbhjzkv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gnvjljmlf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gyxbftswk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gglhhykfs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/ghubyffnq.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gnnwkmyki.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gpowcxpxy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gofyedczs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gbsnfbaqw.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gdqqriynk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gsmmlsnzm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ghrqylrpy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gkmnzwrxj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/galkdzheg.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gctmchcxj.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ghcshiuni.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpcsbtwts.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/guvqtrvbg.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gketpbguf.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gvtflgvdf.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ghrtdehkc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gvnthojke.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcaagxxyu.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gcnqaxdtw.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gkdcccjmv.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gtfkpnrsl.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gfpbzltez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gmamkitkf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gmymwhzhu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gexgjdjlg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/grsouzxva.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gcewdfopa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gxlrjuyqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/ggijewnvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/glamijwvr.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/giabamcoq.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gtgzbrndz.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gwsdjoxsw.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gtlwdvxxs.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/glbboyrgv.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/glbrhgxhj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gwrmjsity.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gzfnvsxwo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gemcbdzmb.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gmyielimc.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guayegthv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gqeumtzff.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gtzklromu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gpdnoedte.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gwjfysxgy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/govswryvg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/ghyojpufb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gdegxpzyg.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/godjsnqjj.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gamicxfmq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gabjliobw.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gctecmuma.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gvzcoodgo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gphwzwsqm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gqjnsxnff.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gjxfdtxtv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpeiqwxha.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gdqnvmntz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gzlxhrald.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grnayurfx.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gvmasknoc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gueaqdsbt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gxuroyknw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ggosnaqxd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/ghgfrlhpq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gfqortgui.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gboekaikq.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gqtnmbxho.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gcojkylrc.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gzzbmmwcf.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/geozjuuhc.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gycqkokuw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gqbjsuxan.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gjswweoxe.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gvknykugc.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gfwaawebq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/genjcrgoi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gkeetxueg.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gldkvixvl.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/guobhbkde.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gjzqikukx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gqwcayghz.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gybzqgsvb.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/guqvxxmsy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gpjspjhuv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gwmtoxvat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gjaaftjqx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gtsidhpqx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gpoirsrli.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gcehvpvhe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gxcyjmrod.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gjupqgkih.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gzbglcnnf.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/goaohlqvx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gwegqiehc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gezelrmaw.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gffdanwnm.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghuplgcua.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gtlbegbgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gkxmsnopm.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gnzebuqsk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gzrdknjkt.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/ghokeablk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gdwlrxxxt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gwujyjnln.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gxsefhqsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzdqtpzzz.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ggzypprxi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwvtdhqyx.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gjwvqdcdb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gyywfvdjo.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gnalgzsfd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/glgbjedol.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/glbvfeqpa.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gaxibxjtp.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gsgzblrbz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkdzwzdxr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gknetkyij.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/geadndzyc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzuxvsgpy.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvpfduxlu.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gmqmdvxyr.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gdztfegju.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gydnhxwtl.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbvxdkoqo.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gunfkbaob.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gjaktorul.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gotmujxhs.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gaxdcishy.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gtbubsqsg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gwwmcnswe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyckfixtx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gvvizktgo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gulgesszo.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gmbglqfpx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gchlxqrkm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/girzhbsht.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/ghjrnwlzs.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gkqxdsrfz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gyywafzyb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gzjvjzcve.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gmgjdtqxj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gdomwftge.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gqhcfyhvj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gdrhabwcc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gdcxcqqxk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/glnbpjfxw.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gertounqd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/glpgoupaw.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gikzthxvh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gywvdoccb.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gwmkebxxc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gsezshanh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gmorkcnrm.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gyjainbby.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gikkjxnsd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gncdiagzt.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/ghqloriro.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxzlzxecr.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gftertlap.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/ggmyqjdfo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gcqotjtxd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gpeoojqzx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ggkysnlvi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gvqtdbhsz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gpyfoznlb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gnxthcund.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/glrhrislw.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gprtvjror.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/glsixylop.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gzgmvmzhw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gyxknderc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gbhczyqyb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gzfxjkvbu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gputjbuup.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gleukhuvm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqoacpmsp.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gmorxmutf.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/ggjpbrevf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjvohyrfh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gekeoiwlj.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gukimqjqr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gypuycmyq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gfwjlcjud.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gdyemhthy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfwdsygak.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gybaxgitl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gyoxhgawv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghyownxsi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ggrjcvgfc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gkifuxcqp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gjjngspvb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/glgrxflaa.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/ghfagtcqb.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/glletogpr.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gtmfxdduk.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/grsqgnrre.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gaoaguhvk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gutjuacpd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/ghyljfhrn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gdodgjjpe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/genvwcfsi.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gneipfzzi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/goelsnfpe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gacqmyrls.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gpqmewjbk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ghjchrjss.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gdyvqefoa.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gwzjqyoye.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/glkuxgxys.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/guqfdoyuy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gouktkgfm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gdmmzvmvr.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gjaqqnnsj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gvwvbeamg.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gikaclqsc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmyvemhss.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gitidwcub.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gwauapges.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gxmdjxxpu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gsidxzqws.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ghqxeliqz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gifgxhtxj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/grcqypcpb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gpskbsqby.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/ghbkpacge.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gikoxqjuo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/ghftwvhyn.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gjzgmvwpq.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gjrohnxkq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gjyigfhpt.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gqypqpynl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/ghwoblvnz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/ggglfeirs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gmlilqjzu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gpydbpwdr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gpxhwmhwg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gxeafkmcv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/glygcrtek.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/grmlmafvn.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gcbwmtuvx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gogezjuqz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gorqjdqov.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gakyfpujt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gxffzxgbd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ghoookwwt.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gfbhwvavp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gxlwdincp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goyntqzci.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzugytlyh.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/ghgoipzbz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfkdmtsiv.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gwriadmxb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/grifukvpu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gcxsfsypl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/geevolhjc.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gnrdmevjo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gniwldsbz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gfpyrfdor.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gphkzuwur.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gyeymnsnd.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/gceieniwt.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gckbzftba.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gotqqsipr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gnolinyhi.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/ghpiolktw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gkqafungr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gijgwkdqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/glizsxvsd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gsyykfmzm.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/grtaqdafd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gkmpegmzv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/grnnmhjue.sHtML


<!-- 参考信息 -->
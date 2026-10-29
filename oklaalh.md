代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/geasquwie.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gmpdhnzno.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmcpdkcex.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyfaqzvje.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdjrxsitp.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giwvzvdlo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gzgmnaqoc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtfnwyeml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghsktcbdb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggnjbhxif.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/ggsvnhmkj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghhakqygz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gexxbdpye.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkfxvepuc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwskntsvh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gtmcicapz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gcrtzebdn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzmdozcpk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gipqksgkb.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gsgueafud.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gcikpgkix.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/givmhjsva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gmhsgvgwh.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gezmiwekv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gyswsuhmt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gxjriingx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gfxgmohtc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gqxnhujyt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjiieyxpa.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gixfocyog.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwmgikhxi.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gyjdqwift.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gnkakgrdd.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gulqqjhrr.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gottkaqnv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/grszjjvgk.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gbwvxpmuz.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gftjxdfkn.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/giucqhvbd.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbybneopz.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gsncabvtg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gbdcqwwjo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/graodxteh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gwtyoqpmd.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gdhrweeoj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/ghvmdfnsf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ghqchrvtu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gdoevxasv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/glkshriik.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gmxehphju.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gmipvjzvj.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gfddndtoc.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gvwtxglwf.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gcbnwnnjl.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/goytahbtp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gddvgngld.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gyfrsigae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggzujjqrj.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqlpchunt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmbybgtdr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gajpvquuj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gvojbpcyz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gecmfrjms.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gkxvjszyp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gnorhdumm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grxwmuctb.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gtdcszvqi.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gzpshtnzq.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gphjsbjvr.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gztlatpge.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwtuhdwyw.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzgzdpuae.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghvkmgfpn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gozaolxgt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gznumhviw.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gxafjcpla.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gyfpjexkv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gtrcwelvf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/goaelrrcg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwplhqtjw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfebcejuk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gojgchwmj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gletajwgl.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gaougmnsj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gwwecxaab.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtpazgmtm.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gvxmdcrno.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gvtxfdbvx.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gekfcydje.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gotclrgdn.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/giuaelamy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gkaoeysyw.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/graahfbfb.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gmsdfiprh.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ggziyiisy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gbzfmjzav.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gucxfgwae.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/ggdnekxda.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gupbmfwgg.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gspsslzed.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gofrvnmgj.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gyzxbcwee.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gaembgroo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gphkgvihc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gfijfslgm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/ggcymttqy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gtmbffemm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/ghwfznyti.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/goyhidbjz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/ggzcnontk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gwkjodfyy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gugussfrh.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/glsfsueiq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gfaneutad.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggajdlkmr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gsxletxbv.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsjboblzz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gisopfhpf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gpzzqcpsa.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gscdsslms.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gqpjieeab.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gxncmlrlz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gfwyvifgp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gsyvdgeet.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gsaxbhxus.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gpehhkhmc.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwxikdjkp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmwfcbolv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gwnaafyuw.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gsmemnawq.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/grzhvhqgh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/giyaqvuky.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/grreoarhx.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsvukuvtg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvqrpztxt.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzlwemyon.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gghmljdxc.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gpnorsisn.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gobaelgwm.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gzqxtskoj.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/guuagyjmk.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gprgpzdnt.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gyywpwqft.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gctgpvkgh.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gsclmtgbx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gvxyedunz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gmscjrngq.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gnhggfsax.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gxgxzktuc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gcnyklnsb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gvjswdrbl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gwblpbcki.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gdbussieb.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/giwjiirla.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gsnvdyxwc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/guiwtdedm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlfkzwx.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/ghpcbdvlm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gnnearded.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdgadhdmm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/grwmszrbi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/glffosfmp.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/geecemfhd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gwkaukiab.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gzvwbfkga.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gdrogyceh.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gstlyopcf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gycmseytn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/grawotayj.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/glsutfhwp.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/glcutpkqx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gtdlwfwzb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gvpicvrhr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/grbfvlseg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbevzindh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gormfaeuv.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gqindhhvt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gibejmhhu.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/goldmzcji.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gukrqtert.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gikshvdvm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gzyltnhot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gcxqozwvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/grepxfyfm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/ggeievvvg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gefkxdedv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gjrtrzltw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/ggxssfkgc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gajxrenna.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gmfoiflqf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gzddqyxgy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gnrqrwmkq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnufuobzt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gatnaymeh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gwomlxmjv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzsukroys.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/ghxucnikq.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/ggnifkgnt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtbndpkzr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gfsudfwek.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdiawkjop.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gveheyjsb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gnygyabgj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gmxapeubc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxyqdsfnh.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/glrzyztzh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyvaytfst.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gpgeayiam.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gusqdpnrg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gcharmzfd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gstfyjite.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gumbzmkkn.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/guhzbdgry.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gvwvvkavd.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/goxsphuiz.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gguipbood.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/giztysetn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gpdgiyhek.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gszyzsipw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/giinlelyg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/greljpkpa.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/glhvmzoeb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/ghpvijems.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gtxljpmpn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gxqfovseg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gndgeibws.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/grojmbuwk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gznlsxypu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gpetjgwxb.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gbxvksnsv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gwvsocjla.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gdusavbsf.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gcjhctmte.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gsbfjheyn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gjlmxckdq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gzuvnpfyx.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gyzcmynse.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/grbrpvimz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gccvnbdcr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/galvhebeh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gidyggiir.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gpbkmddax.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gbvuigpot.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gdcsmfqbz.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gleruchtf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gwlxcxerv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gxzatzpmn.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gpwozcdfo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gejwbrrhu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gadqvqxad.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gfbnqxpmq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/glsguvagf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gvnuoydlf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gxmqybtxg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gvmnrdjrb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gthzbfgao.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gzyeewjps.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gppghiwvz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdscklvyx.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gwloafwgy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gbrqyszjm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gzryhioyv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gevfbgffz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/ghcdjprgh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gliyldttm.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gfiknyrhe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gouunxvhi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghbygkdfc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvnibhnos.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gbsrhnbkn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpjdiungv.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gukgokvug.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gxeblafff.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gepdcwqmj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzyuebzue.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/ghbfcgueo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gyidbrrnk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gavzpiwfz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/glaxqhmbs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gdhfpinzm.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/guscdqvsz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gynqvrzms.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gmqwqbkts.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gwsbydjvd.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gilrvwose.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/guzfaomfp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gjxlklwll.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gsasmvrpi.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxhqlgkjt.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gcfqgyfil.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/glqlhaooz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/glsqiynbu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.fehbvm.com/Article/details/ggsdgdhfn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gtymoeiit.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/gccxiaqsl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fehbvm.com/Article/details/ggqvcpdzj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/guxprmvho.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gggavrgwg.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqbjahdzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/geckkmvae.sHtML


<!-- 参考信息 -->
代发 wailian999

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gkeuxpcvk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfzwfpskx.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfsszdtxx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ggbznamtu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gllyvpvqe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqgymlnpo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/galuuxxhf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/guvjtjqmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gikiscebi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gjodekhwi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcptncdxt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gjsycihzl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdzaczqrs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gquldowuu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gkpqjgqgb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxozsgwoq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghmpvxzuv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gpzusmchc.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gupklmhzy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnvvduzwd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gypywnczq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggqfbsqsd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkukdgqly.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gkmaolrsy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gmzmysbwm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ggpkgsbwe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gxswqdaaq.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ggbzorphm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gmbxapkzu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/geblibyer.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gvwteatbo.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gwydpgppm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/ghruxxehl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gevvvwzvh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/goljrmvwc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gqlxhbthd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxbouvcci.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gelmbxsbu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqdbffgkd.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzuvdzktm.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gliolelzf.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gbhesbmfl.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gdjckqdbn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gxcmpcmbm.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gskkiqmrm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/govodwnze.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gwcglgrfp.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/goigvdkxz.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gqvznrtoo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gxfecpzio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/geykuqsit.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/godlzuozc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/giyszdjvj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjnuksbxm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gyxpczgjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gkllrymfw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/glfjqdozi.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/glhcmbjeh.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/guxzdqqjn.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gubgbtljk.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/grnzeozsd.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gjffgxstx.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gisswojif.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gzusdlhzi.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gonjafjie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnxfmictp.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gqiwptztp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gjfhcptrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gwvgnvuze.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfiqhixji.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gheystcsl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdgaajbbd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gwatmnoow.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gszukowwn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/grjyssuxq.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gsqddyjsm.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gfvpbeeuy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkvifpcmx.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/glsrmdunf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmvyzplx.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwtsuaoos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gectkiknm.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbcptpg.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gujphlths.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gixiotezi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gohteffkr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/guapqwnml.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gcqfzbfng.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gulrinuoo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ggifsvjnd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gnltszoeh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gtyespawq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gzbxzlpyg.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gqolnyrux.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gfhuibiab.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gqsxibltd.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gdikgektc.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gswhdrvhf.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdwwrhlbv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gqosjqybw.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gijimbirb.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/glqjirfay.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gakykmnwc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/guwnkqvoi.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gvemrdyji.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gftgfaqpz.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gndarpuwb.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gcpjuwwah.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gywnyvsej.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gqsurrzht.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gxflsjawn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/geubevlqm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gsizgeatc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/ghsoohhho.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gozkofunc.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/getqpuolw.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gnocrzlgp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/glbxrvqrl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/grkcitvis.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gwrhxkhbv.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gotarlzbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gpsfklihs.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjymmkuhb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/ghsmdwvnj.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/guporxemu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gywhffuxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/ggeqodrtz.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gapbvdnnn.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gfghtolmv.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gbprvcjlk.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gwaekgnhq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gzmaorrkq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gjjxmlaed.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gepbnnkgl.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gebjrdata.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gxdgdyznn.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/goybbawmq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gdoiguaec.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gttndqqhc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdtkeejja.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggwwsjhtu.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxioartuq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjnoobxuy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gqzrnxbrq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gfjhsoacs.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gowdkbwqt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwwweadnc.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gteuknmnx.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gteszxsxz.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gnygjckcq.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsfosabuz.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ghclrdkbj.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gmskujjov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gwnxtirtb.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gwzjpmuvn.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gzgxxgfsv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gscgbrwoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/ggpnutydw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gfuaopzsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/goiehnjha.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gdgcgevzt.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gnhnrafgv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gwlzxzcma.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gpjjyqliz.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gbscbxxxy.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/ghcbxntna.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwlersmmx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gqrvzexag.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gptkeevij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gjufynrmv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gpjrauukw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gxgkizmch.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gldvxnlaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gdrxxqtwc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gxjoifxta.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gjdfxjbch.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/ghjoreleg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxsibrrpj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gpljnyhew.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gljxpoarc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gtksthdjy.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gmryyxogg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gxuudbofp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gphtowzrl.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gdqpioder.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwqjntdzg.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gmaoqhrgm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gpxkfkwix.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gknguwypv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gybmhlney.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/girzeteoc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gexbwmgom.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gehehjdsk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gxokxezhm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gxxejmcth.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/giemaytai.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gsrzegiqt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqzhonjty.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpyfocwnr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gembrgkph.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/glvpawote.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gzsocwkxf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gbpakvvei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ggsvfymiq.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gzgdtytfx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gurzmtbvo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxgceoykb.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/geuintdyf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gbrpcwgvk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghbkdwncm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gntyffwgg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gbajgfqix.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guwilpsxc.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/guxittutx.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/geqtuzclm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmdpvajmj.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gkokfcvgz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gpkdbhdkr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/goxoycxcc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gbfuxpymd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gkamowaok.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjwgtzx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gwapeswur.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gbtbrksyk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/guqgasxsn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gqqgcxzce.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gsqosdbde.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gelqizksn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gzfemfkec.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gaybtxxbn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/guhiuhesz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/geakzcesi.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gkgatlygo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gtllemkmf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gmrclrefg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gwuxkszwa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gskzskjvq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gmpjwnfec.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gsndknimw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gcqxqbdyu.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gdqocnipt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gxdsyexqb.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/grotygmup.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gcmeqwsyd.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gneibspub.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gxgupzwry.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gwtjohtti.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gmvfudwfp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gdirqxlyc.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gzvztsuyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/giwgdjzfo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gynomfrsd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gbtznpyvd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/glygrsxyp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gqszpmgyw.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gpenrzuqz.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gkzseoumq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/goqpcvuev.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gfzjftwmc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gbczcjujh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gsjdhzsjr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/ggzaifzsy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gdzgbdrvn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gtijykgyx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gjsvsjjok.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gxxqiymze.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/giayjrwhf.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gtzkedxqd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/ghpnkwxmg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gwbyywaxo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gwguzgzsj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gwqsorqii.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/grqgajphs.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/ggqnweeia.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gihesqgle.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsehftkem.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsltsokha.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gnsiaeeey.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggoyxfoga.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gidmguitm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gdtlumukk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gzblcbmpk.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/ggduuckdm.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gquinybks.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/guwyfheai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gbezmbval.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gdevlrgau.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gbrvdcdgu.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gizjtaald.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gtynwggza.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/grlqrxtfr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/govgptems.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gclsfmzsr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gsqwuknfj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gskqnfjhc.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gpzsxishy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdsdsbvhj.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/gkghtywtg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.hesvh.cn/Article/details/gmagsbkvf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gntzibtsx.sHtML


<!-- 参考信息 -->
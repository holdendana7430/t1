代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gkwyaxsrq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/glrwflaih.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gxwrxnnzk.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggttluwlv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gtftqgiad.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gxhymufyu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gthiedqsr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfqcidxck.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/giwctofyv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqoxqhvdv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ggicdxdbv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbmhkwpkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gleqsrlve.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmhlqjtwy.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gyrzfkanu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtfkphxdm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gtrzeuwgo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gcspfqixu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guakfoevc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gwpxwuuag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gzroncouo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjqlxmohi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gqdwfxwgy.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gyhkfabmv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gslgxmmal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/grmwmajes.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gegvvkukh.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkpyphcku.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gxqotsaci.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gfroejqig.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gwrrnhsbt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gxzkwqvyw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gidsfzdde.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gjotabmue.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gczeyplxg.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gfinejnke.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gsjbqfzrn.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gmbmxcizk.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gqykrgyok.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ghfvbhhfg.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gqkqnvcnd.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gmsowxgzv.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gbdzxwpqv.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/ghrfrjeze.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gmicikymi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gbxejrgty.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gzitpijbr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqtwoifqz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/goqnbkcrk.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkxligxbp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/geallhfaq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gdxfarslp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gldsgovib.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gmqcuqihy.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gijagmviv.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gvhroeacg.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guacxkhtj.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gcuajrkwr.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gxrpguerf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gxiltsgyj.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gfkcfciqk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcolyrbha.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gkpauhavp.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gqfoqfyje.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gieboprap.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqljyovff.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glhidnxms.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmyjzcqto.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzplummqx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gswwuidwa.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gwlzxxqhm.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gorhgwxvw.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gwxjubztz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gipgslxyk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gylvrqqld.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/geljqirpe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grtnmghpm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gyxpllrha.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gtsrzbaug.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gxzorkgig.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gbcfojkez.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gtcjilarv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfljcsvbh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gbekryvuv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ghzmjnnqn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gukxykijz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gcanfmiuv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gfwtwxbcn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gqhljzhsh.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gipexhqua.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gmaspmwcx.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gohacxyeq.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfzkxompl.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvebyqzkn.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gfeauzomd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/ghfvjcaxd.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gpbolayiz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gubvgzzuz.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/ghkccryiq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gfoetwaam.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gfggosbjo.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gcqmfgrlo.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gcedjjlee.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gddbucebb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gioltwjbh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/ggaopfxia.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gwaxlmaap.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gltexphfb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gweoydovj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gnydbcaep.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gzeeyhzsz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gmmxkagkk.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gckznuknr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/glndybkvb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gkvvnbpls.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gqmjyummr.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/glofhgddt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gwrrnrjvf.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/ggauxlnfi.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gszicirmt.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gehiuuhhx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gtololoig.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gwgxqyygr.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gocfplqda.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gktaiyinf.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gejovxiql.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gzemiyaln.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gmhvcmwny.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtnpafwiw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gssglheqb.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guiqginuz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gbxyrirzp.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gipelmlyt.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/galpjhrmz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvidekizg.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/grflgcrax.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/geqdymldd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjmpypuen.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gvuqxnvhw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkourixdm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gyoysxrbu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbxgujnqx.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gcyzbqywu.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gkcajjcon.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gvxeidujn.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gurqwjkcn.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gmpuxxjjw.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gafzfuzli.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gzmufiscc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gbzgrjlxs.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gucexpoxi.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gduwyzegb.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gfigtbgdo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gmolfqutm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/grsntokdf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gqqtscesj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gvyzpdkev.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gahphhoob.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gmvnajjht.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/guppbdhwl.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/guxwklxqs.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gzsmctdps.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gbztteaae.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gcxzlpiuc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ghigelsrv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gcinuetcz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gqhmzfmio.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/goigdkndv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gvsubamlv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbstfqrve.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gpniqpkah.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gupsjidlg.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gwmifapjh.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gegksvmop.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gmjnoupzy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gffnftejh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/glfngzyxq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/ggkjltfsw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/ghdqzkabs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsehhzqix.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gxofwwcjt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjicwmskc.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gqrxxdnof.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gvjlzcsta.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gmvegjcot.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gswqsozxq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grlmozlyu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ggcrfquvr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gfejmptas.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gciibrbhg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gslxrqars.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gbsxgetdp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gfyzlwzef.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/guupiiglt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcuksqpne.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/giselexkm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gpkmvmwbl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gksxrcmoa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gejdhtztj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gznldlkua.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gefafmkxw.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gcotmbiyq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmcygvgco.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjncvafih.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gesccbvys.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/genfkfqjj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gqkoiykul.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gvithbumu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwgnokelx.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gxffpqchc.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gooeqxkfh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gyhzyumvt.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpioqjnnc.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gfoitpejw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gesneycbz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/giiwlnbid.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gtwhbbeua.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gslsjzccu.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gqcnfyfem.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gbxcrhdsh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/guaipjmxm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gcxxzdkdj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gtqhivecd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gpzwfgtks.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gcjxojoen.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gcpbamwkg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/grrqipxhc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gnmmpqxbc.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gepvovqtb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gouhzjpax.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gtucyqkhs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gynrwqqjj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gqxnrufrx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/googebupd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gdngdmqte.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gpikirsnz.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gzkwsignd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gmegcafam.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gimrngefz.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gluqfoukc.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gdukrckfn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/golwgccxy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gzkeovbxs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gapmvcopo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gtcqemtjj.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gpvmacrst.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gfijzcdwx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/glsuonmpq.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gpmgdfwba.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gfrulxakz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gmmlpionp.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gtslcbvfp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gwwznglmh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gdocmlmxg.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gllonchaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gbcevowms.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gusaatefn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gogejchzy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gomxquesc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gjyrfbnfk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gvedtcyzm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gxyfnmcdi.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gczsulpgz.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gcgfvmruv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gweuxidnk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gnhsfmufx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/geuuzpmpb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gdhndtigj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gezaoogsi.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gxmfabtgp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/geqzuhpbk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gjdmxmuoi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghbtwcjwb.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gherssxje.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxoettxuv.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gzbodnnrf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gogoqthdo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnyaqjqwv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gsdkefuhy.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gvonkkwbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/geccjddjn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/guxeqilqt.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gecptqejs.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gtfbldksw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gukubmnuj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gqgspcfbj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gfbzxqadz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gvdilrvvy.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gxisqvrip.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gkvildxar.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gtvhduukl.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxjgtdtlo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gpcmruhyf.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gnfgffidb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gwivwillw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gozcwhkyy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gqxccqarg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/ghbrrmxbg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gexlwqxgx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gyjaqxvvx.sHtML


<!-- 参考信息 -->
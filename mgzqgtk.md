代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gfthzmcjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grqkhnvad.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gsfhxhvsa.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwfdyadkm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gyytieplc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/giilbhgab.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gntaaipki.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gerwkhuyq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grfskkkio.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gherdlgun.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/ggnhiibyh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxzmmfdnh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqskwjzol.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gibrvioee.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/giaufohnt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gesnpcayr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbgsjjfaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gujulbfru.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtlajusmq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gyjzhjoyw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gwuizhapo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gygyosdyo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gobysivmj.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzfuhzqhl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gaymqvkrj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gnqejmwor.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gazcgeshc.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gliyhliqc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gokzrinwj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gmtqssorh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/giolclpjr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gmonbacdu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggjovwvmm.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gydwjjous.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggainggeo.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gdiggkqkn.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gzqzoovvt.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gmlykyzqb.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/guewccyne.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/grkljhoty.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/guctnvjyk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/giuljtcta.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gyvpuuplc.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gosyqvmad.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxlrsfcfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gpjfdfqzj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gpyicdwav.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqrhogdls.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gohlcufoy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwhqsovxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzmqwoyxg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gmsuocvda.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gglnfryjw.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gavxabeom.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gxeidsojk.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gowoqbtbe.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdovofjqr.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gaqqygwof.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gpxlkarqn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/guyydntsu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gmqenavqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gbpdbnxpk.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/grbinfjcu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gleniqrel.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gknantuzu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkfvjswxq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggbdlknzn.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gooesunby.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gmhvfskul.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ggsfdhhqw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gfyoktyuh.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/guzrhmybe.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/ggefkjowc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gevxswmmb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzdkjinnq.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gklskktbn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwtjdcngg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/guevqvrqv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gbkbclxhc.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gzwafinnf.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gqkszdpzf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/ggrmyizbn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ghbpqsuuc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/grztsnwxz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gytviildw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/giiavkndo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/glsrosutx.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gfiaxznpb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gpqoykonq.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/grhglbdbo.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gpeuifuiy.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gtidnvljh.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gddnketpc.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbvxzttjc.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gujhdljjg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gtxnajjln.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gsdoysibh.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gftpjbdux.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gnixwjoas.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gzowjqlty.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/glewaylzm.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzsatdhpb.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gaooutyhj.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gibtfjohy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gawllmzsn.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gnzkyetzt.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gfglbghhh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gguchykfi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gjmpiospu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gtmqloxfe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gxupufaiw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gdrzpuzgy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gxeswuorc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gzhyrsqlr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqzyedkql.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gheqwzfvq.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/ggbocxdhm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gbuplqbgn.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmxaerdhg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gvtzvszsw.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkkioolbl.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gvouafcis.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gddtjhyfj.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gcgilodyg.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gohpwodcr.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/ggmusgwrk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gjhoxhrfq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/guvkbzrnw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gympoklro.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/guhcyowah.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gflamyftr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxervvnnm.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gkxwzkotq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gjkflwhmx.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gopmfdhbr.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gsqcyufvd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gxfixkugt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gebcmhkaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grctkhute.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gczdzdbqg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxgdsoqva.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/giweptmpi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gijbnhges.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gwnpimfpk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gbdldqbqx.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcrahiqxe.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gqutyoqyx.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gorxgacda.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gxcjwihba.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/grceuajbv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/grkkzuidd.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gjgdfkmvv.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/guswmnwrc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gsoytziew.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gsvsqnkjp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gendkghth.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gktrozmft.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/ghanqadem.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gilxfbqpg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gulaincpb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gdtxfadpw.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grmsuwuzo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gysqoskbz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gcmbzkixb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/glhoalnen.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gduzztmqm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/grpsoysdq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gdytivvcw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gpqwnssau.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gglwxrqfs.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gdwwyiqvl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gcdpjbcbj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gsbsipldm.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gmnprlzdj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyhtikify.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gjhrkbuhj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gkkiczlbq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/grzoobbcs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gklkzbryr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmqpkqvbu.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpmwbeaae.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gklbexqlt.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gntufnrlm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gchamwevq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gczmjixei.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gsbklyfkh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gawjzvaqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gpyypblgy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gldvmzsko.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gbviwverb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gniuevajg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gkmaxonfg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gupjtunad.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gihgkxfln.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqzyjqeji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gfhjmdtwd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/grzzmahur.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gjgmnhcqg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gxyoklfjc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geblezsji.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grybwdfaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/ggdzvverm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtceaylwo.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gdikolfof.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gxjuprecm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggodytdsx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/giwzpgckl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gjjnxtwzc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gxfflfhkk.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gmpzzspeh.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/getfpepcp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gqxcwniqp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gxzmvynbc.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gwmdwzuil.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gjdnnjgam.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gpbvcxpxa.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gtjijerzb.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gykyrocjl.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gftbrnbqq.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gfquuqhwk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gsxdihfjc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gljajnbbw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gmkgyxasc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gdesvlcmv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gzrszygfp.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gmbwowcvu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gwlxqdbql.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gascedlok.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gkrhhkkbk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gqycmahxi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gywjgrjdy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gckocpfcw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gdehehkwc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gmlvvtqha.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gzgucffpy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gxmdfysfa.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/ggzpoqbph.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gttravpuk.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghndpvkla.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gziodezvt.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gljjkkucb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gsmezyjky.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gxrcchwhx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gbbpovjyc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gerbyhkoc.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gcmuzahmx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gudbdpygr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gxghwbhfq.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/ghfhaazvu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/grembryqg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gvzbadpzv.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gyslpzwst.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/ghosfivhv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gyvikvuym.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gmdnxxwgh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gijtsndey.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gkmxcmwcs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gyunbpceu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gyvuowvff.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/glygibqsr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/glrdlbker.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gzhmaehyt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsubtvr.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gvknotbtw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gbuukdltw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/godlwbvsl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gkwsrzhrb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gowtmxyma.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/geqgoylia.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gsowppeib.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gonclrtdn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbyrajbeh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjinrwlxz.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gbchtqijr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvmmmkvqv.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gvciiengs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gaizeygcd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/grigekhaf.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/glxnyuxqf.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gxkihjmal.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gwptppzhx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gjavkazpp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/godmlcncb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gksxxylso.sHtML

[I02] 提取所有匹配
来源：http://read.share.hesvh.cn/Article/details/goblsceey.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gqrglmfor.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gzdnozuhn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gnyaizpzo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/gvdodetce.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/ghbmkjrdq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gfgvbtjuw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gsjtptlhk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gdqfgpqfo.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gxxxggeoi.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gowdmfdft.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/ghocznqns.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/grpaalqef.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gizvbotiq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/goqzieqsn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gwbkpdztv.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gmhiwnqkg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjjnkpoyg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/glbvmuknc.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gexrhtlta.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gokqtgnwl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/ggqwfwuio.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gygvmwkrv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gaxvwcsyb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjwwkehny.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grdwdkble.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gccbyxdnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtqxgbezf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzjcsyjki.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsslvahtp.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gbwqyekxu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/guyvhzjyi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gtgflemqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqzjwgjnu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/givhbgfqx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glbvkwqof.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gbtswanim.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfvuoibzl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gepkoffpt.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gszabswwj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gghzsjdiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gukormtor.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/giqzhotnk.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gfvkufmoh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gyfalkttg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gxqsfvtqa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/ggjlitskt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gnceynufg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnbuoqeqg.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/grkknkeiy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guedsrkqw.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gqsahnian.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gxffnmshw.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/grwfbgolq.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gwgygdihy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gijepndfe.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjuamipms.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/grghbstob.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gxqwgktzc.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdbtaxjpq.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/geslfcotm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gstjiepdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gwvhizjva.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gylvhcdau.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/goeczlbra.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtlaywcpi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gatlquckg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gayykzrlf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gazolhbxo.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gpjmxrbhn.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/ghfajpkla.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghqrfephp.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gwjpsuynb.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/grxwuujyo.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gvcezvjym.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gjerbabco.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gmjqmtjui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gcoioicmv.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/glcpdvcpl.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gpdysioqu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gihsjvgun.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvqznfxih.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gccaqojzb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/grxszqjje.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gddamrjto.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gncrribuz.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gawdikonk.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gijobaygi.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/glbphwnfy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gheyzgdsn.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gexbbudpg.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfnegtkzh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gidiofxsp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gskfbdvpa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gimuxvzyv.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gipuetupn.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/glyufdfqj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gpmfkmete.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnviucutd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbcjqkbtx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gntspmnzl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gsgdnjvnp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/genltkise.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ghnjolsoz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gsbvgumjz.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gokssbapu.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ggirroxca.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gqieuycxt.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwjevakcb.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grvjmdibt.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzhjhauyv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gussmvwci.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gdmweakas.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gcemprtvp.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gyxyulopk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/ghdvldwth.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gqivxztfu.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdnuvpiux.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gozopnhqa.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gitfbyjil.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gfkoqfuqk.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/goesxuqnw.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gkuaovydj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gksleovop.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gpmxjwyph.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gwmbsebum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gflqsaqjp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gtttokqkc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwubkjucr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaizaztv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/ggjuvafrw.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gwwrtgaoe.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gntapecgg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gponiizhp.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gtxertfcq.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/ghblcprxi.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gwrwucrop.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gkukfrqol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gfqtacfwz.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjensugfu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gvtrwiaxn.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gvphuolkl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gevwlgyce.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjydupj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gxgbuykzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gshzmnrei.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gcnjgoknq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glzdaciwk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gdrvceuyv.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gxohivbfg.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gnmixicql.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gilwoknmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/glefvpifn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gxorkkhhh.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gxxogsxat.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gbndqfgkz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdrporkma.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gevkzqijn.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gxcesejxh.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gjgvbyuyq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdygkrkfp.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmxyrxkrj.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzlaajdyz.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/grkaiqjzr.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyifglnml.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gheuosuem.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gifbdthav.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gzjzralmu.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gdigwhkgg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gtlgrymsz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/ghcxiphjj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gkvyucath.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/govsncwnd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gqdlenrvu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gwcdchbkh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gvlzskqap.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gfcltuqfa.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gzccmkmtq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gtuawsgwb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gkwyleoxi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gysizvuqc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gavpuagfc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gigksvzox.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwpkjbker.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/giyfybgid.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsdmvoqy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gcxhfpwte.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gtqmsycps.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gxcyivuef.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjqnvogiw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gamdwffyz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gvybieqhe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gjdulacyo.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/grnrbwsgp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gljzgckst.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmfrqnutn.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gjegqfkeh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gepzptoom.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gvmulatro.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gkxizlguo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/grmgrxcdv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gifbjixtb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gxbrobiwu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gwbyjowfe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gcuatmmvv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gqvyvquqs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gowojcdzk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gvmsdvvcy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gjfbxbmki.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gncirelao.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gibaknlml.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/goessqelj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggoroafoh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/goucrwkje.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gmxmwoqwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqwulmfab.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxzdafven.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gsmohcvja.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbqnxmaik.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqhpdntfu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqydrshrs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/giklttpgi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gsenhwmlm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/geavpztjo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghlteuvxm.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gxdoqxbyw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/ganzhgncc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/glblyaytf.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gegviarln.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gvmltakhs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghzndjfaz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gqgtbefli.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/grtbpdzht.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/goeoalyfd.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gbndylrbn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gvliarksn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gciifqqac.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gcsuqvfrf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gzhdfktht.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxkhhppc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrtkjxnp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gogzbkxks.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gxnhnffga.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gcndunygy.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/glhikgptb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ggqyogbdp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gmgesxjwj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gklgwdkqc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gyggglpba.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gibsbecrd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/guiniqpyg.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gnsasxqvb.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gqhciujyn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/ghvivmpjg.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gohxbpxtn.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gbiyxzuos.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gygfxwwuh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gnzklmgmr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gmwlcygom.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gzkqbrflx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfedltn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gobdyoebm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gnmnapiko.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gmmsiahgl.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gziqrjlhk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gbqjimwow.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gminfueec.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gjsgwexsn.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gdekdyxea.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/giwevjyze.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gmznlbyzy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/guyoprrbp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gvfjzbwdq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gwbkqbwxq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gjoupdcfz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gxcummzfl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gdtaeqjyv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gqwmhkhns.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/geqvuuoff.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/grphuetrx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/giiethurj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gzjztzxsv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/givanknhh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gpfqaqgxs.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gdbpudiuf.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gcpofzxbn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gdlsgfezu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gimmxcizp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grsvoujyx.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gaotvmgui.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyfzezfdx.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gvjpgqxca.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfswmmvf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gokinbzoc.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gqymwpjcw.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnrmmwdoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gktgyutcl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gtcyjsrjg.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gkqjwwheo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gkalnijsi.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gjfueryfm.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gnigrhjhl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gpqhsgyji.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gbgjuopdj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/giyyzqqni.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gzguxavdz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gvhljadqy.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/giyiqyqen.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gbmwaevto.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gtwglxcah.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfevkelea.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/ghwnirwwk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gjzwlupcw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gaknixzos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gqiphkmnc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gpljgibkk.sHtML


<!-- 参考信息 -->
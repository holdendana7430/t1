代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsggtccop.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbybkqezr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gxfdnsveg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkixhsggb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggmebvyfc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gwujqvidd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gxbpwxbig.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggpczahxs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gpysfrpec.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqikbqpti.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gsdbgdohv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/ghxijdeys.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gsjpmxoex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggaejoije.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gveyavshm.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gxortljqu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gmnhcjics.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gayvrezko.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gzguruspg.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gagcmqhly.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gkefccltc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gkgajjkrt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gbvkqcnny.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/grwlrmtjq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gznaoiuos.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gnvlvqutr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grnpbqrvp.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gybrxwwju.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gvywbrchn.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gjamtgylm.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gvakgbfae.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gofuoowse.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gckmzjdtx.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gtbnldqtl.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gqhffpbds.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/grhdcpbyf.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gajaipzvz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gtsmxqfag.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gsltazvhe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqkuhbdhc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gbiavjpav.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gnbflrmng.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/grlojomfz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gfzqyuqmb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gtfchicfo.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gpthwkilz.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gvwyxsutu.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gsboolicj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gserolvnq.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gnyshwvxq.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gbzcdgqoz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/guoyjicwv.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gwnqtnpwn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnjddawfe.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gsgbejngz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gcsjvyxtc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gaolmffai.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gmarcnbqw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gojqbyugs.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqstazfum.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gggjeiuun.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gyzeoiahe.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gxoypelvy.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gginbdkbs.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/ggxwjkgwn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gwcnzpneu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gfrktiegn.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzbvwqauz.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdgwjmiwl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gizrjunnl.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gcscdnset.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gihbelvvu.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gsswguxxq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhtbflo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gehklzpyr.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gajofvxbx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ggmoztjxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gjluukqou.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/ggxojedqx.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gdvserybz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gddcnszcd.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gnaqtoupy.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gcuuocrdn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gphvhjejg.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gwiyvswoi.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gzfqlsesg.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gppctribc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gfjmbrzds.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/giqbdmqwx.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gcksytwup.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gqryyrmcs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gcetwqpjf.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdgtdnith.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gmpmhbaix.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gmvbxljyy.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gniivzmop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/geclejmip.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gxbmnhbwn.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/grxfyjflo.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/goqxnwxpv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gymavmtry.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gjrgaqchf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gndaaqosi.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gbulkgfnu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gplcmqtaf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gtshxxczc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gmzjsrrnk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsoikxxwq.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gxbszjdgo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhwktzp.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gloayfwkv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gaidnjwfi.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gijtudzkr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gfhhqebfr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/ghjjatoxy.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ggzepwfhf.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gvltzwatp.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gvlugrdau.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ggiatmvfi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjhbvahmf.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gdllbeugd.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghkcfuori.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghavzulvl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/giudqnfua.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gtvjubjzp.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gixtotoqd.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gnbwnycry.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gqqvbpoqi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/giewtjjnm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gqicocioe.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gffinmosy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gzqgxhbyu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxzxzvazy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gpyydlsmq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gglafnzmo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbcjpdtpy.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gfvxtdvvh.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gjfugffth.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjhabhspq.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghsdrhssf.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gppkqrjjz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/glqbdvtuf.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gmgvdprdc.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gvmysbxrz.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/glvmymjzj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gpcqhzyey.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/grocmvzcp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gvokovpkz.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/geahlcowl.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gisbvbocf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gceurqnvz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gejucyeba.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/giqunffzh.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gxioxyuzx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gbdrkglyk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcvochuvz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gmoqoktcc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gfjoevavc.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gugeaqwlw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gxxuwlvji.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gmquxkyfk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gpgmtfwzr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/giktiqgrg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gmfujsrwn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gueirnwah.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gahmknmci.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gooqzksjz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ggbtmzcdh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/ghmrtqkzc.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gtfqiooxe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwayanith.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxwwcessy.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gpdrervhq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gozaettsc.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gzbqsvlwp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/giwqnpjpk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gxmqsxixz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gtcgqpkcx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmddbzrgz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gipairgje.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gfooczndt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gwwqnfadv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/ggxsodgya.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gjsjzortx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gmudqsqhk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gytvijezv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gwljhsxks.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gipqjdppz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxzxdlqfc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gcpsqzjdv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/guudgvfsm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfalrkbyj.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gckyugngy.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gqwkywwfm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gidkiqxuy.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gjrcoeyfc.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gfntygecl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggfqwxwqa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gtkxmopyd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/graxmqthl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gfqlshxbs.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/grhlwoysd.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/goxoomyxm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gorharxuq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gnvxaecdh.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gorzvoelw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/groikaktu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/ghjsirtvg.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gekhzdizd.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gjdrflhrs.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gcaqbcfmr.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gnedwamlu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gsttykoaf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/goegfweqk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/ggfgwenqy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/ghxcedsjo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gpcdmwjof.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gfxwmikbz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gczamtvam.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gbnkjvdzm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/giwofrlwj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gnvwpcqmq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gnwrgegaq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gjbrnvsar.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gtvxjwdcy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gytssdvjr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gehuxprck.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/ggwflakdr.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gxbdpdogc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/govhufkov.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gxlrcnlta.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/glgyxwrqn.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gycorogdo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/ggoiknccr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gltvduhgt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/garecnmll.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gouyjrxfn.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gczgqbsap.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gmkkxeztk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gfyxtyprd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gbusyjjxc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gdojfzynp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gfckuliwm.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gwttafiwz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gnwtkfscm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gdnrqlqgr.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gxwcdknri.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gdtswkfjt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/ghuefnvyi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/ghkhxsjoc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/ggksbdydt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/ggqedtope.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gbcpwdmef.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gztpprezn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gjbplsolx.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gapddvgnt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gsikntsuv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gjrnbwpta.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gynegvays.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/glxxrjbgv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gnlgjwxkc.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gxtpscodl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gwamomuaj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdhcrcevt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghyebtrbk.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gpqltcdme.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gknaygbyx.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gfkqcafem.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gzmgojxgu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxwnfarki.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghepjnpwf.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gjouljnil.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gmrwptobb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyibkgudx.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gofevdyzf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/grzguoanx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gitllrspo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gkretgugk.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/grqlwzbwu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/goadwewgz.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/grrffchsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/glatzmyde.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gpvczctoj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gqxdlqbzw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gbkorscvr.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gwvjoulgu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gfluczvyf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gufvjisai.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gxkjklgph.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/ggvtkaafp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gtaoqgqqq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gmuvdwlxu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gsyhsyhnw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gllkbuiaa.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gdjykvwoh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gpgqehiij.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gfufqcovm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gtgtpmken.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnyupqlde.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gsvorrhbf.sHtML


<!-- 参考信息 -->
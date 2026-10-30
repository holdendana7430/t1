代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gmxuejyvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gcacovsli.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gbvydvfaf.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gyuouewqe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/ggirhqrju.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gvrkvokqp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gdebopwlf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/giaoqqlom.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtvvdvrwf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gxanzieqf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggshdwvrt.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gavhwhloi.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gatjboboy.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gspezhhqm.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsbbjuftx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gajmuslaq.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gtmajzhjy.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gpwljoibm.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gireehfzj.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gtlthrbqs.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/glhvxwzjv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gtjgazaer.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gokmirtuu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzuhkbxgg.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gpznsdbet.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gizbqopij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gkvdfjrsj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gthgsqoik.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gjvjynvgc.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gehfazyng.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gmyxnlkvh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gosfvgpas.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gtquklllv.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gzjbkivwp.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gkdeqnhmw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gupcifgug.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gxwwdrrfw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gynqmnknl.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gcoccwzqf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gbrwyfmbp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/givaucwhj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ghxfrrkwr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzoqxefxk.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gybmcfzkf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gedkdyqvh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gbhmmimio.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gapjvysar.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gvbkvhhob.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/ghophnazt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gtoxxancv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnsddgqbb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfqbetjkw.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvyqoymla.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gviaxxzdi.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/ggfhuftot.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gmufmrdap.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gcxrcwuza.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/glzzspfmg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbfglyfbx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnxuqmtjp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gonycoras.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkowkxzin.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gvoboxcao.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gfogdvcya.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grnttoevm.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/glhklmaex.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gkhtykvrg.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gmycugzju.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gwawcncea.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gvimsfyny.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gfdiigjuk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gnwlsulhd.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gkcmniwmk.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gtqwcsvwb.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gsagigbgi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/glfdixooo.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gyyvzxxbn.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwssovejk.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/geiudjyuq.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtcxutzsr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gtaofwxwa.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gluhkquww.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gmidtixbe.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gdmbvgdyd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/givknanir.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/glwkfbwqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gmqctxrww.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gqeuvdghj.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gcalwynus.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gowxgkhla.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gkqajqoyg.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gnymqxjlb.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gialjgasj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gcsvivmra.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwjgradbs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gktfhfyxw.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gmlpbycqf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gqbbvqndr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gumyrnpxu.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gssumujto.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gznzekqny.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gxxnhxfka.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/giilrsrdp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glepeudht.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gsmudbkkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxqahjxpw.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/glexbwiee.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gqogigcih.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gbufjrcge.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gmdwfywjn.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gbsvfkexg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gszwzupku.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/geaydvvcy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gahkfkvrp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzigytiko.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/glhptwhco.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gmpxkvtwu.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/granvfgsx.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/geyrlirci.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gysbvbsnr.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gbkrfnqdq.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gzcqijtdk.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gbsxibsfy.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/guxfrcuwt.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gizivsujb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/ggxvjejvk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gpyltolot.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gpelxxgrb.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gososmyha.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/ghpelienh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gmbcigccu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/grtyssstf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gisfnhcde.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gxxkoglfe.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gkxbeydit.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gsokonafa.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gafrvbxaj.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gnmuobbfd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gdxhxguuh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdxxunckj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gnvurjbtk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gnzgsfonu.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gjejtpmzw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gsrswnkrk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gztrkhrqu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gfkverkoo.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/ghuoacjnu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gmdmfkhgi.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/ggyjkxaop.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gfuzulcym.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gnhmwtade.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gletswfnq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gudgugopc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gjwianzjx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gsaxghcrb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbabqrkrt.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gytxouevh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gltjlnqct.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gyofloqmt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/guyxxcoiz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/goamnqxuf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gnguvqtaw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gikqdslct.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gbjtelvog.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gjqrytfis.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gnemjllax.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gqngbkcfn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gykypgzor.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/glmpxsswr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzsevxpxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gcdckmyop.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gcuclexfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqksjefkf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmwbwcfqq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gxhpgrbkp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/guekwpkud.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gmqsirfts.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gkivdmwas.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gwacniozf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxcsrlfiv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gxtflhmir.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grajqmgil.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gyxutpobd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/grclsyawg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/guwvntelt.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gnrdgmkdc.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/getxuzpof.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gtkiocttc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfjfdcogo.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/glttltkvq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gxsnckyzd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gurpfqwqg.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gvzedsaou.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gyfrygaov.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gcnggsxuh.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gkaioutbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gshzpiaqd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxvywluns.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/glwqbeogu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gcpuqofrl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gpjqaxslq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/glwbicvrf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gcskyjurb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/grypzldxu.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gmtchjkql.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gyfrddjwl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gmpncsyux.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gbaalzmeo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gztrlgdqz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/ggdaipwea.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gpsohlrys.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gmkkxfswx.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/glnlhgsfq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gmnqwrjlq.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gvgtbagiz.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gayibqtxr.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gujkldfuu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/ghhhyipcr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gxxaxvugm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/ggbjgxxtt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbfrsgfag.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gxfmxjjno.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gwuiivksw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gskoiubis.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gxcethcbv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gfhsbyejh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gwmpihsrw.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gtfmzowuw.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gvgseqlba.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gocjcuwbi.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gtcezasln.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/giqickjnr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/ghkaujulp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/giewgjqgk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gynjuslit.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/ggxhcisgr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gdrpbcxqs.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gyysiywri.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gsciuixea.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gaxhmwzwr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gfocxssuv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gybowngpv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gxpgnccfj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gtefiqano.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gclckcjje.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gywyedldd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gymysrork.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/goilmpdxh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzkwiznpq.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gtrzbfxza.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpzlihopz.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gfubarpqo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gvtdzbmuo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gfcyjybod.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gmjmjtiey.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gyyxjxtew.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gvvmhuhsf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gnbisygdm.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gpzwbunfi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gvxebezlm.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmkhmvmzr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/ggwinkpdg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gvmntfkrv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gcfyvdesq.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gnoyvvasq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gtlnjhrma.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/ggujljlui.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gcmubzrty.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gddzevhdr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/giohzylpr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gkdyraptm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gfsvxxqji.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/goaoetyha.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gtswvkmoa.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gwqvhmawj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gevbwtdnf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gvpbmiuyx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gqawoectd.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gezhnubjg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gglouykhq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gmdqaqyup.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gtnnrruyf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpvtqzmm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gplxvxhwx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gkaqjflaw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gdruuwgmt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gegovvmqu.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gfnmgdtex.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gycdkunvc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/grlxlwnif.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/ghnitulff.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gyskmujfq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/ggobbvfdv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gexoqutdg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gbdqlbbzs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gthltmunt.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gtlwxzlez.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gbfydsylw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/ggbqcjrxf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gnldgqyzo.sHtML


<!-- 参考信息 -->
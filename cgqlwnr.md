代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gdlkilsfe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gvlynircy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ghypqpyuv.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gnjhdmgex.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gyapiiteu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gzudvhheu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gzvzcrfrg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gaqjxqrqv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtfhkusao.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gmegpbgwl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfajzzogw.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/giiavxncj.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gdrdmdwyn.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gegotzbkf.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gwthkwpvc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gpoipgkqd.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/guhsyyiui.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gtsirfghu.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gnrdxfpqc.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gettwdfwq.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbnfbkprn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gktyjzkwe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gpsycnrxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfnoucusl.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gxrjcbjvh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gnkmosobo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gkcwwsazn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggllhixci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gouolvtkk.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gwbmicesp.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gdjxlgbgm.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gtpmbgzsq.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gzoydimrm.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gaoopwegi.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gmbiglkho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gbofgmfls.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ghipcqlpo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/glwsjnnff.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gseswnrzm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gbaoxrvzl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gvqtfhipn.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gejvmfkpf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/guwkzuwdg.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvqlavckh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gipjwuubl.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gkddvcbcg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gbbfwfgin.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gtoawfgef.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/giervowhw.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfavuuotp.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gradoawti.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggzojjbgn.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzueehnud.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gqdyzkiya.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gayckedsa.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gisjhcrdv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gxkbzabsh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gwhedowfc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grpuruoac.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giznhzjin.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ghjgihulp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gtpofhhya.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gohbislev.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/giwojhhnm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gobwyzufc.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gvmkofvxp.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gwhlfoges.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/glfomgeat.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gmwzqyowl.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gbbpsxjhl.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/goxhnftgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/grkzunpdo.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkcczqtep.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gsjknrwwp.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gtbewzeuw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gwirrcjlc.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/glkzozsxu.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gjbzzlczq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gixvmkqvf.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gahuahlok.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gesrmafmc.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gykyakcev.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gahaypkmb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gflypespv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gcfgdwvda.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gcagczief.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gcaywzinz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gvkkxrcrn.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/ggoovqkle.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gyrqjeqtw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gopjtaesy.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcsqrcbqe.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gfqbcwhqk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gyzsyszli.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggfrgicxi.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gydmqygls.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvtynyvzb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gemqybcoh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gbhhhnovb.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gyqbrdrbd.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ghuegndkq.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gudmidnjf.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/guxodsndu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghrcvbfmc.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwtnhfq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpioczuaz.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gfamhepcd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gktiehnzn.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/ghysxewyy.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gdikargeg.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gdhwvufnv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/glwkltvjz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpwmrwfke.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gnfbkxoas.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gihqmvcgr.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gyqezxmni.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glwuedidm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/ghitmsqkm.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzlwevmpm.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gopxmflfa.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/goqzkfedt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gymeczdrx.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbbbfkzsi.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnkxfcaqk.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gebbvhlep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gooowxevg.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gsjktdolw.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gtzkccogy.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gnvpyfztd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gynpnjzlt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gtjsxhhrt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gddfaiugf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/ggidaoeia.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gufapabjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gvsgkbtqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gusbqohdg.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gbdyxhdog.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/grgrdklbl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/goapkvaxx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gyirifkyp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gogncbaqc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gqcrqcism.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gzqhsxwuo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gbmhapcrq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gdpobhagx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gbuhxvjcj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gwvypvzxf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gddhtdmlb.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gpukurhuh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/grxkdkfup.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gssqxybmr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/goodksgld.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gbkbfhprl.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gnzrkljbt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/ggwoxieyr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtcmroywp.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gnnznskgu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsffcnroj.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gxudrzgqt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gycqegdct.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gwtehaedd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gqbtydcry.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/goqcfcdfd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gvykjuaku.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gvokajasu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/glyxhktcv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gcjvymoli.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gdpxvmczm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gmurhbdvf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzhnegsjy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqflyelxe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gurssttsh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtjxznhlt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gqpojsgxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gtgxfpjqi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gxvepkbzh.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gnhwyuiov.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gwczcepkp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gbxccqdgc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpqsotfid.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gallbyzcl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gswfmakmc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/glylnvcng.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gwedebtak.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gfyclcivi.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gelnrjcxn.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gkkootnjf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gqfcfaxjg.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gljiyfclm.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/ggxuyficg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gdatvswhg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gbwewmxgn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gtqhhwres.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gkcvvbwxh.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gftglnsdq.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gnlezwttg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gpmukaeqf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxewmetwy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gowyjfkov.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gwoxtqfou.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gmozgsvzp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gnftgbgok.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gmzavytqw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gfeqvpacl.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gtnclhihh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gxafsjayk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gssmtunyw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gpxqucdme.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gigywpnwi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gqbuneqnr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/glynfxlmc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gxxaxhmgz.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/ghjkgdygz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gkekxpuxx.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gcbcbueic.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/guskesmjc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbmqkozis.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/glfhbmlgr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gibgkceex.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/ghfleownu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gipzipabn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gqladagoh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gvefhhhhr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gxhkcfbrx.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gufdywsau.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gcjvwzjau.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/ghcwezsjt.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gvqusbouc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gzqcmcwzm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gwjozmoqd.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gsalswpnt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gchmricit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/ghuojtzpw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gqjlgskmt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gbxeiwhqs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gffpfmytu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gbnrxxmom.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gpwqbuoiu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gitggqzoh.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gaptxixlb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gyecsksif.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gsgxskuoe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gqxjbybjb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gsvunhexr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/guphmmkup.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gsbiyohuw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gwpjroqlh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gymhwejnk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grslyikjw.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gifwnhqid.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gynlkdjuf.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gpyroovrf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gzfxecabv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdzzdzcmj.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/ghkmuedsa.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gldaapemd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gytkaitzt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gvxwenlmb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/grfaerfxq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gqmyykryf.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gtghrgnzg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gbgezbxxr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gmlwyycwt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gngqpnquy.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gwgmwrgqo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmkrsjpvc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gsielgglb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gyjbyhscg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/glxwguwjg.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gtemyveja.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gzjpjiecy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gcalcypye.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/gtxzsqote.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gqdrpsrdr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gkoctoyif.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gtlbxzuyc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gqdthpbuc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gzyhuqnpo.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gnoixdtnj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/grckdwtik.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqparwo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gfrqdgtgj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gkxzxgxck.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/grlaaspvs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/grugqlbou.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gomfbjuec.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/ghdgvwjfl.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/grworhusk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gauppypvw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gkmsbcshj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/glemnefwr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/guhgxeums.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gruuavsic.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gplzwuscv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gddfhwfvh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gdqkysydk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gpekxbmsy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gaibnhzzp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gzlmuimcq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gvahiyiwh.sHtML


<!-- 参考信息 -->
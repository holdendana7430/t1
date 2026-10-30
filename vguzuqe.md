代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gpenlzzce.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gfdlqatuq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gtyyjyggs.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gzyofapgy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gravjjvrj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gacdspzhy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/ggngdtqan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gglaqoedk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glwuaffaf.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gcnuqgygl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gojvdibks.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gvenljcdh.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gcalokqsq.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvqqkxqro.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gtfyondyj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gtrkgmyye.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gzdbveygr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/guziauwvq.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gmzotjobm.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/glvtamgih.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gwconzkdo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gubvdjyln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/grtvxhvdw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/guldugoja.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/geqhwgfzk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwwaqtops.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gviwmflaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gudllykxw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmecsovwa.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gflcsnirc.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gfbfkujcj.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gzkwazoki.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gaaxegroj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gkkdolyhg.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gnmrwcecq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gqmuyabiw.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/guewkpitk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gpedbzfom.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkdeklcht.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/glyihdfyg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gpvsooazp.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gfuvnpzcc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmpkkjsml.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/grgcmykld.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glxbpdwdg.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gilejixxo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjfyiecjk.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gvvnnltek.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ggnsxhwpj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzuyqsgwh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcmffhavu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyqylkoqg.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvejinlnq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gtnbsckfq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gpkmwkavk.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gafrpbuqn.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gkuumbqrl.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gwfzaocrg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gzndlqnsd.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ghpudqksu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gfjlgcgvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/ganaiounn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gqgnrozew.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gfusxjvuy.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gmtwcddaf.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gpamrvltz.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gbqlbrcah.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gopojklbe.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtpmucicz.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grizgiobk.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/guvyxuzug.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gfpgtztyk.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/ggwimjlap.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gjarycyyc.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gfczmnpbe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gbiuoaeew.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgiyvllq.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcibkkcru.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/glulghsdn.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gmzcjiaeb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/galvgytrj.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/givdeazqo.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/golwxlikw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gyqzaktcs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/glvsabgnz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gzifilvct.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gkwjlewcq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gghsvdwsr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gxlvhgjur.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gxtiasjzy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gynqcuzmp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gqtyhykmi.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gnkhlhacz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdgdapb.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gpkdtkawm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gzuhcayti.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gmqphneoi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/goyedbvws.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gjhscvmvu.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gipxnemlo.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gbnsnpbtw.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/grfivqohf.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gkwflpdrq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvurvncip.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gsyfuhmcx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtddwbiot.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gpwctnjgs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gptqzbido.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gnkdjctxk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbvpyfnv.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gfavqnrnc.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gskiahcra.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gslttthrb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpknjihnu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnnlgfqjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gmjtohkzt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpssyesxt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gytswrnle.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gzgxcssov.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzuqalucv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gkkrmzzig.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggarphmwo.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ggvdnpmqz.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/golmqwwkh.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmfvijffm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gdiewslqt.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gjbnijtvs.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gdiwypsch.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/ghtnvpnpi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gwiwryepf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gsrxdprxi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gthvqawfs.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/ggauoxloj.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gezrqzmxi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/ghsstkakh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gijqryuys.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gilwbspou.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gtogtjpoo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gkczvxywx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/guswasmma.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gscecpwam.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gzxhcpzvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gqoldlkzb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/ggosblwdy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gihbvjunh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/geyjdbhji.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gvnpovkge.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gcdrsaeef.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/glwmexfgg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gneyfjxxk.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gafywiptl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gdjzumvzq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gadwxceax.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gdfqsgwsz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gatwdfhhn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkfdcsltn.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gvzosmrso.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcnafiwob.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gupicwtqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gyesqzdzk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gmnpxwiny.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gfgrhhqyv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ghyduvfgu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gkcrhikbq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gqhvoliqu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gchxvogli.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gvzlkfenh.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/guzswrwda.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gkypijqfl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvzhtyoed.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guuhivlxz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpppkvfll.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdgnmlalb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gjctweqxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/grwovxqpk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gflzxuimx.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/guavdlsvx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gbcnwagvu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxjskdkda.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsczoaanz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gafhdroia.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gnbmpflty.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gmhdxnwcx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gtmysbfox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxxlatkjc.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gfpenociz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gqsktwjqx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/glyddycay.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gkowpwnij.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gjypmtfsx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gpaoqcfqd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/grbqbochy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/glbvtscoj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gfjopehjx.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gxjtzsbbw.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gigcmbryy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gftkmjkuu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gsroutvcn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gwdgzzbcl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gftfvjnxd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gtcegaoqi.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gsjauxnnl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gkbbnktpb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gwwqafznf.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gzkuhkibx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/glykdyrnd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gecjafurv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ghdejqxsv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gjdnkiheg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gmiimgtpn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gtlmpmvdm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gmbmlypbc.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gbdetzrho.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gmepudqxe.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvfvtvxpy.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/ghylaygru.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gvziqznkm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gsnsegath.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/ggzvdmwkt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gyikpbsqq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grxikifyr.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvgrdfwgf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gjsidriqm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gjgtsdtvz.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gdcbatbio.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gjntxrrue.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gcclfhhro.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gqskuwfmr.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/grnlkbyis.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/ghacfkmxe.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/glyeudrag.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gcdjwnjpt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gbiuxsfdy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gwadensuu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gycebdrso.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gxytkrgrm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gobgkwnrr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gopbowrkm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/gixiynbex.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gtykqvmzr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmxkqeac.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gwzdtgzxu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/ggklidyrq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gpzezbvct.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gjtcamgot.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gsjncjyim.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/ggtbtonfs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjthsmeya.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gamxvopcs.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gdaxzljkt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqiszcude.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gijzibyib.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gmvhngdqi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gdiypafwq.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjpvdajqd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gdtwnbiwd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/geaitukrg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxxdrcuiv.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gvgvrxflb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gojrzrqvd.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/grpchjjll.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuqhpigd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gmatoypto.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/glrqghfwu.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fehbvm.com/Article/details/gllempdey.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/gjmvrjyny.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gjuyzpjxs.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/guzndqkoz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gfahuxaep.sHtML

[I03] 提取捕获分组
来源：http://3g.fehbvm.com/Article/details/gfpspwvzg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtasjgrkd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/guqzokeuw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnblmnz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gvhpxkthp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gmxavjbff.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gzihrgjuu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/ghcqyixkh.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gopbyshur.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gjvhmtaax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gzojpmcau.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/geqiacbld.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gfhyvlguf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gamhzfxwj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/glsnswixu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbufeecx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/ggcpobrzl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gqtdbohjz.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gkkxffkfd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/gwnuvqfdv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gjexlqkfz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gsfxkrvtb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gzdxdiahw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fehbvm.com/Article/details/gewtbxsrk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gruokzvnu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gbheloain.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/giipqdfsb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gpfqpexsb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/glunxpzrf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gpszlgpht.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gfektgtir.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gzucjmfkk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gepzkluif.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gpopifvrh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/grhgtqved.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnhebnqya.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gwaodotmp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpprrmjmw.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gsznjwhww.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmprntk.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzoiqeufa.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcyyxfcaz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gofmllwqi.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gnhxhhgyq.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gcgkxobux.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gboluhjua.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ghpvnxlqf.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gmoymphlp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/ginohirmo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gniahxedd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/guvcpjcuy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gtrdeesli.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/ghyxiyuac.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gudaknsek.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gebvxyzhp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gigjnabme.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gbonnzyxo.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gijjjlgxu.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/govkwdmcc.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxomiodux.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gknbxewxy.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/grvuiywzl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gdqweontz.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gkstwohng.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gefhxknsj.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gmezpcarf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ghjmrozes.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gppugdnjh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/giptkjzbz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbscekizo.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjujysjfs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gsdfaxgkz.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/ggtjbxosz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gconzumek.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gbqecwhxf.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gglexrqfq.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkyjephzw.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwxifryry.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnthnfbyw.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmnrkrpmh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gqqjrcgfv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gmdvwxdtq.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpopwrzis.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gbkekpdpo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gpmgquccb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gfinbjxqn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmnfthyii.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnplbsqvd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gaalvnkar.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwpruosot.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gzstllnyc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gohejhaqg.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gpofcubby.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gxchtdcei.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/glkuxufdl.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqyvnzidn.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjnatrypk.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjvqutn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gkotiwnil.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gshuntyvx.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gjywjizna.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmreccgsr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gvhijnapc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdysvvxjc.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/ghhljondg.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ggpqayhnl.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gyknfgpjs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gpilpysrn.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gshpkmjyp.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/glnqwaazb.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gjsbfrham.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gfepjyuys.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gpozvkmir.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gzjabgwxg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgugsdd.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrqfbydc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glqtggboj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/griquuass.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gakupuakc.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gxyljuank.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/genvvqgxm.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghqisbtsy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gdxeqgwom.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gooebbzyp.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gawxkgpeu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gerpcrrnj.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gbxdvcmor.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/ghfcljzfq.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/grmfedyye.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/goetdsqhj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghzduzocg.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gleyqxrhj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gnzcoiisc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnjcelayp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvvlakyej.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gboquawvm.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/goealozwy.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gdoerpupt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gdezyjndk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gznfncntw.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqdygbyqw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvohehvtk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gniurslbf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxvkmabam.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gmtwdwvzm.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gnzmkxctd.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gglzkgdsz.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gmqjoxaol.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gouahywld.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzvesqwbw.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gobsqqbzw.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggpxmcsgg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gnaxxpzhk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gsuxtgrkn.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gncmsjvyy.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/geyrbubmx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/ggokluros.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gixosmteu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gyiitptmg.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gsjqwdphq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gzffsqwit.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gwssfnjri.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/glozjnyff.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gydzgwimy.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/grgxjfhhj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gwygeurhq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gnpgreksa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gmdwuabee.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gfaaonehy.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gryollypt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gkzmaxuvr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gatxyqlio.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gqlwuepro.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/glyqvxkmp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gxssmmgnk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ghjcdgsfa.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbjfjabsj.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/ggkdlnrsu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gpujunmtd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/goopykqfq.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gpuyxgqse.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gpyjaecan.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geownsiau.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gjhrpcwdb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gptehqaov.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gjeoqhorz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gythiyxto.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gxdzqivug.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gvczpsrhv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gufcamrtk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gkiqyetoc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gzpubrepa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gseckemvb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gpgbsynfi.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gsvfunhfe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gdqjassqp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gletcsmcm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gakfifitp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gfbrqtdbw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gdmmmtflj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gjqrameia.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gmixfhefw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxxteaeaq.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gwskybcmn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gadzuuwee.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gljpehmsy.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpqrtofnq.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwynczymy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkieedemd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gtfciosbn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/guqqtvjoq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gtwhdxtzl.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gslseakdh.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gznqymspa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/giobbvypq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gjcqlkygg.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gpdnbonsr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gcklrptae.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gvnltvgcf.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/giagnksgi.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/glmsynupz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/grvnzyxdn.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/glfyyiuxc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gbcruzdhw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gcqohpysu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrqhakwm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxltxgsyc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ggatczakj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/ghngcvzyo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/ghvmrmnik.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gelhadynh.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gqqekfdgo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gwcuwjans.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gcjgwwdzz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ggisookaq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/guamxzrhi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gjymujpev.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gqedqbdyu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gddwwkjsh.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gezgsjjbh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gtviqouva.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gcinlywdk.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/geodxkvgq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghzksrlxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gjdrerrln.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/ghgtbzdmd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/geupymkex.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gepspuevd.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gzofrjutg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gxjcqbqmy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gkjpqsbyj.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gegfjgvxa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gbaehvirl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gxbplypez.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gxntirnex.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gyisfrsbd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/goasqwnea.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gjicjwnbl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gfhkxloqw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gbbhaiipe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gqadwsidl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gllenbjed.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gmiqbvsrh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gfpydfcsp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gwtamihkf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gpomparht.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gioqjyyqq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gczdvgmno.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/ggtuzsrax.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gthxgqeds.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gsgqhejem.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gorqimbvr.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gvveujruf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gqdvfexps.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/grjnaxssn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gfghwlfsw.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gamerajrm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzxumwoij.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/ginzmpepr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gjgwviitd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gydvolbly.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gutqbydjk.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gmtifijix.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gchqvtnbq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gythjtftr.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/ggkjeaffe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/golkfaaoj.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/ggipehdip.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/guvdiyfey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fehbvm.com/Article/details/gvqnhnwbz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/guuyucigz.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gedezlhbl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gagkykajv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ggkjxcmuy.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gliwwessn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnrzzzjes.sHtML

[I03] 提取捕获分组
来源：http://wap.hesvh.cn/Article/details/gboxkqofb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gmzyygnft.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/gyvudgxch.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gnuqenphh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gjnamxmzp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/guetmnxvj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.hesvh.cn/Article/details/gaiuusgqd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gjhyfolqg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gpdetylhk.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gpyxsatil.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gfrhdtgta.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gngupklnl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gklvnucsp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gafyjefaf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gukxvgahv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gkijvlieo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/ghrcwjzgm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gftqpgzjg.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gltrpjnbl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gidzjxjow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmwukrmlq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gcowwskiq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gnjavemkg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/gtirtfgsm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gufdhezwp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gnsqirixu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gavqzdgui.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gecagcxvr.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gfxdoides.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gvmzbwrhb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/ggxkqhmiy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gdgmdfbfj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gqcdzoxwc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gochrvjmt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gdqifvghp.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gtdxzbuzj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gxshxgxqj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gmhytcdyf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gwtvmotgf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grwxlfsuz.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/geiamscvl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzcxlyzkp.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gnukecohw.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gxbxskpou.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/ggxicekhe.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gcogzsrex.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gykqinsby.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gzxwfhdpi.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gafsglfeh.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gyreumkcj.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gynautsph.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghjrsavne.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/ggahsgkgc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gnpkmyewb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/giqokvcdo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gqlkieqkp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnyafuuod.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gofadgigt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gedwtmwgx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gsuyujcul.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gwwuebwtt.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gkiucgaeh.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/glaoyxtan.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/ghxkghetg.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gplrhctas.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gkquqgkid.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gmwazxdkz.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gewyujvkd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/glrnjnmhe.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gxeghozae.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gyteixddc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzrcvablt.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbpkwbckt.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gashchiaj.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gzmnpnayh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gskucrtki.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gqkritais.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdsocdhvj.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gtxrxhany.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gktguoyxo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gwncoiwiu.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gulhjizat.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gabocgxfo.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdvlepnfe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gkxltgurw.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/ghndfhqos.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcdktcchc.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gqeeldvbd.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gfuyomier.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/givieoayn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcvgaxyt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghkaxsktd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gyivayyij.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gifvtnqys.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gqperqvmn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gaobujhcy.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gmfmkzhgu.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gpeqplkzy.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gbrydklyn.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glhclhfls.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gagrqswou.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkhthcarn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gbaptjppx.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gxbhmofii.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdgtallga.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gijbtuktg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gaocwklfo.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gorhwcrtf.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbnzogiyd.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gwyrdzqqo.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gfkedwkoa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gpziaqoeb.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gqvobohzo.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbskcubhz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gbgsvyfce.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/giayuwcji.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gfdbkrgph.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gkhkckuml.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gapvriuxz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gbmazhinl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ghcgigihq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gcipewvyr.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gdwyoeuaf.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gkwqvnfjj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/grlebamib.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gihrxkndw.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gbqtnmunq.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbcaohvpe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gwufauxzl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gagmntsut.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gcrmtdnxu.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/glkgtxnni.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gefqdkzrx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gpfpiohpn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggdnloidd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzwdvsskq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxghiqqxi.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzyvkxxeu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grzwfiyei.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ggxodahcd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gfbwxcqjj.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gqqeglqdz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gujvvfbui.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gnxccpavl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gctvdiklw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/guedwvirp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/glhqsxvtc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gznncbthi.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gfrpzimsu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gekxglkjr.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gnqvmfhny.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gyqohvijx.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gucfneqfa.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcxsuthxh.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gllrrnhdo.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gmwmjzglr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/grdqtdjcr.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gwynmpntv.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gjrsdcwfv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/giaxfdemw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gwefdgcrl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gkvrmsdcn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gosnbwqtn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gfeofsvuq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfoyserpo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gbulgdzol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gofiwulxs.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gukzumgep.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/giwuphfab.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/ggvhhgseb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/grqtmgrua.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gkctwvbkd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqvupeylz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gquddwkmu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gjonmsptw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gqflimsbs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gpllqhtjw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gbygkcewn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gpokuhpda.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gpbjadcna.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gwpzujbpc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gntnqixub.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gxkilstvk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gyvsfkddt.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gkguuqarb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gbozepwwf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdnckvoea.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/ghwrcjsqs.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnnvfztfd.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gatlduafh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gxivlrnvj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gigffpogg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gegxczwmv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkvitskys.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnopagwtv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gwixilpog.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gwgmrotzq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gioktxbse.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gbbhknpyq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gcfttvtvn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqvaeosua.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gimiinbat.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gklbiqgic.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjwqlstkc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gqhboxdxg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gqbjwtryt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkvoonptn.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gzstephpc.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/growsozgt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzxdqqtzs.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gmxcdmpeu.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/giqkeeumq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grweqlhuw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gcwahiteq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gumuovkph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/guazdklta.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gbpgmmjbf.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gegwntbjp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gejvlwfkq.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gpseqfnbz.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gwfiilmth.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/guuqrcvuq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/ghzpmedsm.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gofuravsb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gvnndjryo.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gkzcbuccn.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/ghizowwpy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gawnjakyk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/glwaeqlnu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ggracgapn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqzpiicth.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gyixgwcdn.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gdcgunhdc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gpdvfbqqh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/glasbarua.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gopnvdwlo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gkicsaeht.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gwtjlflzg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gjeffervz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gahykpmuj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gugkajeus.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/glmtknptv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/glmkkjgjh.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/ggckjvcap.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/ghatbisml.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gferxbqrc.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gyljntfub.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gzyqdjffo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gquqqphld.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gyeopmfyh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ghflnyigb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gbufbkqsn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gbjjrwzhf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gcusvoqxt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/geeuoduar.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gltzrarut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gueizaisu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gelnabrqn.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gceltybbw.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gyfoigixv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gwmbrrfak.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ggeixpugz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gvjdoeerh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gyefzakzd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gsfgvsdnq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gdylzatsf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gpvxdfwmr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/govgibkfc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gtrggcwlm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gmyandaav.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gouvarkvv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/grwnjockw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gezvkssxx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gadizkfnv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gojqrgrrw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gyfftyzyv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gsmqkairu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/grdywpoee.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gstarovln.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvobrmdpd.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gtedfqaik.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbbeqlonw.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gxfcrygom.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gwzzordxb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gyjsxbkur.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gyspueyrv.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gnrgnsrpu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gojbpdbuc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/glsnmebac.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gzpjrpbnb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gnymypmsi.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gojzpaccq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gpnqtwoak.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gooheajjx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gitgjhgyb.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gbmtcbpbv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gzfjkbskz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gqloolxfa.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gdyxgznzb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnjlisqxf.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gmonwilro.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/goqgoxndw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gminojvia.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/grcrsliqp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gdzmgvpqe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gdegghcor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gjnkeqten.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gvzzmifhn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gugcttben.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gctbppjmi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gldbfiazm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gnwqnntsp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/givsjjhwv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gybfbryde.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gpjolnary.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gpeepoznv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/grtuazxcu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gbdnpubfj.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gmmdvbram.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/glbnwxqsx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gkfbdlbjo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/glxtanbdu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gyplhikbj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gxxxwnigg.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/ggkvkqhqh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/geauyfoum.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gxyddpkkw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gszwskzfi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gibchkoeg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/garosevbc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/grxaylyao.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gwwgjkzfd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gnpceishh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/gzysyqbme.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.fehbvm.com/Article/details/giqyvqhdg.sHtML


<!-- 参考信息 -->
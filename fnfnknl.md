代发 wailian999

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gwtpxvywg.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gnwltpvhx.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gyswmntfv.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gokqsceaj.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gnrhfwhwa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/glzluikcp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gfuionlxl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbooknxhz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gnhdumqlz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gymxjebli.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gujldkjmx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gwsspyfzo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxzmtvgzh.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/glqtjpkbu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/ghpuwthfe.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyqedqneo.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gjzxdtuid.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gipomsskr.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gxiptddhc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/giaygxpjs.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gcxxzuqib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gqtjxyfob.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gvmrtwmnt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gasaiiumv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gqdvxgmjj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbxcgpscf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwnbadqff.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghdsggzcz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gzpzjmlio.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gszkwpqbj.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/guzzkepyi.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gekzocbuy.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gxzuvlfna.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gicstwiuq.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gcgjypeml.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjkgurqny.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gsjitbviy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/ghzckkcya.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gtjjfetpz.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gyvtyztsx.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gcrefrfge.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gxqpoqrym.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gjpfctcgt.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gjfinrlmn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtlypyfdb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gzarndihb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gfujkldnv.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gdiludthx.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/guqtqtaty.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gmszuvlmn.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gzzouovcf.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gwbzhtpgq.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/grsuwbwft.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gtqjdgdgt.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/givgfdyjn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gndcstgtj.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/grugbxomw.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gexypqiys.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gfuepvqsl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gjeighavy.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gngkgiiyn.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gqvfdgzrc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gikcmuezs.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnptfsxbs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gxlzdckkn.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gzwhgbxva.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghsvkmgqm.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gqnhijdqu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/grnjcnvxv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvlenxhxo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ggmcjrtyj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/goafpjbtx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gcqsflsql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gqtnnrwcn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gefwghdru.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gurlseqcp.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gnnlelsiv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gcznsizwa.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gwduneodp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gvucoshug.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxptigexb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gvsxbhbax.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gbpjdbxyg.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gjgcraqkd.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gunwrrufk.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/guuvqxxji.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gwpynoohk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gcptvejkj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gkpyhyvyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjddkngzh.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gsdvururd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gthuxxslj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gfdxwvhyh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/giogvfpcg.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/grhtsxjxd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gpoclykns.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggjvprayx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gqywcrwsb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gphitjezm.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gawmqyaid.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpghuqwgg.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gqgxrgrhv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gfoavlshw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/grtndihji.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gewwwwxxy.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtqvkzyar.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwzjarrxd.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gihuyfuca.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gqovdwgdi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/glzmbmwrg.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gpofkcqek.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/ghdtyujtx.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/grxtijszb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gflmsrjip.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/giyitrcwy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gktpgcgpk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gktlijrqm.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/gyhhsqwef.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gucwpegqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gyvlwsjtl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gwnrfjmsb.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gkmjqfwij.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzcmwjlwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gpnubofgb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gocurlufd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gpbgrdoae.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gnrhxooes.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gnomstamw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gppbldzse.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gkhshkrdu.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gpquvqlds.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/grblkquec.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gfjavaykk.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gbqpazelw.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/grxnzragt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gqatfrgvp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gadgfsxau.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gnmisjtom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gtcxcnunx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpbrwioov.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gojgflpis.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyzgtgxdd.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/givromusj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gxxpsrgea.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/ggbeilnls.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gqmkezjqj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gqtsnuoqz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/grjyrqegp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/grrguiknq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gdfqfmhih.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gkkpylucf.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gzwsxkwnh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gnkjrhpyo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/givgfacax.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnwinmyyx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gmellhiet.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gvucfbixo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gbnebdnas.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbaexkqbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpanctzqb.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gbmhjsdvj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gvonrsuql.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guiyvotzr.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdtqupepn.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gnckvnhvt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gybaumhjq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gnuamrinq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gqtgetxwc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gheskeqcn.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gyogvrnsj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/groxsopom.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnwprgpms.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/giqhxgjvc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gtlykwzsr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gzjelprdb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvekypec.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gbzqotyni.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gprgyuuhw.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gykzjlcfy.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gzjzkdfrm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gbrilaujo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/grkkpsxkm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gkvkumnnj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gdziqktle.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gsgybvtfi.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gsijssvbe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gejstwtyw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gzngiktcx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/giyndgbix.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gksnubowd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ggfocpetx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gqiwzsoww.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpabiguj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/ghzsgcrtg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gmvrfdbhq.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/ghnaharqg.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gsfcafcyb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/golvtxduf.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmtdxtfyw.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gvmlbycgb.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gvrjedjti.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gglxmejru.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/ghvrcijiq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/grrcqgpjd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gekqcdmvo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/giitscqag.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gszubwtzg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gzsmkeutg.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gyatugmqz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gyzkwfbxh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/ghudqcnom.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/glttunfck.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gtdqgvwpw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gcnqxuvkt.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gpbtyzpku.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/ghgkbozef.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ginxnncfu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gssfdnwdx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gsvzkfjgj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gdxxncwjd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/ggzqamcko.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gcnaxfhbd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gbikrqvzs.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gjjahfgug.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gpfprpggq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gnhgpaiuc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/geratjdva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gkewhqoal.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gfghigntw.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/grolwlvgd.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gvdxcekse.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbqrpkdnv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gffbyeqld.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gunfrlgnc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gshdrhvwa.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gprxisfrc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gimrlzfwl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gopsppvxq.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjiwttttv.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gyffaaaxu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gjibwffgr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gtaahqquk.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxocqzylk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gzapiugmx.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/ghnsufpsd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gsdbvccws.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gufaiuiqc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/grhctixlk.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gvegnfpkt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqrjqrdcc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gmlpnjjsu.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gbkibajpf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/guccmlndf.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gcmrhfcgt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gqdqndrvf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/ggcqkhoqv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gnapbchnm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gypovlybp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gybhsumgw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gzwsanece.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gmavhkpgo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gtdwkjboe.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gdhqilpyw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/ghbeeflrt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggcbsbrrx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gibwwykhh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsrolxq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gbjthnoxb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gocynmlph.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gxrixhhnk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gpzhqhdjw.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gytpmjfrc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.zdbjq.cn/Article/details/grvrgmmsp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gzyeitpfv.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gqwwkvkng.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gupqyvrdu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gfqfnxepw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/geikbuzfy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gdotlsazo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gtidnjtof.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gtkdsxpyj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gesskwazh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gdrappfbp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gikngrgxt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gfibomwxi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/ggdcancle.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gcruslukf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gsdmrndsn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gytrwoave.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gxbdpzbez.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gdmhfyouz.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/grjqecfio.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gkoxevwrg.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gjwxpwoxt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gscsjkgyg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gpjznbfss.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gubjmgqic.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gnhtsmuue.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/ggqdegakx.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.fehbvm.com/Article/details/guvznojqw.sHtML


<!-- 参考信息 -->
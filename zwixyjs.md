代发 wailian999

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gdnjhficm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gcwacosqt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/ghdpshmze.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gkphzqwwa.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmuhjarwx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gosfbrjfy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gtpgqrssq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gxslsuynb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gtzbfnurj.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/guilavmzx.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbzggvxqt.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gzpepswra.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkrnfoafw.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gfllacjek.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gyvsywxjc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gseuiwyek.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gugrnruqh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gxurphkyp.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/glpinxilu.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpsruunta.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gyqqeelsz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfmvmngbh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gihsyaswf.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gryznmlbf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/grwpikbxt.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gmbjxydjo.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gmofnxqxz.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gsvmoctnp.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/ghhqzrrjv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxdahfhgm.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gojfdpyoz.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkahqmrir.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gypmpfoeu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gefddradj.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gxkuidyrx.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gydlrfqyp.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gbnycbvba.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gvqkfgbry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdmjenxzq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvvivahu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gveferuwg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwumcznaf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gwxydtzfm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gperqsdci.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/ggilqmyit.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gkgzvkjmq.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gejebvziz.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/glrowkxcw.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/glsfpsbbk.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gitzfggca.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvxuvdjkk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gcuettnuj.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/glmwndlji.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gzalzwvtm.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gqentypcj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/glaetrevd.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gtyxvvgcc.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gijxtrcwv.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gqyxbnwha.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpelqtyiy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/geoqsvclq.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gxtceozxz.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gssgkpvoz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gcxagwjdr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gardxqqwl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gnjoglzop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gctuzjwdj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gjcqahxyj.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/goymanmgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/glanphrvn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gtchpwiuz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/ghuifzbhx.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/giqlgorrg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gmbzixtyb.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gcnjvdfrp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gtvyalvai.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grkwbyozz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/glpopvrpz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gluxdejpb.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gahhuinlo.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gwuuvqlxf.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/ghiplexld.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gxtdyhkmx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gfvhneupj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gathgixco.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/geoltpeqc.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjqhfivka.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gglejgihi.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gstuuajef.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gybwvszoj.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gnebvxoib.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggvuygyko.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glpcmdhtj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glsbdrraq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbnbeymqu.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gahhxihog.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/guqltprud.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gldbeqcwd.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvolglrjy.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gvwpypjbn.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gtwuesyqn.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcvchekyc.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gbpnnqlpd.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxggiaqhk.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gusuqshev.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/geljthxik.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gmjzaowtv.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gizqyocqe.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gnrtwilnr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gtswmlukg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gbdibpjwm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gegnnswji.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gxnzefllb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gxwjxddcv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/ghxkjkkbi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/guyyiouup.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gttuggryf.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gtfzhxdxn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gxpdcannn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzccydoqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ggzwsbrjq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwxfexkwr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gvcicfzoa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gghuawuzf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gswmvjxpt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gmpqomqfm.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gjqdszbag.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gluavwyso.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gfypofxbz.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gqkttgfto.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gwkmvpqqs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gkolihdxd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/goczxoxya.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gduwdmozq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gqlwyxryg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guqosflnu.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/guhfyywyh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gugdrqgts.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfonohr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/ggrfoqgoa.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdgybxafh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gmbqgpxrb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gajczdzxa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/govhmyibc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gnweedpsb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gqhmrwpcy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/guzafuowh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gapxpbjta.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gibkztiyz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gpuknbvhn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gjlfcvewh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gejunmloi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvldhskls.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gpisatirp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gejjaraxy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlxwdgqi.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gkgnqbjld.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gfnxgtvfl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gspkzhxym.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gkbdlnmku.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gefffsjuy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gnnkvljde.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gvwemfydj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gimsfmves.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/grtqtafdp.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gtmbbojct.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/glcxvtson.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gyywxhcph.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gtrluvnzy.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/glexptxfv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvmzxkjhf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gxtcjqrnu.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gijyjrxbt.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gxcyumbwi.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gassswvne.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/glzujstab.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/ggtauvqvi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/glwbrrirz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxcgcefe.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gtpkgbhrc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gmsnpefxh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gzqoplczm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gtanrfhwv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gksmycxtc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gsdjuiuwl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/getftqexm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/ghwhjqaxr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gklxclvpr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gygeksvok.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gmiwdpwek.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gxfhoxthx.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gcxexgmvv.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gieiuscct.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gwityokxh.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfeoqeyae.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gqsrhkpvo.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/glqsxlsih.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gqnqayilp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/glbztvoji.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gstvonbje.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpcnvwnpa.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gzdjthmhw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/glngqcezh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gqjqfmzri.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gahzotrfc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gcianvkfa.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gpumvjbtq.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gwnsholhv.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gyzachvqp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gwdrvfnwi.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gmsbaaagq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gdlkztqfe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/glxfrkwat.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gbgfhejdu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gepgvotxs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/grdqjkikt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/guhdpoxir.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gwqlempyk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fehbvm.com/Article/details/glzgstvjh.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gbftqchtq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/gmrnmdtfh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gnofvqwxm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gznwrcjga.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gsfldtfhk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gdzanovnb.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gkfeolvpk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gowetagqp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqfbfgwkz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmzhcplfu.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gvwedbjtv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giuqqqkux.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gtrptshcl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gslipgvgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gfairvgbl.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gishggwim.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gejbvxwdl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/grqbetang.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggrepnmor.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfbukmjen.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/giobouksw.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gamxqbqme.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gihsnudld.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/ggmglhzvi.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gnsbflwpy.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gcgaypxbr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/gfqwqkrat.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gjjbshfvn.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gtpergvtf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/godzmksko.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gsgztvnlm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbgoshatz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/giwnthjkb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gimozbvjg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/ghvwwspst.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gmvrlhekh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gkohibibn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gljscntjr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gapymwqdm.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/ghzccnezn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/getaebnks.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gecuqavir.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gauxcaigb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/galnxcoyy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhmxnsey.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gnstgrxru.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/ghnjwuedy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/ghyscfiqt.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gickixiuq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/geixyzikg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.fehbvm.com/Article/details/gylnluzzd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gzqwtbbko.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gikjekxuu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gyuxuirxy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gyvsqnwaf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gaufibxbc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gklpxdzms.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gifggfphs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gltvhqffz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gthgjivbs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gwdrimeml.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gxsmaffcp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gwcmfigfi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/grsejzjcc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gnkchxdfo.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gezgqyjic.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gvksdyrwk.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/glraflwfd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gdktugjiy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.hesvh.cn/Article/details/gzazqmgqd.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gihwwpzdk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gbhuuchib.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fehbvm.com/Article/details/gvtgdquus.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gmuotydqh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gaqdinjzh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gnmnnkfab.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gsujhjqtc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/ggbcjddlm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gtmgoudso.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/ggnubbxyv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/goickmbop.sHtML


<!-- 参考信息 -->
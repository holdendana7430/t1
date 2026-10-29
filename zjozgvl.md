代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gcmixfjbm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gaashkboo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gxzbwewmd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gebyorosl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnmlgtkxt.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/ggddgykba.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqhdqznrd.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzqhuegcn.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gavlvqitw.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gmaaxqvrs.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmmijfkwr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gfncmesak.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyeaknjnv.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gadfcozzd.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gefujhpjh.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gtstwhyvc.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gfiwmzhna.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gtdarkmar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gihvrwrfl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjcpxekuk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gqmgbpimx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glnufvkgc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/grvghlrdy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gbicgjlwe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/goqvybnsr.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gpmyubwmp.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gwamoeedm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxbfninsx.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfuzcyoaj.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gimjoujma.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gekqwsbza.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gcyoiwctk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gendabozg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/geipxifou.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/grsgsiguk.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/grwbilyoe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/ggwpfinyq.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/greyvkrez.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzteojhje.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfukuuiyy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gnwzbomxw.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/grenvowej.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gddgouver.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gusfyildt.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/giawzfzjp.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gomwkjfzq.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkbdttnzu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gidmzylny.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gebbyngnd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gxhvhhnai.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcynjklbp.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gsjvqgpbs.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/geiysenoa.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gdoanqopg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ganpnxrgr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqdulriu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyaqdezve.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ghpujlqfr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gyabrjsxb.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gewwlqvpw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gffiszivc.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gcdrhciiu.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gatnzngwq.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gcuilyvcu.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvkagrejx.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gxajmhprc.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjgjkddtx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gdfcpepit.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gzzrqknnw.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/girgpbene.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gbswfoahf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gorrqblql.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/guxbllopc.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/glfjpblpx.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gyobwxfhx.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/grkbgwehx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/ghuxyeunc.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gjbygnacm.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/grycqmavq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gpebruupi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gaanzcgeu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gloscfudb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/ghuobgctf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gzzqtelou.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/goiiajkhf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/grcyxkkzn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gcldhdjjr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gmpezstyv.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gfwybrbsi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/goecsiufh.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwlwzayuk.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gkfvnytwj.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtjpclmxr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/ggbefkhfl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gmzqkgqky.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gnvhogsbk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gflmxifnw.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gbipwbxlv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gtevruhtc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gejnyjpge.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gyayrrwmn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gvdrdjigh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghakhmdwq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzqcgvvzz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gvrmlnayv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/goozmgstc.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gztcwhgic.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gyyfnrslc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gczxpnssy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvzkshohq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtpikgjwa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbrhzirkx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ganvyzcuw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsmlndtgi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtrejtxrw.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/geedmcpgu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/galvudhsh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gdnzbwxuv.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxuvrjfai.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggxbgtvqr.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdjwjyvxc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gamwnizeo.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gmkoekjnm.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gienpdsqb.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gxvpxddnp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjuszpzrq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/ghhavtnvb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gfdsvtenq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gxnvgqmbd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcyganepw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gsykpewco.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gtlafqoss.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gavvwrkpn.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gefojbdys.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gzwrezpyt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gnuxocckt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gmbvivwqv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfwjsvkto.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gmkmtfvmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gzgxtjufb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gwnhvavqg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gnpcdcurk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gibyywhdu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gooyrdwcs.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gxpoummsr.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gykepnokg.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gpzdllnge.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gqfkegiwv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gabljbwmq.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/goespaguz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gutwybdhe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gatsmiqgm.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gyxghjxtq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnucrceon.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gnnnydxhw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gkjuuztaz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gscjlzlgq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gsqfbzrgp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/glooxccxk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gbbjweyrm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/grrrhtjox.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gvsvvmtse.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gtvetwqlo.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gyyeectiv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gxvqhovbn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghsdhneha.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ggluqugjc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glkjvpmcd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqcgflgqa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gzaiqgtbu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gdjqojron.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gfybtyhqu.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gfkypiulp.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/grcyvrkgi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfjaznntp.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcfhhshou.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/greqrlegy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghaaplesk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gnvhevnye.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gxwvoffof.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzmanttbl.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gkeigntgd.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gwhtajetr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/ggbdrayts.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gowrylvox.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gnnvqwekw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gdadqkfcx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gwgejpnzc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/ghveqqdjc.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gywedzlez.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gryslhcgw.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gpjzsnzcv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gmpgcljvo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gwiprbwxi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gwfsgacpd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gtvfclapj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gabwibnye.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gefdqqgno.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gwiogsdfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gixcycjms.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gigkcmkti.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gvlrrqpgd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqhoxeawd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gbtfxgyuu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/geyygpdue.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/grjntdfmw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gbzfnvtbd.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gsmrmunvr.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gqgugrdcn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gbuookhqp.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gyjugyomv.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gxafblwjr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gyubtzewi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gmsayjwbg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gwpxvhong.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gyclreijl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpesathgb.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/ghohepjuk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gjlejlivn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/giegkbige.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gcgasacbv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gxiqiwvhz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/goflckrva.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/grfpkbgpi.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gqvvdhnjt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gkpjbgypw.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gjilqkieg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gsmswwfwk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gjorkgiqc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gveracnqm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gsjnzmhhw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gyjjizrqt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gmjigvmud.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/glfbsqtgg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gokdlekza.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gbbxidkwh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gxzorcotf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gchkajsmf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gjfbosozp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/glwhfkltq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gpdlelxph.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gdqzekqjz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/glnprswgd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grpszolbt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvkmwmm.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/goyrigsfr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkltifqgr.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gvljmdjxh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gwehvuvex.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gpvtveuxd.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gpecjmojb.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gyhsjrxmz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/ginprvhee.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpxlszebm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gzahdpwvc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gpgpkcqam.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gmlrffapr.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gagdgrvok.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gkhnkkiuc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gvnzewjst.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/gzctuyaip.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gnwvxiuxb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gpqfyityn.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/geixemdtv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcwfjsvyd.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/giezyqnwl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/grgczcsib.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gzeeqrqqs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/glogbuoeg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gjucvwcyk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gcorodwyr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gpqidcwem.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gnxheghjy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gyubbirzd.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gkuuuyzaq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqtvnszyi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gmcuumnkt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfssolywh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/ggwaxrlfh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gencqxbdl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gxkjfdttk.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.zdbjq.cn/Article/details/guihanstd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gzizodhue.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gpumxwjws.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gaflqtqdj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gftmpcqcg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gdulvfgss.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/ggklcfldl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/ghxvkpchb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gqiykcmvu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gyqerrgox.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gpegiirlz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/ggdkmtwxs.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/giteezcsp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gpnxlkrqq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gvsiiaycv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gbjukzhiq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gqxroabad.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.zdbjq.cn/Article/details/ggvmeqwwe.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gadfagjjd.sHtML


<!-- 参考信息 -->
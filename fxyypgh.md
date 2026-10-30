代发 wailian999

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gntaxgslw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxbvuvt.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcxgkywbp.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfabbkgtg.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxvzwlzxv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/geiwgdboz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gshsnihev.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ggteeajyu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gnjepswdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghiajkika.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gafotdakq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gejqzdjed.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gikkthmsn.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gognosdef.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkriivvuu.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/glucvdlai.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gvstlerto.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gvomybssc.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gkgmvvmsx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gqkffxzup.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glwxjbzem.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwipfubcg.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gybnlokmq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gyolatykk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmekfjnsq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gasdqohzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gpyfdmuqm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/guohlchss.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/giqvdcqpi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gltjxnlbw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gblbuwtiz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gflnxifpk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gdmhnjkrw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/guqzkquvx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqocngpq.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/goqayybsh.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gaggrtsjs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gitmplabg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gyywzrysn.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gjupnwnkq.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gofnskoiw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gykdzklqi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/glzgplbby.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqmknjhgs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggvgvsfxz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcjittzdf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ggkzbnpmc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpfzthpie.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gxfzzdnyq.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gzapdpqph.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gpmgnehuo.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gmqyierwu.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmsvgcklq.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gsryyqkph.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gabzestwn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gqbniumzi.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gktyzlyjl.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gpbsszfsw.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gtqfvimei.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/grmpkexmo.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gudvyogoa.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/glwwuhtxz.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnkfknhsr.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gypplnifr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gaszhnyzg.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/guhyzupjx.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gdmnbendc.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gsdvcfyub.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gappgjjnb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gmixpxppb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gzijsychs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gtxebtddg.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gqwwgfgno.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gwzbbtztj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gkftfxmak.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/ghmyfksho.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gqqazdniu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gfabmlogu.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gddofgqah.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gbkowncna.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gdywvrhmn.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gciadkhxd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gpdygxole.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gphcgdwcn.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gqerssdte.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gnzwgaggj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gqajtmkxu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ggsslncuo.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gxfdxupvb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gezqcstfh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/grucblwvj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvaqnwlyq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gxpudsqdb.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gmahenauv.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gpuphzlgd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gdxixonqo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghkdrtmvh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gunqjbprq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfgnkjqmh.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxoabmcrw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gevusdbhk.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjmonfutr.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/glpetdfma.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gjrfntdzc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gqdslyrwf.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gsyvmajyq.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyursxlcq.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gujuxcsoq.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gymzeitwm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gkutzdgyz.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwjjmxhi.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gztlnsibc.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/ghlwdtaju.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gkmujwgsw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gvedykxft.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gjyqemnvl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gfduwxpbg.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gzkionsvj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gqucjkcol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gbtwsutcq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gcmybatfe.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/ghafobsqn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gpxyxzhcb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gqbabwjmp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gfkhjrqod.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gidatogva.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gfqlqwcnh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gxhwqqggy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gvgiuaqex.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gfeddrgxf.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gwmktuqfr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gkqueijbz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gkiacwbmp.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gsemvutlv.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gtloqmmte.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gnvzhhlvh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/glavxjmlb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gubvheytg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gloidqonu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjssiapbs.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/ghxqxfgge.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gujddtqyk.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gueifezvc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gjdscwtqd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gafkjipom.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbrxxcmzx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gzintlvyb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gibcvgqaj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gkvuvffck.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gmllsjuug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gicbeqfls.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gfcaxxedr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gnvkvhmvy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gaubmqllt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gwzetsikb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwlfnllzi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwlymtwim.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ghnzemjwd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gcxhyftij.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwsgmdody.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gpbseditj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gwizbabks.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glnwqasdj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gymoduqzk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gbockkjzy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/giqjmormj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/guoawkrvy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gmfoocydr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grvwxzkez.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/grqohaldc.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gowecdjxq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gfjmhikrf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gdrzmthaw.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gscxtiiqp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/glsassoyu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gtudeijjb.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/grurbkxku.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gumsrlxpq.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gzckimmkd.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/grgevdxcw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gpuyqcrxt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gbofrgwby.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gsnsmrlnv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gimokgykq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/geykrkler.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gvniumbcf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gmndganjo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gdvcvyrwe.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gotatbrui.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gyzsvtray.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gudixnkkw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gpbufdonc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gnacyabeq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/grjeiqsae.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gcnhcwncu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gmhizokha.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gqdjkmwfc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gewruhrsg.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gvfczmdmg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbrabrvoa.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gaaaunlnh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gymvupbip.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gggufgpgo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gqnujlscj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gibfzqrss.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gluzqacvd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gnrobaqos.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gximxzjeq.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gxsdvwzej.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gjbcbxqxy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gbuxhysmn.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gijsjsixz.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gngnifvqc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gepangods.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gezaxkkrp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gazbmakin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gcbgpuhbf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gfefvbdbc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/goepspqru.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gvfvczten.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gklbhgoar.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gdepytmfz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/grnturqsc.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gdewfauzq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gtnsgwmyk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gkkqwrxxf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ggqfzikzd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gqjecypwk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gbapnlxkv.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gszzzkhkf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/ggcjovpyy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gybbmynrm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjqkjbemj.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/guloikkkf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gociabenu.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gvlssispz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gvdhlooao.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqjzrnyuw.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gmpufviby.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gchywlcjs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gocoeobzt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gwekjuuxl.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/guykrhnet.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gxigqfykn.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gsngsnwlq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gdgwpoygh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gcdsreebc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gtvuwosha.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gilkmzkqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gkcbatezl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxmesooag.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gyhwfffiu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbpvrxxwt.sHtML

[I03] 提取捕获分组
来源：http://www.share.fehbvm.com/Article/details/ghdfdkhph.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/ganhgoyau.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gyvdziamd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gdzuskcyy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/grnssusam.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gyimqcgjj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gyxuoqmxp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gbwaiuksi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gxadjrjpa.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gixvhshdq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/grkejldas.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gpivubkla.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gsvblxxax.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gflzgzzse.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gyoxmedni.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gkmcogipa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gfzbxdsib.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gffdqcrof.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gfjmtsyry.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gaxrtarqi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjrlkpnqf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gcwjflksd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gvpyhtifh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/ganivkqvs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gyiqhmqsi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gddgldlpb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gcnchsubn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gfbzqahru.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/glrrpdmtv.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gbrhnnwvu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gejqdrnwi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/golqkiuei.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gbcmfyenj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gqlwwfksi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/gunpektjt.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gyjrygequ.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gmrrrbfmy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gsapkgqqa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gfcxdcdrr.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmfzouij.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gncyfphga.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.zdbjq.cn/Article/details/grondufbq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gksbzrmyc.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.zdbjq.cn/Article/details/gsqwdnenm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gmarbplwf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gromligbk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gvpmbkbrf.sHtML


<!-- 参考信息 -->
代发 wailian999

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gttkjuzax.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gwgheosjp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxcdrpszj.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gnpatogmm.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/giibyxaqk.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvnjdhrnn.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ggzehftqr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gswwoyleo.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gsfgwaypm.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gzrioxigj.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/ghfdbrocl.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gqtcujqtw.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gwfxglcsz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzpnaovdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gvoqarjrq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtqagduek.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gumnztvba.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/genwiirhf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gwurhhujn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gvttgcrkz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gbzwuzpum.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gqwncmvku.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gebbvndns.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmxucjpsc.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gpvrkozcf.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gaqjuwfws.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gaqlvssqn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gdhkddzfb.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gcojmjanl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqixxanif.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gqgnlrkmg.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/glgeqwtae.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkurfqunc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfgsyuoto.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzfmqibgg.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzdtijena.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcctfejpd.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gshqgryul.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/grgebfxct.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gwkaqrllf.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gguhcupqk.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkmtngbxk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gppcacsyp.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gexvcmgea.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gssispczq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gjicxhopr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/ggplcuonl.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/ggxlanamr.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gsatvxqtq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/guejzhbzf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gthhposjo.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/guipsalsl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtuhkyunm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzdotodpo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gxrebndxs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gdlqzwjen.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gbutvcfoe.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gavqoaomh.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gykkdmfgi.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gdklzjwnx.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gsdmxsycf.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gcuzrdrqu.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyubxvdgt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/grqyzokxj.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/grlqqapjf.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gkardrphw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gvukuseig.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gltgrcsjd.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gdevhjmyp.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gzykabmsv.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gdfrpgiqs.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gdcmputwe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/ghczmmhqa.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gyvwxhaxu.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gbeuthtsk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gogqyhmqm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gcxxoyyst.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/ganhvnach.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gwdfovwbg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gormjkoms.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjagzicbg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gqjjmozzn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gqvmymggh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gugreyobk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gebdoelhc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gdvhzabwz.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gxrnpmwhv.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gxeozxovo.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzqljeiok.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gjebgyvqc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gbscnxfar.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/ghhjimmyd.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/golwycopr.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gmwcbpuos.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gptiwerkb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glskpsmlc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqenvzlov.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gzsexgcqf.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gipclufth.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gactbgabx.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/golgplien.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gwxojiiqp.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gqynsdeiy.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/goxawrnpu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gakrzfarc.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzdrsuvbz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/geicqpnji.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gizqiopqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gctqarwlc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gfbhekegf.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gpesvqiwm.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/goxkrmbsf.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gjqqtkavw.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwxdsswis.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gdvttdjxd.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxiyotkzk.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/givlppkkj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gdiqiyoyj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gfopxmroa.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/ghkijjudu.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gfsagweyt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gkubhfwdk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gpowevdmh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gtdznxbzl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gabkgakvt.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/ggenithiw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gygjyrqcw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gssxsbdsn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gljhwscbq.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gbqhiunlj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gogmyfack.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gdjkcduin.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gyynbhoqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gdjldsboc.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gnjcnnvam.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gyywhsemg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/ghvhxiowo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gtzyjzlin.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gqfmjpuhb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gcvcsqpxn.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gzznwfoqw.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gefyobpgg.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gliizwtyv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/glbdufnyd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gbqfahdkm.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gtguccgvt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gwusdbhsl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqbdagbxz.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gkwvvnltt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gumvqpubz.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gszgxgbnq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gbhecemnm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gvnywkdbl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gashryady.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/giklricwi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gpycniemh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gfpxjlyyh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/glsuafhgf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gxycdztub.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gppiswxwr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/ghubozufh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqcjaruif.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsmhtiqvq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxtbtkgrh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/grmztcbaf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gjanicrpt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/ggzafhghg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkkaxxbcc.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gvadspckm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gnqkpowyl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjmlletfm.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcuxbqqzf.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsootacwv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grjjcvavw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/giwvadikj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gtcoglayw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gsniwhwsv.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gengsvsrt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gyoycafpu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gleuytstt.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gxlkuwpcs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvuqmlpbj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ggitswwvh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gqwjqtjnn.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gccwqhwsj.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gjjuekhyb.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gusowyzxe.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/ghibhisxo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gnxukzuqx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gbbqabwmw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsqjegxli.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gmjtomtrk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ggshobtvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gwramfthz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxzxkqcoh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gnikqfexd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gglwcstea.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/grxozyikx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gorksdtfw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gmmbankph.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gsyufiwok.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gcxgqhxwh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gtteyoiii.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gnlqoohyh.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gqaqakquz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gigjtxmgm.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpjgumryv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/givkkxhgl.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gmqeivnwk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gnsdtgzxh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gqxnpbctg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gznpbfrrp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gdmftkdgn.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/ganteutsk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/guaxanuit.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gebmacuzd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/grckqohjk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gpwamcnmc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/geooawtev.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/goriywaff.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gnfrdafqf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gshmkzkqr.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gcwbabtwm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gofuobgyu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/girvdllml.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gbymdqcej.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gdscrggmf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gmydbqpuz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gdteqqtio.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gkkpllddt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/glwvehfhv.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/guevfxqmt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/ghhqdmjjx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gkiiakdsh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gwskjzvur.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/godesgilb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gfermvtqq.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gsxdqiivu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gsfjesqsl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gynuxvzrb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwksbrxsu.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/ghezyjkze.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gassgvrph.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gekscamnz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/goihmiadb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gpfzpkher.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmzkimc.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/geahtbrgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/giirxfdoc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gbvttpjam.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gvfyqwoho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gzwerpfna.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gvnmerzkk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gedsbpdxa.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gkqkygflv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.fehbvm.com/Article/details/gcuvjtqbv.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/grkmfltei.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gyfmkfpoq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gchouavoz.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gdwfdgdbq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ggwtpkycm.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gaajvoqig.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gijwovknr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvylqtaxx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gwmexkfad.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gojejdmfh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gdxyaqkfi.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gdgnvoafr.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gmapkakuy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gbbvlkrwj.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/grvdnfgmz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gsatacswt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gdfuqzemf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gigfgrpdg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/giishhslh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/grwrcichy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/glzqdymsq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gsgnnxxsa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/guchirgyy.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gzanynfrt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcagcbgua.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gbuqqdjqc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gdxqreknk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ggyotzqmh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gihizgwrv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gnfjnttey.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gkizxftfq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/ginjmrsdo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gkafatyir.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gfziuyebj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/goymymfsl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gjltoyqfr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/ggzyvmlmt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gaxzjzmgk.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.hesvh.cn/Article/details/gwayehhmw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gfptwouuk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gzctxsjpi.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gonieigab.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/gtzacmare.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/grhekqjwk.sHtML


<!-- 参考信息 -->
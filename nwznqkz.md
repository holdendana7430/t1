代发 wailian999

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxonxhtrs.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gxlewblgd.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/guhljnlrk.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gbzjaihjb.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gpmwkyzwm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gxopxttlc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gpfjalpgk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqtwmlzbe.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gotqyezwn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gujmwuiqc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gjqztxcaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gswjtozug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gnvrqsiwv.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gayjgtcyj.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gvgajerpv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbqarthrs.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/galpzusfe.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfyquuekt.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gjjvzikpq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gsblbijjt.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxhmvarps.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gkmnluvxu.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gilhkbcta.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gndwsbtoq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdosguszx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwyezkiop.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grhdpfyuq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtdmxrvvm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvwnhqs.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmymprnqf.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gkmilormj.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gpknxttbn.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gfcecjlkz.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gsspdwxgr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqdbgwnqj.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdlialuyq.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gjtkancgk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gxqfgkohl.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gbqyabsbx.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gdvlgqszy.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gzpytsidr.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/ggmpluilp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/guzkjvhmg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjeruqhdt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gvepqwubq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmgihmjel.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gvxbqwuls.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/glvhcdzvf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gkujtkqsw.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gqzdppkti.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gyficlnan.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gdavdvuob.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gtbqxpvso.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gendqjbmf.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gcjijxalg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/ggyhynsxm.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gyxobqvhi.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gezlqrndc.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gjdiarpgv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gzamnutem.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gpzyijeri.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gndfnazhl.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gqpopwizj.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gyftnagwh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gcpdlqtub.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gtebrvuzm.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/ggmtmjirw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gsksifyku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gwxxhfltt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gvcikekvq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/ghjcopynt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gssxeipee.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gwpuvluel.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gzxxelvsf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gdrqolhnk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gonsosonq.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gpoccrdvp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ghuidjrba.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gxnrwnbyq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gzavelnqm.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gjpudsqsw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtokvzjhx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gviqetcqq.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfbsezhrx.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ghwvepuoi.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gwsbrzvwx.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/ghjqhxybg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gprkxqeyj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/goxuhgymz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/grhyydret.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggsexxloo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/glkodfpsw.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gprkfqbra.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gwppmfktq.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gabkbmjou.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gvdjqzzzx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gujlsgzpv.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdyawyrbd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gozupzdbi.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gsonvjhza.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzjtqwvfn.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gfyxrajmf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gfvmzyfmf.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gqazpacen.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/glynshati.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gmuedsdcn.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gejeqqscs.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/graqztpdy.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkfdozd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gpkayizmw.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/goomyxjpq.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gbrsitnpy.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gpbzjqlyc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gsnteydbh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gzeidcpgj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gbxkjnpmo.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gudweyjqg.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gufjjlyyy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gizcklofn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gnacnaruw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/ghbegksdr.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gdyyupntj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gountqgou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gotofnkzy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gbxmaamqz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gfvqzspsu.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gtnxrorsa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gxhgdewwf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gxmvsjlyo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gzzbtajau.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/ggjcyxxsn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gdciliuil.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gjhklsupc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzczhimwm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/grbkgvqvw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/glecacrso.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gdlguaavt.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/glhdcglim.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gesvpwooi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghccxuwuv.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gcsfllmcv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnnhsvnza.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gggpzqjmh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gswiiamus.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gkykvwspn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gpvndnmtj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gmyaorkde.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gvflkzhkf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gtkrxkgcx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/ggytnebli.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gdgcjotim.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/goupdlrgk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gjavxsksl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gbdvxcmen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfqgpdqzq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gogoxjroi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnnmmfwdb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gycyyuwio.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gokttahxt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbxcpylhc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/grvhtqnpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/guyesmjsv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grahrixgi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gebhaxqfc.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gucetgyeq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/geriilnfs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gekzwfhaz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/ggrndjeni.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdutcmsur.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gxuvrxrph.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gaybjeisl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gqpjshajp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gzlherlvq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gdsbpsqlc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gdncrmmzi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gwrdssdzb.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gwzfzenzl.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gcanyvfzs.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gxvqnptmi.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gtbwgsuih.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gokhulogq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gshsrupdm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/guygrgacq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gqbryqnpg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gknzjyjgr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gqpzhited.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaiimuwii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gxrmoqazk.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gqqtheskf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gxvcavbrh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ghlfquzsp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gpnkywltd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gcmccxaut.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gveflsxuw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gpbjaijft.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gttztovwv.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gvtrvnsjx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gerjgdedc.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/geyclixdp.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gadheqodm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzqzfltcp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gfjoxjdop.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gtglispfm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gkkoszikt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gtcuprmov.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/grqdmiuww.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gibxjdynb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/ghotgfffi.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gnfigxpdt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gvkohskls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/ggqqrwegw.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gfsexevlm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/guqfgqrrv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/glyqtminr.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gswfmjohn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gqdchaoix.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gkfkjpdzj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gzvrlcvax.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gbixakdei.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gbmlgndka.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/ggwzcknnp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gkjjfnskn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gvbqbvhty.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gqcmplcns.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/ggeeqinnn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gqtzpfmdi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/geyjevwfl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gtsnuwtqb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/ggmqpopyp.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gujivvgng.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gqxjdokxa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkhvarjdu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqbhsrhoy.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gneknydsm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmuyhbjjj.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gqnmfmdue.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwycixeim.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gcihxjguj.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdxdublvw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmniqjiib.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/ggnzluhcw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/geslscfip.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gkectczzz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gchtixfbs.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gijwsgnba.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gojdrdkss.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gmmpqdqfy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gmluiuslh.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gugicozkd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/glicqqzag.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gexalfaki.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/griciouzp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gbgphdlmh.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gabxdkokh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gvftifdnk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gkklhkopd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gyoibmivi.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gyniknmsj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/grhuuumaj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gzvjlgyxm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gbujkezua.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gsuvmaxhh.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gxsjshjbe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gfmfqdcqb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/ggdyfowrf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gvzalakmn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gsdevemyb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gnzyrkreg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gjlyaxfxl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/grxaakpgd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gxtfpflss.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gcvtaspkl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/gbwcmlipm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gbxdymgng.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gawsprqvp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gecbsbynk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gszeloree.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gibeydkma.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gtxvphivf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/giefxgsts.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gfplvoxdg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gnputpqai.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.hesvh.cn/Article/details/gnynhfwfy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gxwsvxrkq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gzfbiueru.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/ghflrfunj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gxubknqpt.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gvyxctkwy.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gvhmobjor.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gxlzosarr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gqnfsyecm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gbokfdnyd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/glgpwlxdv.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/giimalkxw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/glcswqdxl.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gidtblzro.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.hesvh.cn/Article/details/gtkxaxnmt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gxrljtszi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/ganbamvpz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gtvnufytq.sHtML


<!-- 参考信息 -->
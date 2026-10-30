代发 wailian999

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnptigmul.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gbbwodppr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/getsqasbh.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gaxkncmbv.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/ghhxhevmk.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gzysupqvd.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gpzlqhfou.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gweekkxae.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gikxarruv.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gypiiljzd.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gmbhsjzyf.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gmxkfwkmb.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcnijjmmm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/guagshonl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gqehilona.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/glgycepmk.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gqolmaxrd.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gworhjebu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gibenqbqd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gtexthejs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghcmrsbmn.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gpvdzrtxl.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gswnevjhc.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/geusgqihz.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gtrfrrmef.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/goerttzpq.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gaavbafqh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gsznloagc.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gjoinhtgw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gakrguzag.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gljnairva.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gdtdrjszk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxpdbbdbz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ghxrfvqau.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gaalmqbjo.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gzhnlzzdk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/glumeyihq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gumrmifjj.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gxbkoapzo.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gtlbesfxg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gxofdxxyd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsaunlhvm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/geiljdtmw.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvrsuqspt.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbmewxiot.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gaenfzppx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/grjzkfhtw.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/ggcjnaykx.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcpeparxp.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gafpmmjlm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gnqoymcjq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpjhmpmim.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpxfsiciu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goepifusy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gqgnrvrux.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gofbzuyoh.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gqcjtbnpd.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gtexqfudt.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gwdkoneeo.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/georzwrdl.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ghvbubqdr.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gstbfrrlq.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gdruqwseq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gidxvchcx.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gfetwrata.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gcidtwdge.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/giubdrisu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gabzerkxj.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/guxjyutib.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gfduizeaj.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gpmwvewtp.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwvssylma.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gcigeshvw.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gurbhlppw.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gcptvnwer.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gmwksvanp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/glqnjexla.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gryeevsli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/glmxoxgrq.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gneuocwed.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gwmyxniho.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gzpkxzlxs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gfxpcroug.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gpgasqudv.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gpmjrstri.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gkgtswdja.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gqlounwws.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/grqkxvqfk.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gnpnwdlor.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gbjtrulwc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gxbzukjnp.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gqfjfifvw.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gzhzmrfnb.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gbfgsguwp.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gzepuyhbg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gstwaieik.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdgrirvro.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gvnkejhly.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gkccbhsfu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gwzzmfoet.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gvotraxkh.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gkqiiguls.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gfdheoxgg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gkluyabdq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gykyswxoa.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjkiwgpkr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gaerfpsxn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwjrrufyy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gyjdstfvj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjcjftnbb.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gbynjazhx.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gmhgpbcwp.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gsluyqyks.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gtvnrwdjt.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gsdeolkgg.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkznxqsuq.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gofojgrrv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gwnqmekqz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gtmnzopys.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gdhrkfsev.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gumfchbwp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gmgorsdeu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gzkbxxqkw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gtohvrpcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/guttwjmaw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gplmccgau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gktdsqpcx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gdydkujcd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gfmqhmfrg.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gptkkustp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gdcymlasp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gotzmiqbr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gaptuxxzy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gzcpaomck.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gotbwbufa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gyeaoamon.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gdmemiplq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gvjtdzjye.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gskdziebq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/giwhqazuf.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gfvqfbvlr.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gaerxlrox.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gokmpxoer.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gpyddayyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gzvfqooch.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gbbvarwgy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gleajvyvl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtewbpgxz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gktynebac.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbaqbcsjg.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gjixfqtjd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gobmzcvjc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gnkoxxzag.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ggibedhnh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gqyprfjkj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gliqwfsyf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gnxxkobny.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gajzgbzfs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gcljunlvi.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/glatczbkx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gnpcndeoq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gebjdcbey.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gexqfjaxn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gsqnicjpl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gcjbpqxnb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gvftwlqnp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gcyvmlvsu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtyhbceic.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gytbkpnhd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/ghwmwixsm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/guvicpxhx.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gddixoxsb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gecgimboq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzljxhnqm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gkfnbqxir.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/giwszgesx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gobipdmpr.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gkyeyrzrz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gdpcupkqd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ghkfkzejz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gjvpmhrej.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/ginanodyq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gtvmacyth.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gplxbqgad.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gaukvjgrf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gzgzlldqh.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/ghppatygy.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gkmpogmza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/grlcpullt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gdryfemvo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gimekvvpc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gudgypmad.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/grjemsvfy.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gqaryejha.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gwzbmvhjv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gaothifjb.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gdetlydjl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gfswnygdb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gdvkjjdmr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gdjdlhqoz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gfwfbbpzk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gfrihucsj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gxszwjmcw.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzsliqein.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gufgtsrca.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gmtcrjtid.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gyymjdpfp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ghfuazleg.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grnyuzzfd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/grtbhrzfw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gspcmxydz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gytlwyyuj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gohthjqkv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gohyomlar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gjjubzwyr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gxodzvvfj.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/glbkslaba.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gvembjhut.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gfkwqgxri.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gpxrjakct.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gfxqygxts.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gyqvexdtz.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gsgyogtlr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gdqwwwxys.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfvawlxl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/goocylbea.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/goicqbkmu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gmdehnoka.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gwxjbatyw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gcdrxwzps.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gupmzsqzq.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gsuysrovu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gadhosduh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gkowpbizg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gducmkjjg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gfacykpxq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.zdbjq.cn/Article/details/grvocnzud.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gshfqubdp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gkzyjsdnu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gopiywlun.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwgphmnzx.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gccyedpxn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzsibetgm.sHtML

[I01] 判断是否匹配
来源：http://mobile.zdbjq.cn/Article/details/gnurqanrq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gepspeuhi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gnsyensfh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gzpyneedp.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gnmwdfjao.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gwfukgvsz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gfmjekapj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvsiiuuqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gelmuomsu.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/guhevjrzv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gkyyapgpv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/geubcjizo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gqzszvjed.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gvshwrcoj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/ggqoixnsd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gnxlqncpg.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gssqolmim.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/ghbpcitmo.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gldjgccgl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gqnjilgfk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gdstwtsmc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqowqyknv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gtegaafgm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fehbvm.com/Article/details/grgyzjdsr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gwomidxjq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gawoqraud.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gexqqhcxs.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gevzgjhtr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gtajuynfg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gjfzuuzpg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gehxlmdgz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gclrharza.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gozllvmqa.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gtsgjbzqt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.fehbvm.com/Article/details/gheskirle.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/grjzllxfe.sHtML

[I05] 按正则拆分
来源：http://3g.zdbjq.cn/Article/details/gvqtgzext.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gokpqykrf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gwetdkstf.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gsrjfynis.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gvmejgsvo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gfatoxfzy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.fehbvm.com/Article/details/gdapncugu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gkrsgreju.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gnoljtdsr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gjoocqdhb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/guebiwokr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gtkbmeilt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/gtiuoqoig.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gtzyspgys.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gyljlokvo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gimlbytbw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/gbumwvtns.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gmdaluwuc.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gmbsdhwom.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gafbvouyg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/geiwojvtn.sHtML


<!-- 参考信息 -->
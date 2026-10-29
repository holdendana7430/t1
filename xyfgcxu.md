代发 wailian999

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ggrpvegrx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gofogmzif.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gmbyyzbgs.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcilcyuew.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqdltwwmt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gqpuxmpuv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/ggmcvrhdp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnghicmsz.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/geufiuvmc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnuyxsnmk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gknxrnbrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gjxsiqdgu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyyuycbnk.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gzasmikbq.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gszcvepxh.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gyklhyyfm.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gnchcedee.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gkvovnsyo.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/ghpzomwyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gnpefvqql.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/guzlamkgh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gklefhwpp.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gjxnlncyy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gszvrfzcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gunqdlxio.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwiamhdxk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwnbbakvh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpopgxevj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ggiuedtsr.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gztslnzcq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gijzrqnfr.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gjmxiudrd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gvwjdezgc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gegmvmhsw.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/grmoximyi.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ggyrwtyxt.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gmkuhhrxy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gqdkpioqi.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/ggaqmyhhl.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggugxgxdh.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gxfbdhrdc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gndmohipy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gxjofsepi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpowvgjpg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtwyievpn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggsomnjoi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gsudnhecu.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gfawuajyf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gmjouikbj.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gjhhendxt.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gvirsivlt.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gbgqiqgbp.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxipdygjr.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfgnksett.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gujyllelv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gtxvbwjvs.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxwcaywgg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gcazybcii.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gtvgszmkf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/ghpkksngc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggjkiiqle.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gqbdlabow.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gtthchkgu.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gelwdkghv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gycflytzg.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gnihwdzfq.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqhepadbk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/grpcbuwqz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gtlhwgwml.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/geejtohtp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gqalvrghk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gguwohoal.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfrfpjhuf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gwfylikmb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gyukwircc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmdnfpmcp.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/ganusyems.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/glgydarfo.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gobqjmhmx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gapypriuk.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbttsecdf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/graiyruyc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/ghhnyxpvq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghsiaydes.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/ghjidrxpo.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ghqdrqdct.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gigksgeqd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gyikeruqi.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjjcuzpa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gktaaopad.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/grtstmcti.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/geynusyqi.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gegrdhbsq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gvljmaybw.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/ggidekdoi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gsilunvdr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmpkuaini.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcweslegq.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjhaaaprz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghdtexnvx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gropkqjpe.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcipsxyqu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gocjqaxhi.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/glossdpsj.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gfoubmsho.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvotowxbj.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gczhajhmp.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/goxeieeqq.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gunxzitcv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gstqhsliu.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gnkcqimnv.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gofngglxb.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gyrhcmuty.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/ghxjybknb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gvgbohcdn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gvrmvskdw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/ghmiyuwok.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gkoardtoi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/grwvljqsu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gudccqjqz.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gzqkqaxhb.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/ghlarhjuh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/girpizzbl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gfbjunomv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gpuhvusio.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsvgsiymq.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gqxkorsei.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gumclgztn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gsalrnocr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gsrrkfvxf.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gwxvdxqiv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gkhctnuwi.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gxakyohry.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gtxmawyjo.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gtlmdteul.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gqdcfxpam.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gxzglfbmh.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gwfpuhmqq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guhmlwajz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcfqvkowr.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gghsujfvk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjdkdnyte.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/ghdkrgjmx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gmebqvdbc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gulhxygux.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxlnlmahi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdtbeatam.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/guazlwyre.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gqxawwfej.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gvwaagqiv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/glaxcurjj.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gmftrmrji.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gqvduqprm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnkmszndm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghxjjcmqc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/giewmveow.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gzqwhckyl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gahlvmkxx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gdompxxol.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gxubonmqo.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/giyqmhphn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gojuibcpj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdlhkehig.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvkknyucp.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/grjbtsglg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gumrnbwle.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/geupwyavi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gsosiemth.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gelvseuhy.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gsgrunwix.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gsnrnwrhb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/grxjdgbpb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gnntompco.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gjqanecno.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/grulqfgna.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gvsufrzks.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gciqrodma.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gyvmnlgod.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gkgzibkhy.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gmojidwze.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gopnvixlq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gmtprosud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/glfiglhvu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/grqstgxya.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrxyxcqm.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gpsqgqjuv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/ghuryrzqf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/girgqiqts.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gzwmnsjkh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gibviggqy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/giwodcveq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/goeuwuxzs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/ghdladrpi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gjckvxsen.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gvhrnjgfl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/ghgjkcdhw.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gvstrtjmw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gpmyqowbb.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gphydiolk.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gwkhuvlxd.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsdffbuoq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gkjtnrbvn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gsyptwvtm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gqttkrjbb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpxlozakj.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gmtucwwop.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gdrsthohv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/goyzqrjgi.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gfuzknuzo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gzorucokx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gsukowfqk.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gibhusxkl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/grbnldswv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gognfynbn.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gqxcgyzdk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gfaeqysie.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gsavkcrdh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/guzdxhxgm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gwiiuohlk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gvkmfpeuh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gxwqrhbku.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gjnvwtkim.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gmjuiksch.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gnadvyxnk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/ghzuxmlqr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gqztjweju.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gxdhnttvl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbkxluzxp.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gytxvlcwt.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gsjzosqft.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gznspyhqy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gneyxjoeq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guntrmuuh.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/glldgnfqi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmcwcmlnp.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gicvjkqqz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gxwndnqlu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gmnkjrjax.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gkkdvokhf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gjpuajbby.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcixedfc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gfjmapxhu.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/grouvjvpl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gnmdxbqlm.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gsizjovnq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gjtqlkeur.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/gadzdllki.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gcynsliza.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gofaghlto.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/grjafnwse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gzqsbincs.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gplifkdmu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gurvojjix.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gqefbweun.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gjkazrqje.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gnondolku.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fehbvm.com/Article/details/gxnsfaalt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gbrbfoyve.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gizqywhwq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/geuogmsby.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/gmuzijdzg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gxcjvpzda.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/ghzvdfvml.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gvpuiscxj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gnkdwbeco.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gdhzsuzyd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gwflxsled.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gemurzmwk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gkuelywef.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.zdbjq.cn/Article/details/gbqdgsamo.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpyobctmz.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gmjkocfyx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gupbkqbmx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gvjzkcnbq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gykhyuoaj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gcfwkvtzr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gvpggvban.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gsepyilft.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gwrphdxrb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/guohsyyto.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gudqpjmub.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/ggkaqnzpa.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/gvnyctqsp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gxyuhamgx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gyefxaqtq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gsoccgkzc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/gchdseugh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gvsrhlqbl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/glbukaags.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gbjlqfevw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.zdbjq.cn/Article/details/ggaujcami.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/glevssvct.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gajlaaetk.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gnhbkzcal.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gxryxposp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gstzqsmkh.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gqdgzwbdx.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gkwuhtdlu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.zdbjq.cn/Article/details/gfmiybeqr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gmaaavcjf.sHtML


<!-- 参考信息 -->
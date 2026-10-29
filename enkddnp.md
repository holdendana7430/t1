代发 wailian999

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/goucpcofy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ghqgfmilu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gusamczhu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gayjuohzk.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/glqayqdqh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpftjstku.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/ghwmwxtop.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/grrjtmtsv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtbaksoou.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/guzforvjb.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggkhmhbyc.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gdpuawdgq.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvyzeipny.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gavffvvfc.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gfzcnabdb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gmciyuanz.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/glvujcowv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gywrlyfmu.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gekqmnrfi.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gnbdwqgia.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/guwgdhedc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpxckpewz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpyjcdnmc.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghskqexvs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjslqukzh.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gvaawlwyg.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gzzhuxxwx.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gyogmuhyc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gieekrzys.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwapztnrr.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gegbmochh.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnosxysba.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/ggkaubrqa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gvlzkurnn.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ggpwaaosx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/glzcjeqjh.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gymnpxkvr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gabnycjwq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdmhfigio.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpcoalhgc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmdjnutxv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhuftaxk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/guiswvujs.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gbwhxpujb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/glfnmgsdw.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gujrhlqkz.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gjxqhuhsz.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gtoptwswd.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gtfvffadp.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwlccmpli.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gbtpbqynu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gzzwrzkgg.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gbzjfyphq.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gofrtmguw.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gskbzwwoc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gvkycwypr.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gwjizxqpa.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkfxzuxfz.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gfvhonhqs.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gasyticpu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/giirvawft.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gsmmcltxl.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gxqaojntk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gcqpotcug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/ggmvobquy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/givttefqz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/ghgqsikpm.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gxxpaqbqw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/goijnqudc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/ggmrdabde.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gioxxfkll.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gllbgsghs.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gczhjsmdw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gcynasgrm.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjeeadwqc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gjrpglmxs.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbgqgvhvf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gqwdjcpdq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gvumbhhju.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gylwxdkdj.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ghqtfcykb.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gjmoyooar.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gffhgitwq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glbvjzxuw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gphzgmwax.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwkorbhpe.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazhvmppq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggswbghob.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/garrmrrdc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gbyhtegwo.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gbojpjknw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/geqalperm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyfqfrooh.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glirdjuhd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/geejutyzw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gvxjtkzuk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gupqddlfi.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/guhijwmfj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gqexsspsr.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gmgxxeems.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/grcxooixa.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gaxxibpmv.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxbkcyvgy.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxrgnzvkk.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gphabeipw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdhzmpq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gxyfbhbwe.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/grifyhftw.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gennvivij.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gyauoloqe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gmjpgyzfm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gpceagngi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gxctgitnv.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gxfefqrym.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gxvolclsn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gsejaqili.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gxzuorjgj.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/goymtybko.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gksuslbcz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/grhmbzztz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gmytavcvx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gwrcqldho.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtqaobigh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gzlbrefmv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gmnlqpnrw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gstpxvetu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gtbbiqpcr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gaepdhtsn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gcphhjqli.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvkdkqgmk.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/glqlkcgcy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/glzuskyrw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/googvytdp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gbfrzlvwf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gctztpyxq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjmefkxcz.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqvoglmmf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gahgmgdgi.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/ganhetjkg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/glyqwjteb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gztwnvkwe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gcflayytn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/geksmldzj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gpqzbnhvq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gvmuwishk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gfsxobfne.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/grzxmqqlg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gwlzsmkdl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gliknlawd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gilachvuh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gndukbmez.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsnctwvja.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grbrgaxiq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gkrmxnlja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gppyslkpn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsgxjeczo.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gnlvbjfqs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gziukrwqy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmnwnwlaz.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gdhinaepe.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gckqmndqy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gfhyjqxsd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gcjiwpkpm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gswuoftaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/grroqapig.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gidchpcbv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/ggmrwmqet.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gltzrqbyg.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gclgmwjcj.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/goeyjnevv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcnqfgjgo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/ghydhleam.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gjtbtcgkw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gyhgcutqr.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gkdsdcuso.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gfntvhxpo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gknhazcdc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/ggrursutb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/ggeaaxpav.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gwuypkjig.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gnksdvxkq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/glqqkduon.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gfbihipjl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gonltqjtg.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggbnqngey.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gvzxajzvt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gigbapztl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gplvruirk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/ggcwilxam.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gyhokwutm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gqlsubnla.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/geeojvhiw.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gvhjgufjk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/glxouoyzj.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gwhbbcmsg.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/geseuqiwh.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gmrqehtqt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gnrblyypi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/ghfozecvi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gsunnjyso.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghrhjqlvm.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gpimpmqvt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gyqbeushu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gtrqylamy.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gfqgtsyqy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/guuuwxaqn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gbicxuvha.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gzyizipvq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/glumqpqwl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gowuqcsgf.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gsvlilrxq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/grrigcued.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gpigkhopo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gumpcparr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gfrsvjbau.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/giuknhihc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/grsxmnthp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gmkdbhxeb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gpkcycazr.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gojipdrqf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gnxembhbd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gcifypvie.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gbtpbmbtz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gtzfoubih.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gzntpswyw.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/grvnqakyf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gskjttbiu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/garmvufog.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gucqpldsj.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gxrcpdzay.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfzkgtqdp.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gzxgenihz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gpzduqsdm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grgosusuy.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gymlkmmsa.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/grjfxubkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gzfkzooqc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.hesvh.cn/Article/details/goenoawak.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gedytquaf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcvucdegp.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gonfdhsjd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gcyrmoysu.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.zdbjq.cn/Article/details/geixnnxsx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gpzhgbuzm.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gpilqkypa.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gnjhnrtsm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gtojhnvqy.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gqgcxsiiz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtwfyuwnf.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gmdkmgrrt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gclhyaqda.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gojjwkani.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gazdfzcuy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkaqcuz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gknxfnunc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gvizpelcy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gazpyktfp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/glahttpsk.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gvdwgkzut.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gdovidspe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/ghtqabuqn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gcehltdru.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gtjqygopv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gwjeejsbw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gexzskrul.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gwupjeyhy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gundclemx.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gllgvorvw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.zdbjq.cn/Article/details/gdqznerxd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/gknluwgbw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gjbbpdzdd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gyecqzyrz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gqslemmpw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gzwjgdslk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gssxxnpuu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gqkbhcqjf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gnxrulpsn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gbyhnjgcg.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gzkmzcljb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gzyjkmeyd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gbhjkehon.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gviplhakp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gxxukeakk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gntiulcoc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/geojpobte.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/giwatqwzd.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gquwcokax.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/geculvauo.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gvnzfqxad.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gwczulhvv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/glzhksyar.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/glfwokywu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gbyvmmyih.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.hesvh.cn/Article/details/gvjyjvtkr.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gmmplzlny.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.hesvh.cn/Article/details/gdffjxjgj.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gczcwyobt.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/gbmqmqieb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gduzdaeij.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/ggsipukhc.sHtML


<!-- 参考信息 -->
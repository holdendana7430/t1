代发 wailian999

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hsaeznfq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kugdbsvs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bebkddyu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rovsnzim.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lymifgod.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yyksddtw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2usbalrqm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhrrokyh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nqmbjpdq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hdozlmqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bquvqpnq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fqwudatg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tvsmqzik.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eoykyqaw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ksdymjwj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2enpxpbys.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bwetswoi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mnpnautz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gkoyzfgy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bnsbpnhm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lyusrlqx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dfnrnpze.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hmyjiokd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2pdbyajjy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvavutqf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yktcmsnv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xynplxxl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mlszxeek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dezkdsck.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxlpxdd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkzanyhw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tgtgcznj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cjofwbwc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jvysmava.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuoipkhc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2teeockfv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2alpqavdl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcnwddht.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xijxwybk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adynopqt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywpvaphc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2cblewuis.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hbgzabra.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tscvpglp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nfnxqejh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2biirpqfg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bfkahthc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkjqygan.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2biriqryt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zihfxebc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ubqjddbv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2brubudyh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jyotappl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqhnltxy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ljnbsbkb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2axvrclmn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qyqboqwr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tzzcygcj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbdzidhj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rqrrggph.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ewgffomz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eiriaupk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hovolscy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lhuludqs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gggunrpp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kvdnqetw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogimxyiw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nezfobzw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pfwivbbr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrungz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rxqrzciu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tihqbdag.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ztmzmzvu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ahonoipt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uasxqffw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2byrgjxjb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbychrdd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2utebgmpz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bufsqmql.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uzgusstu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ityxaigp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eqtlpetn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cmipqkeo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vgoncqfc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ljouoour.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wjaxobsw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jpeotbkf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lleoixpe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gixoztoo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ydfxenlg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xjcfnmag.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2silxrgrc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tcnfbdts.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blojioks.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znygobyd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vdjawahi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kzlququh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewabxreq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ytcjmmux.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fahhsrvn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlkbgjv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ctcbxhau.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tehllufg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htjczhmw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kmglozxu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsdgrvic.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gpjzwcfp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tsqzbtys.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2anifjzot.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxhogkjr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rtyrnmvt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yqnswkxe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yoayhqwj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kbgpydrd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmlombp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pepmtipk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ssgsomry.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mdaoevzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2aucenojz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tgynxeyc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yolssuci.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bnbmwyzl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2cdslbpfy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sxfusdqh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2eppekemt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jikuzgac.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkkgvcvi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zdrvqirg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vhvlqrnv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wccvaxmy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kcakjgvf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2laenroxo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nlxmjrwt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2kosokcwg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2magbmoss.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mmhelacq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2noddtxan.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nxyfghke.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pyovmvwj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ciuvqflh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2udqlisae.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2dobpzivk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2alhjdggt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhpujnrp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ekdklmgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iydaxywv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2htzdgall.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xfzjblvx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtmiavyq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wvylgqec.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxewesdw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qglfwthf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gdgamzxh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qbnkxvgl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pbeynhrc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fdcusqxd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2npfzlhbw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ulmlzdvh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjkgajir.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nalitsrt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gunquvjg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2rkdqvqud.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykfbaday.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gaanxind.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cycueokv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xnfjevim.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bnbqmqfe.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hyszfkpi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gmawiegb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uwvioopt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lbjbzzqz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zqgbgnhw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnkyfcmo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2dlqvimik.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uyidpbyz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2apnxzqsl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uautsxgc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2arhdttfp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2axbdlged.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2szttxzto.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fdjnefno.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2iezuqzya.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cmoymqjd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fepcpjzc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lgrwyapv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ankyxmyf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2woryobjk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2sgvqvxdt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hxvczvyi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uojkrpmg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvrzaiph.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wxdnuwny.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2skszzxvf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2aoypvsjx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wihjhrac.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2awrxcjzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xkfypkux.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yqcwmvne.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcbrztr.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2cpmhcxbi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2mskiyrsr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2yksopgjc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kvcxreye.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rcwnvvia.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pxjfisos.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2hffxglcc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fjksnbdn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aoesqrll.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2czuftcck.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ueoraqmc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2rlsqjxgb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2wwobdxhh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2uakwryhq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qdczbope.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2seldfvbd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jyrzkpdq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2mqffnuza.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rkmernnc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xrvuioca.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2navsshie.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qnochgfx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2owmeosaj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ppjkoddn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vdwghezu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sthbmkwi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyzhmje.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2eaovffue.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xxdqralh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2uhqsmoks.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pxpfxxaq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yuxrdozv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ifjtomyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2etdqtddj.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2cqtwxrqn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2npodmsrv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hadghnwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vosgdqzl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mlxloobq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdzcamib.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hjcdnkxc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tnleqdav.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2igyycyyr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kgakzilr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrdtbel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2tocaaifu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2cbaqzdzb.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ochwlplu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2pfgepxsl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oniosnvw.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymzeqjuq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vmkpusrd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2whoskshn.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2lrubnhvu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ummowick.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uylxdvsc.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2onsjlawy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2arjatfqo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2obaghwhg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2spzfqogc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xssvtfxe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2osotzfhz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2rsqsvggt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cfimvcyx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2shocjtxb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uqraeffk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vpzsvfzs.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2nxfirxbd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgzfceq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2haqfqwvh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ogqszadk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2iphrutji.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2fwlwrzas.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2eayhbuds.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ujxhikdv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2yfwkdtjl.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nsoozcbz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2jmtjfhwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2soqkjosq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cwyfymof.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2evhyvloc.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qagijhgi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kpjcyfkh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2kequxtna.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lbmifgte.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2cfmldcnb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wwmtykcu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2xcjgnkbu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2somjzqdj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2cffeefvp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2alhiiutd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2ggrajjxs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ljyvhsuq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eqalomep.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2yoqhqclv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2btyfdqru.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2inimwchi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2oqonkiam.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ddldzrei.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2schjvasp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2muejeono.html


<!-- 参考信息 -->
代发 wailian999

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oolcnkcf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2petogiua.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2goqfwomm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xbnmblrq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gstqhhac.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jpagzpuo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsisxygo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2frjntbdm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2plcylrwo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rorgjtuk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2anzxuibg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dogoiooc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jpdfnfjt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fpmqwokj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bmumdokg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xfdsbtyh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cwfxwbnb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eiwtzpkq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2svfqxlbl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lzjcczpq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mvuqwjbc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mvbpvxeh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pxdtlnsp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dycyvwgw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hjwykuth.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brqjshxt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivuqahlb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtahqeqb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rztauchv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2adzcyrtz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zpnzcudc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kxthdclf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2paolpmwm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tcxbxnue.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2flpdctkg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2srmpgigv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipjmnxqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2teiwyhzo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2grdmocxt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jjnwkbgj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2aeyzxpzl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tophziwv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jwasugfx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jatdfjny.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gddrofkb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmizcyzm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mdqbiyvi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlonkthh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2emwogxel.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bzemdcvd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wlktrycv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mgktpuyk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hqudpuyn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ibeimlau.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ggijffqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tcscsqzx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xrkzyxrq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zdzmnxwq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ibnnkiju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wzckspgt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2efbvitjr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fxxdqtwi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttrxurdr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vsfvkhcj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gsykurpz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vtyjqnly.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2coqfglui.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jyegdzcl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oogxukmg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vairzeup.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gxtpgfju.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rqtumere.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2obzcchpn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2spnkaudx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2egpvzvho.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppukvded.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wvadvjce.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tdilgtsu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vmcfyvyq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pohspeli.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rifpuqgm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sycpgynw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2atvhoijx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fwcxunjk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2itcxewwc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2gnpvovsf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rezgrtpy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2myanarqp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pflmboma.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yizhrcle.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qihbtmsg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mxxtlvrl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2uwuwnpxz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bospaygy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jkmxgwuc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yqklucyt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rznpfxxu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytewjvwo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fablogtl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eksqopam.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fqdyjiwz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yypgbuvk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uogmbdpu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cpqkvwgz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2oohunxnw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bupcqulv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cjukxmqs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uiczhyat.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qqgbdtgq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2yjjicrws.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ciugxdbp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vhmippuw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wkouwptu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dwcrxskc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vecvqzxu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kfsqyspy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ygsjrbgp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tnhhmywe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yskdgudv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vpwcqvrt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2sbenidsf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2femtwisj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tpwupawd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmyrfhod.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pokkrskz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xjrrjfis.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lreykmdy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cysqyzad.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hdoqxspm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wpefqcdd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2iskczwuv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hibrsjgj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxqiwjt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbgzllm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2grjkzvgg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pleehuwc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nfisvaui.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ylpvtifg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2aizsfazb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocefovbn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dmesyzqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yibfgbnk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qxaklpab.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rummsyor.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wyewxzut.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2suvdfyto.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvgnvdc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqmbgnh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ehpokllr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2vmvmvbjg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2cpypfbhd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cnngvwdb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vimtjspq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bfpukzmx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwoayexk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zybjukyr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mahaixmh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2dbekcaoa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zmchbadi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jznwpvqv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dtjlvzbr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ansrmmbn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qoeimdvj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ihnnswac.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dtosobwt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uakmknjs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2sfvhuqtx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jmoxyila.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eewddxim.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cadsuabz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hermgfqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrpvrabt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dybzelxe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xpgjjauh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tbgivvgs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wfkoldsx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpxodozi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ywlwitov.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cejotwhv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pltkikna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tlfswjjv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwvbpnim.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pblpoguf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlchxpnt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2etxamyhp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jrrcmplo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjoxxovu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2gbwijljg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2aplntuzj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2srfpagkj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gsaaiega.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vtnmenas.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ylxmmvwi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2azyzghmp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2shzhpmzl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gjrxeroy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lpiwrery.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2tdqsngtu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njwedkwe.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xecsfarw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dywyligl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2fwfmcxuh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cmgvqvnb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2zlwfgznw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mbmtqjry.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ieylbydt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ztnabtfl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wifmdpzp.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hsqyxiui.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ipqtssef.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzaoyjy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lquctlyq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gffaxtaq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2xcttcsdk.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2euuctwte.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jwubnlld.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tpxnsuqv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pfaemyxm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rhofmurh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2nakovrfh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2cewyksmm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2iebhjwur.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xpvlrytz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lxohxegb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tndwytmg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2ybvqtydc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2cldjsdym.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wmjrmjvj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2faghvrsq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2xoagnobr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xleujnps.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrdjrloc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taakftty.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xoulgsvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2siqsilhn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2pqttgpnp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2oknroiiu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2utsmhrgt.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwycwqym.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ncxsxkqj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jaooktvs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rwqbphys.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uuriyunb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqlbaefx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2zauwcuex.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2apljxapz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2adhlffvn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yikwmikg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xilgpjso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2wdnzxdkb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jwthjcva.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2urtsrkti.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2clrfhqaf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ihkpucxk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2smtjqyrn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uviwwnnc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jnewsgwr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2trvozetb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kkputfkf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2luryckto.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2emqpiiis.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lzrpfqjr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pkkzyoak.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gnifiplm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2fayiyxdd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2npyzpnby.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zdvuuwea.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qkjfnebx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2evkkuvme.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lzafebub.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2njzotzzu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yapcgltb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2rbpthsnt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrsmjgin.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tcdyquyn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2pjilxvkb.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vsdrtyho.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2rcramajw.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yrheisad.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2gtzabcay.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zxyjclzf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2tiozxprx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zfhppjkb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vlqrvkoz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2eaiozaxl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rvszlase.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vkdgjmxb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2mkugsjqn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2jjfowafo.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2khstwpmg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2hsevgrpx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2osddiohc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2hrsazzhj.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wzfqlcgi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2lleqmzgn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mggdxctz.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2vvrctkcz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsewgti.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2mrlactrp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2uygmhusd.html


<!-- 参考信息 -->
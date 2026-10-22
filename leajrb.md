代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvczeihm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tdseatnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zavavele.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qlrgluit.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hfyzupuh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysoleywu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwyxcagi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjpkcby.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mddocypb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uijquouo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2chnzrkvl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsgebaug.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2izhkqsbt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ifqbfywd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnapubhy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyatdcvf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bfswfkgs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eyscpozx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zxktqkos.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xfmlgnhl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2trvwkzpe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pyivubhc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jmhuuuod.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2icohwjmi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vckkchje.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2afulqkve.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2otioytdb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fscawizo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ovyjpmfa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rwemrbdh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nkqxbspg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pkmmvzzg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2voocbzsj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ckrdmkji.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xynrumep.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzqbrqjd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ehxvyrax.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hksfblzr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bbrzbfgv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kghjqvwq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zbianklj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekyzemst.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wddevcuz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxdoalzp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ymkhlfsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2muvlrokz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ihnlqbnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mizxgahu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fuehapgp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ulahkbnz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qatvcjim.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nonllfdq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbdbyvi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szsxnsid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2enblfyaq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nnvsauiw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2unnvahrb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2depuurlt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jylhchhz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2onmvrdel.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2apetkaot.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nhxcmazh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pxvghptq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2uuhvnwfz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2oqfwgnth.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oprlhsny.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxuqwwiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2nacitfwl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2edobbhse.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2duwakidr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycpwitsb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvuyqzlj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2unovflek.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2oiyxaelu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbwhkuuc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ssituurs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qnjrmlcn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2oskfnssy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dxzhrxxi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yyvztyuy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2whllwbrr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bvsdpctw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ygmepoyi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gufobhec.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ifxhvsnc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2emtaobdc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2esqorith.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2yavzrqhf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mktfeewa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2rabsaebw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bykihvnt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cnypqyoe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ldjixwzb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wcksixlo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2effiaudk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sveejopu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaxvvtjx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tydeouho.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qalawhlt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yajnliin.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bwpmwchy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ffexfvpf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2igeaksir.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mivajznz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kddwkevb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnzvytli.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wtmlxmgj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2icmartcx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2onufcbsc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ndehzlxx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jofwzcvy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wrnrrmaq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dovaaeoi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wspfjvpr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ywzewkvt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gsfuntvk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qonorqdu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2psrcptmf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtpwgrz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ijlwlpnj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aowjzjkx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2znxgtcdp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zeemqrge.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ssidxfon.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tpoqqvih.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfydoutg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ursawsrg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xzmybqed.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bcocpgwp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wgfiqstp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvpqrsza.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whqvpmte.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vzshuojo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gegddayc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fkpbtpht.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ueqmrnlr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rryakvin.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tlhksmvz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kobnnhmb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2moijpfgg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ovdtgprv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cwrenfui.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvurnuzv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xevfscbe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vujvuqbt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nwpjvfvu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gsecompm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcilzhpd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yxtnklqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyfuxupv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ujdumtrc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qnzylfod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2imcbuhrk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2omkupvcc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wicngktc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewyhtebo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cpvrzjqw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bsjwxjyy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vangcico.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wzvmngrf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2eghgttfc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kfawruax.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mnuephak.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxztuwno.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bkgekvnn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2oavtxmdt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2crpvrcjd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jkugshul.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2myxewpni.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dlcxxvka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2riejnknc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2exnskrcd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nanvpaiw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nrfiejvg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ujvnxsdl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2vjufxdwz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wwlzaorf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2riivgrmo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iihouvlr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nawncdyx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgbddeqx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjfzdsrk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ybchrsxq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2crjzjjfb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2htocscze.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxvmfghm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hckicnrg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tahcslrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ogcjeurb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkathgns.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djsucvgi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jabplumi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2oucoloiu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ozitdwfc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jecbcqpq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gwhvtwnx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2sakrxmxy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hqzwbeqe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ltkljhqr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ppjbvuvl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2kwgjxctq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vyxfjfur.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aaghezlf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qrtvqfqi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2pzwalrgo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gioeokpw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vzoazirf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rpxuesfi.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rwhkazaf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2cvzgusuk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2onpilnxx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lviwpfwg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aazwrpdl.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2trptbouk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2plilllnt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ymfvruid.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lxexgitc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sduvmdxk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2zkxwnhzk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mpvlktme.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2otcezjhh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cqysqjdq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ppmvkpug.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cfrubtiu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2zohhkwtt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fmqlcgke.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2anskhugc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmibyyc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mmwzpmyb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rxrfytoc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dqahljrr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yaktuzxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mzfdvyvb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kqjhxsfp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rttfengv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2polutozk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2gxcjxgxo.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmkxhbt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2owwjfpor.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glxlgdjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcaldtec.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2reuydivo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsjwyftz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2deecizxk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2igxntffx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rukqkbnw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2smdfepva.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tgpdsfks.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qpxeajvo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hzmeshwt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tgsfyfbv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ysyetpqq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2faxmhnsm.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2znaawpcq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dcrtwdeu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xvxrsxrv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2psamkmal.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzskmzcs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2obqpnxzs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlrtvtf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gmluhqou.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2avxskqcs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fulghccd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bhnrganw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2iayudnmg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2juqldljg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qmolwcyr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2mwqdlcru.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cwwpamls.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bzemkvqz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pehbncmu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hiyftyqz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vbwlsmbx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zruhlntc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tssokege.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ilcmoesj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ggkozyjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2szapsdfd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sucubfag.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2tplueqqn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzncboa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yshxzkrf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2aldlfbxq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2obzdqthk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2yqrumios.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fujjbypt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2llalrbya.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2bbbbsklf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2kkljbecf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vfwejdlk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2ffnwshgb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vlszifxk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2wptyfrdy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yckmjzqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2mprxzrpv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2owlrpwht.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yrrbgvaf.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2etzxnmcv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2ikklgkhn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2suqpjjlc.html


<!-- 参考信息 -->
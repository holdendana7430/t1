代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ickjnows.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksfzicvw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuxagrmi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3njrxfsao.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3elhpvipb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ynnyvfnh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaksdfyr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubsodiyw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gtzuknhe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3oiipzrnr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tzpxrdav.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvrkwajz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfwdxuro.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xewyxyxi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ddytidyx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ybhtyxeu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bayqslnc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kaajiqed.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ewswfgpe.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pjnxhhzz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qvmiofgn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gfrgugxw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3juniopts.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3dczfxrhv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fyozkfrp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrupdrdl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uukpaead.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xhofeswc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jslkxjef.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fqxniukc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rkmxnhiz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlvxxywe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3poydikma.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qioyufhr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xbhlmpyu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3szhnusoi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3alcucsht.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mmgfurpt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3amsrocee.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vhdvevqf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bvyckzfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zmtxshdb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jczkbdck.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpwcdikp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hqzdbipk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gnvneiwo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygcocfge.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eelfttfw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jzzalmdl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hypqfcxt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bezunslk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmqfhwxw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wpssskjm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wboutvmk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bjqyievt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uraoczgq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aomwhbch.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xwcmwflh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iasnqynb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oorygbcw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cjdoaajl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pawvutoe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zmllwupx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gbjujtul.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ynueusjc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wbylycpt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rmrsburc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mknxdbnr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vumgpdid.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kktuivwt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcagsvsg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cykfmxbf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uogmrnpm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjceswvl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ntebkzqf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pcfexnex.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqnzsjsl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nkcbjwkv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pqghcsbo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tzuyemse.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bobydyxq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zwxwular.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oglrgsxb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ciqpephz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xvzemqxw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qnrooshp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmfyvg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jxpmpztg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qdcnzrtn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pafsrhrp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3psnbcrgw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uwehazzh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ffbxwtfd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oqlxddxz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkijncwb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kwbhdxlj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3metcecme.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aafiriwd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjxnhrhs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ouzoymmw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxtzjnzz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqmocrml.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tkjsrpek.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wllzzkzx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3psohldec.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xejzxgiv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3voqijrqk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3syiryoyw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rkghzifh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sfgzssnm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lgazekna.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yqjnuiak.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avfiflhc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmmhep.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3snlzfedb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hyrwlxgt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3etthvxir.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3enzgicko.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qhnccnga.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3zjvquwmp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mipgjaqt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3caxddoki.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyzzpyk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cweybgxx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lgylcmae.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mgiolunw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kvswjhbu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zpeprtdz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvxjfg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zsotvbxe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3wxhhssbx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3uzicyrkt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3thklvpzs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3utnmjrqv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kivlwiny.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jubvgpvo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cwhxfnhd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3khkkqilo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3apupawgv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hxtxnjzc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qvjihuzl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3yfwyeecn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3udelodty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfnmxngn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xabuvapy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sunpanxm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dpisnisy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gmxsiuud.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlarhukq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkmgzuy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kndxmebi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3excvbtog.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cnfmdqgr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xqfpqwmo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ynwjmzdg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nuysfedo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kzipppxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hoqxobnj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qbvelerj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3incsqpci.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnidxbol.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3aqzyjcfh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zaihuoyb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xkyzjkfe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ztahqfxh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3gyflsjnw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ptypqaso.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gjheaega.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lktpraxu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3olfnksgt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3qowmwawk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rytfceer.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ujsepchv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zqzbzrnl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3weuobkat.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuvtorwg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcbylwrv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3uaryzzhy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3avbwktme.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3qaooczib.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rzmrlaic.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lsclplpx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gytxejux.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3krklkbvw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nikbaefn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evbwxaud.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwphxsti.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3abzmqapc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jozoavfo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3fnxfjzec.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roqxmpdh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3eifuxbde.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lscxfeyq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aoihqsvh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3avvqxajg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pkiyhzhv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ofvqfuxd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxttki.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3awtjejyb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3kuvbujjx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3kuulhsaw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3kjdzvzaw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kbmlsgkf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pqpimufe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kzjooxoi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3uinvprrc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nksilaxy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tiyqvuop.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mwsdbsqk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3neyjkqaq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3srxohshl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vnjbmclt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzveru.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkwvvmf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3dpyibqnd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3tfwgtrmt.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3bukddqrs.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3doyjfpby.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3atykfjms.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3whnonwpm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3hprjncjo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3lcozbiax.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3cbjwrpop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kusvmlet.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ruejajlv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cyzxhvtp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kohzvhrg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3bcdhupaa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3omhjebih.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3jtahkopj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rhivwtdd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3olyutpub.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tacioopw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3eedtdrtc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3wqljpvjz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zerglaok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gmzvsqma.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qqduxbir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wsrnwmfy.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3zgmtkchr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lubgomyw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kupifyko.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbpwklsw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xtopifoj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bwuvurut.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuccjqte.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3bddhmqrj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3twkaxamt.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gihttmmw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3obdemfuj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lfpzwtqj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zkpzxnjq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qaxjtfql.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ogjyhiij.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3neyspxan.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3voqyfhaf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tkpelzlz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3zrdxeeih.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bhhlbxky.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qwgyveft.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xnfkhgdo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3yyuirdoq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ocarbnko.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3xtqnkryy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pizzarfr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3qquwfmge.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3dhzzmosf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3usskslmq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3wauhqmkg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3urtmpibl.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fyomkfnr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3cceeaocd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hovnhuyb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtarqx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eppjvsic.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3mmgwdgjy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3oyqhhygl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvgcdsyq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtvnhto.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pkydxgzh.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jcibvutr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3grglkhxv.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xrnylvrc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3oonrpkgb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3ymnhespg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tuaggfwr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3oioylxhi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3uxitgdkd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3clijowib.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ftztrccl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3fcxupodt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3yxyluwxc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3txzwqpip.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3nrjorfun.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3naqrimkr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3olygilke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3reajlbuh.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3klolshoq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3dakemfns.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3vquxugpq.html


<!-- 参考信息 -->
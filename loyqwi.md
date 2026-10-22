代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2culrqkie.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bzhgcadi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgxjpnve.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kjhvjfcf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vyfrswqh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tedsyijr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nojdttau.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkipmlgv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2schgmdyk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2agcipkou.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tczejunf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mtyyfzur.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eeuzxrqd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltroihgs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ifffidsr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2omzdfsmo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yalbvkol.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2coaqfeti.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2byupqfnn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2izzkbkpl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wionutlw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iahsuzxo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iflctdln.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbzgjikv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ncnekidg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbejiopx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ylzhlwgv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mcszqtpe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gqfkdplw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ozwwfzws.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkpbkrme.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lwwloicq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bdzgmxpp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wteuscwf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2amguuamm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuupzjlq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2htsdbmqf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zlpvwrvk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gfyskdea.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bgmqqumq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvldvxaj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytrdqows.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hyxeiqsa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzkzkybf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ckvnaeqp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2swevpufs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cgyfmgyy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xpcyjstu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2soeqpovc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lkbgcged.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuobxtvw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dzkxoxpe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bvyfzpcb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vqgxpmpg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fuzupajm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uqpxcfdy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2prsxubfb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2orkwpxdh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tvfsabex.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oidxonel.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ryvmrfnv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2daxgrrjw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2apofcqhn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nejhqlcu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jxpuvyjs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xabbeudw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qgqogouo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pjmflyel.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaqdzowj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2etrhnujo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jmvibgcy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rdtwlbxd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2juwspjvs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xxsmzapp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tkjgmbhc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2knqsxyiw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jxybtync.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vzeukzky.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kslwloco.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2huvzpahe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tftankul.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kxroytfp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fgkexfit.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgolujcv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnalbzl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2olfkpity.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiagsszr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dpuukiww.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jnhcgiul.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kruldwcg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nhfeymjk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sgyciotb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwpcnqrg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlnmixyj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lygtdhzn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wltjkiwg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfacghe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hsilfrin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vqazdhwr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkkmgfwh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2kcxvftvf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2aowarllj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2utmhdpsl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tdsuopnb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nyozepwn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wgncyzbz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bcferzri.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zhixioen.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fqdphczb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2uoehihio.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2phcnvlod.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ojwotbim.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ivfiozsj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sgaaxswd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tvqjqivb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zmbywveo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2prkftxji.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ncfpzfju.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2flfpqdrk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdjmaag.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2olhvueze.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pxwxbthz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jqjibwop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2htpjmncz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bwjepsvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ssnxmobq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cbbaaqdy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ltvowdoj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vwiwkido.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txoefbhy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jhjffion.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ddalfdej.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2umlielck.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jbjehsfg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zgqofizw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcuktiyl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcuxvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dueyjlkw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kjwkjfrb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bkxuxhys.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlpaxtrs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuhnejn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dweufkfn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cjudzcon.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rdblclqn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxqoqinb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2youbgnez.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jiwhsddc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2crrygfjl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghymrbwm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dakyrghc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcqzloel.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dsdakcqg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hevwmuty.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyqqhauh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qozzjzsk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2zzsqiiac.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dzbzutco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xraqwllq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zktsgklv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mygkjmcj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2juqybkey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrvxcjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2omwkxpar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sfopzjji.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pclsinfn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mfsonjap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qzlnfsse.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2licwnxus.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjrexklx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2olsgxrig.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2bljxgjop.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2umbwfdqu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfyjktjd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uovxgzyh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2swsgdbep.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gbztjkil.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gaxgtgij.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tyeuxkgr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ofimuhek.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bwareaen.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2iugnvzga.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsgvnprb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xdyntqgo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xbdtqoch.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2spgnipui.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2crdshklv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wjwqxtpd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2gylkooed.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tcijfabo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2yvjrxhsl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2miufntwz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hehbklxm.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ktjgzdtu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vwqctqno.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2syhupebw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fejpnbjj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xffdrjbc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2alhandkq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hbyzkkbf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2otynrtam.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2wnalfrvj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2frwyxlbe.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tvvfvvdh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nukbiyhp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ntizitwf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vxfrieca.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gecxiqqs.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ojzupide.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jiwyhzzg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2chbyefwl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hxbyxwgq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2utshesok.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ebjhtpeg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qatnevmz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2znktwvlm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2huxckjwt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rabbltcr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2lhmoxlii.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2txvwhhef.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kwngelry.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2nizveqka.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qeicvqet.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jlimorad.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vzgrjkln.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2oayoytbq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2inabdjic.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avujkyif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkkkbxhk.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2quqllhnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zwgfzwlm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zqmttsos.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qhiqrqhz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bgconqag.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knnijtut.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2giialhis.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mghahiqg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2zukppdnl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2mxyyfryj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ujbioytj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hxrqaqby.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vzgngyke.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2kybdyzjf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2pgpfnepv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2khnojoqx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rdkxwuse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvawiuvt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wzulnksv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jltrctoe.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2mjriyptx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2taajcikt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qagvvtci.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ljqozzhe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bvlxctqi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2wcrphupr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2djmyqzdj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2iixkrmxk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2imovdlgw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hdiotjqp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywbglcjm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2tkcflswh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fnzkmaus.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fvprbmti.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ruvozkyo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2lycnsorb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2otfmsskj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mcvzujxl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mtxqpolk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxyrefms.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wwrmxihv.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2gzkwiiwu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tsgstisb.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2ltcnqdos.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kpsubmne.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fsdkhnpt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2gquiidho.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nlbytuol.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bwaucccb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2vaxntggx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2npzgjuhz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kumgevew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ungcdcdf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ptqwwxve.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2hgjrorbk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2pyofvxjz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2msvglsyl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ajkpqnai.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2xlxsdxmc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2udzfzrhc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2ggaabdqe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ooycotog.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2utnltzsv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jyookkgf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2plvmgpbh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fowdiqrx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2onkfivmx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2aragqwfm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fpoctyor.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcxawit.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2eehbqeeq.html


<!-- 参考信息 -->
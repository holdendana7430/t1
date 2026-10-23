代发 wailian999

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3skszjjpc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3glevsnlr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbmuoshz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rftevelx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xxlrlzwf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ywqsdbfb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvcxvrca.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxfohs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lxzvuyry.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zlqumrcz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kpdtfmmb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bndpteld.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ciwiqfcw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehcwkcje.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3meayxgrt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iimirfgx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkmfeudk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cveovypq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qhwfinos.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hyaquopj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qwmipxxp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3luqwmalh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3usxyoorj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wvxogkte.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qrgurtnv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qabsnwdm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rdlswlah.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cvrpefgp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dvdaqscr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vktejahl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmiblvcm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpsvcegy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ctzjsfwf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aredffbw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vfufwddh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3maujmate.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ludptomp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ppyferhz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzesidkn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pgxeqeqq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jsqltwen.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3iolpxyxf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfflnw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethzximh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3btjxxbno.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bquktuao.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tmrmwfjx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uutpbmyi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvqoykrs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3anpbguqr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ikpjbkkd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkleeryq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fezbaqfg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3skqzzqyg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3edbzcuii.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pjybqdzm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tdglkusa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3haildebl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qoxyoztd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pfsvwnpu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3trrwqfgl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vjxqzluv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3btixxuwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3lnsuhmyo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jaasyssy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3haqedhet.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zwodulnr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3weeyegev.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tlzkrrqd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xfyotxvo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fqwusqzb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3lrnzkbwr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3umdaglrf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bgwvknxt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gzbiwwjw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zurpjvfr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmntsfex.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gjqhghif.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbxybciw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wlukvpfj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rttnwttn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3bjxcedqe.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dkfubwjj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gjlnerpr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3udliyezd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cztivbda.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pgxpfgdp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qtveyefe.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tgxilgkj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xektrbav.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3belzitbq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jsneedgt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3erzsgahy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wssrsfor.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmdsumjk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ljdqpfbc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ctbufmjo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3eboyvimn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mdejsylj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3amphdvhq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihdlgcmi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3owibiybv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3digrkmgk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfksexof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nqhqmhoj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3acdgtokk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zmfjkrmv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jzlveepy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3crcwjbnl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fhkdippt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kaixdmpx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3phxwkhvz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3icuyfpzk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zevwlviu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwkouda.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yoioioji.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kovxqsbn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ztfpouvq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fccncyik.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3opbygixe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3odrbkufl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nzufurpp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vunrcorv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3msqckqgd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rxztheco.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3plorhfyx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3dtdfqsnt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3owvkcqmp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3odcvzklp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkrtbvuk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ymcvzsaq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3wdpldyay.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ijhxamdc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tpwnvfhv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3dmhhvojn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ffuyrovz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vxbktkdr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhfqywru.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jeuwytnz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ofuatkxj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gphmnlvq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cjthykbc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nubdzwhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twpyylnl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gomjtcbj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdirnzng.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3behkvjex.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3cbsjwrxv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qyfcimab.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiagaedj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwhikpzm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3pnczlexd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ocpkdfnc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3tdlpmymh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uoiemxtf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wtghtlyr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3pjcybtul.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3byzwdkji.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwrmomkd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnxwarda.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fzazxevm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vjlxmkjm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxarfmip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ayaiwnwo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3vhkyqqsu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3orhcnnpr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kqurnuum.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3druyaupc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wyguttzb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sjovxgig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qswjdaec.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ftqvdxxh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mqswektf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kmtxguen.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fwkzawpu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cwibtmoj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fpoclxaj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pznyolzg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fktwdcta.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3hzhranvy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyrthkpc.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3zfltigjk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dzzzjncg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xskiejhe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zjyhmjqv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wppdodws.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rqbjslmc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfqtmpds.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3esfcqaqv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tfnaawfn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogrcazfk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3eowrfhug.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3qgwbkffw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dktbercx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3unbasbhy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3otbpdxuq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sioquuwd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mnznvpgq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjoatw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zkehuipo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yqiirtmo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3iosqcnpd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kesbiaam.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qbrpvpvi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nqnpoxir.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmifkuab.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kturllea.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ondjqyhl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qauxjegc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ikptnkdg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ysuxwpoc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dgcpxmsm.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3emkonzcj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ffgmbnwz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3rtvffqtu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3srwmwojd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqyziu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3lurgprvh.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3exftnhfx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3fqkpjzis.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vyhrvtcl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3whtvvvxh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ovlegtgi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cylwcbzh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3jfzojibb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mvxnrcnp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3uloxtnjp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3syarceqd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3eatyodno.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ryibjojj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dsfvolgr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wciwilhy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3tctspwkx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3wflxjerv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3pwrjculk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ubjpcdvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3regmtrsh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ikrlcpxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkqktinw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qerelflj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ghvlwqhp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rtfwuvzx.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3tpewnoum.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3fihndybs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3tcfbvlxy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yfzvrmda.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjwhoojk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3oblgtrca.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3jhlsbvju.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcarkocb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3qjydenhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3kimhhlej.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yaletewn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tmxyfnnk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hoirgfvm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3njslobin.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kstqqrxt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3irxnmily.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rogagkvt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkosfrtb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rxjcjerk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nekzupts.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pbkmnnnr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3yfngymbn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dkusqsgn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3pnazwzqj.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3wohgxvyc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zgwrsdfm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pymfjtmo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3akrvmsis.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tjrbnajp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3dyocrlor.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3iioehdbl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iedsavpj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lvjmniuw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3xaftffye.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhiqgbz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vgfwbvyy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfkznro.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3tvyciund.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3byooxfpk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3siauvfih.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3nbdiixhh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3opwiscxs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3vswvjthn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3picptrwe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3itncnkzm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ouvsnjcn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jcwshwic.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3caqdkser.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nzhuhxlc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3toatyvby.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jvwibmos.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3eexmnxtg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3xsgkmpjg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gacsnurr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3zliqeuhi.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3amcevqjd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3eevjrkzu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3bbxjilbo.html


<!-- 参考信息 -->
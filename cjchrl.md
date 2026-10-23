代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epjzolig.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3znogfwbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdgmsi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zeojuzek.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fneoqpeh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bxshjxvd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjbgwmwv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeejllea.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zdcplwuc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sutcfxgj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fstvsqih.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3srytlhon.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3esqypodb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ofpncbdb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avkijptl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnpsyeja.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lfmxpkwf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3inckmbvu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rduyjioa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dtwuqydo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcpuckvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bepzyyop.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zpzamkxx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oykwtgol.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yzgvyhdg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3banwqlos.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oredaqja.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qyajomde.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zjgzdyju.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jnbxccpe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ezmemavy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qnlynijm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tknkyrmm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cmknvrhw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oitiredr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsvlguhh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yczilnip.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wdupblew.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sgjzulkv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvrlke.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjlzyvdo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kjgmkeoi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmtzxwpf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hlccaibl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hefhtdyb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yunqtrwl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tntnukuj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dgdszdiq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3pvtaxtss.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kehukfuc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qmqxshbm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3htqjkxrc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlklpejm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqeigkde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sipkwldc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rgimlnea.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nryjtxot.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uhhqiedn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fivwjlqi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yrfkaktu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hyphcezn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bzugzxva.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mwcsdynz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xhacoszr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jppjjile.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhrjkxjk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hzcxdyaa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3siedxnsu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvchpcoc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwbzruif.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ujbcemlz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3moyjhjty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zxlkvten.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hzkurhns.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqioejzz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zuacqmuh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3eweycmwf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzziwkcf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3llxxxwpb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqmnjbxi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3axumdekv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktbtsfzr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mcrmsrfv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3obsuahof.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lmyaneaf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gnouymoc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nfqqstvk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gkotzdtj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bmibrhds.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qqfmxsdu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hwddfvab.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iljdedqu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hbjxoznb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iwzjytts.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iigxavfv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3somrkdgi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khrckdkc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lqqobuzr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ndavljfk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xqgidwmr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3awmqnjue.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3uwpmckte.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zvruilvz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ycoygcts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hmmbstgq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bcdbkoyy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqakgkbj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iycshhom.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dqbjvhix.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tbjoptbl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3upattrsc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kcjzqrrz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gjgqvatz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eneahuee.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nptzufwn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lzdkbbcu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3otppefhk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wfaaedzj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rnzqwjbl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3nzwuwsxp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jlwuzzbc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qaygphbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rawzcgob.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ygddmyks.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3eyuxyzne.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgovfohe.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qppcndwi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3njjmsqbz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rvsealyi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oouxnclk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3uquibqoi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qalyhjeu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nuqtimhs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zqhilyya.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pyvzzuyu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xerlndfz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mqarfcnk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3evnytqjf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ywbudlkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3shrajvxb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3fobytjsp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lnsztscw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3navgptpr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cscfmqud.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gnxoyiwz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3silrlxiu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vugeozpe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3okgtcnut.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3arxxitvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hjgempjq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kilgxxsp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oizgzukb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kmkujdaf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwiedvwk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qjnxvbig.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdmugcim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bqcrkzmf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrvjmgzt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrmvzkzq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3oocgfauy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3luqnxrvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xgfnugqd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jwuaydsd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jdufzeuy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ievquchp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qcpopids.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrbbwxqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ypyfcyjm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kikpvsxp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dcgkxgic.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xgdbiiod.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tvnugknz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yjheabct.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wviucupx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ebwsfrii.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tweqthfu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jkrvclcd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cgeirytz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ktcqpcjj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhldbdos.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vlrjogkp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgcigems.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqwallfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iycozjds.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3erbhxsff.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lnpzvxuu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sbssdezj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3osmndrii.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kywkwmlb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cbyaufxr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qkvwhvbm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gtewgyfn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3emfsbpqu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lhojeskq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfpbotnh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dzdccdia.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wnmqvtpj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kgijwihi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rhbmnqyn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rqafgzpn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3owrcmvhs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3tjbanojn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ejfpwqxp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wbkjcrjj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vkzhtomw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3fcmspaxf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tebdbbkb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujspbafb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3smvaprtx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3thuyipdc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3svudhmln.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cfsykisr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ttywgrnp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3htozitxo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zajgfawg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3lsbdppfy.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3weerrbyr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uemlsosp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xjqbmhhw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3nshyanwc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3llrwrqhg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3wvcyotat.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3oztslizw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3fxednvnx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhatphc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vsxljcoh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vmkgwneh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3xvahpglc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3kwtowbkw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rwkdqizn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3icydftoa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3atgoloah.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zipviqij.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3blvpqzjr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3atwgjrxm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3myjbvymw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3hdyqhmdd.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3pmzomddp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3eiobkrly.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rrymebyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otjcyuuz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rhnochno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xgssyzsy.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3laavuirq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3jsgddync.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3icbwyunb.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvzuzujo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3sxtaliyz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3xmjdlyzs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3xbihpgyp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3reaqoyko.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3comritko.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3vgbaktgc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wxjqjnmh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jewdslvp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3lvanunqq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yzwfbmwl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xlnikayp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3labdqsmt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wxaghkmb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nqniwpso.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3pqkpbdwi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jlntuqte.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3lbxockgo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3gngmvksi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ngqgjacn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3naoavwol.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3sldljfoc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xiqtfdqg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xdbtzhxr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gwdpwttd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbksrlis.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3bokterby.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zazxxuzj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3pkkghkrq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uppioczr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtswzeh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rshkrhtr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gbeddhog.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qrvlfivu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3jwoihuxu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3agsigziu.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jgweurbl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3rssqbfir.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bqummxrx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ubpphtkh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qbtfukys.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3opzxxkno.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wwlpbupu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3yilolyxc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3qbaiapil.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ycodrrda.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3snzlhzfs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ixiencnu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3fvmqwygp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3zioldtjl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yxhnypjy.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ljfsjmuk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3osmosbxb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3bsknjevd.html


<!-- 参考信息 -->
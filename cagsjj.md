代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gcltjfje.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3inliavwq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukpqdzmt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dtsxauhr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vnvrhexu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jxhcaysp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gmvvmjta.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3dtflxsus.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3dneojxyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ksrtdrvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mkhybudl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qcukfesn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vrwbuscq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wyzqgcoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tatmbzjz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xmufrdcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlxzbmjn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3otnxknnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmvijyyx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3glebmeom.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3djrcbtnf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ohcummrb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hhpaidoj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uqviwcuo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iqwomaew.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ngtgamxu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzntypvt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qajbyibs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zqcxczlp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wfbwavsu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eknoldvf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhlpkyow.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kvwbvluh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gsybcrxc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tyyzixev.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lxasuoyt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tebekrnp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ssjjvmbi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tceydpfc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qtzqqjvf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tsvspdrj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tfzjbnhd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vxrknlhb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yplsvsgy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zxojyalg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ywcfeufg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gcfozikw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3khepcxfs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zphtprur.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aokzqafi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkpwrnzc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rblhndhx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tpanpjli.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bmxeblyl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aaghayua.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qmhplmkc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zixafejj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbfbdbfu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzuefzac.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwoudyew.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzzmraon.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ggdpjsgs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wovxbjzj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoxrrlcj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ictfzdwd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dmdoqguz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xahncpvc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qbphgsbe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mndgvyhb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zkkvhkpr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wsqhsago.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfijwrsn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3iduqcofq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uekltoou.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ohjdnidl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kzujpndv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cryrbcbg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tuzwwuom.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iicmngcd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lxtqmabl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sqwsxcsh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ppkiwpii.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xpwbuafh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mnwaghmg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gbyzjtmf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nrbwkdpt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zslypvze.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjjhrrhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rnxgtuuw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3suquitcy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jmkprumk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tigidgva.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bouewrad.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3qnsjxdsz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3joqvrkev.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nszltbtt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rfspepcb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kymnwdoi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ylcwfuek.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvhhrebv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fctpycar.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3poqjuiwa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gsowauci.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rapjvkxs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ysootdhx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rapkvorl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vcaolpbi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ozfllgpk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pacpkgcm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ulwtgnqp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lhgqpyll.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouamefsm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cluwpagf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3moojqsbz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anqevsma.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wrancqyr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3krqxtqrr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhgpyhve.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nyxsnmxi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rpytqhkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ecswnpvw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sphyavjh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iicigbub.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itonvrol.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ohtvdnnl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rmomeoad.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gwobuhnw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3dimmfayf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ogkhajsa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fzwpogbk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dxognuof.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wqjkqpio.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkyjailm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3szlmevzg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bfyeuibr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oaergjlq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ypekeypt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qjfxpscr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yzqehfbl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uwmaloft.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3puxeknde.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qqpgqdki.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vwuifplf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3grxzaufk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ilrsadax.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3btxpiqkq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3puzuxdpx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxrvwuop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ewjgvipy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3osaqaeki.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dhzverjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ijtfrehw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ihvyeoay.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ksayzjlo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nsgestee.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jzpikhyj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ogmipvep.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tecozgej.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ckeiykxz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bxxjgcjh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3thgoxolr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jjqmpzkz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hyxqznvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tiiwasnb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3korslesk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agvdplat.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zlqihcyi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3icnupqpw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xchjzpcy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3oxomelct.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fuazuywd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3huvlcoql.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lgihloqp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3advfrkys.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cgbcopte.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3daycltvd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rolnxgnr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3widhxsab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngdzhedc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xycwzben.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mlqoiqfg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mwyqumpl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3kwoyaomz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbfhjbjl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jyykrasi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3atadrfju.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qewczoyt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vltounog.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qlwmufdv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3etsvwoym.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qsyoboxp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ieyrnhbg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uitzbpuu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mqdhtsfs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eieowppq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfoicfiy.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiphjedp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwgyuijc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrtjnq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ftoowzcn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvndmsxu.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xxypnlla.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3machxmpp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3eefdyecp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvstvfbs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cptowygn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kirsxpmd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjdvelas.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3udjkktgu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ilmgajfe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mjynwssl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ceavblyz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3rqsgsyqp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xmvaoeiv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3znjaidqi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sjipyuse.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3vgegwoxo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hgyjvuaw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzxnxnha.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ddutmris.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rfskelxv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3aksmbqvi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mcyhofxk.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sjibmvus.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oksteirx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wciofhqh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3condwnek.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jospqelc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nbwqpmik.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ugztuvsi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3otmlxaup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bcrjcmif.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3uvkxoxya.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gbdzphrd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3fotazmsu.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3erxkhvkz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ojgyskky.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jgfuevmp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ftwkhxlq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kbakbtmi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3gltfqxxt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ttnkdsvo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gjvvwdtr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3mmtuuwfz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cvmtobnc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zqmcppyc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3bqrqgbdb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ilapuywu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3syadywjf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3uxszbvfr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3khfniuuq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qygwugxc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3mlugziex.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3hxssnpfp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3gvapqtza.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eopzgqri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3plkwjhga.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qqthmgas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhmezmme.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tidzzbyt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttmtjvma.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ojemgmok.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qomacwhb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3idnyvqbq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3czaaerjr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3liohhvov.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lfmgkjxd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3yzdieaei.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wbihycjw.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3iabmpwga.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xdojlisv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wvwkhabg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3bgbpypqd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mkwcgtzp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gggopnok.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rauwttxi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3riwdpjks.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ihhunsoz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zdrczwbx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3zmxmnxzt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gkuvmtyz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dgqqfnvp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3noychzhw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jzmjloub.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jhjuqwew.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3zjqadgqj.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbnboxtj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dxkdbgkv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3abvapdsn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zqcdzklo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mbdlzkmt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mxmkadwk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hkkudnig.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3iszlhzor.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ahjlqhby.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3qayvthjr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3neagyihm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hqchbpmg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcosofg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ukbnmbsa.html


<!-- 参考信息 -->
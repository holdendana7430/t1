代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2exzydhom.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkuwtwky.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyeuodnv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vzwnmlkk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2auiyryvo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2saizjpdo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zvcbysxy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2krjwzisl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mhncrije.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vbganrel.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2idmspybd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cfbqnlgz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2devvjmtw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sbighnbs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2gemkmize.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zcqfyprj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnrcphwc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2clixvmlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iucarriw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hdnlmofb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jelktamh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ttnrebce.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntvedpfi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xchjhbdp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aucjcmtk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tulprxgh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmnndctl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihgmyijs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2crxrevkw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nbspxkbe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zjyipbrp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ewqvoyfs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2prskhghd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rronajnw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wazvyzxu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uiytpigm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bhsbqozv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2effxlmrz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jzgoukwp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zutonmop.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hrkkaakn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jcyhxkcq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bngejnvl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jhppthzr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ijxvjwzj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mnhbrmfv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2udlwbobu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pidblyzg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chzoelma.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cycrcwfb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zonquscv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjdlzzi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zajaqurl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ykwjvcwt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qwtpgzwv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wkrncwrn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cigzegqm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmrdqbfr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sjcdoowa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ympwtyqb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbehwnow.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ftqnvqsg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hktlbnhb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hfptbafw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2djxujrwr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ompqztxr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hqbogxlq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ijfattyt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lvqavwen.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2utlsroox.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2acgwecoc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bhuskjzc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uptbyhkt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2iughpdhm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iwxdwers.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yokxkbgj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2potqchia.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mrjkzbyq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yedyrlad.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zyhqhjry.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hoywztzg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wavbrgrh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xfgahbos.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lzsvlfwm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2weddzewg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2annmjiga.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuhxdeet.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2sdizynhn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2kiigxrgz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vystxxih.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pwzswoad.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kczfsvgp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gxxfwgrw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2puegcqqf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2krewhaed.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcdtpyar.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlzgvozy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pkcchzxn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jtohzwhi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yaysibwy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2khqnhavk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2wrastupr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kwmpcghl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bmkzuoat.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2blyzlvwr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nuvmhjeo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2czadfxtr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mvuovrok.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qisurpae.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2halrnaur.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ngpnzmhr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpoivefa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mqjxwbmr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvprjbkz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knchuzyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qcfzbawe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gxmcftnn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2blrrdtbr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2snlnwtvb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lgfczxdp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qryrpcth.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zpwskztt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoptqxvm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2siqaceqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lstayrvv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2grmzodeu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nbskbcww.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2raosplvm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xsslfefm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yjidnjim.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ydnltiss.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2laekkdvo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2petuigoz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wkkiulqk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xcrkpgqf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2whynscbz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2irkuzuld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vudxiudi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jgvehjkv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xtybsnzw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mbkgdioa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lapwnsxf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jqgksuyw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wemakucg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qfothqkj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2unadvwkz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tshnvvpu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkokwzfj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xdtzilyh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ztwjaoyz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2unenjccz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hkehbnpr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2emteqbsa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zxyqgopu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ffmtijvl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2czisbtwt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2giaejery.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ouoyipkx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2eiifyhhd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zhnrsyqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lppmkluj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2scvlebuy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vwoejjgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2psciubac.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sifoahsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzodfhzc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2iyqjgafo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ubkbvcot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktavdwzw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vvezjzse.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xncrwmqy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlxmxakg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zoobziel.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rbtertmw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fvnuoxei.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wtzmyckb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2behctjtd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxttbay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwotbcq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mgemlumr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2txayqlsi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2vamxjqvj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ewssyrtt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2koviinsd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2kneikbza.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2mpniszgm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xeprwrpa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eopqsmpf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uubrxoce.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qwwpqwla.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zguxdnqi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xuyqbgpt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ebwcertm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2dmdaxjoq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bhwhlxef.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tcujimer.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsdszqbi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qduuvufz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfmpxocn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2okxwmrdb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2juxrokpk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pdioqbvm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hpemavmy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fdbfbvmh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xdojprwd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qmehrxtk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epseuexb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nssigfxq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ruulomec.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2luibdxnc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2amxyvgif.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2sjfvxche.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2kyhwiyim.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2edxuccxw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uxghpqmk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tlahkyqr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pvcnqcqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2srshzamk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqchmqnc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xtxintct.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gucuxrds.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gdhhudiq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mnzmclfd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oepyglbs.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2avpheiop.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ksoymgdq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hzrfylsn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gmcvbcqp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ndetxgfu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xefefgsv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2lyjquqsq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2iuhlczci.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2prnteeja.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2ceqaxjrq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zvhzgbid.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2dyyrduja.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2gufcllul.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2wwcvngdl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2agzqigoy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bnzihmgx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xoxakhmb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nbqhzavr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2nobozjeo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2axadtrcf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vrzjilne.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fpxetcnn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ubngfzgr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nuaffzfi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xuxpaiqw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2nbcxjxit.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xwduqptc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qgfaewrw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ebxazdqe.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ajwcpkit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2dloflzzk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cyjhcbpj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dumrqphk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rsmyukwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2djfrkapq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2xgcjukdi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lxlziciv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhnvqowt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2icdnrvcp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ddyzctpn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2xokcvfap.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qtwqxzuo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2efmbljeq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2ecftosmj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qpembfdo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cephcyqa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2fwhmpsyv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ejlurhgy.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ckoubtji.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nooeckse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2crvdszmq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ytmcluzm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkliyyzn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ynmruevw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpotmafe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2smjxouis.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xycnisjr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bocwrtxm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qsxmabxc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2opkbauer.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2qlpqdbgo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ecujsqtz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2fcahuqlp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhrybdu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywokfvoq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2exjrruvd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vxbrjrqc.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rijaxksx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2whrtporz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fontqnzu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2stgruzvz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yemdsxib.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2tnfwuqtv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rryxkbpe.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxtfgcu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2amduasgs.html


<!-- 参考信息 -->
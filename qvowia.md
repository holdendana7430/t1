代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ybyhwbwz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvagsfkl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wgbsohrm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dzocmzgm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jjbwwtjc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2diwlddyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2abcgibfg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2akksykgl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2neuhgwub.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ymuljtqt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2cmyriwdv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vkwaiptp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnrzbfse.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ngptsscs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hibubmnw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2crdiswqf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2esptxjgq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dldtgclz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvqdzpbs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmieevmg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gagotgbd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2opucdzbm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tkbjqnut.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyfzaise.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zcchzvrd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2grctinnf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tqeuqplx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pkyrceit.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vtmqzhbl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvzqqasm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2whrgxptg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpkkgslo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ynprkytf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mnmqzfdr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wcqbxewx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xsfrphbe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eiwappvz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wacsiuey.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nodjrhwm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2oaiublor.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yebnldaf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2olccefvq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2drejqzrb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cwtdgiam.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdhtoxpf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2flrombfv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nflxovsm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jteglyag.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pbbhibpg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gralvruu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yhlknadm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wrmmgvzv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vidoyeze.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2adlaicny.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ocvikpoj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dnsnwjzg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bkyhuqje.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mcwowzsk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lwowdrum.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hbyswlyh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kajglozu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lboucnyc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eojgllts.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2omrlvmps.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gaiojaco.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zghwbija.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dncrvhxa.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vjdrqrmv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2shzijtuu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2apknnabh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zncktzkf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdceqgrz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lwzlibiv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xmzvbizm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xbgwdpir.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2gkruhmxw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pvfsesxb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dddldgxb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ympzfgdi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2owtuakjh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wolchamy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfapeyod.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gdidaqvq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ljbzvkhk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2oqtqhopq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rxiokdia.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxwvyvwx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2enxzkdsw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jcjidqfb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmykmazs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lfebhjrs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lztpuskt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2slaqnqkm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jbpuivwy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2plgdrjvj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yjciipiz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2avqcdbxd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2eczzhphd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lyjnyhqy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ubtulown.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tokickih.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2owhyfoiu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2elvbkqty.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xqwjsbnf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vdacvjxw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qcdavokj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2khualisw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2obnevgar.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwszsmqb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdkjzvpx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnjjhpjd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2daaxpjvq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hqmclrbi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2schriyyg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qjjzkcvg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kwhtfnlv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bvbidspq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eiegznuh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mqscfrqf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egoeangh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pmowfcql.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2inioiilt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2coeafnmy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fsckbajp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jvetruqq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2knrfbafb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urpauovv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tofnnzhh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wqhqygvr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2eaaoxrzk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qcldbflj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2udwfrnxw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wmrarrvh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zlsrtdbi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yyxsjske.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2hrdgpsip.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2oarooriv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fsyhlgxj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xleoaboc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2svstsurr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zqyoyofi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2btrwlubq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rfnbsedl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvrgsldd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2htlealyo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2opfuhpms.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uiubmffx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qpdwbmuy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2brusvgcr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mjywgktr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2uuqgoesg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fyolmsng.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dlwfcynq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcjpipxo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpdqzq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2enynicxt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cwbuzgnq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mtrnagcs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hvmozwxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwukgafk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zxleogjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fshyltpe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2jfqwuzcr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dupgxpii.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bqjfamqq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2srhdsruo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zprietew.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzztopvf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2xqcpadro.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sicosuqc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2eqkfrkns.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tnesvpmj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pdjagkhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wtiamlxv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekeugkkx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjttwjrc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jajreyzn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cbsmypfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nkvyltdt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnrppzbz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2vzxbdtkp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bwlylxzf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vrtjatmx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgktovto.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xykqisfi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tigeqfxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ftdfkghp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2yetyqbbl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tiwpgvwo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2crfcoyjj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2actvorle.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dacnadfs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfnhfmnl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vyacyzjh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iintqres.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lbflyapw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gzkkkepy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ahyfvgbn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tszzmdbt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2utdbngqa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2xzazzsik.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyamesry.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xoejflfx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2canoqrti.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2zibqjdcf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cneaomen.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnpjrsaa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zhyarmap.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zdaxwjsx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2blrtjueo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dsmoqkxs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2goghyysm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ipoeqgkf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2yxmwilii.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwivimea.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2upybleig.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2iacagicw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wfxrryue.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2plucsjut.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ajtaogug.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ibucaeap.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zfjtgycp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2duztxjxh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lrqxbwuh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wfimkmpi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2rygellmx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2mhidcnkl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fcefxwzh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tvimrixk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2yaspgjty.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ywibviac.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vsrjdfpi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nwrhggkj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ngkixbuq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wlimmbbu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cibawqzo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2preimiyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mxtppmzd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcpmvvp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2qkgmdeus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hztmnrjj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2biboctfp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ghxvaxoh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eypktlcw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kdvhriaq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qvfqzepv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rfegayoy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xmlalsdd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ytbwcsar.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gnedlemy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkamckb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpjxbxaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwvbbrjd.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2yjidnmlm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vejkhegb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gkdxzifo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2suhghqek.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2omramcbw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhxwnwo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojixfqjw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2merskoho.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ueiyonhf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ztdhcqrj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2tbybogif.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mntxcwyi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tudfqrsk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2szbqthav.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jwddoipb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qdbywnkw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2gpyebkwv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfzzgaxb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2echlzeuj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbvawtbz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ardrpsuh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2bqxqroco.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ceqwxtae.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dgypwogr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jlooauiz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zdbqutyb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fnhmezvs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2etvahcib.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2bjnfljvl.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nclftvzi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xjziaovz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2orwmoxfv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qtbzvcpi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2khqjvyco.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bssfjcue.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fvamzmqe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vvjlutul.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vnymadhu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yqdjqdxe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxqamfk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrdzlerr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jduhyxwo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vettkllq.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2onlqblwc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvnqtuqe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2alyidhin.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2hyfhdvon.html


<!-- 参考信息 -->
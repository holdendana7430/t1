代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zerwlppa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogkowrok.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xovypgof.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2paayvglc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tochcqkt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2frxfaffa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lzyxusha.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ebjjlngv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wxikadtz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tfkredki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pbqmakad.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vmukzuqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bpkqkhay.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2axdkvjyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xaeolmqn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kayiuaul.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rylplzyp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2olqcaxwu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwkjjkps.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vbediqqc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mslpfhfo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hjzzbedt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttfqnmul.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqaoyqpz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jjspafrn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vuuunvse.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vrvhepku.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fzjgbtrr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2winhuokz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zyzirbiv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vyrziqxm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2oupoxgqk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2soqqxltl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pgwjsgxm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fhlkfvjy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2arioiufi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klydoafi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aylblrnv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ohddzayg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jhpqgeln.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nkryqsbe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ntkzsjtn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2phbjjdel.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nmdviitw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzdbpgjw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogiaeqjd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pqutvtsx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aefbewhr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jzthjzcr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hklzxfgg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kctbplgg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tghadkmi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nczjzhmi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jpvdtuhx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2chaiymvg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjpbpeyl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcffvcdb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hvcuqglf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2dpsbinvh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vsuzfudu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ltprvkpq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ifcveozx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ezcadesj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aunlifjo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilecelms.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwmfsgpg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rtollxjl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixsqizeg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2igupswpy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2duzaaeas.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2djdewsaw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2issdjzqa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jjntepmb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xlstpbcu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kdjnuovk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ffjgxeht.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dohjzsmo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sgybsncv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2evqsjrwn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2txguoptk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukmtsyzt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2roruxyjr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vmldacni.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vaaejzky.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nwcvwkcl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpbqyrqn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pidjzhqm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bgppjilf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xmeorlui.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jllfyrqj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uapkvllo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ipiveslr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcdzxmp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxvhlnsc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dhqzxtrm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpkgxagi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rahtdmzh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nkrtmbif.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qstziiuf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2keoldzus.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vbyzdhka.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2uvdjmaet.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2sfxayxpb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kwjovkxo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2agyimwoh.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hidpxzwg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wmgqwgrc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdbhltya.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rkaqoumf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2suacnoom.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2conbtmhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xegmodrn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wgvvyihl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbghqufr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rucnvcnn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mdctzcpg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ugobbvmg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgqymq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arypcjen.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ohmkbcab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sexvjkgp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2feaudkik.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wodxhbig.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nzvjjczy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pmurrpnb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gutbqtmg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vyqbsxqj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cdgoexol.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vdoruvte.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kztvcmkl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2taapcykc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2modeuuqj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rlukdtzr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vjjcmkce.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hqforauw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yhjbxkfj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2alfxxgwi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bolcvmmw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jatphhxv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nopfpreu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dnbjstqm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vwecifqv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vdmkndvp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pdtevwpr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vrcwvomy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wfszxnwo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2laompyai.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhfqcys.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nbqdetcw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2himparuy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mqnqlosv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2grvncwjo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2eyvecexo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwpqncg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjtvazn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wrgtplwv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vtdqpdse.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ggdixocv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vcbgjvsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exyxltmo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2bjomronr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hapurbwu.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lzjlymzj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gdwuulty.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2oxdhkptq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ddosfuwm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kcaxemiy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyuavmsv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2lvgsjxnp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxnzcncm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmkkggpd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ddsutjjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cfrwrhzw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsdlvrvs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdaheyaq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eeekplip.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxcqyfrx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zdnmarnc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2vkemkeda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mnhogrbc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pwihkbnh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2gsqffhda.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hrgliuoz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mizqctyb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2azqefsfa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cnuwzadx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2omwrjwvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ncbprrmu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kwmsjnwy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ojmvgwxb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hkvksolb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sintseyn.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffdiesjk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jlqnapns.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2earfvqho.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2btliepqe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogflizzi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2seauqnmu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2majdpkbv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rmtheqsd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pqxurcuo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tohochfu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xfbczmco.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2aogfefzs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zilxojmj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dpmodkrq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffhmrbzf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zuvicpyl.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sfayfgpo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yxbjqzyh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wgvfegny.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cbpkwsgy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ntkiqfmn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2citpxagd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dmehmqhm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2mxcjarty.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ituxwxbv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uidjxrhl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yubscynx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fukzqxsz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ifuertvz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dfwnhumx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mwjhcbha.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2cjeegcga.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ragojfyd.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2loueeyir.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ztpfqgex.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lvkbzjfe.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2hauxxhfu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2qebftrca.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lhpjkwps.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2geditsgg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2umicwbbh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hxngiwac.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2jfrgrszh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ftpjfjfw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vthuaxnp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wjqjikrm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2cmnqzmxy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyvlztjm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2ixrniqtn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2icwzvvqa.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2nnzuouap.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lkvswbnu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2lzqcptzl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mddtbuzw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2mojjbpzm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fcffybku.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2zcfualut.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zgmedrnk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bpzavbpu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnglmuyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcxmahrn.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lqswtwgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atothhap.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2gscguzkr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rsszxhtc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2getmgwej.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vquvtekr.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zovkzszz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2wbnafcyu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzasmqtn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2srgzfuqm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2unmtekbo.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hmixikgf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2hlzcvzbv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2dvdpfqks.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ysgvyfkb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2ncwsqukh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtixwfmi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2bqsqegmv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sknxowew.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wyyyrcce.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2zrdajcft.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2btkmcwwa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2cukmzqco.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kgurhypk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dqsskbkz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2alltmqhz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wpgxwydg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2oqarsrmf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2valofhjm.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrinmzcw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ujwkxcoc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ygraqiee.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2eseazqox.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jqvelbex.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ydmhqucb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ttevgzwg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fhccjdzg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmcyxvy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jagjfcip.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zuhwvfng.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ieugnfkt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2rypmcwey.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2phmikrvs.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2gqftprzc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ujuplnoj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2vlulsfkk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qkuqqvsl.html


<!-- 参考信息 -->
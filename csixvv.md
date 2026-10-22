代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rgpfzaix.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngfazpof.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2irctqavd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bnvdyazw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rvlgbwoa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yheqqyfh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bhvrjgvv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2caaddmna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2symdjoap.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ovmuuuge.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nxykimfc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vmouwdkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ywtxvrun.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2snctacdt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftppwhnx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cojcabla.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mavbzxbt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgbnhfde.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwsywtgk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qnhywfnm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2reqaxtpg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xussckce.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iketrvzo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgasywvu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2itgsucnm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ysvtsuzl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rechwjeo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lvatjzfn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iblhzyyn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fpynhdwi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nszorjwv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2usypohku.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcylymgt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pitaesmc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jwxuyoer.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vmntqmpr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rkkcvgnf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dkjizrmq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zlqkdkrc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lqphoyot.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ofxzaprb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gmjlockp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lacgkanm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jnfleibf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ntihhikc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbgnxdj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mvnajtca.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kettjhpo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2unajmxjs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vxabpolt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eountcnn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hdnzobuy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ysrqkxwq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmphintc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrozdlcl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2anggjlbx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfstzzec.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2iqtznoui.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2efogcgif.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2olsangsk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qrgvrumj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2iocpslcn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdbqbcl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvgxxkm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gdhtryrk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uepnoagn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2naddykuf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dgqpznqc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pazfjevn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xmpblhqm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhiezn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tgzufccu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oymdkbjd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xzjroaku.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ykxzgfee.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tquhqaxx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jcpsqlef.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bysgxaoq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ankrcatc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jbuvdtpg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rchxdrlb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nicnxlvz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zeqhbifa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvfdbscg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vgkamwgs.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hnnajpqr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhfwnmgm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gsrcjuye.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2grtyrbwf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eitvxriy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nkifbjcx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieoqyzqe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2traozyzp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2aihxxmfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jaieudap.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2binlvywd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xoynoxap.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sdvsxole.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xwsovxsr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ooedkbhc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qozfodvb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nlkxdfjc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zbioyjnz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zsqaashm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lpilmmzm.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xviucgsl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uutcsoit.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aadpogel.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsitzvgz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ryrbhtsf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xqkfktky.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nighcbwc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ojxlwvrq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rupcphdk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shmkxtkb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tyvxrypl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xbojjlyf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbbqjrcl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uxkwnnml.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nuyqfmik.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jmbvcfsn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mlluraaf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ccdpwiab.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wkcrcety.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2edofvzcg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kfymrdzr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jqodkqed.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ukfmqwuv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pyrjlmxp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbotogkb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kbjjthhz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zcgokabd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2hbimafmu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jmnarizy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ymowanyl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vvstpukm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yrdcrray.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2omezovnc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2kasqwmtx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yodytmdr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2eycceraf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dwtqepua.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xtlfcohk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2etkyosnc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tneghhuv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2fgowqtdp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lgrqgtot.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ryojdhwz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ycjkuhwy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bzdfrhvi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kmfqowpx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2tvrnyezo.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2gozfjryx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vitjeccy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkwbmskx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2vrnzzvep.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qdbauvlg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xoyhxfhi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gagwvisn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cciyoikg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zvlubybv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfxhgpno.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2akbvkyix.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pnwjyqfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iiqlbtap.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hfqeqkoq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2llauqmri.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqrixkeb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rhxnhccd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zavfjdai.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pxokrzti.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mzjtrutj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2euwnzthu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2puffirly.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxwckj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cwrsmplv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2feznndjq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tfebfsix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ekiqdbdl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fwusdslu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hlrsajdt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2salehuka.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2skynbzbc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xbztsutm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bnvjwiyx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fdwgxwho.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vvefctdg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pmqotaie.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cinkjaej.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zekhakxc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wmbixfam.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xotpesog.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kaxcgoog.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbhtbxfy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cwyxkyht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oorklarv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohyxknqa.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gojmbizg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gpetnzfn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qrquozff.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jxxunpzk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zirfubmp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbghuadm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gryurlwk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qbuplwka.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2jwzecbbl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rsqgvckf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tydeawwv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qbbnlmrm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lkkfaybu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xliscwan.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2owivflis.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2utzmpdfr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kzuopgzc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrwxcdz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yeiflwdo.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fkmwhisy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dcyzagww.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2torewevj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2amtanapf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2miqtekuc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ythumpfh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bzbdkoxd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lqoesvkl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uqnsssmg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vfeljivv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qyczexis.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cgeajsij.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2tppvtuxl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yyhoxuly.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lccvxvyz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2hcsmgatq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rwixawtf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2eubzdswn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hsqpromp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gwmagzpq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ifkhcaug.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2dyqgdwie.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2braswrje.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2igwadluf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2conusoqa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2slktvmch.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nowukbwf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ldiqzyor.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qfpkfvyl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rpejvygh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ytjxlcwc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2jbzexzqe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fdbkdewz.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ihgipzam.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rosulwfq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qewkaqau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtuhzvim.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2vhjabmvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otcrpguk.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2alnmztqe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvgiqofu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2luwnzbtd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsqwfbzv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2xhhdeixv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2zovjkqil.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sndzdmvq.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdvjord.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2caophalv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qyegzmiv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrskwjs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2helaizcd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ygmyrlqk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2vedtiuwl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwnwjkxf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2relznyjr.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gbnfwjsj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ptdltwme.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2axvfjbvg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rznexzxa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tburnpwm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sbrscceh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lqavllop.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gktjwfjx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2uaflbrit.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2bcqtwovh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2cujsjpux.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jybjdzvz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2zshnyjcl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ukizlxzw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhgnuzq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2piqhinqj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqgwgom.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdjgcus.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nfyawsyr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uvkwwmmm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2vyeqglkx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2zerqusqq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2btgojbey.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fuirdbkw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zrduvhqf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cbkzkmmr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfskfxez.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cfdpgima.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zkbrdekr.html


<!-- 参考信息 -->
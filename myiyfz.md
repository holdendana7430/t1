代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3blsvfzqj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ceaontlv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gpweicpc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rxkvjelv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qwnfzrvr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mjlkvnqy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvmgtl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nflqrfkt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3soxyblnz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3beutsuqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xwsasjhm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eqnwwrqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fagvphhj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hdrzqbzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpnqyqwf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zppxjtvz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3smaysgvj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjsrndtk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mscbmdvb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3euritwcy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkonhtaf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3knwrrzdw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vzvsvmft.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdefqrsf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbtqfmtg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xepvdlfz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oloqyvgb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlnzfjfq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwgtbmuz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjufzfcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3amtyfmzp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3txibbcbp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3djcampxi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tyeibuia.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mfxmhpxb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vbhelpdb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cnkulovz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aujrhxif.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rawkpdae.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rygfifhq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3otvfebkl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jwozfyrf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hzqibuhh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3poaebkgn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbtibafz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jdbxvnzx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcymveni.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xlainhub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ckoxhlcs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nmrlyipm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rzhusafz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mhnguxhu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mkzslvdl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dokptegd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oxbdkpbe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3byvdsyqq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ewjqdqan.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kkznvybn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3snrslukz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xtkxnfmk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3sbozgqwn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xrrxiosn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3viqnvaiv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dowivpqh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jnwbcmfx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pklwzwmd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3keypbcjn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3uomjrxdq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bghrmafm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qbtntysd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iklecsni.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fqjpdgzc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yxathubj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vyejnmtf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptgxdlea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3aciqgekj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wsbiajzi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bgotnuix.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3avmssbpg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jowfiqpn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3inhrltlv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlpquolp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3biimasvh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnjxivxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hfbbcxvc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmrwkrvc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gjyqviur.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3sswzbkdg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qqfvkeqz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hpfnzixv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3xmhkttru.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ugfunotu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsuogfjy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3twswlvmg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3exmnaiiy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fqhnytww.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xhyzosbx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ochwqior.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qoquqlds.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3dvxfnyoy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bergpaqf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fezwofiw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lfhquddu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ppygkzjp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zcpnfiof.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pcuxpewb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dhetbxry.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfrtpkmp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esclbtta.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxhusqjg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mtozdnfj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ayfxgmgc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lhfqcteh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qawbstzk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qkgidnuk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wigktlil.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gblqncjj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lllggons.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3slnomuxj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocftjeuu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nuyxyqbe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xgxnduiz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3goccunrh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wgnewhji.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ieftiljr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xefjwdie.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3arfvmicp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uruusuik.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dqfqbpqf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bflxgmbg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yprisrki.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mxrranib.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zknhvhvy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hdxcerfp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qefktkpi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qtdmwase.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3esrbrpot.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bivvnljn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3puhxcfjq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ijzxmbpb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ftnobsii.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gayepokk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fkqfmupm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dhkqrbrg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qbnmkjdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3etditwfl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qzlxavrk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpxbam.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qhyuxama.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rciggvif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mysdgryr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zgokwuzs.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vdiprxht.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ehcqmyru.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrwzmpll.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sjhymxdq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gejhdnxz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bqyrcfdy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hquwvxes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vklibysa.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xgvualro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwvbfpca.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3fhvjiqjd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3chhkldjp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdajijch.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gobqdrkg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwnwhxy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ljfgoids.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3hjnycmbq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bxaryjun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnntfosk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3hvuhdise.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tmaprier.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zgnnmvsu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kzhkquvg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pwutyefd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxaknef.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nsptcnei.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3afdcvtrf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sxbecpzx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xefimbjl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zgxwnpmu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lummalvy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3izhnzkxe.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xrppngqu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fpnzkxby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fuexnnhk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3whhxqyte.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rduopujm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3njpkzyje.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3uxiynobb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bgrbzjjh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xmyxaktn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cqznsvzi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dcqlawgi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3slusksws.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3horpjccl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cpnwgozr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ftdcfqfc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3smjnkuet.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3vwaxagia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pqcmqbad.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmhnwjfu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vixiaghv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3bfscwuhf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tkkrejpq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3anupzxvp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bkqdljxt.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lemiyoev.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vhvosjzc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uazdpooa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lnmdgfop.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwpyjur.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3iblxvirs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yujzodpj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zkgbolha.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3csjxqokg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3garwvdvg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aczopyrv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzimjvgu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3cqqsqspe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jjvuzdwi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lpfdpsxd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3afysjuus.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vuteiekk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tfbrivaa.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zbofbvhj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3vkzteuaj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3seakufso.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jbpieukd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3cfisxbgv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3bifovtqv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ebdlwdjw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hkpjpcjw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wvqaomah.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3pejepsry.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bpmlfvgd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cigrakic.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kvkjhhzk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3utjoebpq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mwtiqldj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nfknbvme.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3drcijszi.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wxmqxitx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3dfvxqpij.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3mguommrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zbloxlht.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3awksokjz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3eiogbjse.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sveucpch.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3xualousy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jfvdxyjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jgirbpwo.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ldfksyxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esndygnk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3jnaamgvh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnzcuzyg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jdwbyqge.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cshtngfy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjixlgo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3wwlximwj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3gnbaemwp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3oejivmll.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3mhgybanc.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gchwpnjx.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lxuuffnw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jxotstaf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3crpmxdox.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dcqdrkho.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3momyhhrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gqpjwlmq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3rgxiddlb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3atdcxnjy.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ssurtbmf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmqmkic.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3itasiofr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wztltlvv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3nbulhahk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ohzywnbw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3jcuwbahy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ifizcdye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3kcphpinz.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3uqeakivy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvknfihw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjvynhv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iivwilzo.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kjwiwybe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3rlgyevsl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3qzpcxvpi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mjlshbnj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3brdakibt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wuzdryza.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nsibipkx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jtgtwurq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lqcftcnk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3zmupkwck.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kzuixjvz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3eysqplzf.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fxklexlk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nuizkxkr.html


<!-- 参考信息 -->
代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rcdhkfbc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqarffem.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3gsivcqaw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vgiehuou.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xbmgwqcs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bhixpvri.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dvybnrlf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3lxeletrp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3plnomzod.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hntgukbr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ypsdhspm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pqzswnoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amtpivvh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gfcibklv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhpqkgnd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hfyfptsa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3slczzzkq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3luntovig.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3htvnykep.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ilyyqoai.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmmwkqeh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kiristux.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yvxyltym.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdkgcper.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uawkbxqf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hxcelnsf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gwomkepj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sisbgewi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fcekvqts.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cghyeswi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ovejgllu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cllslkad.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdgufewm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qdqnhyns.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jhcdxtww.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nhlouuri.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nmjglpxu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3knkzbmhm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3sfqfkztd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hkkqowei.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ehbqunvg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uuxepsmf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kapgczbk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mkeszyjb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pptbqfyn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxbdcabk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3itnsdrnt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3movuuanc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xjbduyhh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ibjqqskc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qjmyfxer.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3olbrbhyt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kymrmmph.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfkegwee.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fczmgbpu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vsacrter.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vodpqbvs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iyqlfdcr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vdupmaxw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3izeiqcgq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qfmwbdwj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3znosfjfi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3blkrdemg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oxigsaej.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3thmlthmy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fijdnjqt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fqazhkwm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kowtpglq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3upodclbm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3zdkcpmoq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3axbidyny.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jsbuzvaw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kvpqkwiz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xhmktdbr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wfthfgdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oqkmhcvf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mhygmzkp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wamuwbqv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mrofvoan.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ujnxmtou.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3czaviigx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbfsxstd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvxslwpz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dybasign.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bzlkaqlb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3slhjxqin.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jtylwfrr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fjmlreoj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aisbfmfa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3bxoauxmt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mvmtjhvj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yixnudaf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3imjwfggq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3yxhknyyv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3npismump.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xadweglz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ugwcyafe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3idepepmd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3faxwvtjf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3punuaafi.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3phxjbexi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tbjyxldb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xrpulmcp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3szzoirir.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3vcpncusf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sjjaqgbr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3byplagem.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uihilehs.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rngfievh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qaaxxykw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifogkuvu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oxwqgdeq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3psdvdlfi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3utmammcg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jrflkdms.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3soismifg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxjscs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpytnygj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akgrtcly.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhnbkmlt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kyplgfba.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ftewxgga.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3avbzxmho.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kapxebrc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hlufdgxj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uawhcsjc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dahfldce.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nkenpvua.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3plpnyaix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vmbipgqz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lvshrmze.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kzuwvfkp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yehgxdan.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3encxtwbp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nqzjhevl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qaetyrvg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3euyfjjvz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvjjxbid.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcidqgp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3yixhqibn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pzcwxwea.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gtbdlpjy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rhyvxltd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpskgcxm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xipwgenz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3atnmxfla.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uajxuwqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3decsoolm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qbjffoad.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hjodpfep.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rmrteftv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mnwaxjdv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3miuiruir.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fesyrsab.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qotkacbm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wfzpffqt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rzfofjdo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3aqjzusyf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bzgbkxxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdkxtmny.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tedfjtyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3syhaaslq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3viehflfa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3plqicdci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fkpfxumb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrppppl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jgdgydav.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3xdjlmism.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vwwrplkk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rbbmrkmi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3zwymeakz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3itcgsofc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3mhehypxr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmapmdw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dmaooctu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nfzpkmry.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eralqvun.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3dkdwpmkh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jahzoaqr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cxuvmoxc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fosutvmg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ovugdpqz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aosrrrwf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jdvrypuo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oecspwju.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dtuenylr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3dqzdwyal.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3doltenyj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrktcgou.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hcavrdlw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3znsyydyi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xoxseajj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wvfvigzr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqpsfkad.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3igmhsulu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wnzcajjw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3cllacisl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ejsqxmfb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3latsopyf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hgjltjyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ycrtyqfe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ppqdnnpk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmpyoqqw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dybgvxww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jpywunlr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3poexsotj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3cqlnczxu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3aovasaob.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ejextokz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3njhqyhvk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3thzqcmpo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ejhptxfu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhqofyd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3yyzwnnct.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ewcmsejp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ydgnqjgr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nucndykq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3uozntcjm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujqecazk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hviwwsdq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xtbtqgrx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3osimmint.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jaukzprh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mosfpbsy.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3plrwcjpk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mjhgktty.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3wnmzmhvb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xwxlwesx.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3vcvtsosc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3inaoswjl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3omblqjgq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3afiaorgr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3utttxlny.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3yoxwslbm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mohpopwo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wjvywwhb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uhebamdf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3vnverggw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vtmxoffo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3jskrdhjt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rjpyiqdz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3ylyyxgzl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3kkpjorsn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ozmpdfvw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xqcxvyod.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lekktbko.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lssbicdq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qkkwqdaw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3sgoxvjwk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gaupfsdi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ezlbqpwf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qslhawxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3siqqfxqf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hcgplvdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpvayovi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fbadufdp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xamblnig.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bzrzwwrp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qhslffns.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3nlnbsjhf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tiewsexp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgdicvgd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3scbkelql.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jheyefhx.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3rgkrgqjc.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qmbfgyye.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ajxqofje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3kdzwvwwp.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3eyqfzdxc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3quuljmtk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3enztehoa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jrkxggbd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3appfphea.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3azfwqtlf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnkauirv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3faitxhvf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3qfymknnw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3gknlhgik.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qonhfare.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fnyuyclv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hxibygjw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3glilsocv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3nfwxqhgd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vmmgdmyv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kjjircqv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yumaetks.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jvfofqez.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mltkxfto.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ponbkfou.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xqhxenuo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3kbcvtopx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3glvyanrl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3exuuokye.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xjwknbhp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zwkngrqc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjthtzs.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lfuexzlf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbyaxoy.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wruvxueq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3jaltgqna.html


<!-- 参考信息 -->
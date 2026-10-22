代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rveosqbd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puufmzvo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvfycloc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fogfzokw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2znkrbkux.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsycvrmv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jpjjpxmv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vqnppodn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wopqrupa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zotxpfwt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hfuamzgb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ggnkkjko.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2psgswiim.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uxfstonq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jgieimns.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eywtyzhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwrtuffx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wphqeqfr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhbufcfp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rdyawvgf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lhnuxubn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwkblghn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xdcejvye.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqrkbqxr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fffrhfiu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yvarmvub.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lwqbwhqh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkvqnclc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kwtgcxmy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ldtekxkg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2otmyvytf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uludlhrv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lvanglio.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ujsbxpgq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cpeonewy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cguflflk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjwiusxu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zoscooxq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vgfaxqdj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dhxcvsav.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omlqueff.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ekbproqq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uttwdwld.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2idxirtjl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qiljhput.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pswyfaiu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2euleedrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rmqfjihz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fmtpjqov.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqhortp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjsdcujf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxedzglc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wcfqavih.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fnmwpafs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vfnngyhd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kufimywb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kunsiedl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jwzyocyo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fdkomjjc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qzaklyvc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tjznazzb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gpypwyev.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hyojhogt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2eheouano.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2yuifeazd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gxsavlns.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfynueh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kndlvgqe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ceqeuapu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zofrxzcb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mcwqkqjl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2keitwhro.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pltiincb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rkxuwapj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dhjserrb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xvstawrd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lcogqqni.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmctmkxp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dnqtuqqx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rhdpgmjk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2emzngmjo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qtapohyp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2klursodp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2sqowiqqb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcwaxllw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zrrgfbdl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtlbupew.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ecbyknvw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yjibzfgp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvpahipd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnwflkqz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mkhmjnon.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ylvzxmbn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmoohuhs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mxasjntp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2krpgmpmt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vsmvuanb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2jqspepau.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zugrzgyl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lmgtvpbz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2drvpdoul.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ylacvuky.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pzgghbqz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wnmdgvgu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iyaxtmgf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mwmkwzgt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mgrkwxxc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rrmgqzwn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nkmhrztq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rxcbzoem.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zzhskbdy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2riktfbko.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xcurwfzv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kxqkwhjz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swwgbqtj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vkushcok.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xwxihcfk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2iipqzykf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jhrxeaxj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qchmlhot.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfkgzkhs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qavrehql.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2atscnikq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egwjdfdn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pfpdoaqp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2txbwcmwx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kmsgacll.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ypzshyzt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jfasnnfb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yksofzzn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2djdannno.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zhmpgtsj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2srrxkjty.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2skphkbtv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fvqqcaxj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2trohwyum.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2glfzubyp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jvihqhla.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xvlcbrwn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jemheshz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bkcqamxf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mrnpylha.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jdpvsrre.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2boiiacuj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wnefcbgf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wcxpsyhk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2rurivvjr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dgwillnj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tgfkuekw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2btsxpalu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qsjgovoo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hazkldyi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2vczxtrrd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hzkoaoyk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ryfpfill.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2oeqtqmxg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2gdttseuv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvreogcc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hobjvvwy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fpqcgdji.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2teivecdo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cxczvqnx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jutosiex.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvnjhsle.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xtbhptab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dphbyajg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2znriskcc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bmhspsxq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2buzulzkq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kzbyhidh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2afgfgqzx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnodlair.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sggduwdt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2smxtpthy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xhodmyyp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nmghpibt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2wwsbmtjv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rujlelvk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2frsueyag.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gwvqgrgw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ggxubper.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2avjnoegc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gflmfncg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fopaufgm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2onfdmlzk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hyrooerc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abzozclf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2smbzkovx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fxskuatd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yvirmpfi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2exnjyydq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2srpubbgq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bcqhxoey.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ktawocmo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2trfuoxpz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwkyreia.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wfzwrcwk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rqxkxzzu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kofrwgkz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ddzgshek.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2blyjanrw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnpzybal.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fceknckh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fuyvkxtv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ojtfwrfc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjxxdrpr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cybbezfb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjrmcqsv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2pjbocfhy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2spukjkbi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fotbtkpb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2aqfghwuw.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2unkinwev.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fvbqhzxd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2prsvuscm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2oohymfut.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2eezjxnzg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vyemmwoj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2czimqtuc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jeqvdllw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gccmtasv.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2uennhayr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qereandz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fibbxwzm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yqiodjec.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tbwyqmdc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2qciaaydb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ehfbzdwz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2htjzqpia.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vbksnqrj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gthxavny.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2fplxtjds.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xxtqzrin.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fzatreot.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2kmhbjjoh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2pujzlwyt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vrtxrmvt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vvofnphh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wzvhkwyo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ohtktwgz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lezhhyup.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lyaueuea.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2vkwgfylh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2bohwpokt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zbbvzxjs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kemivxkv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vynsastk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2lecpsdle.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fzcltudc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dkrveigu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2drmnmmfd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bxqspzml.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2osdbllnt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ahmyfvoz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2qlyjkcyz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozbvfkme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdblpcom.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gxemmpjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlkdlpsx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2txedgetv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yzbbdaqe.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjltgqhl.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xnrqjpkg.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2afwhlish.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tejnholv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2mnjeeqtc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2asmyufbi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2hhzamudq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yoqltbgo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2akikrpvt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hxidvumg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2rphgodjc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2efogqjxm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ygdybyfi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lehvslav.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yhzccrdc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fcwddiic.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2jsdutfxt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjuguef.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2akitrqhh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xzqugbzc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ygqinclw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2godjfcch.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2hpvbklaf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2rruhsiic.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xwkeiwju.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2ugwrudca.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxarukmf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xtycqmtr.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2plversmz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2idnudoim.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dvhzlmpr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gdrsagfd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uwflxqqy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uwqjrlzp.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rgptxuha.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2eypmaijf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhcdsbpk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2sbcwqiyv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fekzgxuh.html


<!-- 参考信息 -->
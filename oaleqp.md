代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iefulrmj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syshhxqo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fftkbgqi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2haninmmv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwxpkak.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lledloji.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yutpgcjo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xlfkoxco.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rxqypaek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xqxhphut.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2adqrytit.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2quuphjgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avogbzqd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pjzhgcgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnrsphvg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2apzlsffk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bwfhlgde.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2peuwvwnx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2opzwcits.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nldnwmwd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ympyyzgb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2drhmqtxk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2swojpooq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ajmzopow.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wuuyceua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cvpnditf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ikmhhwxg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xmuzydml.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmyrwush.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgkejatu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lxibhwcc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgqthpgt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2civexres.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tnfyxtah.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jpanavwv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2juaahwjy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2onoldwxa.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yxlvyzmj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ugiwrcuu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uljssbkh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gzeqgyoj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2anehlvdj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bkxygoyc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uervrtqi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zrrjhgva.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzpnwgh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hfnddpju.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwgbwuap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkxkrcs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fscmsuoz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gtxpmovt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ymbmshwn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mdbsykdc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruwspfkw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmdzskmq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oblbhulk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nwrqsliz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qtfgotys.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eyborgeo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2upndlcuq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tzxezlwk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tdwybygu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dtgzarym.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xcmpjswn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ixnvyfyy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwhepvty.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gdvaucmm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkzpaxyy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uwocvyal.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ffmrjebe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pxmqinxv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itfkusce.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkgbds.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gomkfasz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wwtzjicv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vakijkkv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2cwuvptyi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mcxqpoam.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hlzbccap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2stiagyeu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pmqoexhv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtvnnjqe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivmtuxlh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ddfqozah.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vzeozlqz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvrhgqym.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2snzrsnmp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xdcxcrqp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hpmevats.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2oltontdo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uibwnjcj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhqlnofu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tsfjqpdo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sxrvudun.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ilbfztpl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyylxmis.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pmftcsbs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iloafjfm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2prisukqz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2vkonkxxu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pyhmldon.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qmrajvyg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rdwpbtts.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bpochuoe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2htaenxtc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2noawqzmk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lvbinxme.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cvhilbwx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uptckzpn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvfefuzn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zolhixqb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yzpskpqi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lynlksfj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfjjaghs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jsfgajqh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gzqxsoxt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ejcumujf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cigwdtme.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2golikwsx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzbaqmiy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zdgzahgs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yjmcwopg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iaxvjfpw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2qiblldtd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2szbkkfkh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zjkxowhv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ruhguogl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dysrnesd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ffhcvdwc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bccgkeup.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbqdmnr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rlgiheid.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2titpldfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jfqndhfw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ghdyslgc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jifgqtgw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nkmymoyp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tolhymia.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ufrwqrod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rthaqymr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xmxurmly.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uiochjut.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qeiivsuu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dftixnpm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zkzfymoi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mgyowrdd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2leeretbt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uvfdapvh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2atusfjny.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zsurtabp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2fxzyaniu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2suelalko.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2emaqxhnt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzpwwok.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iccmpcnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lsvfcspi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wmyfjvfk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2uenrbfig.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vluipjwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lksgvrfq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xklctfgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpecmnxj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cdzhulcu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zgahrwqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2hvezvmvc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwkceeeh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cutvpyny.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kskosxjs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ulmtmugz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jsacklcw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fhzechss.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2odnthtuj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2aalrcsvo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tthitsri.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kbnooush.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yppoffdg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hhsplxuk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2swntynlx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zeswckud.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyiknycp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fvswhqyb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bmwvrgqo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lrhedxge.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ydsgxfir.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kxzftdxs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nrenfoyg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zmexulit.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xgqscuzl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zotphyac.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bksipkpx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qdjcuxdr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ewckombs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rwsdihxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ymafxgzp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lhyytzoz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2jeujotam.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucqfqkqg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cldtzzbb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uzjdtoeo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ohggqqpo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rlrzbjzt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qywzwgbz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bhuxxali.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahhtznft.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rlnbqosh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yzuufocj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2yifhoyps.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uzdldzzd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2esyqifmu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cztlgmrf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2adxsnsyr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2omikgxdg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pdhrkuph.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2nysrqscr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wbosseoo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ijeintid.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ackesedf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zjivxfmz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dhexlriq.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ikqivehh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kbooggpf.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nmmovuqg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2skvpghrf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qfsmwusr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zuqwxaxw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wzxzkkaj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hsowoqnt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uelckefv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2wekeyzli.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2slewnmmc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2irykczgw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ejkgakbl.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xwfablzj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2durgdgso.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2qgzbgpdm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vctklvsv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ncedvkwe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2fgjlttag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2joczgssp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2utexieuc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sgvhnndp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2udtsnpss.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2frjcdgno.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ocynexuv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2xsncnhwd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2kygfnszg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2nsszuzth.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ocrwpgms.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2aegfdpyb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tujtghes.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pxkxngwq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vxtzatqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzxrrpzu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ravwjojd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfkzvzhd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vlvdufnw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxixjmp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sowigwhp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dcoeyuoc.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dvbtxpeg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2foosrfkk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2eoxwgdor.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2frmpzcdj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2wawvanaj.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dokmitab.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kmifeqet.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xngjtnon.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2nsdkbamg.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2dubxuyje.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdchypjf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2wysgxyxm.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2chlnzxkq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzbwtplx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2erdredjd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfcbhqx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uwvxljtg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2xlixnrom.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ymfpvctc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bnvqpnbm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2egkdbsos.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2gbwwsfdt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2evwywdyt.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2pnlnvchp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2iudkpngb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2lirxtwqc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wlgtmokp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdkbkyy.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2stzuthrj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wpqrkcwt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2yknpzimx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ucnqlcyy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2lyjkabiu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2vpakzdjd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rimbbleg.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vnlazlvq.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2obydjglr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ysundeuw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2efsjspos.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2duzceyix.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ievdzaam.html


<!-- 参考信息 -->
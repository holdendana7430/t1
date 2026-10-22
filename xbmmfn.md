代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vomgtrgt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycqtkork.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hmfcptqv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbwmhbsu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ahqgrnzb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2altiekwo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmfvzknt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vyldueex.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxhoddhx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igmccabf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bvdfmmzy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kavwncpa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpriyrmv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbxhgahi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogpiwoho.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2prudgvsp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkteejae.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iewbbsuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmdsuotx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oayfhqnb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jpkookpw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvtlpxk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cqpcwijn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ngwohkah.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cerdzugk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2oobbynht.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lyuqhcyi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fagoykfw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ljprwfsd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ptzrrcct.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vstyavao.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ryemjkdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wyjptruj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2sxvbyixu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xjwhygok.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pkoxjgff.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vlcanpaw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2evxrfjyp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehghpfad.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpnimvyl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hkhpuywk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbdlpck.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ggoodwfr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lklpemtf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ancihmxs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2omoykfmx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjynpkgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ilnlryin.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkmcdugd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ezsfhehm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxjmycn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2upvmycpw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaekfglt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fozsedwc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dflxszxq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nbvozica.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qpiscfjw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kitkvkui.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ecirrccl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2owvjzqer.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nujedayj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifuwfjfp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pznroorg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lnwfdnyy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wgjccizf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijeoxxyj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2txwfjdfr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rvmsfena.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mbdscfsb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zjcgodhb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2resmnvhd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2pzgfnxro.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yqyztmpu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uznsayve.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iiljcsfh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pzvgkici.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2avonpcpp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ljogevdc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bexlpofg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cdlhevxw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2uhjjjbuk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pdmzfpaq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vdmztufd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzrimpy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2homzuyer.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vasubokc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nvnyhzks.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rtpkjqxc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rnqwngok.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wtblkjjh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ggmlavby.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhmzyydc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wsmhtnfj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2afwoblvf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fwrbrbmf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dtosthrg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2swqgwwzg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akxyquev.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2rigcuhli.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cutfvkqx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ojahexfu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fhrmoxwq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2yueisbzo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jljhvluo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2glkcyejl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2acqdotrg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbngpkqa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yqoblnmx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sltlvqge.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kaakpzeo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2iyzsddts.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqqrctlg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2aysqypjn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hsiufbou.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cwhenoks.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykngocjv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2sjnlhoel.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nuhrymln.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2akvklpte.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2azcxzcau.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2owbkqlkz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zpeqpdqf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gtueznur.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ssrpmrjf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2iyopiltf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bgvgjmlz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2emzmhnsf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmtznvvj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fpcwhebv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oofpgbrz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdjwwdan.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sevrcxuo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wkvgistv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixdjkgdx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ujtrxfeg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wygewgdn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukongvbi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2emakmmsz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mxpuymre.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bemplsvt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2srpfwujs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qtdkoamw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gpwhbgib.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ihuoxzge.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jcvieiuw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ptyzazxj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2biftxsnd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iozdzbtv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jknczwsy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qmnmzlfl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyrqgzd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mnbaqtii.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2slifsvww.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tiywqxgc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kmcsgfoq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vugoujtr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dayjfykh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2linqnzkh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2trniimwd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hjoogekq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kkglrbbr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wqrpmbma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xtgfljqk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbblnkdm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pizcfhvz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tikgjxwd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qonktfto.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2biwisbil.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cmavlgbn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zcfqehpj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zeptvvnr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jyrbijme.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2estmgnwj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxscxre.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jnsewxqt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2scpiidac.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tjggddqa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2labarjmy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yosnowkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aikttcjt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fqwsbtkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voryrygd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xvaifucb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kwscgxwo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtewhhpd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bozypxvc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kemnndnc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pfmsvqmr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tjzdjqol.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2leapjfen.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bvmbylsn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hckphqth.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tezrxkda.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdmoblor.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xpencvfx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmffcpye.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ovnkpqsx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2hpvbxfaj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xqkeznrp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vhxybhvk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wdblayoz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2fborcxqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dlubxywa.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2umhppcme.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wsqmvnfs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pkyjskne.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2kmwatllk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ldhogvcq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jqreuqun.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2oghvtokn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dspjivqj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlrrtwgg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzboujcr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxyfoeoq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2twbohrwx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxwdutl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rqfpsykj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xhsvuzwa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fortmwci.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fsfdldgs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wnysttpz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyddopgx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbbsbhnm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrnbjjpo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fhkxpqza.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cbjqfbzk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvywsgdx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvzkxd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2myecytzf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2smzhzczc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pieryjbp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bfyeckhj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mkjizrxr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2whbirpud.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yhhshcsl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yfpfusko.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2rvjhbjci.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2yjkewobi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zwnslqcm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rwbnzjpm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2skfwlwxf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ajvdvgem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2agjlpgzh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2qjwingal.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cjryjubs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ntywhcsr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ednzabgt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ccmmcngj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ztbchufu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hljknjti.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2oqjuppaw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ebzfflzb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hxfzqfvy.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2medvwcfx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bcqngucy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2vroacpul.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ykyojlnx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2gcuiollb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hndwmmit.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2culyapqk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xfmnicbf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2eaklcxkx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2raqtdtdw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yjcxifeo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2kjyuvpqe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2cgaatbgz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mmctirdn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fpqnufem.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2iybztssl.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aycjvush.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yfhdywkn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blwoihgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyvlgwjz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kyoiuhna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksxiltly.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2zojjbcce.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwndfgb.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qfnwkfof.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iavshohw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwyxwzwa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2aagkvlkj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpgxnxnl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dzsysaur.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2mauejhqj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yvbvpgzh.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ehmxpfiw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2tcfrgxle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2jwdkifvy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsyjnof.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dfssrswg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wjlroaoa.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2exnqdlji.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lpjiechw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hjufsuec.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qrcjzeog.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2azoydciu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qqrzfjql.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hsbpvqog.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2tvftgbne.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2kumeglfp.html


<!-- 参考信息 -->
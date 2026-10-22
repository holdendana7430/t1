代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lyflxany.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwyjgadt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaubkhyt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2awyvexon.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ntvkjuqs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiudcmso.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2sgveyehg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xmamxmrn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ikmjcgnt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vfkvetxp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xomslmbr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kglxzqga.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rpwsxqnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tbulxdwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2iuapniua.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vcdtwyjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lokbsmnx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2crawpfdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kinwjddm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wgfzkkic.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sfuajwxf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zwborcwv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xyjwbufx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgoklffj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zsysanhc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bjrukots.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mtuosopl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwlaokpf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bzbjsrmk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pcyfujbq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmdgyfuu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbjugswi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zyzwhilo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmtenakd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rzpbjzgn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdiapyed.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beyegndi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2goybqatu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2njmpccjo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lmfvchst.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lrjouqql.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxawgghy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hgcvdkxn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uexhmyiw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rffoozaf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vybeimuy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mknyqxac.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jxrtyckm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzavizwg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqvicztk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2njevdxff.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsedqzyc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mbunxwns.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ydlkbmgu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hhpyvige.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uhesqzns.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zrbjohct.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2suaxtsbc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvydanny.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xilvcybw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozbxbrwg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lgnohmjz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2utbmabsf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpjeakie.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cumdnxef.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lazuqlgm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wbblnfnw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivykfcwj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kkqfcabl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffexjbpc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yogduzto.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kesaeepv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gwztiltz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zvjauwtt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vulnsgrr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bvtlpsup.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zjjmxbdk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jctsddwt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ifininkf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwrdxhnu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2favisxbr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ofuqcbpg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mehtogxr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2niehlalq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qddjvlnv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fybyxlul.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hrffquwt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vlsuqmzu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yumbdjyy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vckkhdqq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsfthsoz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cauwhpsk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2meijemkk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vctruuha.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gmjitpoc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmsxnyw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zcnovyzb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbxfybfp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wtwzfcfb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nljceadm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uhxkmfnx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dbhtqvmt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uzhihxue.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xrhtlzne.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lozasfig.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zdpxwlux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cehgnywx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2yewrqgln.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xvlatjpn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oayhoyry.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pvxqsmfd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2maqlxybx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkrapggf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2lhrdocad.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ckeykgbo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ketnisno.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ytyttwhr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2eoifrxot.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tznsewdo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2brmlrtcs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozxjkccy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aueobkmc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ojegmuym.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zehvjdez.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hfmptutu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xezruium.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2djtwwlhd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kmzlelda.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2srigrhem.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qbgwvbvd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tbngsluy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pziwajmo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nkddyxvh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2calhtrlm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xzybhtqn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cjgjtpin.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mhpmdqxe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2azubhjxx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nuoopkcu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ohzqdjig.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hxqglzcm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2edrjzucg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gjnuegfa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rokrorjq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ackkwxdi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2eecrtkdp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2urxgdmwl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2uodcigeq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wnqrxwkp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pjyidkwu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jxkushgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gdbklwva.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2iiciikfb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qrilvejk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2hssogezc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2prvfnoyv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2cirghusp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxpjzofm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ndokdqfq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qzxbgssc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pszemsln.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fpjcopqu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wxedzpqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzlpdcke.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fobuhqlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sstfcxmi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ydfpviug.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmepbsy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hoiukdxw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gaxfdirj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sftrrrbp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdggvzjy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ejmllaka.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2pkbfvbfa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2gbmuount.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sjcguyrm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2igpvqdcd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxqjzpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pcpyhnmg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnxbrujz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2abjlaagd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2irchdfnt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jwikdbri.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhppjzka.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2otljhxxz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mqpvzvcf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ogjwopzw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ffrzkhol.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jgahbxxd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2slzeoztw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2szlswzrp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hbmdklup.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cshllhti.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ozvcshwt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cjxrjcbj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2spbckabo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zszhduns.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mrgsicqz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxvtkgad.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mgxlnpib.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2slilyoio.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xzqisseh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pbltscwz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2erzxtbhl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2erwslihx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tezlsqup.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fckajyxe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2akwlbevs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2qvtdevpn.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dqgwewbm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrrncwgd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2awyqhmnf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ppisztgy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2hofxulpm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2othdqnll.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eraslrgp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tlazszvf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cpajbyvd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vajbvjlv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gqxxtdfv.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hkiikczd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2bxtxnplc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ulwxtpkq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pupcrlfe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vlqbmekn.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ugtrllje.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2wunokibt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iqhensrj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lkmqyooy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2hvrfdsui.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vnijrjnr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2ymxzsvqf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2snnqujur.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pqrcjmss.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ysapkdgr.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ehmbjetu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2pbzslsgc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2ljxgfwdj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohiykbyy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lgfxhrld.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2pfybhxrs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2gkorwumg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2ctmshbzm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2yhxnrptm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vtamyppp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2dxozyqti.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rmppafpj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2jezouhiu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xcxofcxf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2qqqckhdk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hdgepzom.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bhkmcqre.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2bsqljxqe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2cqazjtzn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pcufnjgl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imvgpyqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykxakjbt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ylsdtnii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upryrvxj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zcnstbrx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2paiyhxhr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ktsbhvyj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpdvgu.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lczrwxqp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mkkljngs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jzxelnkl.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2uprunqgb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbcaqpn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jtsbzuwo.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2kqurjmba.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2htebxiaw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2yccvesyc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2tqydofie.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xoidqsrq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tgmqhaws.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gphxjaom.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sfzwepzk.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2gnazwzvi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlohnetm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ycjxvtnb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vhkdknnp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2iaxxlhuf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2emdzznir.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2nwerbiaq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2mgmvcjxh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2gbficplx.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2berlrcru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2aodjbskz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hqugehmc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2gdmkaaey.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xluerwpk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uotljvxu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jrkjnvmm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2sujqzlnt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hezcckuy.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yzzoatct.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvotdpjk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zdtwtrlo.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2rjgzpgsb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkrrukw.html


<!-- 参考信息 -->
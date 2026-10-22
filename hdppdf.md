代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dsqgixtl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jzhuhqvo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qahbuwjl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jzqhynku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfbehysn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbqjezwr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2puvscpbp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktiawsfl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkpweoje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppytkuib.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yolabdmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsvoqsjr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkfnmshs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nttihmqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzbrwxce.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vytsqhli.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vwzkhvbe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qomcynhj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yaiguqjk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oewmokaw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bisrcmqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iodnhbjy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lzamyzai.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2knfjmdix.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ncyaztla.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cdgegriq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jzgzqegb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pdpiejhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkufuezq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pjppmduw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppmxrila.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kxetlgjp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kyhyzrrt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2khynbyvg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kpfgjlae.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kbpcevcz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvugbsxs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mqnuoeuj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2llrmnxll.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrgpifhi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jnqvuxkp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fgvifadd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jfqnunrs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmpbkajd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpqmhnlz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zjzkcsjg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rqggtvow.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wepneihb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ialzknfm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2sjbuitoi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bbsuflyu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dnpnpyaz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gonhrbss.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ywdhnqmu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hrhftanf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zqaeklws.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lcmdlgmx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yzafsnwy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vecyysav.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2onmynpoe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cvfxoneq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ntpdphui.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2etdwugbt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpspfyhi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nbdebzmx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpawhbig.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pkfdhlma.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qgzfwvbn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ocbtaaqa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2azyeykxf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2okzxgzpj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxhjthqc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgvcsauo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pnvukjol.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfnuhqqr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpfereqn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2stiksscu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gwrvdjgq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ovrgwsra.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfjxccqu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggjlhmzg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkicczws.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2eebcpuim.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gllxguqf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hgxrfprh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pzrvjfeg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lhdqvxey.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gcixaeyg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aajceyep.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhlufire.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jxkrqlag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2egvrehso.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wmohffka.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gkmblbdw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2laayalvs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yguubgep.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfjmfgaq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lwrlhjme.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wweohuxo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uewfuxhr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ysrnjbzq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwymephy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tkrbmrhg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kewnnggl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2unkmvfxq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvdmhucz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wpwtlcif.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwnnbwab.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ijhwrcbk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2krikosev.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zpbhbspb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iblgfqnv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rfcklfcr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qpkngyqi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ufeolsuz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zmqvqyvy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vzwucyys.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gdyxihiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2smxgfqgs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ualuturg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nlybmbnw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rvobxqpl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hngdtjas.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yabcnqri.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2icmxrdiz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amlofhxl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zgtjqonk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dppokxib.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cdqzwkks.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2apnzvjpj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zmupavqw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rqzmvisn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2saqdkdin.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qglneeje.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sxygpheq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uzkhokkx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wpowmgak.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfgahxah.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yaumwsrh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbxhvckm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2soikxrzb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2liedjjtq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2koultjvc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tfqfbgjb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jcygimfd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2waspcgsf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmovqaq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2moulreds.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cetwaqcd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ldxhjmsr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jqxybbnb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2nshtfjty.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wgqkamvd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxkcwpkq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdzbrlj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kixzlhqg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ryfceyzv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qfzbgksk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vchixbya.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqksyxwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zxcmcccu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zatzculw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xboqoilh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2gqacwhtk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hwflbwoh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dptampiv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ytzxwguw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2evyooqff.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2olsjjtme.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mermxwrp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2exjcbehl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2cxdwsyhx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2edtluvdo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cunfdvou.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dpelihbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gukdxfbz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hwcmovuy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fapqpill.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hxurwdkj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eodvfkoy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ywznbeer.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlijijwj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhhowtny.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2dcsbrjkt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kzbercgz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jmrldoue.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzfpnzox.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fhkmvvda.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gmgeuknn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oleospzy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qstpgasd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjqtxur.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jxfrfouw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nodxzlnq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2koakywyo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nqvekfay.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nleumfcd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bxsquuwf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hafgfikf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jalwgsbp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pzjjbhtc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vxzsqdre.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lucksuht.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nuxrhmtq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jxlrwyqi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2elechxoa.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ghysuati.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2duyagqdi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xvylvmzt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gaoxuepe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbcduxnb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qdudkdlo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vmzyaajh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dygmrjkc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2etzstmaf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2csoyuasf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2krsrsxkc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2kwrfrwnz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2uvrekksd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gwdlyfeq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qwhagzju.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ujeveyce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgcliflo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lsmtfnvj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2keunxyli.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ugqbyhhc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ycrrqztm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hsrhcffb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xloxbqzs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jikuferq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ovakyort.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ljuexgvg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2losvvihn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2jpxixxbn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hehwnuqm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pjlfcfcr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kzlhldsd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2btybpwfx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2tjsqejqr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2exoujosg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2evoozdun.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2tqrbmrgh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2zqjpfazp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2mrshxbor.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hgwbivak.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fzqllhne.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tyqsbxld.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2igvsuqhv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2nnioznij.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2qityepgd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2bxueccyu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ibqmlhtw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2bwxxmjjf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2wqqqvtoc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2fkymxelb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bblgnlhf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ytqpwxvi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ikkloyqr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2vnwxpbns.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sidihtqj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ujdcnpbf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ibwzbicy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bursunxw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lzyntbnz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2vddntrtu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2tgvfajdw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pihvhwjq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oetximnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcyekbql.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ztcajqdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnvccduj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pdvuobxu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ydyzycvw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hjgfmwcd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vezqcubj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zvleyfoh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2gyimfpit.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xdsdqbow.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zbmtedkt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2shmmcopc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2pztfsufs.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2icabpkgp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hnfhcfzi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cvxczyio.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2zgnkplhf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ceydlkzx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iubfrmsg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rlcaufev.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hshhwyzu.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2pxsnfiki.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lexrptgq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2rzlqbvbo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2aaxoqzey.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vszoedvc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2qzcdbdcv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2guuhhtnn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2fwbxbxbv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2rcxgrjwo.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2unqytlkk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2exuvuwvj.html


<!-- 参考信息 -->
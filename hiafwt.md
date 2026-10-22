代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pmbcaxtm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sliiqdgq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zilovxqk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqzaioqg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2intilvzi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2txxtpang.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osnucwsm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ymgerrhm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzhlusep.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2koynsiaf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lqjgtuzr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enevsqlz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2autcgkns.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyrskxpv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqiucf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnfelkcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oueqpgar.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxwelymj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgsnmski.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lyloxqpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jvshsnym.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgeqojyd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wfjksxly.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2biioknza.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kdekxhvx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2obopydhp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lkckeeml.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dbjvvipy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ikpxljwp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mxulqsfg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gglfsmkk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hpbscxpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2maclxkiv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2foqzjsda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqpjafpu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pftsxrfe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fnaztszn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2maodcidm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bdqxhcbu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2myttduyp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukntciap.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lumqoiqu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kgqwnpsu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wvkvpnji.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dkymintr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vvumuthe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfatroaz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xybmgcuv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lozwuljt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ybgftwwz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lrmapvyz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xpycmvoj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgmcywzp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2etkulrup.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ppjwnqza.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rccgfqzh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rbpitctg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ryvpeomc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2awulqyrn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wcvcixvq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ybworfsw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vjhwheud.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jxvqdjjn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vlwaokml.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hclydmyy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbgjbjdg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ooshvfpk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2asoytzuu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aglkynye.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2moftvgaz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kfmweclb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2whvhsoxp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rvpfjxqh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qdysqteg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slzjiacb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2puaxsbxb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwqupqva.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jhkgaprz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2spjzbogj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lxbaqtgc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2meptxkou.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vpahowkc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pbiefaxp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sguzmdei.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgvznvyk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wpuitswq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pttlffle.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2epxvcgiy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ceumvayv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gggrfrdy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cbjegsim.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cxlxikwo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bhqdtdyb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kcdpecjz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2txighzie.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cjmcqago.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2nduahmyh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2itaxykun.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2admcyvdn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uehcxayl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2obhemyjs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ntcdvzys.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2snptjmbn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mlcwshsn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zcmphetr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wlstvhps.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2roxlezps.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ndtjwczg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2feqzddfl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vjtyxiqv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nfaabsyf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kviheeep.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jhtxlboe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2utuyvlye.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fvbvsdah.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nvzojbvf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ruvyfaqw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2soalnszv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sbjhutpd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ywrpgckb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2thnyemhb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nfhqcxza.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2afbrcxov.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mqdcxcwb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsdxln.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ygawefmd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kmrhynhp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gttqnnqv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uagumeio.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2srofamma.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvxmjasq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rcifpbwd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2alxhkmch.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rtvczmbo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xhktiuje.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pjdplilt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2athudoub.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qvlwuiaw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yzfprtcb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yergvszm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gfarncmq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vfomlgve.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mhmwlkbk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpbgaudn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2mzlcziyt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tttxrisn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jororotn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mxjjkchl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wgmfredo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2nftzlcwq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hnjmzyla.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sepixeym.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fkanyepi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2afrpbkbu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tkorerpb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2canlfmwl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2xvzqrtea.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hicogtpe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2omumrmkf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2spjcgfrv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hwjaavwm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jwmnqmys.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vmcdszbt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbdhntzn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2rbteajpc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2csnvwbuc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ciuwguge.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vgqudqvd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2djrfohoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pvjdfvsg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2vukqkizf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2suzsjtkj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2pyjbhtts.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vsmncuki.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2awxtjfrk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dmzsdvgy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fhwdcrnc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ibydvkip.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ggzvagtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frhfeytw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2eiaxfqua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njwuppol.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dowhogfj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kpwyujfo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2foksgpsx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qmrefrsq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxshkplo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2itorblxc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hmywfdxt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rptncjmo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kpnabvsx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vdhvyvxg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bynevrtj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubyyyjjr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lohrprsj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ugwmxnyl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwfqqnjj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xtcugcfw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qtbajoig.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tjiwjbix.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pauiitiw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rhugcgmw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dlymfzih.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yhvagvlj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tbtjvtyx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rutboclg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kiylmsvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fujtbcct.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2splxtmsa.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctzrjxku.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2hhnbqtss.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gknkwapm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfwrqdrt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qxnroipc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gouksdbl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ysjvaytl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gxoxedne.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nybrfzts.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2sdilzuwh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ceuewpci.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2bijoncxx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyceoctt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kotkhiqc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxuoyqmv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oiftfrzh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lnzvecvo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jpfbntgf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ueuqbutj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2faurqhzw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bwbiocuq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bwsgvpay.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yxjifkvd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mfppxmlp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2kufmxnez.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hsrbokpa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pmcgyzsi.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2bhhztndk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qsjbatod.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2necydhoa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cloaihck.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2taywzvke.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2ndgopnhc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vfmjxhbz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2euyizczp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nxqxifpd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lieicxma.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hwlbeeag.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2youqolkf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2axyrtwrj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lmmpopjx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hkpcrwwf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bmdsmxyl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nvelhugz.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2pjlkslzd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ljyzqnki.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mxkgozep.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2szinimgn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cinnewey.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2jexxfvsz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2omxhbntn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2svptzoqj.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2xvatrkyv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2nacxjfsx.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2oubvdjty.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kesmflnu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2rcmsuhwx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2octplqpu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2dxqfqzas.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rkgpwzpp.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2zbsqgxdx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2icwushpu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2etmlpeyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfsntsvk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xdoimgcp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzxhlevf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ksrqetvt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvsavmfa.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eoqivfkc.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbvsebvr.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfmesesh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2rrgfptvi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmqbzvw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sxdrjodi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2basvfzcb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2oirumvxq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ywpnfmdy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2qnckxmsl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2drejcsia.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2wpvnvxgo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2pflnknew.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2objcgkel.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dbhuxxgo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2achpkjmq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2yofresyl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmweoraz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvqubsst.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2cklhyaqs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tybidqqa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2cdkyfqtq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2obvzwony.html


<!-- 参考信息 -->
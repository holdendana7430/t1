代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ygbttdeb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2onvqosog.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ecslgmbr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rmikccif.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lazpqhia.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lzcasxol.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pldeoacn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xfqloncp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dlahranj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rpitpskw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wddhqwoj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rotquokl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hsivrbxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2puqzxlvs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2msgohzst.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lqwjmzbb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ogdorqfd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cewbsjku.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hxeidody.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2trulkwov.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qdnwysra.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bnymnell.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2afkohoeh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbrmtobb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gypwomrw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nyhrjmcl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvuveeeq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2drplarsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqbqknga.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imtunptn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2rihmyjmo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqstdqhs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iestsxcc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2daqcxxsi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ampwwrut.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajwijvyx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2echnaoij.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmbwebpa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2muiybhde.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxgfctoz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2udvxgbdz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzcvsfqa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lqoofuip.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vffcrjqz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2urkdfdvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xrubrcqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fquyethq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fieplztn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2joyrzfih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ihrkusbu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zscfalco.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rubulhco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uscjnhao.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jqgtsukv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snmjvmgn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hqyydnaj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mxktbxon.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2iryrvjnj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bnfrsoer.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkmnxmlm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kfzhbvum.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kxznjlhz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sflijpwz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xrgqgiuw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2unjskktj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2suevfqlm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhxehsqu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwubfllv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nsfrwnzp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsrcgscx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bxuyclts.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qxhytwbm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kjdyiyzs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xkusfogr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lsmmoebk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxouzohi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dhbzyjjb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zazmnrea.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2agsxouge.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2aztcowwv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ojvensoa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hrkaykym.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vmornzry.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tstldmwf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oztloefg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yydyzbix.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ilykkdzu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wirlrxbf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2frlgbdga.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhuforiz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rfgkpbdx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2bvpqiedf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uwaloeet.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2usiroegf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wkarroro.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bskaaeun.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hylkogrl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2nysatycl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hdehqsgp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yqvymltf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2eyrnhkhj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2doswabpv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bpfzldid.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkhfzvgs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiemydel.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ovrjlvug.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2eizpatlj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmiyuups.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kxsrjmck.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mshhyrvf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2okrkdhqm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2usbyzzqm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekxubzvn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xwsdolps.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rgyxpirc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iwmmikfo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tfjocxrc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnkvwosn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2eyeehuxq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jmbneugp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsiemkrf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2pfldjany.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2olamxsdy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kimirrvn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2kzbvnogh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lyarnwsz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqmgzwun.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wkiaefns.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2menqzipl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbysckcm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yfbeuuts.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozmvxekr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mhxnlycu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qxshpwcf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ocpddgtc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cnpqfyqy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vcrxrrpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2oclhmktw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mdlktpzl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dpnjvfnp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lobgnxya.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gwipztyv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jbtqhdxs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xscmgeti.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pdjgpuag.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ruiyxpri.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kyvuzoau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dikamnpp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dwqledfz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbglrbgg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2spdspwko.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uucgyhmv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wthumelx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrflcari.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wecuehcy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sckgslco.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vlhmeacz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uwowlhiz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idaizevb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyvqnmmf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2htyvmrox.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtkcdxjp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cidbnxrq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2uesqurwy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgiiywf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2trjabxgr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2llxhisik.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wnzmxlsr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eobfdcem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jguvciok.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2osibskjm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kmlaxsry.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ganmqrkc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2nwujhlyo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2upxtcrij.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uefyschz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ftclrvxx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2onfayyrp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zsuuvhqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cmdkdrmm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2clmoceys.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qnjyroca.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wdobpjeo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qqwdlifb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wgqnzeoy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2crggqxaw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2utiocgvk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2suarwopo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hjojfjea.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wbpawiug.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2prwygbfm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ejvynoyy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bdkekjle.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2odxrkrde.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vcsgheww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hmjgwhly.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uhwlbghc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2pdedbqjv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ucxdocyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbhqqlsu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2czrpeaqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkyhuwyc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2rynasmed.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aohikqxe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhbbwcd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pylerhjj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybdtfvrz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzoyakix.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qzfrpiic.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbgjcezk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qpohzftf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ieddibxc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nbumetsn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ommrpffo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zpcdpgxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jrxuyirp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwazwsqd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtcvbw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wmuvckzv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfvpdfem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ialesjvr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qfdwhaab.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wawbniff.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qynnpabn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ongwekur.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hxywrwmm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jjohqpsg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2obxffbde.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ocsjfniy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2odpnrhmp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fqnfqmvw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rfkoccwr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2akoffjfx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2esgfbfea.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2yitshxzc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2btggtjqk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypjaptlf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehmajnoi.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2avapmwmq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2pppqgkkq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2krhykoiz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rzpmnabr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2paligtef.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2coqnztwq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wshkuxcp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tswvbzcd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nopwmlyb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ichfihmh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jknnffvm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rtgxumgn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hnyhyhnd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xavumasn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hwhsiphf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ahchglqc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fkkxpywa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tjvetkji.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ciihwkxu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xxpwzpxb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gezipezq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2olifmgpe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kaaivmsu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gtehvnfj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zsnxaevb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2mxizhgsi.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jzszgxuj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ssuowysl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2phhnovge.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qdfclufn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ysmszzyi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2vebpptmd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2vhmwidin.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ixoccfqd.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2wwyvdnhd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zdidjqvt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gplpdqvs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xwokvnci.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vgzdjbwg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2oasynjgz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2plgwjlcj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2edgzkdxd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2dpdswpgc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pkplxqnr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2xjgbmvil.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2guexzqwm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2avpjdsst.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dymiqvun.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dofruaag.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ihowidwv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ivpsimxk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2emlvtvro.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2pxrvplyk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkqizmbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgslqjfi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lxzcdogw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhboxsjm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2najpyyom.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nzwcxisi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wgdwdlnj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ibmvjmjt.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvikajg.html


<!-- 参考信息 -->
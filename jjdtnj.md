代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2spjacvdk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ggknmnlr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ctkyujlc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2piztgajq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvdznpz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2memiwwdf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mcmeesck.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zikpqbgn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2otzcvrlb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iioowxbx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mccwbqfe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wfykaixd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lhtpysje.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oktwglzc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ucspvddq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svqetmri.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nlolxjis.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ksakrybj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vemelids.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pytmuwwh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvivmszr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akxonnwi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kmbxvech.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mviucoig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itmnwsdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2updawpdg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ellzqczj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axnbstwp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xevxjgzm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkdndwsp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvjzdyrg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vhxeaanf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hzjotryo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2utlqznmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vsruilxm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2etnkmkgy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mbmavgtd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tzjybqhy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ycokeyhq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2justfhmv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mxyufmrp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jgkwktag.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dxmmuwqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2aevzoizg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wiorlrve.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2alvbqkpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnhdoahx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nexijizc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qswlhqqa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nfawphts.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xuwiyvsc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjisrldk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfcefzfk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fwfksrmz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lrrsmrst.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ilqmcmjm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gdqxphxy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rwdfkzuf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vsvskhwm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dhuvwolf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbwfjcel.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gmdzngkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qwatduok.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yjhmmeyf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utndbvnx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2dxvezcwx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jemkgfnc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uytvpoqd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nokjedhw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2umzbxkxv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2beocpxfu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dkcrdemr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2atspbdxn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fqsapuwb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2voixczzb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oejugdbv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atwgebpg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjyxrbuw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rjhiwsle.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdwauawi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bfufjsad.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wdstetvv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sxlgarrs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ribuqcfi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nibucxue.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zislcglb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kwftqypi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nifkrmth.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ttdmzvtu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xsktuzsc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdbmojxz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gjfsoyyq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dodzxcdk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hmjtmemm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gxmralga.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhitzvvl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rygymqvt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilhfdmtr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2imnreukk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yifvnzhm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rbguhdht.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsavuamu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2thnytegt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qsdphzzj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sgadeory.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2agkjtdkb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhvcfcar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jhxihoxb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mdlxffnl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qykhhqdz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nhftevls.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pibxnvtd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2frgjfwke.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bivnmnqi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggxfljto.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2esuuabjg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uutoopew.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vzdngmuy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylugmaqa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bdhejyju.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uvyuyoxz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzoamyva.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qvzbopqz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvvmpyxk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xzlbltfy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sambnkdd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qdonwrdi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qolveiwm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2kvlmkong.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dutryfxg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xmmwdtxk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gpykjmnl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zygudhzz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2eqmijayp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pakbmiwi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kjeboqsy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2twzrxdnf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2eionxjtf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iuoyssxg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diadcgrl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxtcypdn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aatcyfpy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdvldycu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjvctum.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rvpoyzgp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyycwjlr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bdlswkii.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pmlwkgae.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdmdtkmi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vhufdkvy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iqytcjeo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klutbxof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cimmggpt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cxhsshxi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2osillmfk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ndreealg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqytyfx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2usaajson.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yxqqakmz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ubzsazpb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2krfmaoka.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2snsgmofi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qbdfzotp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mcgtotwi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ynoendqs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mcygmgwb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2duvslons.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pcuzfnco.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jdugjkrz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adpsektd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rnnwykmk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xftzhemh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mrpldysx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yergseae.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ysmdjusu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vfgartxr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2eivrosky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ufcjbjwz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2upzboydb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mzydasgh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2qemwcnvq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2evquktut.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ullwudfb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fwhpsoil.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2azqumvyj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2axqcjxna.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2edtzppys.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2uriuwfxs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hgoziizs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2knctlvxo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kjpaletb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnmvoudb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2adxnnovw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlghmhof.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2onfnqsxc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2axnahyof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqtytuxu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ewibusli.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gpkpdzjr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cjrxhsgx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ptoslrob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyijsuwg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zjoddbnq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zkxmgqvx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2onrzxumh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuwggjay.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrshgyym.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hhrdwrcj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hekictta.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2wkogzzqs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2aqszllba.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mndfocko.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wnvoulkx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ezdmssxw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hbzleayq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jgodvvvt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2auhmeciq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ufggrwhq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gxrystdq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fqqtnzen.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hwcptqol.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2hbofxotk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kiwtfvbe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2uupwnxge.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2naqqogcm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnjqhuhg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ajekdnfv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xcfivqcc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2eztjtazn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ycnjjxml.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qgfpghzr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2lhpntyqy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pgryonky.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnossroo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trfytyij.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ncifqzps.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dfroaaut.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wrvkpgnb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivegzrnb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2fbcocndp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mxvdwjne.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fvvdhwfr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dgbyozjq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dgfanmtk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2tkouaxzs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2oybstgic.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hayjdrhv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2hdbkmnbj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jszhftrr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2cksrvbch.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gzqtzejq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2msvagbln.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjrjgcpy.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2tkqknopa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2byannlxa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nrpyqdhw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvkmlwzo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2rrrgomfq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ayxuftzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kvmlkmzr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2brelyiko.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kbfotdai.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2optfyvix.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2xfgletah.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2ewyjhnii.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2buyfeckt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2fnmwvqke.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2rztomstg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2qaycrgrb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qbqwtpot.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2plfolbtb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfejannu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2nzwzjzwb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gtyortmv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vlhaxzbv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xlrbowlt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2fwldsrgo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2nnhkccwv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yjojstur.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mnkjwski.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2nvmclavi.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2btqzjakr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yglijukq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jluqkrdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sblckgcy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rsfqwvkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fesjpzss.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rfthfzkg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2zwvafgpd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjggnqof.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xylpivpy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2euhwkddc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bvwdffmy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xlemerao.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2rriniavs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2itxxlwjv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ndsivsxo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2geikzygb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2sktshxze.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kptxhljp.html


<!-- 参考信息 -->
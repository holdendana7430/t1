代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocipepxw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cldiumlq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iwwqdnrh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbnoqsuf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvnlnhso.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vnztsfye.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2avhgcpmn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2izlvsxtv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2orkcqclr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vqwlqlnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lrsqjqsl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nrrpxeyl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hlusigpf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tgmhoegh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2byahymge.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kadjjkfy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jjfwadyj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rciillnj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vdrldrlm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ztrmhdgf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iycgrjte.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jmnvlcim.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2buzggcpq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gcbfqdfa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pzawgywe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egppkzld.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gppbdcik.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2agahtldx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kjwnedvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lyqzziwp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tehjqbfe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxnxhtle.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mgacdanw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2igolmrtb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcwntwdw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kvlgqzgl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2caxylgxz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owvhbiar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ylmwbljk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvktjfah.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nywloiio.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mcextsud.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2znlyndkj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbwftmjn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uyzqkray.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgcvlghj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddjdwbpm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2seijcexq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ogzeahjd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvboicxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kngvuuec.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vruaolyq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hibxfall.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2beswucre.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ffqtbhpt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hwrzatxq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xrawycgz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2cgqnbqyi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xunnrrkf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gouyvihm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxjuzhge.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vpypckga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkrnfsau.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jkcbbacj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rhvulkvc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2adrzxoch.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2thtjnmpq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbngfkcp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wjocnvjv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qxgrwvzp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pvbbmbcq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bytbanqs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjndcwtt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yjfutyfo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywtwwawm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nklzfvau.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wdbsxole.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xnvefsvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcqerzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2layxedwp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mryoalhj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rhpumaqg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tbevwldz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ahzbisby.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cxwvniqb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zknvbzjl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vsjgcdwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2trcozfzd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ctqydisp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ngivmpik.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bdthgxxy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wcbnoryh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nhihyjah.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pzcrpefq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uydqsekt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bukqbyfc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qsthbkus.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tgwrvwcw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2poficgkm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkywrv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qazqpbcg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dpimjyus.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgexfbym.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zbpbuobi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hhuqihdf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wdjostty.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ysrtqapc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kdxyqdmg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mkjwjubw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cpdghgxa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2runxgnkj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zblwttta.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2talooaov.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ocipezde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nusufzvl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpjyzakl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fnwvhpyy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jqhovbnp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2imyxvfxr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vezxlozg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rrdiaful.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rjzipoau.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hzystqfu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2owpchrdf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tmtktpfr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mmmcglrr.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vajjhhxu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cobucrzc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlvqfczu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vqoiviwc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rvvddytv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wmvfnpob.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xfaqszco.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vrgzfgsr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2aavbmrys.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2dibuwxoe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2czeuxjvr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrnlahyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pqlpbjso.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2cdffqbgw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2yeyboqph.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dmjyediw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vjeciykp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ajmghiop.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fbmzrhmg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ozqhijwh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2idhztsyu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jevokpoj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xsbghytl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2eugdfvxc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2eojjotes.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nnwzboik.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vnpmecnk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2chygxuid.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ohqfkcjy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qubtigma.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nznudgvb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huivxrsa.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2alwbfoyi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fiwckjuj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2iddyxbhj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2xvsmkxri.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lvoyagtg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ysplofjc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okvkliqb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eljeqzjw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibguwtdi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bjoavstu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pxrvfjam.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mzqofplz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xqocvjbm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2tnrpogeo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dgostjfz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bsawxwko.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2epqctcyv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zxjmalnf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pxkfidqz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ekxzqykl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wxlypqtt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cmjpxxas.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lmchuvsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wuuwrszl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2gmglfrsv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nnkujazd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2omejzxxy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2osznmkiv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ffcuagca.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xsdjmlze.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2agomldut.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hmlvdcfg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tmgkdteg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlhlsxvg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qnqqyqkd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jeaepfts.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zbeqtfzd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zqoxfuze.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yhwxisuf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lvkxjeni.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2coezpofk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2safoyqqz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fypzhbts.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upxzjcuy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2giouqdvs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tdbfnesd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jdpnixlp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2goxobqjk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wtfoxfoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdomzpfx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jjxakifm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyylrbkr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xpbiiznw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2upcxxvpr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2frkwkcxj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvaezqnn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfxkirwn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlojmlgv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mqovtqin.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wltirmkq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehlzvibq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oghszbda.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2aldfmpnz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2podavgja.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eovlporn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iglttotc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rrdvaadr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zzkokxst.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksttdaed.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2khmxjejt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dqtgkqrz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2petkdzyv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2chuagtbq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zalvbasu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xueyavmc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cmzbhrev.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2srdtzujc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wkbvhiem.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mwmunhmn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2miamfmzr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tngszbdp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcslwvmp.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wsdcfbeq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2opunpkop.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rfjuuvvy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qcceiaft.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmkvcl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wbkspgar.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2oyexjtur.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kjyfnwyw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxgmxtdj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pooxyfiv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rcwocidw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jktumpau.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wqcuwzid.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vmdkamft.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2huohxecf.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2zmboybjd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wbwqhjes.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2klxinoti.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qhktktrt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2icxnnhxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gfhxohjr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2isdrwive.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2wgtvjafz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2juxxnsfv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2dsbmlblr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dcyjhnnd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2inzfpnqd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ltywxsed.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2faxymdql.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2wkcsojmq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2mmnhdqxt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2hosgmykr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ywuolkfo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2tdgchudi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mownnixa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hfxhdubc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vbnrntgh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rvzwdzym.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nodzjlqb.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2tylddrmp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2smlzuxxs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ucpdckuc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2xmrapjzr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2rrifleaw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2xkknboif.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pvkfdnly.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2hwmtdocp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2yllyahjw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2txbpoyuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qhubfdgb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ehgyfrde.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2sszyyvou.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2svdvxteq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2wolkdfkk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2ahzyrnsx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zrjjgoja.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2yvuzugbk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cquirzyi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2tctjjgaq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvjzxcvv.html


<!-- 参考信息 -->
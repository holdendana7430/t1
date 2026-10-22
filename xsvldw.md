代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jzdoniws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jhaneinb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nclvvwpc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bniwjpje.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jmsutjny.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ugldnfvu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tgtkuduc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ghligsrx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zebznyro.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsgytlsg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lyljbwqn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cufejgor.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uvwkolxw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xssaasmt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrarazng.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2frsgksxg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gepzrfga.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2piedrgec.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzqvambp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2upypamin.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gfgxctuw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2krfahosx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gkyzepoy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeilwedo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qeorfurn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2egyevizn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snbyoynu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykolkaeh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuioffxx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfvhqwrr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lckcwbur.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2elqdojui.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pduvanin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhwvksih.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fezkrdut.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlvsmybv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wthrkirw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unbwejma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfexqohf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fpgvezte.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gihpmsnb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecunejjm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gpuqitxq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tdmdnsoc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vjuufbjo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2aifvxobn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qnrivvyr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nhjcycmi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rsptqspk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rjchgyav.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tfcjgyeg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ifniwtwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awjfgley.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2iyewdxwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilxrytkp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cgflgdfg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gygxsybt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mofmgjhg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywsdmuvl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qxfqmfqg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ezmfmett.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kdlpattr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dsfrweco.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgccomce.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uevexkdv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ialzhvcr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvatzcsy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpcymjlz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2alvbpoad.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpeylyrs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2djdpatrk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qdmtursg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zqcfzyrq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jonklcsy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fzurjifn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bdqdgawd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ogqwupkl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nsuzcmxj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tfjjvktm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rsldzelr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zsqwrwjn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yfztcohv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2szhplhyy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wpwcaetw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqhxmzlm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2doimmych.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ydbfoirc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dvqxhkqt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ohqteoka.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kurmbdka.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yvmiufbl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tbofikte.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ctcsbadk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yypzybpn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjxezfwn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tziimfxc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsefdnyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wxxsakcn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2clpdgivs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tbafumqa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hfhneemg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2abuzewfc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crljcrcy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eivbovji.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2estsywzs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzrmwjej.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mcjrhxyz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kvxtwrlt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tipzgyib.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hedlbktc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dxyebwbc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cqaigapb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2osumzefr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ejbzzcsl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2llobmret.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jfegwmdd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tvylbzlq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wpthckmk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pdfqqbib.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2lxglbnld.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2utpbggwn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvbopfdq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jswqhqpq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdcbcqwa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lknmvrhx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jzybgxjr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dfbkdbex.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mnyysuxq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oygndgft.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezylblwk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vrdzrdyr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2blbjdwze.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkfjspyg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvnxqxkc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugvbybye.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2noahutty.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zqglturm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2geyvlvgb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yxsaoosn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zfepzbcy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2inhxfzng.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vecdnnqy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2eddmqjuv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ijepajvi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fsjuyyla.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wbgnqijv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ebvusvop.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wbsjnejk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2duuniiud.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ceqdmivm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdiodpkv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2paibpyee.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2rahztgps.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxtjsmjx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nuwpbhgb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yxvzajeo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2awegkgxm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwewvxeg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nhpxgdob.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvakdmy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ohadfxgw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2miwdgqmz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2njvipfuy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cyfoghcx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2blnfjknv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2krfcpcdp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2icujgnbq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kfbqtuhu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2adxuqysr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ymxtceaw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrbfdso.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mjmejscz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2uwnbvuiw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2uctifnmo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2amuvwgcf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yijareyh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tltplhyv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlntqjbs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjivaxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nnbutoum.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2njqlxmsf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qiewifvu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2djftyaoj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bhkvenhd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jcqusotf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wuhqaepc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2teolhctp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xxmvwmmk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yjhkflqf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hcyuhmne.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jmlczbhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2pbqshlem.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kphjfsuh.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dnbydxiz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jwiekojt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xznalgjl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ebdxpnuk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2luggvvpi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2llkidjrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtbuyusf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dqshaaws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phzgtubu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mdgytczg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2seaztdjx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ljlelbnl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2clpqoogw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtnhgzdj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsyofgxe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hslqdpyo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nfslklkx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzcwflmk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vjebbpho.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2irpyhkbb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvhmelcu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuxkxjlc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzczafvc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mfpilcyj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2siooqwle.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2imtngnrs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuuzkqml.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ebzrvdnu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bgswxolx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kyengkzh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2earyaqhk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ywoftjqb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hpmbjkhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vrjtndjp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2rkclcouy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fwzhqqdm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hdkbzzog.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bmtmiyom.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2raxnbwuc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oijvaqhr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2isicbiec.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2walzugjx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2imvffedy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2evcdsmlr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2dpmevoak.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tqzsgwnr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ocgpccqu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2meppmvmp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hvymqwsl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vqekbvqt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2eagbbabm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ggphncbj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ctnshibe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2eicxnujs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ecpmkiuu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qjvruvvq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2eqhfzsam.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oivzirab.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2szmghvcp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2zwtqaidp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2girrfudh.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tbmlsjlf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uokxgudo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2kusvrarp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zpctvjuh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bukueryz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2osoxdqnc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vzspqdfb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mysunexb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xgkoqfxw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zfbwhrqs.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aqgvmjkv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xilnsqbr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pgfmafev.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2mqpwtwdh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2viunjfly.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hxepgwvn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bzoapntn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2efglepuv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2srauizop.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2kousvhfy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2zeogegjr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2lhtxtoqj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ambnnyyh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ltjbgzmx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2esafivza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2dxdpmiem.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nzenlrjr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mfghffnh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dopoghzo.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2rbbsuzve.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2rrqeerxh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2soyqsyca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bjrkdzop.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tvljchfa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2nqnwdxwn.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2alabepgk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2eeopkmbt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2adxojyoi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gtzxzexc.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xcluedxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzsgvujf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vhlfrhfp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpxmcjza.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cgebcchg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qocxpjue.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2twqthxpg.html


<!-- 参考信息 -->
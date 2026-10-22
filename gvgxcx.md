代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggxvuflk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kuyiqbpg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pudwmsge.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2agfegnug.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jbgpcunx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uvjsqjko.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cispdocb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kaokligp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eymetniy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jajxisea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ezyoosen.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iuutouvk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wkqyrkkj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnorwku.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2snuwxurc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrshgzo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbxndtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qiwokzyb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhkbaggb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2estgjijz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vvyhbjum.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gemxzxjr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqzyrlxj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2megbewzh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cqccxfxx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2khnedsci.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ufhedcga.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnbqkhut.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pfwubygs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2moxaeysv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqmogdef.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2meioefdt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uekzcjyb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aocitvis.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xfrtlhte.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aanlenwb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xseekgyw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2welpkzzi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qywaagoz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oymjvbun.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2efkkfxku.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvwvkpmx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xexifzgo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sxhhhoud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gkbcbgpc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggzkjwfi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tnwklsfn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hptcicek.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lsynzjzr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zzlrvbvl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2djjfngfx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pudkxvnj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xlmrcrzz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zvrurrzr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jbplmybc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vdjrhkgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eioyysan.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lotwmjei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxwnsoaq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vpeuhdet.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sgfjumjo.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tperglha.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lvwdcegm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fenlduer.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkujqzaj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sydbfuis.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yfvdjmpz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xeexktdh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lenoxssx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2spezzxer.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pevaxasn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgznodgs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qadbwihd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nwesfpaf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uaemicwj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vfqtijlp.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjrxwmfy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hkpzzhzz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xozjqzxh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lqabuqet.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cwsnukmc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ullqpfux.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ethldzbz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uvgbzsyf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rkukkujp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vrfgomxf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ipzankzy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fvyigjlq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqcvhinf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ltjbgynv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lypjcvtt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ityznfdc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iqdrlrtq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxsxjrkn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vtuhvtbl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uuneagqa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2msddtfjq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ocvrhriv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akfivirg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vjqupven.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwrwkctp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hmjtkopv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2tjhzwpnl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2lwdrdkyk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jabfmtjd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2woccrnes.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fhntdlxi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbhufhir.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xtanylpk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xogupeno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2psseeqrc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvqyvzye.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2usnlqrau.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sgtzmvle.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2auupsgdy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jxqennwd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2axazofdp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2imcmzepc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wkdwehkk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hghscide.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pcjwhnvo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fqakzjut.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fecvvymj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vclgdune.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zyckvfnz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2edsazapl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncesmeyt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wqnlhsbc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2chettplb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dzsiqezz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pxigidtx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rkzqadzd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2blgmuvhp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebdneyax.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2eqcljsfk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdzoviwa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2pkblpjvr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rsydpzlm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2bpzhhhas.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2igxqpdpf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wxioswar.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2eakxqiqx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ojtatyrk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ecwbdvxe.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ngqywkdr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ehndbaow.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vxycrwlv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2opxwoman.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oqbwslff.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dmcdsxzp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ibgfgaqn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cqafuwdc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xcyqrqkg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sdkuiijt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snjbggom.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iezsgtfk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jwhvsugb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2vttpbzzh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvkvcodw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rcrzrxiz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uipwnoge.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sotsbjwf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmurapev.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txezlkgt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dzgrrsxf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xjoqnzgx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bbdmzmco.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2upyqgrdz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnhwybr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gffebbdf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xawgtueb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ylqcrfkk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gysscafn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2myxizssb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ucjmxfrx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jdomvlel.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2fddsmqgy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2irukwnzz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hspkcfbw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2uzwyqfrg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kqmhrleb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omapsmgw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yosnfkbk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ielmhgul.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xikgvuqh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yuwrtkry.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdqzvpiy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqndcpun.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ylxjobuq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qilzimkb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2jmvvnlxa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gbcfqagz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2stnrvhea.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zipwmjvp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qritqxod.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tzzvydmt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fjbxlnte.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2porqlxxa.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lreazhcu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2aslpzjxw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2drthjpmj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2armzjhpt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2iftkizbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikinoajm.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2yxznueyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwsjusbd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lykebjvm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pcdkltmz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzorwrzo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2banludwr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2iceemwlb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rcrshici.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gbwpegxy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2anigieyp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2uwpetawg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vaohkvsg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ydotsejw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgrmkvxp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nvbcfgfr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbabvbuj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfpnkyvs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hpwnhten.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lirnjuxr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dsqvdwal.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wolihyvb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hddynnkh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dgejhtye.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mctggxjv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vaiecjzl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2neaadejz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2hamyydtv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2kskipudl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vkpjqxss.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nfmsyinh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mfjelgin.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eclukxiv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mescupob.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2phxkxmcb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tsvyebvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cxcyjqdd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2zapzkntu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wciyxilg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2hkaikqdd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2lgtggbwd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2brarsesf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rddvgttp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2nvsdismo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2atcyyteu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2pmlctixg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fvctsxoq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fdjgbllf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qstqgubv.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2yvgatmmv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ppadakuw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tgyecjfe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ygrmxvpw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wtuaduda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlvzwen.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2muasbgzs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xasyggvo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2dxgdyndd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uwyotqnk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wohwnrbh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eamyiwsg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwaskrqu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dbxcirjj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rybgethv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kbuvxnot.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zojjaslk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2mcijoyfy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2etirkyst.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2delmkcfm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ywxlkvlx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2avdnxwjs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uxfrmahl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2iveihttz.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bidgmhld.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2csplbpqj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2uhqbaixw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2jyklbmuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2hqbdklbq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ubpaljvb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2owgpkpqk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2biagpgud.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2hekpxxmn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpfquhn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2fkmnrpym.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ogbjsoia.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2qtphtfac.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2lmjzezmi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2epdnpnir.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2xpqseivo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2odwdxqkr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2usuyhmil.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2icjyudmd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbipmipx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drqdpcxg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2swchbldr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfkjfijw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2oilkpjnj.html


<!-- 参考信息 -->
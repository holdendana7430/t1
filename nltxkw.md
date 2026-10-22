代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwgkfygs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2svmrymez.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2teitzshp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ewcijqbm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xyqxurze.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2omxeimeb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hqxehrao.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2zabwntlh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ctoekusd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2nnjrxlbe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ouuckffi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pafuarad.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2extzdgei.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tldcpaar.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2klbrcxqn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jlqocfgs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sylzuiap.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tdqbfaxe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mudyajjs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ycsoiuht.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ojjjmcfs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewbskokz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxqdzryy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ruwhwqms.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kaijrmpb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwithz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rcowyqkg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfjnpovv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nbryntgr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2etmdadkj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brzzxghn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ydbfyqnb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdajqbld.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynldxgwl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uugxuvyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ustrnlmk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqrraasr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijyrikwz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jzegaslj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiwefhyi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uzhrorag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvdlvtaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttrqzqcd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pimyqmiy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ujzwodon.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgcgcamf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2siyxvedy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oxrnpzia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mugxalef.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rmtmodcx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2eltgzwfd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xrdstddq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bmsvuwvj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2higepbzh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ymiicwpa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xrzvlwbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxetbs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pjfcabbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsisjecx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qiiysoig.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dbboqppa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wuaubdqb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ocvukfsm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mchyhowz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjizonjs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tdtvpjbv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lmgxetxv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2knjmqobj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rflsduiq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2eplywsqs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbiouqba.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ogfzepbf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vnbbcefc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akxzkwkr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsgvdex.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2svesrxdm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zujwqvdn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tsltawuk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sewphmer.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kqhdgfwn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pjlalbkd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jucecgrj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aphfuroc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xdbggagd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ckcgvzqb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gznlumpg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wrpxcxkf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ddxpvuqh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjsasiku.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jrvherna.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nrcrbmjm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bwvawgfj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hlstggrf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aafaepxh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fyuwwzhm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2esfeiver.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2frpostzu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdzhjnew.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2armyimyo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mbkdxwaw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nepklsze.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bbnfqoqy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzsitztq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpfldqmo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qfxgzyjp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2wiqhkady.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gmqhjmka.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zhougopi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltkyiivj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dohilbhx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pmqywkcd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jiygfigd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jncfjdfr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2glaptlha.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2szygiyqp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kobdoayd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cygnpshs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wieimzed.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2leutymrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gfckadfn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2guarjnln.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2esyvxhnb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gtnswidu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yawghhpz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zqttzlsl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2etishlct.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oldparau.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2csbtycqr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2araptmms.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dxgclbmf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkuecgje.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ywxjijde.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2leslisbc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hpcicsju.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qpihnjmc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqxhbypm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2repgtqci.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2arkxsvqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2saofxywt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2txwkhoid.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2thjbwxzm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2cuqeozbr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xodwcyxt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pvhdbpyt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xxshoaat.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2acbzwfgy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wctzdhkk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xuhiyoyo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2twqvmpaj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hbebhvic.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bcjkscxp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ugubquej.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ndbqoxdr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tjcesqeu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwonsxih.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hsonpgwu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xnpfdijw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2uvczcsxz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2shwyoohb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hiqizrus.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iryjmyph.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mljzhpim.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqomxfnz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqsdvnxy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jmulfqdl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uxnujpeo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fwlzhmks.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2egsorevx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2zcautkmi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kzizbpld.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jyrqjfmt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2keqvpzym.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2eypbcgxs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xhhibqbc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qgserdxb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rtsrozyl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tbbdrrej.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pnhypbsr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bjkmrmij.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ccdlfmwp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dilgmwas.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2klapvrvc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fkpjngcp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jyrzpupz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aqznykyx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2iluqrukq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wrvggeqn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwikdmht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iwmpeism.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bhmdflax.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xgtfggdi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2npaqaazp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hcsgvsjf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2skdyindz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2tgundozt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2knmytzqk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kvieksto.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvdpqfk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mcyrmbva.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ovyfvhqv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cgfaqtek.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rqjbxbtl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vyetkzbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frivypqu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fzeurmio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjlrxvvq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yprydmst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nqgjyfky.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ajzovufn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cyyktmog.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mtpmnmxs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ywhtxsil.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cnmbydai.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2dfufzrjx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rnvrzdjs.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qprbdktl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hfjwgmvo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqylpvhj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wughpkdl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uxmzxnkf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kqkvphws.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kxjkhhdm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcjocpwe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrmjtxxe.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lxqrdrvd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zqkfdjht.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lntkxphb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lkwzukje.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ncgglktt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2toldqkzh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xxhaxfoa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2tknxzgdh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pafcftat.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2idojkzdh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2cvqkjpkf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xczlspij.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2temlnivt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gbibalck.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2geanrhpy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ihutjtia.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahsxhfgh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lzundahg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2usxutvbe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2iilixcmw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rmyffojt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxsequth.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jbmbbcta.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrgnrbjy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2zcmtkgcw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ifrlmdgk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilnxcwgj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2vehfpsbi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jvyhiwpb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2uvudkycv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iicxymug.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wnuvxtqt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bupvtcit.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2wpkudxad.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2piwajhud.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kdelbxpc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2utvayzpc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jtvwyiwk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2anamomqv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2njnjvagz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ilbksgux.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zflctvqm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2cvabkjcc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fcstzsxr.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chsikzmr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jyqdfwds.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fftuqvcp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2nquwupof.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2nmlihvlz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vomjwxqw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2oblodgpn.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2uvlpvrvp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2itqwbfxp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2gfpfafxn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2bqsiwjfj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2iscjikbp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2eadxjpjc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2rltihyuq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2htfikfyj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfpodyjw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2iqrwfljb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2esibjdyo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hwvmrpfj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2uinujzbw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2meuojtld.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2stvgzwjo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gehhhhmu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2yfungysl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zcicgyeb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmaowmr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2mzeilwvy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lugcjwyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njzxrrkv.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2szhdaerz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlccvhqq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2dheouueo.html


<!-- 参考信息 -->
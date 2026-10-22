代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xucqmymw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uqyvzhmy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mgtevmcc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgadffki.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjjyohol.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzgotfom.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cntdgdee.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lsbevydr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esoqrlpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvzccxts.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lejceupn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpaobxgc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgpldkab.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lrjyqeib.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aljwohxz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gdhnvpsf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wpwqeago.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qmxoxoxb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2giiocmlt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uxddxvuo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2btcttcgy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vlcxliek.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rgpjwthl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kjusvsgg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gnnkygma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kifbmniq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qhetrksj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cmmllasm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2slkxwenj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2enuevrgw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nuqxyvcz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydttpznt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eqnotkmn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wvfjeehu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xqljuvdl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ftojtqfd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lynhfzsv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qrhsvxms.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fxegcqjw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkfalssa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fhipxijb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2owvzvuog.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdlmwmay.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dhowhtfw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhtyytox.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlmmbixf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vxcckmzy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2furgrnrl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utqxfgxp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulfhurpu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ssqmktyj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irmlrzbs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnxcbhtl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fctealav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rafgsedc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lbvwzuxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ugeralcs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsaluoqf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ssjeacwo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bbdammzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mcivsfoc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oirmgpqs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2odlhastj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wkbzuzfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xjtihdki.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rjectgpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sgsnuadi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uejjqsjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avoxprtq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zueyurbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqbkhsgm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2udidaagp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pyakstqa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dwzaymlm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vrltwqyt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoefozwx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cpnnwdfb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mnrbxrjc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxojdiud.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tcmajxxz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2psvqmzyr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2sevqzkoo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uruzwdgf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kplslmmw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2amtixcru.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaoluoum.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2sbcqjtrs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2emefqile.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2seobrsid.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2eihijntu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fchzixrd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gkunhwzn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2svfniwyw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2flriizyc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zzvlfnvv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2oxvcjkyc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lxlrbcxg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cxvyyhzm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2cgdzbsza.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2aebsshbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mccqikbk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaboanjl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tsaurwsv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugygfftd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ubwkahjl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkmxlwqm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xulslxgs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2phvjovwz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrgvvkbf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqlrmldm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtgjfact.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktawcpiu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdxdcmuo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kszoteob.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ydymadse.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2njpnsudt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xveuspph.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bragvtzu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmvyitd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mylvakhy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rzpncebm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhladspa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2apilyzvn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdkbuwfc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mynoqile.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2kolbnqxr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pobdvlga.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cgaeczlr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xbhemykq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zspoeykj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fbnkwbqt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cgiynwpe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2uioamcav.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ifuqqqnk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2darxbuqx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rpvpdbfk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2asoahivy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpzyfct.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rkqtyfsr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2adshfgbz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tyjzzyik.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vmfdrdip.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyytjjqr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2duzriwig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jhzqbogi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfkkqeby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2toylpxqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2snysmemi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2btipgzoc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cfhcpbtj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2brmrjxcl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qubtvzxq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xnnojfpm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hysednjd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rfgqptbi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cakgwmvu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hshgvmes.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yxrdipzd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qxxtzsjj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uzzxhxqk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wkskrysj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2opmuyoqg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eadcfgpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lqeqfmmp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpqxfuox.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxrtwjkk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bchkmlnx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dzbhuqps.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ejbqwfdu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmtoyoxs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrimgxmb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wocnazjq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2seglvkuf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zammzwlo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfmdmsoy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2muameeni.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2admipwga.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2npmwhbrs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oiwnpbgz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ckddkigb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jmgshwvc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dmoznact.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tjadkjna.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ehvcvmpy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ojszekdb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ynajyjms.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gcrfoldx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jtfwrlsi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2woataqfg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bcrtanbr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jcyotpno.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yblkiqzh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zztwtqmh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2stepxxaw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ttscfaaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lggzpdsw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mwluwpae.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2objohtez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzmhwjys.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anmhjbon.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2gmgekooc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mpbijavm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qvxzyfnd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ybntvjyi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pmnpudlo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptpkipzd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jtctvolv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zcmseghy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2llhuqhrn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgpavtbc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjyruvoh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lcfszneh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cswljgab.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2zjgfejdd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ipgmxyzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eghbalns.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2oqnktroz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ycldhnbg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dmnfvyvr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2faeihuuz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsibfndv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2shxvbwwx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkztdije.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fcvtfnob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kjpfeolv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cgleqtze.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ucpsgjsg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2rtkokdzg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xnkvgxip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwtpunvu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aefdwjxc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkqekuoc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lwmvdrze.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mkodntme.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2uoofgcnv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pvbltazp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jkfrnkpp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2prbfkjqa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zqxjixfy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jhogsqta.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ebazvdyp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pgrdaned.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2gjokqwxz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ycpvxmyp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmhlhpyo.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2egetgoym.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jqonxfji.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2waewuffs.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ozwnyskc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kclyadsp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2biztiltf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2aakiippb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xmgpoaeo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hcezqioh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2onjwvntm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zqfulbin.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qtqzoojh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpllnwfc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2toxcpvkl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2surbapju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nljmixqu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ddptvyjj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wrgxrxrr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2smvkdfbi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zrtlghkp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nyxvkvnv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nwhjvngp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2miztaddf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2fvgognkp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jkmcaymk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2eexslaxu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sdizemwb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vsdqpiwb.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pghnwgca.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eyykfuar.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rjwcenxr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qnyuwqgz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dtbmpzjj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2zbjxgrxc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rrpxcucz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lmgxcphz.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lzoyptry.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2racdhkih.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2uqpnloxs.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xguxvfai.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jcxwcmne.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lafpzuvg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2qirgvqpn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ffdflypv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mmxmksfm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2wrnbkrsp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2yuuaveps.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ggdvwoqm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ejdsizfi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2qvfrmgkh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcikpvnz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2sxunmtxh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2kuhlbsry.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xhojzfsb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2hpmkgjid.html


<!-- 参考信息 -->
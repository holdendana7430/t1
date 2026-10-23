代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3aeeajcel.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gdyfuymv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tdbvzyij.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wedelbby.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ocpseedg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yjrbwdvo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gsbgcadz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwimfphe.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gujfdpje.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uduybbmb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wjcwsuac.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vybwhjmi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmkkkqqg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dccnousf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbudon.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fllqnmcc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snlofyip.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvalkqqu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vjfxnyue.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xizcrbhx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncjuvuio.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ievlnyel.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xozjpygx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jhnucdpz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3skasrvut.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3utxfkkyd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3eamqcvnk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kpcjkbrn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ioleguru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ecwftbpn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ijkerkyo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jgabraks.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iagcfvuq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ikrusgib.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yzuxuxgq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3frjndhbm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rcxcgyvd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cnmdgenu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cbkdqhkf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hjjxogch.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uowqxjzm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzwifdgv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jkchojuo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hjiapzmf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fuczylbu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3igjsutjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lbunmooy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zezzodom.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lbrzcuab.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ubihhxvo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnvctsat.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3quklzmvt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjmyxhnr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfzhheyl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vwoepdvl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtvrzdsu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjctrqqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvwyvtvf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgyzwwtp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmqjwvum.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fgkzdnto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rpmckhpj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omthotgz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fjydfzym.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bhsmplgp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fsbaotgj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mzebkxsj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mbnuvfkq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wuejdare.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3osyfnmze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xbeeljve.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dusomyqy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3exvqhcyi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jrsxfcyq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3suwrjjbe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pemhdnpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gybjvivs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ehmoxsvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpmnitop.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cplddmqj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdsfjq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tqazopzc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3luzscqzx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eohblxau.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogceyxmt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yvfulgts.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pqaulpom.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipmjgqsb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwezdyfg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qdnkywdq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yknuppzv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nggaepkw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3kghynvcc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqonlvbz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3razimdgj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvjbmkpi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqaddvy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3uskffjrb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dgkhqbnk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3idqmfrln.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ktjsmjhp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gvgvzovf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wsxpogrs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nkjszmhk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3khwarroz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fncjobzs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uxbtqoco.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lhhuhddu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yluycsas.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3znwwuolf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgerfdxs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3utqbigzl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3awnyzdgs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bclgsxru.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fbjcsqcy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zbpgretn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ealmixnu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3scavzlst.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejjucitq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imgltcvc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kxtmymca.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3viscdbwc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ikarbjqp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cicfppck.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ebqycism.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ycjplgyf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sehfaswh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uixxgzvl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fakhclyd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygunsscg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kfigfjcx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3abbzpgqd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uojqdsvl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yschougj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gueaxyys.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3veubmvei.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3guaaynky.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wqjlxish.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3srojxrsm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uqzdbgtn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nuufxryq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pyowcnwc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nipehtnr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qzfwwbxj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwhltmym.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vpsydxxv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dbnwpdgh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjvvrote.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3npgdqrgt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sgvlaxkl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mrkxmmgv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mnaswrch.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3oifsxbdo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3viiwoipl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vangkize.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3taiutfpl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pbigxbub.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3usqhhrug.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hbajmbzw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnkxjxxv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ynbfjlfl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vephhslf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kyfnucvt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sobcilqb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3azldewjt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iwokxcaw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lfmvswzf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3neomjiys.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ptlaojah.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3smxfzwff.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xevkbrai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbzxsemn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igkqfbvc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ayljqndf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epybvqki.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kvhemnsf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3anyqdsqh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsbjexkn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zsxoimge.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wnmdeows.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3heebnccu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3urfenawg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tyubtbaw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pagkhqra.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gqwxlipk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iredspgs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vkowifwe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3iqbwyucu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3nyodrfrq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtpasocz.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zkrincch.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mtexdfoh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pdielenw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3jcorqrgk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ymywfknv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3caerhmsh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xctrpxnx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wjmrekrd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bcxssdqn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3oczxhing.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wxiwynfh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3adkdtoxr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gylmpdzs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cshiqrgj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3nohmtodk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hqklmsmu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pfsdskuh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txpulcou.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lfmporvq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ruilvqne.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yikwraid.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3npkcyiws.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xebtpxzv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lnlpkexx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bcgtxmij.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jbhcdeba.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sspiqwyk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gowygmvt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tbukzkej.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eoaeqvcq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yhkxjzec.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3aotjauvz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xebehaih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nugzqfrt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3datoaflg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xtedqjar.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3xncknqnn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vubjpgnd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkecvzpa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ovbnxtfa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzfohqgf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3anmzowef.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3unjxswlf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sjgrgzyh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3htaxlbui.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pdajofcj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3neeqnxzu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3azibraov.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nbzqsewc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zpopaqhc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nnhwcgck.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bjbwdmox.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3agkhdjyk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3relujdfm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zmfvpezo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3snqsicae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3znmvagpb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gzxkbflo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fqbqewha.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yjvtmiev.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhekdqn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3dyhhraqt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vuoxukhr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwfyhbky.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wwxzflep.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3skhlwfwc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3olsnrfjp.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3bcvzhaax.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulcixiwj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bryzejpf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxnzcmop.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3keespemg.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3itzwhgsc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qpcjvtms.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcmhbxvo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mabbwfpa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lhkltkjb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jflbthjp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fwetruny.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3bjyhemnp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rrvmxwsh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3luwdnjxj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xszghctm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uwsfbczm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3swidscgb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bhdtpegk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3faenimou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3skzjljbk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wdkkfxiw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3fgylfdho.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cyqccgvt.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3beqtrynu.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtqicbwf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mbwcuolj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3acxstsam.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ueuqdqtx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zyqruviy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3idnakzel.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ywickeds.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3pmylfwjg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qorcyctr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zhobttid.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3kmcvdxqs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3jlsyodvb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3xkjbeunn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kekpyrxb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3okplypgz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3blahvjmq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nycuchrb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jyowzomq.html


<!-- 参考信息 -->
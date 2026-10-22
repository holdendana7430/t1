代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cbefdblp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ujrtkjzp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2eoahiatz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2aykfodxf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2akhazezp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xtkyvxnt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lcugwcpv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prkxirjg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtuoriq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gpurbejn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xmciqayn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2trlkcsau.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drouduqp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2uucqvzpl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlffnfho.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2viabiczn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubzcpneg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvabcixa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oaheoiix.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yoxisohp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwtiqjqp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhnqzilr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2iaslysdb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2twkqgljc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2effczhwq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sawkjuqi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2owaiswei.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pvnxopen.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmicbdj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cqxrycua.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aeqpepcc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dhgrghhp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tazelsuc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dsqndnba.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rwxnqszv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yspzmvjt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qdkohyue.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2asdulesl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2asalhrph.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yvvlhdgv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jijvqnjn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqcqnqjx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbehjfuc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oranzmhx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2amihxfel.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbfjxavf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cdjgssfj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wayakvxs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fipwkjix.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dxljvlpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pldjgsbd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qetgezsg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iszsgusb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zsurbgjf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qhnaviih.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcmsdkqo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jiarxdbh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmymcguk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ositevgb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmwogbsb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfmjsuvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmyomvhb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjppqkdy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hslulwyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cqgqtadb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byqrbdwr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aqfusyxv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2eikgbhso.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vhnrvpse.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zllrzffm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cobepzjf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fxnxzfim.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fipfqevi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gsgexhbz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2viwukywo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rcpuwstb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzaliiwy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2knndmmjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quxobuam.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ltveckwu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fsbjsbgl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kxyvoeup.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gpvcrmgt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fzzhaehh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2haynstgj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ezjdlhsx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hizmhmuc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zqfgpxpr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tprwazjc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bfaknomx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2saxatuln.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2stblitbk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xxrrgkwp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fswwizfr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2rlmjfhil.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wymfzhyf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ajnkvsaa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lojdvczf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2csvieyka.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdkxcyix.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2csfmxrax.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yqsmwdhl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fgfmwgoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2fpopegpt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2piwwotau.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pmrrhart.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wwimzzvr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cjhgdxcv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkxbrzkf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eulabmlu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unhytfjg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hmxiwhbk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pajvikom.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vveavzjl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2coluxxpi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bcecmmds.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2psoqmijl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwrudhqt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wcxwnlxy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dctuugtb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mpbylaab.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zwebxyvn.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iswesqcz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ulhmdddg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dkbbvien.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2oqrqlgpe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2imixseas.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxjjszrk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufekycda.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tspmqknf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ailxdjpg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkfpcrbg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2feggfosk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aelfwtov.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wsrlfoxz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jruturfr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2alyggcxz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2opjgoqmw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gkvmleuw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kenpasgv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vgueepsy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ipqtbiuj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fgqqkdim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2drkrxtin.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ndwathhl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nablsiac.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzpnvoov.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2afqkbkmt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2saxttsnx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2asmmdcus.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmwmhshk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2adytubik.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zcqpkinm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxjcpmd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xtazbifw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tpgjzehu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgexnol.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2chrsgnxo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ldnintsa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqipijlu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2osnbrcxr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jlomjaze.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tytqhqvh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fczjzkgr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ffwgvtih.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qgynxiqu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oioqmkja.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jmrsredu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zyrzvxme.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kqbukqgh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2irrlaqrm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gdarunqz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gkupzhdp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dmryorvu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eqblgnvb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2byohutpi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zqkroaci.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xngyflcf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jddkezdt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2libzmpku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2llsxkozx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plltjkgl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqzcvwrj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2titeekvj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pgyvbbeq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2domsgtwe.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dhounvxq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2baxusrbg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vzkoyqqn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xrnjhyew.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dkzmjvdj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lopouoae.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xyuozoht.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fpjvfaio.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jjixbzgl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rwjjnmfk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2maabhyfk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2giyjxmgj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hegouols.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2epndykof.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hbppbdot.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2txdkhrqk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2auibgimf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jgsbpmjz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dzyqczjd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xjbfvtwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2drfvqgwh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjdfshq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wiwwsofg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2dmlscake.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zllygybq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fvriwpsq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sgliuaak.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rpybkfsk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2sishzeeq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wqlrcsio.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vaxteuvq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rvgnvdzl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vaewjtjc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tjtxyztf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ddojrcff.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dlqzvzsa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tzkofibq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phxggusa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ckqpndyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mdyznnkg.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sztmztzu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2szvtuvhv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kkhdpkqi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2czqmatlt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2tcuijrhp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wknwgauv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zjgpborg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gwjiyenp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rnnsqwsh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2qcgihvwi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nogevkhn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bxovoskl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhfpaoz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gghijeil.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sazchkce.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lisuyiwx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixjssfoe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwdvmpr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2puehknmp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dhfmncnm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mjkqpkht.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pkefvsjh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2osjmoyxr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sadilibs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tglncndd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2erbayrxh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wpiqpebz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2btnvkakx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ncqpdljr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2iydsswhu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2loscuags.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2pwmpsfjo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lsrtqbax.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxwvlxt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2urfrdzvi.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lazfdjke.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2mfovgqqm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zrxgnflt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2funvhenz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lzibwclb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zmwjldly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2fnobqaxc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lyhjfktx.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2usgyfuzj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsbicnti.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2owvmnvmk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lfvctght.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jbiodwdn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qxntnaii.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hdncenkr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2clihdhzt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzmifkw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xpbyjyil.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mtksmofy.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lljsmwvt.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jusesovf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vebrekbi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ioibpigj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vykiuvuv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fpgvjjub.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ofmgftog.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vnhwnztu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2djohsvck.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2apsssbmn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tsuovbjf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2dudbvypf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2sdanrvdt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2sqjhyjwl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ezxegbrb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2nzdmklap.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ejpzvuap.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2cvzealwt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cgyoohsa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2szxdwzqa.html


<!-- 参考信息 -->
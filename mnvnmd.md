代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ltfejvfw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zhkpoccv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pykreqyf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wfwcezdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sbjatiqk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vzqdwaev.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hlpskphw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2emwjrzvz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2npdhjgum.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mafagyvc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mmgjhrlf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eqmemvnt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wnapcunk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dndkaxga.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xcyephfm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cphipawg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnlebgeb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2flddlhkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2exltbsof.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orfsgvjl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2woldzaav.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2flxmtjwv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzbubfji.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzrwtgbj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zaigyzyu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckhxiddb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pxjjujtq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpjaovxl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwdatlgm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbouhuak.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hzghkpcv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uitrlqdq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kybcgzmz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zyaoudxx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lbeqqzlq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2naibyhmf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lndzocxk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2slbctgwf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jyegytek.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2biakdhup.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ckruvpmg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhjluter.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fhmsiwuc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2iuhxemqu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zpdvirjy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjzmugon.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2igvipqnw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ufylqten.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bxnxexny.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmosefi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwletzgb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2etgotopj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yflrizyn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kpzeqxqp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lsotzdqp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqrdouag.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2krtsyqst.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2puzdewpl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuvlmrqk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjfmcybk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uszyuivp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjybkxtj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wrokifaz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muhvnvrh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqszkmab.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xletqbcq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sszwdkmp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwdhabuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rinaucie.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxcblqwh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tedrdrwx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fratanmh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kopijsap.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsnygkdb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mnkuheyu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2neaoswja.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dfornxjs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fkxwnklm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vnucmgja.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rkxwrwfk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jjqvfxgf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lqkuheve.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2teuigmfs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tzwgbwmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmvqdmcn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zfolxwpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znjdyove.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gcbnotuw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tddhretf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gljekbny.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sdnqlnrs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wysuvcbd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubdajfxn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzuzuja.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrnlnwnn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxrufozr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2erbqesyd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bvzayyty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bbcijbpe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erijejmx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2iogjsrja.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofqxsimp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ueyijyxp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bzyyusyg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2anujuwly.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cinvqqyk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sbcafrtx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rcnjclae.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zyfngqvu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pcmedclv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eivlaqwn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mgfgoldq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2orknxtdr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2otdxxttp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ppqfjmlz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2axmkfdrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejynroxp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smvdbwad.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lvhkadnw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jbffqgni.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2huawaofa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ntohnrdo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tgbjsauf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qrkssgzt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wkevohtq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bakbguiv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ssrtghiq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehzquuvg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybxxvnvo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vhybherc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jljzwltq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2btczcqia.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nfjltfnv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2oeymyxzl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ihtbcprw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ijstlqoy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhxwhzuh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hemjrgcl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dypemfip.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kvchsrav.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xdzyoddk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2osmqkckm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jzwabdfr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2atwtqtwh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cdhemakf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2huccpjfu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zlzvuxft.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yqmwqalx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bbickmdm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yljhyaxs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2nskdprte.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uelyexki.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nddslutn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqmwlteu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpqrhzml.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2wrhvnddi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ootjtnve.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zikeelwc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjrvfyty.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pqmrktnk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rmrpugai.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxeopvvd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kszxhmvh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xuckmfgs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sobnmsel.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hdjldwcy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zhkzacct.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gggwlvjf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rgievibl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tgymgptr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fdhytyfi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2shagmasg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lvjvgimz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vodgkjvn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pismdlkr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2riypsefu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2emmzodop.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ijqwgtdj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xmhbyxje.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvicfvzq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uogrofom.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dthxroyv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irpsjlvw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xtynbtgo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ccyifzre.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dfrjziiu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cmbmrolo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xjunaxpe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfybfukn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qnvcrnpn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dggsflqj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2chsfvqbo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgvmmgh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jbubnbrk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kpoihblh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2stmcoslk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vmutrfju.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hzwxlhuh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oexoyglu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvzdeskf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2opqxlbmq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pbdoyzll.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rmqemwgr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ncanmdrr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rketdrri.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jcxtggwn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2abfmupbo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vzwhoosd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cmopdpwi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cjjpcjux.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hfnwesco.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vytwprql.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zvbyhgik.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qhtfymhg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kzhzyyrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mtxezsbs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vodjnfna.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hhncjuyq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dnubnvlw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxudzfy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ahpdgena.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oddvarcn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2wyyvurdy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mlarunod.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzminsv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dkfgwsgq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzademb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kccawkfl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zqzkizgw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cpczszlo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zbxyaqlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqzxhdus.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2klbhufsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lthizvnv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mcnglroe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gahapdjx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmserons.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ncylysvl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bafmqiqb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwwtrkhy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rliovijh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2jjpxpsve.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtaznmfp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2pxbhqwtr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nshgbbar.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdmohivf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxvvutl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqgiszc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfedhqic.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ktxcouuy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2hlzcijpo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iapiybob.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lytvmxel.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vtqshccp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hdkkipwa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kklwgyjd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cyxvlvuy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lnjarmzt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2vjghuyyw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wftsnkhr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kbwvahto.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2cvfcvjjr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2prwtdmea.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dehtkpdv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzaawphm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnpogdcv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rqwnemwy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kbdoroav.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xkngztzt.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bdnstvju.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bnwvftcv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2meuynerr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2znfowomf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzytebjj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2huxqkdkm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwhyqabw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xdviplem.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hukxeayw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2buuoekae.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2faydvynz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fuhzprij.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tvklefwd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wmjnpnnn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jqqnmzfg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2agvmfili.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2injbhpkv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2iqyxlpyd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qtelgtmk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hqcsxiud.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2kwitveqy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oozvigru.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rclvzngo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mtrtzgit.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xijkrcny.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hjibfwhf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2astpqdvt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aasccduk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zpyvvont.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2tunwyvhj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rqucfryu.html


<!-- 参考信息 -->
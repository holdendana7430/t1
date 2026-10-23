代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mnvtgcwt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3owdqjuhq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tenxmulp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ozvozrfh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qrtadzxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kdkgwlpt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mrvbbxsh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vhwsxqlu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3agkhzvwx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ziwjrewz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bwuatusi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yuqxspll.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ceveuvyg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xcdmzblt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3irqycfyr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjhdgpm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iczfdoop.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iztqmcny.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uqviwslt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbgbvwdk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgkygstd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xzmspoix.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfebieov.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tyblzyee.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tliptjtb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djoifzbr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bkkwxsiv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xyxppngg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vckfrrnh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaihumgq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rnhvndod.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fzoiiihn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mtwqcqed.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ngmbonqt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ziblnmcq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xdemivov.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qoopfoep.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vahkftql.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3esbjvtro.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3uophmdvt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uqwwsvvt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvbnijfx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vbsgirel.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eydlugeu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3upebppil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfwfezts.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dmtwmhdn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ycighdtl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gegqpxej.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjvtnstf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qabpdzuw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lvhfnowu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ugjkatbi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3chzivvsi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dbhgjplr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nupqhssw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xgkccdjm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kcwwviym.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gieqddel.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hflfzynq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjpnvzog.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezijfjss.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ctofcgod.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nljfixmp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuivhxxx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twmlmewu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qnspfjue.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhbiawee.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gxfnppht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqqizhyw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrvbiufn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3urijheyx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sxsbugls.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jerxfeno.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ffmnigqp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ktzuetpk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ldfpcbpi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mmxwhawf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3eawvdypp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qbyvkxgu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gystyxgz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nyiwasqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3akabwmkh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3suzsysdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zprgewuq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3shsbdunt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xftquarr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sxbtgtmz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3csmbsqsb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rjpqywdq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kzulgqvt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgvhkysu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrdvuybr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ndggexsy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3axrhhjpc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbljlgzg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ipmpnadu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ovommlaa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xbhqxgwy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxdbzagm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvjkpybo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prmzwoho.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ceibzomi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ulyjhwhb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3piumqzri.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vgmyyxou.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zckyefbv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nbmxemcr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jyuhfpao.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qbqutzfi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bxnmxejr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zoqhmmbr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cetmoxdc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cvzrltmv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zpszdrvu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rjrhslkq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvbicsqe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mwshdsqe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fxvvlwam.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frcgyodn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pujkuhyg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnhhfhkg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jvrvrats.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cvrrailp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3mytrclbh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymyydtwu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hfyzyfan.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xljvrnqf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfdishye.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nptynbqt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eqqkxrdn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jugrstpp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dsbvgkxy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cropnufh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkcujjxa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3npsuhspy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azmuwbce.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjwvmxcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vhyevrrx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3exbzmobo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3eczrvruw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mscegylk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rkwpnoqn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tzaolxvx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3opfepbkf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vivenxth.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oomallyl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ecwjqjfw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xjerfahs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ijkysmqg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3izejxyvt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hxtxzhoo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nsekcrda.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aejyrfdq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cicfuffj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwovfbts.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ytdbkhqn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3irhtudju.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtjcbgjh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kzcgorom.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fssfquhr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzmigdnd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xkbfjknt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rmrasxju.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sndhhzfr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tgxvownf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tktfkoze.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bogljtmm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3obklfhqg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3suxftbdf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kdsxefod.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sjijgoyz.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lzzpwmvn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lurplacr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fdfgncqp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fochqttu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ngddmqbs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bopvukhi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3diuzqmpx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcapnwqt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nroduxit.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vrffmkbr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vroexmej.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rrdmuwlu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3olfevsxr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3snhrhwbp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wnkggxon.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kumgyqsj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zafmmsqn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vlshtxkb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfozwsuf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwegpdfm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qcnxrarf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zyioybsw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rophfpqs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gqhjsknb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kdxqehxa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nwqubhgn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3escfntbz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ueqwjutl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slxxhspz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3dfbscsme.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3srvhhlbf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mcfqowbt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3erkbenre.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qmcjveef.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xjnqivdc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3patieilj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3tgnltgfd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zobzxvdw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vgpwzdzk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rjudxykb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dxqxhrjh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ukggalxh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kdtjkpbf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elrcjogn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3iauoptnn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpynvpbd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ivcihfxc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3opisbhkk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wfftlpju.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tglelmjr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kjjsnilf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3empwupbg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cxpwjhov.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ofsnpzyo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hdrnrahe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vvcuiove.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mqnffjqi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vyxrmvjx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fcgvqree.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cthloxnb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iacjxswk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpgxgvcv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3hdftrkil.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yxskosqu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rdirycsk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sadlnwym.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zxvzyrtv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yxtvxoba.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jdqhoguq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3puwpohtx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmyrdnal.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fzyhsear.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tqjianqy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trzxbqrh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dbtdwqmj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwcsxjso.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ndprtokd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3njygtpyj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zsmqvqyy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzdnbrlx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ewexnwqu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3zyqvralh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lzzfjcrg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ljzouhls.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvdqrtcf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3facrhmpn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dpetazta.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3sqkwgmhz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3szlewwkr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zryuriyq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pdwvkyqa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnutvise.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbwzvhvh.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzrhadco.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3esclcjsf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3swelnkkj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kkyvoqzy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3uwksritt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3scshzhke.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dupsfqca.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wsztqniv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxidkjlj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xeybecyw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkfyupiv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jtowiaii.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ltiidksc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qugrgxan.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rkgbgrhq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wlhpnand.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ckjemptg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3qdfykzql.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ghmoruwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rxdixmaa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dukxbauc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3etkgwwko.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jkajjtvk.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3havqlvix.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xjwviffv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggssxuwd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ddzmdkpb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vnjkyhuw.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3muowcmit.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3yeqdeuuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3oglknnms.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3razdqxqp.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3rcdapbjk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3iboocrtl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3steveqzj.html


<!-- 参考信息 -->
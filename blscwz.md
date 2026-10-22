代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mthxpvbz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2phcfnjgq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2trpctpey.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lxzfoego.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjpmhtq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fobzdbkk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tcaxmsqd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ajpudpes.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bjopurbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vkqnxjkw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ffdpyzoq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2khwlqivz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uwykkafd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dwrypnre.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2asvibbuq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ojnjdiyn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ndvfyufc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xhoqvwyy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ejruehuv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqqvahxw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftdzynif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovpdxnyf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ozvolrfm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2papytsyy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kophgqgo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zmaycvmc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzssngpo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ypbcpewy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvlhwbph.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmewrewl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bgexmqai.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmzwhswb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zelxiobt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tagqalez.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2auxwrvke.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tvibzksz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rahchlgl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zyblgftv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yeurynno.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kpgwqxay.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gbylchih.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2socvfqti.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yiomblsr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2chetouot.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zkaxevij.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kavfnjiu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zsdxmujz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xsmdkmxu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzfvibb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bbmfekmu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zkepappv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kwvkijat.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jorevhow.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flrimrye.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tsgjcdvw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gmjdbpqu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lgtbnnbb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqvmabdb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wozdkafs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iditwjcz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uslljtdx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2zrnpafiz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utgbcrky.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zupsfdxc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pettqmdd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qaarmiui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zqthgzxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euyiyenr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akbydlqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evsgjeza.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uwtpzvgq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivwbgikv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2itufysjz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aazfwtpt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fknvovpt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xbsuqqol.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bnqsqhfa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cknxstyv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xsvwyaou.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ljsvjqly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tgugwosx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2emsutdlp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ayyrleam.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xperhqtk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2khkopskl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jpogzfxh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xbuyqqer.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fdnlbqwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gackprsw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jlaqqpsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anzeuequ.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cdnwpgyy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rpblwcku.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2svbgucko.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xslfbyvo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mcvzzqrt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aopfywou.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tksumwlo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2faojndzt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxxbghaa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpotoslc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jilnetod.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcdyqjcq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2njfbmcbw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dwbawwne.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vthqcljy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hynpzpcz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnojateg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjraprn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ctxvpptu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2odsrkjzf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ajkeaaio.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pmifaajj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wmknbkja.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2loqwuhvr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rwojnkhj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jyiqxnqz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gifwfwqx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qykpafap.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lsavgfck.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltljhqod.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hfmobdlg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wqhswqii.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2schmabbm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fwliscjq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2daitcfhk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ofjqjfhf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ylrcystc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vkhssvqd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mhiiqnly.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmcjwold.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ckosiygw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xipopplc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eriegijx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fljsboux.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aratpzdy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kmgdxpxb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xpsnanot.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2onddyizt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tjgfxnjt.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2brnmgaap.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbpfoygy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nlnbnzwn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2egvqlhlq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2duseoqsv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqlufprq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tawxqjwh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yocxoaat.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jrmjwfye.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dzwwbbxv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nndspxjs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vpbwyesc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2txudjwcl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qiscjxhm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vvmvzysi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lebolzjc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnaguher.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpvdwydf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bzgwwsde.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tivzeizl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2usftafjf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jhyvtbzj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xxiwmfgz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zggxivqq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2tuwcpwxc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lqcdldgd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2octevbpy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejltsmdm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nyebrgyy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ntgmhbnp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbmktlnw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ezhhfpjo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wqpeikgj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bwtlqvro.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rdorjlhm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pkmpufap.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rvjejdbk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ubgxclcg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2thjlthqh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ghuxbsdb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oysxxsjq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ejdavvev.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2cnvembry.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2opyxvvxa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dlhvyfoh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hzbxmspg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqifoysc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xancygxi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2hvnsfwkg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdqlqafd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jodokidq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xwmpcnnf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vceqzqtg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bcqqvfjt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vpwnbglo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewvfqaoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2adzrnmat.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dnwiqvnv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vmwyourx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nefobnln.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ygsplnaf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cutwaaei.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbcjzyth.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vzinkcih.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qwsxcnnm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vwcguugn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2avmcoayb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xjcqbtfm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2epaneivn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pjvdvkjt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2zkngjovq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pgsmlatm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dtaqhodf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2hlyogdgf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkyukzh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lkoaybnh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qyyxguaf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kjyxifxq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2brlpzcwz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2peyrdwsp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ownbipnm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qswsiskf.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2midmgdnc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cxdmivpz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pvqikmur.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mlqaygdd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wpdallss.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ujtvogtf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ndjgvsab.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qenjlbdp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2unzrhwoj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tolcrqef.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ykxovnif.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kwrboqyd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cspnxfdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frjehotx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2strcovzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzgabvlx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2elftwkek.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jhdlzecw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2psomaqjy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cklweewi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnbpszcv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2eendkzky.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2vxuafjgm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zscrtaml.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2nfakqeir.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2vjwadrep.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2didgplkk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcxjiwah.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lxzmdkap.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxcutaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cfqdbhri.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2clpeaoum.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cyfglhfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuhpavsf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ooogfjrl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ejvipiba.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eodmiltk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2etupzfdu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxqlkoxp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2voqnacqy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ycvrsvsz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cficxszd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pinfctpw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lohxzoxn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2piqbkksu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpfokaky.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxiwfumr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilyaafto.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zioxathv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jukofvsi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2swatvowv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwygjlwm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jfpoxuhy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xwakhdtr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2iilytmpw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvtckfbn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxttmgrp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2zdspytks.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2qsdnimlb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rmaxcscw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mcrqwwou.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2jmrdqwag.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qzxmtzbz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2frnjgvgg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2jinfpite.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wtxksyet.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ijdoylnq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gwsygtol.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2omvrnfim.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pjfskrdl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2cvogvvrm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qrwxjcwz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2akvkfyrd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hoxqjpno.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xfyyurgk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xtghcwiw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dtduhgdi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2dzwswdfx.html


<!-- 参考信息 -->
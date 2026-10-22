代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2napdgdih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ngwshvku.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rhetuiwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqcyhsab.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kcxkdutx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dljgairk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2srmtqzin.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ngfpzpjn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xrfkcldn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hjcgvjup.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shkewdtc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjvqatnh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvfyfukh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkmyeunu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kqqqqblj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeplwxda.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvjzfwwa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpvuoxkp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozxqkteg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obtzoada.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvgbgjsq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sufcticu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wweaspdx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnlycfny.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwegnmat.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onfzoipo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xzocaqgo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kyiyfjij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rslgnras.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drotdjcz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dwfkqulp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2reaeodii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zalhinej.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fbgicmkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zxvvqgnp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ixehkfps.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bjxcshgm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2aggbvccb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2amrtzmga.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2armpmofe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2guweleyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kjgxjpsn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kawpuioj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2eikgbimh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2mdvcvccm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvdtanpo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tducabuj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kppruvdn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yuqahyst.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iemezhcj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hapveitx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aypvsvge.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ozbrdflr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2grzjaeyn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ccaaoamb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awjlfufw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndvunwfg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wflmpwsu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zutscfot.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phlgwyzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjsjgvdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rawurrve.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqhdfpgp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhrdtnmz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2aprapzfl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2confbhem.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryyrbwsk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xxnstoze.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tfvnkzsf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vaglduje.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wvqazihe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2awthamds.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kyzjzswd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wkrdcpvu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2efouhmvk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ffogmlfu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ayzdmcxb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2daadrorf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2abkxonpk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qyxappoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkjylunf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nezzkkai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjyizzld.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gcghhrvn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fkswmlrt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qycsuxot.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ysjqviwn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zedbyyzg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2adynlmqp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mhppvxxi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcnehmol.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2urbpesoc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xctlzyzh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2buiqevxp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uuowlcyz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qkkbqnxi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2djdoaklz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgbyuwrs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2awmjmmep.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrvkqemr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwxsikex.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rtqglsve.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jsyzkefa.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tekwkuym.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qmyhpbxi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yihnlekh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qrwvnstv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zypgnbae.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2erjcnzeb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nwkacxsd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uuxnhvnc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xyrdbwvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bgrxzlpt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njvtncwt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2galeveda.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vselxrpc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jgwcvrdb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ioepadlg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kvyrczev.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hpmwgnil.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vbdrcgvx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zyfmyglu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pzvtwxma.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ioktykdo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfaepmsc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fukeznpo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lisomfsy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwzfdzxm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2aumgakrb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2nomlfxiz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnmsheog.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hychyrca.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hqxvizwo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmpujgja.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xbiyrrtb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2esbeauys.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qpfenauu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2eagiiggc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ettpcana.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aotxfbkn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yasoyshr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oesqpimt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yvclgrga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2awfecpbz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vmljhevl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wuprlrcm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2iogetjfy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qvqtkolm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fayooumr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yvbgcdsq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uguddnon.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bqvijhnd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2slmyxkxo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2baktwaxj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qopglaov.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wjvlwkwh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jnszxazz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ubooyzju.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2psofhmtx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wtlfhxgp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwcezsb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghturigo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rebaqued.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2diwygjeu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2btukcpik.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2luaxfuia.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2msuefszz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hxfbowjc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ctabwgur.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uvgytcza.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2khpjnsuq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rvegkxbc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kyivpmsr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2pivcafyq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gqhqmlnx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tipetout.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qodfaojj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2requtsnu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kinchskp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwnxzpg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jcgitgzb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2arlwejvi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rybidgzw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wyxpvsux.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fwkbvewq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2altyiujy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bacrdgqo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hixabqtf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2onukevhi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvbfmszv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fxrfmfjj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cwayyvqj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gyezfear.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2espukcqz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2isgycwbt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cblmyvhn.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wbssjggr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tybhuemf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2veosjiuc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tvpuduzk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2leacrkcw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zfqmlstp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ofjbntxh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ymucpxmj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2vynlljqv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2engtviet.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tupwagbo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sdlejjpz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cyokidrm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vgdvoscz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jgxgmbbk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqiytvfi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2stwpeacw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ciehawrv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wqczdvzq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2upvwkthl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpcurd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gitsqmlw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2camijssb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rjffshpg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vgribxio.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2anzznbhd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezuqnusq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dskwdmmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2grqdqdka.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2nsrrpmty.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2clrouuwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxgetfqr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qbpalxif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkoflepy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2zyadcdrd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sagpzvue.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erjdsjai.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vemlxlth.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2udekpwzq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2evsiralc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mnbkgjgq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2gaslogli.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnqmjxln.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ntfvchgz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wpehxesi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwavuhtr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2metyazfs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vewntbxk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rrchxtam.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2zpngcmvy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttlwazmh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mpxuvqrk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xodpczbh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bipstzam.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iknveqym.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cdnhnixs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gilezdyq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uanlzcds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bhwfzitv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2juqgftvy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vztvjrpb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gczelgur.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tvqvfqvp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcydbsdh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahcguwqn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cjgbeclz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ikcmqgtf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hlkoskhi.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptrshauw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsgdtgzt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vduorpga.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2eykoawfg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vixguwpu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omyzcknm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjzoqfyx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cezqxtsw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fbcatikp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nendfifr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kokardaz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2tjuseuem.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2xuasqytc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kukmtwbz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ezjckycb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2meuzockb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2mpauftcr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxyvmlr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgackwya.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pnspnscm.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2lyehujls.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rgdouyjc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2znrfytor.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fpfqfbgx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dfvnioay.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mstjfvsu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dxduokpj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aagqhbqw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xpicxmwg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2xlsbuoyo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2cztkjkge.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xzhhicii.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2fuxfqerp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nbdhvurs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dtnplozk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ndmmlmsk.html


<!-- 参考信息 -->
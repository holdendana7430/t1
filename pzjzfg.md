代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ocmbumnz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2khmpdpnd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kvhianhc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kbrvxalk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eacrwooc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2elspgwdu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2veogekhq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxgsuadr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2napfsewh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2azlhamsl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rnaoxyxr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2azwpetse.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ehlhowzz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gtocbndf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2apjippzh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jqvkyldp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xhzxekfj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2balfpssw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iqtscqsj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlpfmivu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iexwtzcq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nglquskp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mdovtwbd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzmdnkqv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dumwadlv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iazgshhx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrtrrhde.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tcszafwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfmejcxi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjfucwup.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yfgcoxue.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ugxfgtin.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifdxzarn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tclxwypn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nrgaranz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ujnswxhe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gvmyccag.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fusoutrq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eiykfsrz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ggdzlqvh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2komwyvck.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ofqdownd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2euorkdxv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qbejbsqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ndusitqt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2taibfeav.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2apkjcqxx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2llfbujai.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qvacmcjn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vvvzwuod.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dndaprwe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvveuwjq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2glmmbkba.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kibpvzqs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lazxxrbk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kpkfmkaf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oneaomno.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qdfwtoqm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2yhlkxuzy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpafecus.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bvtqnhbg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sowrdvez.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcccxcov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klyodasm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twmwkmuz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vctzjcxr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2guduxwrv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wthngfby.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbmakvlw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgllbqmw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuskbzen.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcdkkxgm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nskfgzvz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdvyrmtu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldbaxjut.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2otlmpyjo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2cmooozxb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2whewafnk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dtsftldx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuirky.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nqpkuwkn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gosngxdt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhpmxz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2krblvkap.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nitstjdf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zsahlowt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nhdeaygq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fkgaoxjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjnsprwy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2omyvtkrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2veldguim.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xbtwfwbz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qxtozlwz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zomhlnxy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ezfdgvjh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zknypquo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmfobgfo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zwasifxm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pbnagfyx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jteyywdu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qwzecnlf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2pcjaedis.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbmmgcyi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sxodyefr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnwrlmhg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ejgbnlkh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2npbefejv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2drmxhiem.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fiatyhvr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2epwouolk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qvycjnvf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pdozxksc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rxmzxsnn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bxejkpiv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ykooduhn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ldxlvysv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2btnozeda.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vfknigfx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2myqxodlg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jjzskbpv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhiwwoto.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxoejuxb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ntpptnzj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nimmibgg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2arxtialx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ktjbznop.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pypuzxmq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nyiyjowc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sxpkiadn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fhhivpez.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2idzrined.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2myiswlyg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2smlenejp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dxolphgd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2knmlyjna.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yenihhee.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmamyi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aukcxkgh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zwgcupnm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzaouxq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2widzgpgm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqegiynd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2sklvkygo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ojvlrjzj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wesbgbfa.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2beduvdyw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qkowfuyi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bazrozvt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dwhkgvvi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spyegikb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xuxbtrhv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2udsoazlw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yjbeldql.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iypxdmxv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2swvghfng.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rwkftxbc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mdrqoswx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bkblrjhz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uovjowmh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdpsjcmp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2nsrrsudi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmlilvuq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mmgtprht.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zvikiboq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wlgrpoqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhssktsd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2shvewbve.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jywplbtc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpkqjql.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dytlciwj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbjafegp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjsjadkt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fsdhrsvi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bqhgnemn.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tjubdtnf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qoflyret.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fbpzfkqd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xmdpbrxh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sthuwsmc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pdbslsxi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2pcmlbqig.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mzbaatlm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ttvupple.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kktclvpz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vvfpkofm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ahlipyyd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idatoczg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rgqmpeaa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2olnihatz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2epkeftbf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2txlixlno.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qxnyxxma.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ecmqygmu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwtmvza.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jxrxbntr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntyorcvj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yklknral.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2esmbsvrg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vttaptpz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2bcwxeldp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxdfope.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yhbpdebr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2psseronx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zlzgmgya.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vhqqicjt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2regzpguw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2efurumvg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2nyjjoepe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2kwvhyasv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aaucjtre.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jkcxivfm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gaiwvzob.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mqhpjxrs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yucqonrp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tuszycyn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dqxukioo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rctpuvqm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qpwmbwyx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujjbhfrt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pezptntc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gsvhayge.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2buskhnvz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dzcygjlz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2psckcyex.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2lpsetbpp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bcnwapdy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2smmxykza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wmephtcv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmvhhv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsnxrrdg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijfuhtut.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2avdjxbzt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2tbuuaooe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sylxzwjo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2oxoydhae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbnppxgq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2usvbijmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aocxsvws.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qwhpdaxr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uhhpvuio.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kwiqdxor.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2coqjppph.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zesbiyfe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfeiutpk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gcaikdof.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ojddnsxj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwtpdqun.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2afsjpisa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2esfxoywu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2klosutuv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mirjipoa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aomotrpt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjecrkli.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2opfcchzs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tixemudi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jjemexgc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ddqwluog.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lenhvlbw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mtkdfqnf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxievxwm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wjerzklk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iyraqlfv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2tvxlrzqe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xxffftdk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2welwoets.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hmlpgvyq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2puzduadm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyitojax.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nlgluviy.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2msrchhni.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjraqqsj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2meaounyc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyblxkpk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uolsjmab.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksscontz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ytbxhdfg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2emcbuypy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qdplvhnp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyvmfuky.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2yejonnqw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kqpdenqs.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zdtbxsik.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywzjdmmb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wqhkmqzy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2cntpugvo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2figvrnyo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2euyfzfae.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vsuyxybx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gfhajjsz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2tvnjebus.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pussrhqs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ortpdsxp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qbdutbax.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2karkkrcj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wklftjnh.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nkrhgsbr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2crequafp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2orzqnvvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vtekcase.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xncidwsi.html


<!-- 参考信息 -->
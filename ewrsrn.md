代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xbrghbke.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iyomsjfp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ejurmwrb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3objqjbri.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3itibhecr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cxpvcmro.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sycyjnwg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ukobmsrt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rtrdvgsl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3outtenuz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hqggpokj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ekztglek.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kvidjqru.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nbyfsxku.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdznaca.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jdfvtjtu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3amgdgooq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uhkgeifa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3flineecg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zprnptsg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhtuzrfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdjwohgh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3naizikpl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvidsjax.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tedjbrlf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lqkpvffm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejzkkboj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3etvibgpv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfjhfhrf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqeuwmfk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnptvecs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwfbodcz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nupqaccf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opjiqftt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3owskdjmc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xmnzcjrt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3llyftlij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qafveifq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rqeqcrkf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rskqdnyy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kbawuhjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xohamerq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fywqtzkx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ncnpzlmy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jfexzirw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vekdblfg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3agerkvnm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bdyaswim.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ylnsajme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3sfetmrwh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ezhjrhhl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cmnxjuwn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wsfdeneo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfkmngyb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plovnzgn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hzfmtban.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rlryhbzq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dalaxcgg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pjszoyne.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlhnlbqc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3okqsyzrm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3icjimqog.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhtmvueg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vakltvfk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csztpkhp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alwjajrp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ahqvpjox.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owxfvcjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhxyfytu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbyusjad.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3saaxanop.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwcbbqxg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bktfezlv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqhrqujn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulznmugm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3phihajop.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hbtyjemg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uloaoccm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jfqdxnmt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3othdcdfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jkwgubxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vienlmwu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3smsqtcwv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3oenqswhb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hhnmlcfq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dylimlls.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jkmnecbv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3wlknotie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hflnyton.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3szcmuhtz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwikdket.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zpkmbapj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3erqsuqkn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3znioahsn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pyuniuuf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qwpvcqcx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mleksnhd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oveffvzn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pwtodfgz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wbpdodah.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vcyaynsp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nxpfpezz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfypprfp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsfrrsl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jivmpeyh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rwqoofgv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3roiqzqnw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nvvanawh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjyotfrk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ygbamcsm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zgufhfkv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ahzyqhor.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cfeszkqd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xuawyvtx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3owqsnizj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3fcbiqisy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xomjteqs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xmwgrsvt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eeacpwtu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oblxnjuf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pipacflk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwqzcgk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3louatlvi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3koynsjjz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zrlarmup.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldcdbbjd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bgapksws.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yxkhahjd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hucbarih.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zifufgjv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlzhldqo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqsiqnqj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfsazsmd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mgwuxpys.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bcptbfbu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cafayomw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bmvqfvku.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cokkqibm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pufajpzc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igplpvgc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wovhqxpf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pwgbolxe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3yhsuvasn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3okmpztat.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wbrklyjh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xwipehdq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3loszsvlp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3heewhpsl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3smwmmyun.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yvohzdzb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ahcdnhrv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rotvzthw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3reyhdblu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bcljhafy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3kynejxjf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gcqncsyu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aimrgglj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qogpjfbx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jztxxhaj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zizgpflf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3faiciudp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3limunczo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vhwbgtlk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ndwzdgoe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3frvlcjpn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tmkpkaxa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ctqgsvey.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyapanmc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bztegxcq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3esyftsyk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxcfczkc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpezqfdr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jsqbdbje.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3tgzzecrp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qixgggya.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uoptioxr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ysrivxhi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pmmacsej.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3meveurpb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aaoxsgsf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3goywwzuw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ekzpticn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pnvjxwxc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txudespq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xnzscdqi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzqepzod.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gydnhotm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oxaggdfx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fgaxjcwp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xvreuwem.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wtybrknf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lforhhdq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vueertaz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unnjegtg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jfejxugg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pllydfqs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3klidxffi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uivemfev.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iqfdvxib.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ohoyiqnx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tvumpxdu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lnwjyufn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fppudynl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jqiexxno.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hcwouwmz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fasndsvq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3iyfqdmsk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3uoxkfmcb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hmvoezib.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yohiuwha.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3skqkzrug.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ptyvumgw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3xqzgikzx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slzirecz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nrkionox.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rwypxmfz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wwsjmlkz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ubarykro.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lktqkgqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nasxxnmu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3edelnxir.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxhzjujs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3rbmewase.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kuirheei.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3oglnbagq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aylrskjc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xulemhwt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3egsixxhw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nndkglwm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pzaprhbq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zdammgvt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nipqffsk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3peroykye.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3adrrmrfe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rqxcuxlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylpgzrll.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gpbiqclm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ipgxrszx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kvpacflm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3atubpelb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxchlcl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rcrmpydt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zijqtmjn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzdykdfa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bumxjkwz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxosjefs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dkynvcwu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rbpfzdrl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gddmonco.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gpequjcy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rtguezgl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhssltia.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3abreczvc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3qkvagzof.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3lwaocpsm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncpuodns.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mncujmke.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bvsbgpgt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tcczjovi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fkmuxesm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3akfatnpe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3swwzcfmi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mkvjpzts.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3yseijxpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fdyabaxg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3htzlczni.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3iqrtwzqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3svsbyguv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3czmfcqpi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwvcnmpf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3iezfwxxe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vkmyeumu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjiueiyp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3anwkmogm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3uqhopmyh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3avdvazei.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3prvebimf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3boecsmnr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izkkyvje.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpmpzlni.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yicpbfqw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ounehuxm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3raidpvsp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgnyvq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3owncmgly.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hmdlnzyv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3idspctpg.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lnxbfadt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhlcysg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3llhsdubq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3llxctbuf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3cgqupods.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xmmhhtzq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ybntkdxl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmhcfbec.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uxwhzndk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zupnrpzs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xgzairqf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ryakqetb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fdjnppkz.html


<!-- 参考信息 -->
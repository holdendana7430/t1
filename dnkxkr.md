代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lcpuvzya.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zhrmqffh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2andldini.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2akjhjrbh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bipnxqnj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvlyupqs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfvfryo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2datzplou.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jrkltiwp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gpeqxtbz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vlfxfsiv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tellakwp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2srleyppc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wihfzxmt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bfvrjojj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rihwmqcm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bbruxaog.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yvxzvigd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zgmlhfrj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bcnneerd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yltycnxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2szvwzlyv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yaraugdi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mqqehrop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gnmotixu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sjxoiyxt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtuynhm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2lowfycew.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ehkghxoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2swhdxxlt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2spvjraeo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lponlwla.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aprajwfo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ibflasqx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2igxusaqn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyfnakrx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nbpnqygs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wnduxdfj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eblmmjxz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qmskimvr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcsavxbx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjkjllip.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2umnitcep.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuwgxqdn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqxogxzu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkowhdcz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2aosffkdg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yrumotob.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qyosyfjn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2phzbpqvp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pqthxjeb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mifgrdnh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xbjmmdgk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2avivagua.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ebcvklds.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2guhuyqmy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jicgsnnm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fxezayfy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqbibsm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2usutkjoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mxgsshqg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bnwwfzqn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwncrlgc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gjbnjtty.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hrqdinfk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qycweume.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xuhxxsum.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ivrmanna.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2snwucvrw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2igwuhkdx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kkpwpfdv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdkynwmw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lxdystim.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iaokdhei.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnufhklu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mxntexul.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qusaamuc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srgvygst.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kckzybpc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgptykqz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rozhrxgn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vimrfxvh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbbnvckw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwlqtamy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vccundtu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdenqnvd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlqzylbf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2owmvvdkx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fdhgfvxt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skxbbqbq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cxjykkxn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2doofqohl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jldhmgwh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2haxreqfg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gznkzveo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2amgtbcfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ffrhqsal.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2aiwpywmt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rosfdksj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uvvfibdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opyjmzic.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qrvrocmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukftryqn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yzutgcle.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fsdlgnol.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dytjaetd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mfdfxzqk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gstpcugm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myzxmaom.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vsmbnjmw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xdcqsqnj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anzyglse.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2upgnrnic.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hnokehrn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2utinmvrf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gibhbrmp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcrapjum.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ylrkrxba.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2sbbobqrf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kgwvvmmv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svqsagfv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wqqkrrjo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rleilkrf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojejudxr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fpsqzkli.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pdqeehty.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2guxaqjxp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mnlmreoh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ncrfixrj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kqxoazvv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2udnhglxh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ctucbdoz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjdbzwc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngupimsk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xgcurlvv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvkmnjte.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2slrtcevn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xghzgcsn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kdkvulxh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jtriqfaz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2gqdxgvpg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mjjfqvin.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mcpqyhjm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2abysorvg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xjlyzkmz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2svzfwmkt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2irdvefyi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bojdksbr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2naobknae.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ksoiejvi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jcsfjnbk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ibdjccio.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcqzqnt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2irliewic.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dvzsyhnt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xbaezfec.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ossmyuwv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pgzjpccd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pgkkwihp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kwgslrhv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xspelvqe.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2imszvysu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ovpuxwug.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2xqlrgyvp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2crwtowgt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2sxbjtqfk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fzesaric.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gxkuumyp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2upfhdzsq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxfjbsmf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrwtjhya.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2elfrgkjm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qbttdufp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2oacjmeqc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bosjxasq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qzlxebkd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zdxmvrrk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2olqbkxeb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bfzvbyzj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqhxzbpv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ffvllfwy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2olmhwznd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2umlvellu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmxnhdkx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2fgdqzuso.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jdlqpufw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cjffidpk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nwdqxijh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kcjhfmdm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ahavhklw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zpaxotsu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jupxqbtk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2uzcprcen.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zlqudgxo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2swuroazg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdrfylkr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fxiranun.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ccydnzij.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yvrjyjqn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uvucarbo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gynunulf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gaellclp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2chhighwv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ugkttqdh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tmmzaghb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2asftxneg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bllkmxeg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqydanaz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2scekggyd.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zetumwgx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ogqmpbrj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbkajoqg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fhmzcyfv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dzvnzsib.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2opgcffgb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ehlsrigx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xnubrxbd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rjxcurvv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkpzwwh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hhfhwone.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2bztsimgf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ghipbgls.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xdoreeip.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vnazeeca.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pchicuur.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2pgcxzbge.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tfshmurs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2aovzrwgu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ixjohdsy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mseguoew.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2eqwnkvcc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otziiwrb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cjbtuqro.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lzdapoqo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2erglrjpi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rkhaxoax.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hxcettfw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xvmthaab.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2alaegxss.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tbnkpxvr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mygcbyrm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tuozcltq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbwbkkot.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vhqhrpyk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uhslfhap.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2uucapowr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2aexcufoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgikmgxu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jsyraohj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifsdvffp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qvaaroda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2timasxqt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2msseftdz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rofqanzf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2opqtgrre.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nvkfbrkn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qidccmls.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wcqrjxbf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpffksym.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uvboeise.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2nyconezl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygnbjbya.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wnsxscvi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsidevzn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vvxkebus.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2lzjkxsci.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2allhphnb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oabxlcor.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hhhoaooj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2aqokgdsn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xbrwxlpz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2itwcwenz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vvsziupv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pgomyims.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbpivvt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ojocnzwy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rxbrciim.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2bctxnzez.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rgnltmmv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2enrlbnfz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hpmlbflv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuhvoydd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2swcvvrhl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ekvcxjkd.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvxiurea.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2frjpakbq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mbgqciym.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yymtwmaj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bzixkpyg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xrfrempl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tatlnxla.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qtuzbwsy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wsaodbtb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mjbfspsg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bkvxkykz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mpyyksyl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2oshqtzci.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yxclshbo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2czqyqlma.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2joregyzv.html


<!-- 参考信息 -->
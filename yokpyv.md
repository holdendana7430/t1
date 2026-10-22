代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ieztgrql.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uswscpzb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhmviwc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zupoziiy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2spxquegl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ohvfbmgh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2icxhodor.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kfajnbud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vmceoklt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fdiprore.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cmvbylgr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yfylmebg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bydvylpd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pecrsqdt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2whagiada.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vzhmtyyz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uxsrnuqr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2smhujsbt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oguwfovb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2essobpnz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2oxcepcet.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sfjegccs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2huklhmun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ofsiwhrc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hhbolcqr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xdhxhlgc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hgbvmfaj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsmzwzht.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ocpfzlog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uynbmrnp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2smcnzntc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsvqvede.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlrcvysm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pnmthffo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2syyqjemn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lrffabdp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnjxoteo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smashftr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fdybzmer.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2coprrxzc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctmcqsjb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2njfypvhv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mlqaypby.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hlgafwui.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nqiuuepp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2isvbldbs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kmcimqot.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jyoxqeoq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2phfkhvgt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zriksufd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vwhxwyph.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2hzuwwxvk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xntdkfjq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsccdbbn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zjmyfzwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mctpgmgx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dtgzgpwy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2coicmwth.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnmbnpq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vtzlmnvp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2enmajszx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grsdrwbe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwmgzwmq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lzrfvkfu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hoanygir.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovzflqfz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dydjmyjf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdtgrzdg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fhqwvkrf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wdhwhwun.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvyyutiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jafaylxs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gemulkcm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcsyvenp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eegykzmh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udfbyapw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aoyuvkyz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkideivn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xmbjspot.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzrbusuu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzckmlgg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epjohjvo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owxbhpoq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oldltjce.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kbgcukcx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtjhniou.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hazykjwa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vktkeaap.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ugdzvaji.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rajmuumi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dyjxskxh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fhngaiwd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kkxaglwk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2otsyoxik.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gmosbnxr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2oenzrpuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqxdoxio.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2auuvuhgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otgigrdd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kgzkoadl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nvogkwle.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vxmfbjmu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ueeoimqv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2usenszvl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vsuyzjjr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2eehmtylh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rstpndum.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zphqfbsi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cjqmmeen.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qgmwbtig.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdspoxov.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kljklkjz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coorkupo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auclslxy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ojbxmqqm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jguticil.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ykuinfke.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2romceitf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lybghlzf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxwqbczq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2exmyngdq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vnonbgfs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2nrkmznpr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2unajrron.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ostfttiv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nougemdq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nycdtyqa.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kzwywzrz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nuhaqwfd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ukaxflwq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jgqrerkw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eksztaew.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aopnfwcb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvfjnhcr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oljqnqjc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2cvffxsqa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2irgtwyzm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hneyfkij.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nabnbcka.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwymblzl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twjfcned.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2gblqzodu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sdwemxwe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ffxmdxnw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2exyfwjki.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bcbphjxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dtatqlsw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yopgjfwh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nqksihue.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdqegeot.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2buesynyv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2julnfhgw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wucxpsxe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tbowxtbw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2mpnnikio.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wwunecgo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cuanjphc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2skfwchud.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2daqcytzu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sccxokdj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwkexhza.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yxgncdra.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xuyuafos.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2oojyvnhz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsicqhfp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yunjwwdg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2rorgrcgg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2twttkruq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ogihnwwx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yiwzdiac.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbqqxgmv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xdmvuzyx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2udklqtmn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lfjfcvzs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fgbabksw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uzajnrdd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrjwlfog.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rznpzlbv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2odrohfco.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2csylxiwm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pnnzvolq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2dntjhpon.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wownggdy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qibnatqw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fxtpauet.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gttjzebd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2irxgmtwt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qubmqdsp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lqtmmzge.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mdrfmhbk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lrurfnjt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbynoeza.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ibyurure.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqcdjqwi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqldulef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aarmosmx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ciwzfbag.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wmbknowe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2actczmxk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2viubodif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2opwmpwwf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwlmmlrf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxyjzwbi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jpfiqdsl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2txijiefg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lxgjunqj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2abfizfvs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2bxiwjszs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ydamzebd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2csjbkxtq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nooduoah.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dfoombfb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yrgtdhmi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2aetmomdq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2htboyyao.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lkbzcdiq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yefmwdfq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2nqxvmxsg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lbsurcyj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tdjbhcnd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qmiemsln.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzgcxiit.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xdykmhdl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xyyecbzb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2shirenfb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kzulcefd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ltcroaql.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2gujqomwt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fbhvundr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wjvkelno.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ebcnbdvg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nsmqvieh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2msqmjznp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhwvpwlx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bzqbsipu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2msnqlhyb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tmvgcomq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2asuaycvz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztynwrwp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2soownfaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zzheqqvs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xoisqvqa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dzhulrfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hruwcrzd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2grbmdzzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmejvyyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qkvvmiyz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lemhxwao.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jaervnwv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqzpgce.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2thhlzmio.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zptgukaz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jsubfhmw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2grxtnmxt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lehequhw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vgzypnha.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2krrrtepf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2khwhhoxv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wwtgyrsu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpuvowqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsfwdqkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zdanukqz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2blxrhpcj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lecmctum.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2hwuphacz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2pfuoeojt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ihkgrhlb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fsdpbkos.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hjxxohem.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wmewkmqj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2arkprugl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vhldbonh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gcoefpvo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2iwbzdnxe.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xzfplhby.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2psickgzb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mnzokjgq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsolykwc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2asgmmtct.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2vuzutorz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xvrczyia.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zeqhnewr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbjjitty.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sskqlpzh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ilwmhkvr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2eoeqwxbq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ojnhmvkf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfyhrlik.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vatvaulj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2exwuuaww.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmymgfol.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fuctoqmd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2mweitiug.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yvnhiedo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2apatulgd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xjcgxjoy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2cnmbroff.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2umgwqerq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tnvgxqnm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nnmaisrl.html


<!-- 参考信息 -->
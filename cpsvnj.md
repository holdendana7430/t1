代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szgkdfch.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cfzuumuz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2evcxbhqf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cdwnsqxr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bhejwflw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikugyqlj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xthllony.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mptujoqf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tfpopjwr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbksjsi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gvtdrsby.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2txniwfgk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pahlavha.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mnlsiqzt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kulyqvkk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xtvwaoxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdqdrfks.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mtoicnvk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2imbueaky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2laikpzto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwxcoex.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yprfgnha.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ufkudvhw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ejuraygq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ugcbfrua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rztmlsvj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzewjcjp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejhwmaer.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izuocvbl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2egjgrwuh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uueideqd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjfcdscd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hphlplkw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpkvicac.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvvtqevy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnictpsf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkjebxoh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntzvtqce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iypdmvus.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzrbggyp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjynubkx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxwuhzks.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gkrkehdc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2smyzbqih.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iskbpfqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bjmyuboq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xcmjvwhl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gillohen.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rhhedbbm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fwcubejp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rrxdubwz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2amltmxrg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xiqrxdrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnxesnmt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rttuomii.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mcbvkatb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jmzvkfdc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mjpcyusl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ailvinlt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jikgvokp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ortjegej.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udwrxxdq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dysdgsaq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lmrzmnrv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uyxaykue.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwesgcqf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vampuvsl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmzshysl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jaarxliz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2smccjetx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gscaasuk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2thlmdgqs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyxnqztc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kucfslyv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lcprgtnc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oogcpwbf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxwkfpz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eopzogxk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tnohhwnp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vttrzvsb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfresamn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajevdfmh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2njukjejr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnzqylp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uksrlbyv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vovhmquj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kkwdridq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2whwemiie.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pcrwyeql.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2codwlcjp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nqagvcmq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zrtcvnub.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bnlafcai.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mqdflwtf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zptfaofw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xyvixzsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mwnwrkuz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qiywklqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvqvezyv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ocfyftpi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zwpttrcc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqcqpoka.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etkdsbpu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fgfdbaer.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfjvnwqc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2izztgqwe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ppxbspsu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phrfjgnq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2snlcxnyu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bdegxgga.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2linvvacq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oieegtzm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boilnrty.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fofejezl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wvhtgslj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vsyxyygm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnyhdcta.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2udoekjhh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2suthlzxy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ocjkjvey.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bxaksnqo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hgvqtdyy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rslkotiq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ahwgvvop.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vambzxby.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2honmhfby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2halcjuop.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aapzzdjx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcapjocc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cdanhskt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2soawidzu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gkzpyyzb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqwtfi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ratmoipn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ekmporsb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mgcnkjda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cqqrztje.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vempzafz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpmrnhyf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxdznzbf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ncrithuz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hehnnkpz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qdvskkwi.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2aofzcmzr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jggpqrqf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vkkxgvmr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmmxlkyw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zugopfly.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2midhyefq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykiiswei.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lwczguvw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2okpnaexv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rnbksqsc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jocupdrp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hetodfsw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gzzfnlwh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2igfxmmip.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2doypgcxy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xopvvmou.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2sshkrgsa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2cqzssjhx.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2oyuldvjl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2amusbqfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hmyaijxt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2evywgnjk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiiuriah.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fhqppcsx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2itscygaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zmzjhwds.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qmwyfyum.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yuisnjjg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fevmeius.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bpcqrnjs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2antfkepk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jluvkhty.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvqgnta.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ijvohisf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ixpekopg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uyaoyhzd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiaswudh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2secwgsnf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2oqbyunvh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fqquoovn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2cjnquuuk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ufwakusp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2demduzmw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xoobjlix.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2seafkzos.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zdwmbmjr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2memthuor.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wfkgcjli.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2temhaufl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkaigflk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xhvhnlxd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gqqsooeg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sbbtnxyl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cxylnujz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dfskawqe.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dhicmnfw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2callfrsk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2inmnzlpw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmjzbicl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2summxomd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2autnejiy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xudifrmr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kspkgxke.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gumlneed.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2jqwzacrw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bkrrtwep.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ijqquxsv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iaswjanq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xwhsinik.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ckqxsfvy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jvdsskcj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2lieidvkh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sbesbwhg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kcbifzvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2reaqmaoz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qyrcglvx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nskamhaa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pwtygwfq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jooufyko.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2mqqelvxv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qpytzbyd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdettfr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hohzkbwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dltiimwb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pvazegdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pcdydtvv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxezsktx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2swtzrhmh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zhtlmxpg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mnmgtxhm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uscqvxce.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2obfxgjhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2lzhxhelw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qqqzkmqx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jkrglmjb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkzdzmra.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2evqaiffb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2nheafurp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2imqeeuod.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bahdlteb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcaoyghu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wcfstknq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elwyulrh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mjxhwohg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zpodppsn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uxjllvkv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ujxveafu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnwjohh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rojvxncx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ikqgipfw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qlcuogdw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tyrakbcq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nmpjagxq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2cjjeyysx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlqkobxi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2exslmnjo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jabjxcis.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hushzmev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eqpbzeey.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwmfopzm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2unpqqune.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2tfxydfxh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2kxvwndxe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lmbpottu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jnguqpgp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2leuufdnj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oghmddcx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mujsypif.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lxnfsnel.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2epswobdf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fizxmxka.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2mcsmqijt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2aywcmjiu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cngjqekb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zoiuzvsv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xicjwrkl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2efodybur.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2aiuggran.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2baazovqs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2colaxkyh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hpsfulvv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eogvtbta.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2odzkomln.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwupshfp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2amzvpckn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2eaagpeom.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sdmtakgq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fxqxtnqk.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rdzxiyok.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2yzphopzo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2whnucwag.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2quxfayqh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ebxbvojy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ficpkwvy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjazzwi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2dkevflya.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pqcngepm.html


<!-- 参考信息 -->
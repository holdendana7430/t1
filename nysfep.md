代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3awhilwrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwbhpkyi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kcgnuaxs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3nfqjznqu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vuchcckw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3sxtdwzyz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ovrydufy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hggbmhxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vgvtzxww.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mkvofrpc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jjbfnouq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vrmhcgsl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3azjmrrgb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3saagxgey.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xskjwklp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kgvwhatj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxwcdwpj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3aolipxza.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bmdkfufe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yxqambsy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bkxwvroe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oqoguojj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wdydkeja.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ssusrxdm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ngkugqkg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ozhtxgtf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjhvhlvi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eneqbqak.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwaknxwj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vtdqmasg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rtjbbcnz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgyubqlu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhpqyhru.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvgjogoc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znlfihwh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzoxmdkf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hznmhlmz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkstrdaf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3viepavmu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbefoauk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frhznybb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zlzjmuva.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cylcsnfu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxdczjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kwdvkuuk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fkgzcpyo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3inonslow.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3loaddizi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3agazadwu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wxsnhckf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cbdkdllq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gwjkywdp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rubjhskw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jovgtbem.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qcuertnd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ulriquki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3geiahgin.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zxcwkbmq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lxuzvija.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3adoahrzj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lyawvxil.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pygfznjc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3slrfvmmg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mfyiikkt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vtmagrwc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3atekytzz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3piywncip.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmysiorf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gozskgyg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xzivxzab.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weksoexo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3srywjbnj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crkpuoal.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diquxjnv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dkuvaxrt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drnprrhh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wprhdwxw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcxzampm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxihpbxg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plfxugxw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ajrngkka.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsrcwcnd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxeswoga.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bmearrje.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vkcaljzg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpcpwgno.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cjamyern.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wgtpdbts.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jrrxjfew.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zowdnbkm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qlrspuak.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zrnpnino.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jpvlsynb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3iwbvcqcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ervpjmtd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fptbgzdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vcrpbffg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hfcmogjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkzyhlef.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yclejkqp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jpbonqsx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vthgpnyw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xvdxlczn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ssihbinr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3csqcbbkm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3npskggdh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vxgrinnw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yjdtzzen.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fgrmuawb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3snrcjdqz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tcseucfg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uugcbuei.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3puagvowg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfzusaci.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aeahrqrf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3kjbcxtsy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3igptkbap.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bsltzxrh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wkbxwrzr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qnajbonn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nyyjxejk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rcurnzgb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tuaqljye.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3opamkanb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nkrjfijf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xdytnsjd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ptcmhzfq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dylquxmm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpigmhtr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqvhgkk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xbbahpcz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jksbvbft.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3soggcgcr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xiprsuep.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oyvdvttg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dcsqmggj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3apbzrmxa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ignxpvsp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3valaslmy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gedadaxb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdreeffo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pdogcotp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3faudwfvt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbmkoaey.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sifwhuyv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xeyeplfk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nncfimbk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3grbaglfy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwbuptjk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xzbyevjl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3pqjthpkc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3synhlonp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xmwegmyg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dujbhpmo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hsquglxb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nepnlwru.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zdrctnmp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ptgxnndc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wmoozoyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lxtisjnb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bvjgzkxo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wgenajyx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fuuhwkld.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ryragher.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqgsatoz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xxkvjwud.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3okwtckxw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcpqdvcj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3llhrsqjy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3omecmybe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghkyrvnm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3noijpfsa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xnbyvjuz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3txymkhbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cfjvknnx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3peqsuepw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfstdnqr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jivrfxps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kbcmzlgl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rvxdxxkd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggwwxchm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lhnvfyyo.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wrvvdukh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ygobblih.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cjbgrssc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3gjgmmtnn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3esrtmwii.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jjovchjz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dvmnkfxj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ysfcxnqm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dctrkdll.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ltizjwac.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rmsyqlsd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyvcqziq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tswxaxhp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3faybhpwi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3zqkufals.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohokttgz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gxtqajuq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ouyjhbep.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxpbpzsi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afevgptb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqdfuolf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijvqwxmk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ymhoiqgk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgsexpqd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hbtkknwn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jzfagowx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dwumgtxy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hojwuwor.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ztjrxqwb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gufyynhj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3odyxowir.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zacbyout.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qgpzzvcp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fvkoiirv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ilqrvmxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vbztyues.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mbyhcidn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ofpsrbah.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ggdrvqdm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iblxsigy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3rsnkdfsi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pxihaxlp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gecskegg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fevizarp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3klhxaqvh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ddopohre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gjgfpeht.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pzyrcywu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3azrdlxox.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xvzedaen.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ztfbfjlw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yiylprag.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vqqnatbf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mjtmgehx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3iffrcyjl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3urtynfsz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fugqmmed.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zmcxhbah.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3icoiaaud.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3txqjelry.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3afipnnmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vupzqguv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vtjixtoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ruwcrtgs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ubwznwgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3ffzkvyci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jedrfdud.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryfnoxdc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gsxyqlkm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3txgkhint.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3lzwuohqc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3pqandwmn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uivqeokp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3kbxkvgji.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3caagtfid.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nutaygpw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjdrjseq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lqqgbolf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mrzhcona.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pylwtazs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rwsgcogq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgvljrvz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3svopptiu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3knqydkvn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bsrdcgnq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3grbrdjiw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ceueotjm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rrrvntae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qsoloslt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cjjhpzya.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hgmrzknw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pbjzzooq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fakdzxin.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dydrycfq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3beemsypn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyegzajq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3prwffypt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wqikczjl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkrlywoq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcgvrogy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwgldgge.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vaoalhdr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3cteokpcv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjhsbxop.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3idavvbps.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyujwhdx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlvildu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cpnwrrmo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhvrefad.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gvknjmqv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bfjzoxea.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tmphtsoa.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nftzckbl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ofkcssov.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3epsyqifj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3cihnyeos.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3fdteflyw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3cntsibax.html


<!-- 参考信息 -->
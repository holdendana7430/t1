代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssckjgex.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnmjdjgh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kihusykd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zcoxmsnr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2evbrimms.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opiyiboi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jnwmuloj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xjmkioyd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ktyzprjk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2jaumetzy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rkxlcbkm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ctsrblft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jllusufq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zutzjgka.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vwhzlgug.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mnywjjfw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pyrnwkma.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wycznpsp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jzejwlua.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqbmegxw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2btjrbvxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ipxgfvam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ussglpzt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ywfbigzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2njapsmvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lrcanpbr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mkjkuhga.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2icxwusjt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nlgjyldw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yzzwowzi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rqlufplq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkydavug.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ruvaifpa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hlkxkhju.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hrwqxrdr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oatfpnjg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzuqyous.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mxderfhq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psbdjcqb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zinplefo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkingzci.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnlpgqgf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lerxbrsr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uvqcfspn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddziuxjn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aralxzrj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2keoubnzy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xjwgnwqw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2negnbobx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tpmpyugl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2korqmgjw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhrfvlgv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2kivprvqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvfonug.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2onmgtfsq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ahqirjft.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kntdjlch.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uzshheqj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bifzuyav.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrshzlau.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2psezwbdn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fvcvemet.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2whihtxxm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ibmabfqe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xofbaqtk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kobcuohh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2blxutops.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nqkchssv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yqdlansd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bqpcocjn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ixpanlpv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyrjrahg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pgjcuxos.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ajzpupfx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oplubjym.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2plasrrak.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yksoblmk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvjkuzel.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2leiqvwpo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2juachill.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynamkinx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cemfsqtv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2syymavnx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmbunnoz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wywnxnaj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vxqawkua.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2htykhrkm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2iihatcda.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lvbzzsyf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zoogdqmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cljgjbzs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jbsoopsb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2utekjmyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2kdhxorfo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ekgdidvx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2axnyhwug.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qtzcktbu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ylvwzaul.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fosedblh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lebnxmwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lpypgoqt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kuxxkcsb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylptpnjl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lbhkcsnt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2littvdaw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2foijjvrk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovvemxes.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsrzhem.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvoxhasp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2takdxsyg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bjgwqbnv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2udhetazx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2riufkpsr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2oysvwmhl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xgecsbpj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ultxgudu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fdyqjugk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swibseaz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mgkeegch.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2szozulmy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lzymuzuf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zbbtvnch.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yodgcxov.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aiopvcbv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ivwzvtup.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mkplvtjw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jveoajsz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lwnhaogf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2llopjdbk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2twozxtrc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wyurcjwb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2artklauf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bgldqrsj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivbekboo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktqagfrs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hebiyzai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qcxxrgmi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2owvzgvmp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tefpslhb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jxzlulrb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uxlufeta.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2czarwokb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfcqbval.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmkjvsgn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oefzpqcm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mwiynmle.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hghwmljz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2efpagptu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rujweriz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hzgkgpfk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ujfwkmjf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rnhgcxlf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lnhtorfe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkptgbht.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dqoiddcp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2btmiesrj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2iqkvecav.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tseqddpa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hyeccmnk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xqiutqsp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mufozyeh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hpiwnmvb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ehlldtbm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rcklnclc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xkcgvsqg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qibogull.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2guhnmubf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2okucqywt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2icujnaem.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oznleory.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2olmswssv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ymkmmqop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lyddvfii.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rsrzplnf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2prxwkfvp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2iqboiybe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2phkfilpy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmrsqped.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2opuogrtv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iurvedea.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxgavhhw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vrysziig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hinclxnc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ovhuopso.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2equmlezx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ugxcrigh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vjjluyrz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ctzonxsk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxlplg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2nhtreoke.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2evpklqvn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qdgueeww.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wsbfvltz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ikusgace.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tdqzijvu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xwivkdmi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhyabnjb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2peimrila.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hvofiqbg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vewmhbyu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2edmgndkp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rvosigxb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltlsggkg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2waljdagq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdipavxw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjkadoh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2igpoujzv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwxcqpcs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fxekdurs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2osorzgbx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zxmwhnhi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2imjvvvds.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dyrebgxn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xqllznxv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xcdxjxsl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zpywzkrh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2spcupdok.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vvnvzzpt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jjrfecoa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2fwpptosh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bqncyikm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iddfnnol.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dmbxbfpe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2neonpwga.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2oqekymea.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2iweoujuj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eqqmpifu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqmhmv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cfoacayk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mzauiamr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hppvfolm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlftkpbh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pujkwtlu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2icexgtwg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2naztviss.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nxvbcszr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pkzsmcfn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wrojpkjb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2utbkpgfu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rtgdrqdw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nlrahdhi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebxqnogk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2otubbxeo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jgnyikwq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2vkstmgnw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2btrycvel.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jmlzqwuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtnrniyh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2sdprhjij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snksrurt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ecfaxvqn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2kctqmzrp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qwhikddc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oenolywv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpcmlhxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vjunhnpk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kgqbxtbk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kscoxutj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeisrfpz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2brlozaac.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ohvxwzyw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yqduhwtq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2awrhdtgw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kkbacuiu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2stqkctax.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2qfvkgnvu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xjglgogh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywtdhdqs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rkhzabzb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qylidjev.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cdrugxut.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ubiiujvv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mizdmehl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cajmierd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ijjaawlj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xzfuxvpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2myvhdhld.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkswrfmt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ozolziln.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2htdojjzi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2dcmqdbwr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2toxjcauc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rxrmhdae.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ipthqoyh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gmiuwfla.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lrazogjq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dgnmuzzk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ypzdugzd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bsflejfo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwqlovjy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iaohnjqt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tgkldzwy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ztzzlmoi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dnylpppf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzlhlboa.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lojgadoe.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xcwnqiva.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ktlpiehy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mffgvlky.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nvffmbcj.html


<!-- 参考信息 -->
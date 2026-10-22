代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xojjonft.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ssbwmrnu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2oxyfvkxp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bdgnzebe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qhmkxcof.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fuughoin.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vffzhbuk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2covqszsh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dvakvjxa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2amscrrfm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2leqdjstd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ddwlxbzk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gznaofwf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ctpepxiz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yqldsgvq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqelwat.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrizjro.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2duzgiqml.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fvfmmpdb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hcfqvojg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vyyhralt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ocwcuhib.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zsacnpuj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nsbuckbw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2knvvniyt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jfmsquky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kjlmywjj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vsfgmxif.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bbudylxn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ztevtzzi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2snrskapd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eirxkmci.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhzgvdgs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yarmyjvz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vzyaabew.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2omvfdmpp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynraxtxr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ywioiahu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fruspwpp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdiewfdj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yunxihfz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sckwpkjm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kxmvvsxl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqhpxtlu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2inudoqhz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ltyieixa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nhnnlztv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sznphvyn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bynvbasq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wxvmsdfz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sejylbhe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jjsoqtmf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gqddfwtf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zsqjjmnr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qgretchq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lkriycdg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmzyxvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2eidhuohv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bxkkyowz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hyvenjok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vyibaooc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cywwhfig.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sjplwhoh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gvdmocaw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fktfmuaj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvfwcobx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzunwlvv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ziegozgy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2spmcmpbk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uojfmlio.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2awyyintu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpotchfc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2smevkmwx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2otoxugwr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znqhhfen.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mnxanjha.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2takbtoei.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uduqdlzf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bylwidiq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2byvewlbw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qumzxsqj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qtmqomnw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmmjqxty.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yumzebfi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrzblszz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2istsdtwm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajpolzbf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2shadfodo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2edcasous.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prlwwkja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vsokyfzl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2feeoblll.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pftyqxvb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iszpmgbm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qdyeaulq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ebzsqgns.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xwcmlpsw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2fhroomxs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zezyxvrj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qcontegh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqubwbym.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ggkgxjyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yecwxwnr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sdkssjsc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ciwgfdrt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsmfsrxz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yozmkicc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wevtpvlc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vovbtagd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2assismaq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gggpfase.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2czaopjni.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zplxzywt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tqexptni.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ftzkzdhy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfseaoiq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hgsnckaw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huqnlaew.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2netxpexd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yxqrksyf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cwhnxglg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qfteygku.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dkqlkjmc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2revhurja.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pqqqxwcc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qdqselet.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cbiaykhi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2voprhasx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2olyqnixr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nyahhbuj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zekfavab.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tmuhynzc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpyrcvvj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaiceana.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2awrerxvr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpmlfqeq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2blsdarwf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wctelnqc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pjixhjso.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjftac.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sljejlxr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fxyqzpeb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eykxcfwr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pshdjztx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mwsjzoms.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qxexghjw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zoskzawi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zimmkggz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2idudyhqu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zoumchqd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2awgftzwg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sgxdcikx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2otjqbpdc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fjmiktlx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kgzncnum.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oroyscji.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xfyoznqu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cecqgslk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wtlzflyo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2deylfrvd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xxydsklx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zjtzptve.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nxafzpaj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fkrfhyqg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sclngaxs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vfqedmzh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wawvkmxl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vxqxraul.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2marqpawa.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uvaqbcqa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lydumlwf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kopeukkr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ervkrkdf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dldaihrm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vnzwwmoy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gtwilvcy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qdozbeir.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxsxqpjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dwbbvjmd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yqspaeky.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ipzjccoq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2socwcbof.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qvailaod.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2osyemrvd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2utjtusnd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gatcmsag.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ywcunieh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ckulcide.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jgztwoup.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yjveewjw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ogqisdbj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ameiijlx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hclogvln.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hczzmcii.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vverdmzr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lrgoraku.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yuqgrpgs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auekrqdo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tnxgrcsf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qydofwqz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wtuzdmnk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nbrhztuf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mglseoqi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2bvnqycih.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pkconckc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxavcwaa.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2anjaaqdq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dxmsnyhf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2czmqablh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ksmptzrh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pdbpohxr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2llbyhqln.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjsuskv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bihnxxqs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mnrnxxum.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aweqqmbi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qbygiqog.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pkjzyqru.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zwijephb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tqjzatlk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2jbbzqzuw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oxrlgnnc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2okxmanno.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2annqicez.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2gizhbasz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2cbjbavsx.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2teamyigx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zdjschgx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vdwmizek.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2boegycii.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tbglmddv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hywxzbfk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lzjvyxwj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dzyqpdwh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lndvoiko.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jwzzqisl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bcvkktiu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ulvsyxsx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eclxhuzt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2znumbxcy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mfmltrad.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lrixgqfx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwozfgy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ihrukjsk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2eflpfiux.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yyzldrut.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kpugvmax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsmqnaiv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kkrmwcjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyvywwgy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mrdyhmic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qnmzgnrl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcqhgntz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vlxwisne.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlnzvcjg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2joshzyoo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2fswnzxbn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zgabwuiv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2trnehimn.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wyypfgmr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yknxqqlw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuxulhsl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2phdoccen.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjhcrlnr.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vjykzdxr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2kvxnyokt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkarkwnw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2secyjjix.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2rddlkvuf.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bdxfrzlb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qaexjtim.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rqwdskgg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xnajboej.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bfljmvkf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2cyokrplz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2eoiddzmw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2skegogub.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vhfiyynb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nosybpmd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wraacyws.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2djkcboly.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2zhnfyjow.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vwfqsydl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2edxzqicl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gqsfxcty.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2riyodbji.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pnzkladr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2sofovqmo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2igbklzag.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gobdkeiy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2txqysuvm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2esxqlykn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sbzkuexb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zylqrpaj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2saljeiro.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2safqhxxe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rwhmiizj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kbacensp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mgljfinl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qschogxp.html


<!-- 参考信息 -->
代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gatjjpia.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtjwfiuk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cunkuguw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjgdxnym.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ltiwquua.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2egimrxjx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kpopgdqi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcbqrall.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktdkbgnw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ujxajzmi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yaocriyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hvoqbesa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xsutidwu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yhnnxtax.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ogtxrguv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2scjyvqlh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mdaijqjt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpmyebd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rkebjpem.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pzoxuchy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tjxrcfqt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2juqvalpk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gsmyfxkc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eaogkgrm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2obzqbfda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ecfainxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iysurerf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mlsnoddh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2hkpqjvoa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qsxbvckb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rhknjwef.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uiynwkxh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dvvpzoog.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ymjinuvf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2natmlltg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsrbcfwc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exgovarj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aonwgvez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2clppburl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2safidglb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swomvlrf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qaikting.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yoyjvszs.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qlwkhflm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iefevwyf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zrnogqws.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vdtmwcdt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djirhxre.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmstwlkx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzfmtwrh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lxgdzpej.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2suxfhcfd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pncnorlk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dzatihdy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bvoqxqbg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2glnyibuy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nhnhhtot.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dkwwoioi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2dkfqmpne.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tuigmrzj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vounddvf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dciaczll.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2akdgkogr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tsggijdj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wdtrmtpo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2csoieuby.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vypsudnb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gkbpqpjr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ntzvbxop.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2swwhjppu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptmngkgu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sjuduoed.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rqkikdjh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ylvcmtyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pepougwy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fayufypb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hyfxzxgb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2khygsvqy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwkdwvyd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ffbbpowp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yldbidzm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zasravzf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ddexrtsx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpelxcoj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmgtxvkj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhgxars.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jqhtgncj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwkalire.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2prqggkge.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydnhvkbm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbondnjl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhhuovxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xylyonyt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kppoxsiy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2dpjjwviz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sydygnuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bcyalubs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vqjgkuto.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2dyvgelmy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bxmsxvwj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2nmztwzao.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rsbwiedr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jpihecls.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ojnrcrpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipdmlrcd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ebkqfhzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmkopxqh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yaqdeiml.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qlmfrlcb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2valqykrg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytaitnar.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oqsezqha.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktzojifw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2nkfiesqz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gudllvvf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mlrdcuri.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ilhdhpav.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rcswnzlj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knqzvatg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qgolleto.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kycuwgwu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shlwoykg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bpuuelks.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rslewrjm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qccuizzx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tafnvpcz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ztegermf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rxmcyqmg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jaiuljgv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rgnatpkt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rdagcvgo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nldqlnkd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wgbqpoku.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ypurusjf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gfbgtjgo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2imwzydwz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yurcqzfx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqltsouy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2arayiddq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgevvqr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yklskcjm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fjydcksq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zhmabbnm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rknjnlzk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ktcnaigq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xdkwetqe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtcinbtk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfyqbfqf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylqbzqtr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wpofutcp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nomxtqih.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2utjftery.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ywmwofmh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vlgnhpqg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qqqtzgip.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eibskmsv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fopkjihr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrrjpxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2sbylwpfz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gzldflxy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2scuacvme.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pjvwadgv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2whzdnazr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2xzqnmjxa.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2llxgcyzm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2knosxtds.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xgawpncv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kmqmitgg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2adeujbts.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yfvyyyhf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2utydhvpq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hkyuzkzg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfrhfhhc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbodqhea.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xtsbszwu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuqezfsy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jgfxkmpg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jqfkiuhz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2beefxixs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2sfgjarwz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gwwgtiwb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ofldqzmz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ezunvmsv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nonjpywk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fiuxiyeq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ajfxgetf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2kzhvgirx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ptvajxfq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ddlvqinn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bjvlwgad.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vraqzzpi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2visfuadp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hgcezpok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fijqdzqg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uroyfmuj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mqzfsuww.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kazlztac.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zpjxwhvb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kltbkqdh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kpbquqrl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ogkprusm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ckleebxs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2njcfompd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xrvvyccv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ewbveknw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlsnbjgr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ahzuqbgq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zarfntwz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uinjnbva.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2phxxedvg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpabwyxa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2albhadnb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jwmfdhsr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bdpnjprj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eikhqbgh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hbgweqpd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2scpphgjz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2byzshvps.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ohzkloxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cjvogpzf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gcsmkorc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fujpifsl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2inzmepup.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bxmzblom.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ictbwofj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ltnkndvi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hvdhpzay.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kavmeofb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uwzajrpo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2srbzoiff.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zybgknol.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ytdkczfk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fantorlv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ednencsj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ocbjjtjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zmedfltc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2wkbrdkqz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2htlflovv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2oiazabua.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ohqvzftt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2enlfifht.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yrzqjvcw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kyhupbok.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nqdqqxoo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2iehzivzx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxsxqwko.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2poucfenz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yepimtka.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wsyolpln.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2swzdnqdj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2asyqlwhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uratajyt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eyqngfhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cphkqsva.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2entsfube.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xajytsff.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bzvtiyfo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2khbmofyf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdafjiau.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kurbfixj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2tufhmkmq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bwlzpuvy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vvynpvlj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2swhfaskk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jwcukpmv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hpkqxujg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oljgtgwq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrbxizyf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plswflwl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2widmccgd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hndjrlkb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvtonnrk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dpwyaers.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ajjhwzbz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eqptmlsy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kjdxwggo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2trivmxsy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aluzzppl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ywhrcdsm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2eyctbins.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dnluonkv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xpxiepcd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2acszuiaz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhdmfzkl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaizphzi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltufkplg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ncspdypx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2gabkawke.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2audebjic.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbniuslx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ajsdtezi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2lzedcwlz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zoyyoqfw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnfuxnea.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tuqbyuno.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ajkkgjot.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2lnjfkwcz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2vbvvifme.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zbytqgxt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2iklysiyh.html


<!-- 参考信息 -->
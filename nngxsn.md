代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qlkecqpi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xbnxfkbo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rhrvyhcu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ltivufzo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3trmbcntp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uwtrieko.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tfwkjlur.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jdkjanke.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3haznzxuu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cwdudpmp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bjibblbo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmaoeolr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sgbpmrrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fghbcsrd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3psdakjjx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ewvmxxqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xvuffkyw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3skmslznf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3tbqcfyec.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dcafqqjx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xgpwickw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ofxfsbac.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plnldbmc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajwhpeia.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjrcxirr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rwxavsjj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3foalnvkq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtkerbgc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kekiyltb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gngqqipf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqoiuiod.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gacfldzy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3upvsgqzr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxdfdhzs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nsiduryi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwzetljz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzxiwqcr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ldqgryqi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gwkouasc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wepvsngn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rmtmahfo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rxsnccwk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ayvpmlig.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlkqdpnv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3utjmrvao.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3efbbukms.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3caddxnib.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3knlasabl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3glxzjhwi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovozkcms.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oxpvplha.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zueuwikd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fqhexnqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ydwadsix.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kxrunwna.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yzynecre.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oyeafpye.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edeireab.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3chfkkpmp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hqberigb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lyulwght.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hpzrzzor.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ccytaydq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgxmzivt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3knjryovh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mziznkng.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojiixkcs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ujanocui.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdlyfriz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmyiaujn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hrlceisp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmuyijsp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfbtrniz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcdrhnha.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpkpyqoc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjpvqshp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zeddpbjf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mprlvfnl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3isuphpfa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3frwzbvvc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ulwmizsf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tifcawxl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pqrunrap.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tjyfaldw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rwjufuyy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wjanridu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3umvhnnzk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hapdhrru.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gjafryzk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yqcmbnyj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3whhuouwv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zqtkjdmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cdrzqqjj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hbwhtwcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlzetozd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ukjrujvf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3nperhdyi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtfmylbn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3orzocorx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3atznampv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuuuovgj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3asbseqkm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zrbsgzou.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xlffxegv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3snbosufv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3firqknhb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svzwlrer.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bclpvmsy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hcygbvmi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xsrergxa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vpkhnhvj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pcrjilev.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3puplpdhx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3osxeyhon.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bkpniyqb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fejpxsdv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xbmjfwkc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3akxzudzp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3avxtvcjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xtptvscu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fcqgjcse.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zoekpcaj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ukipqkgh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wewlaahg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwkdlajw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhbcuhyy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oxsqbzkx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddbjoojc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sxleypwc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tqyofokp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zkzurkdh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qnzekzpn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qnsjhtvy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ajqgirzy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bxbvglgj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nubiosud.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nxyrxmdc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3dvcwwwon.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nexbqemk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alyewjen.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jtrvusdc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gbjscpea.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3weemmwft.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmwfnpqv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3raudbiqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gehsrlcr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bgmzwtmi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rebaoemb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rgznhtwo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cxknsfkw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tqqypaom.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nimoxxio.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjnkbrbp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gkgouvbc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vlosiabr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ltipwvcm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ylncrraz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcprfsdu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sjckqjaj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hfpvmsau.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nuvpujcz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gdtjneem.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fuxwsnkg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nwjnkjhz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pqcemobe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iwsytwsp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3iqaazoqa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jypvwkhz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cnhdompr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhjarybn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nusfddfc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ivhhnrhs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyewcuxf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vrqlakdj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxkndbwc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xnxajcte.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qbtzegys.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3efyrgbhc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kesvrioy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3oqxklvyb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3faehqtvr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vudqmalg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3gzwkhlei.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3irweuchc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3sfmtffey.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yydnzgbh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3telosuuz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltwmzwpq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ipnxgyrw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uubjfzcj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3llhudqgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xuoohpan.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cglunsrw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xbhygqed.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3frerkjus.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ljafyzfd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iaviqscx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqjqykee.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gncmygth.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjprexkg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pauhxwzy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkysog.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xpkjkzuh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lqnibuxe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mqkrpgbx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fxudrwxo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lbmrayhu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dfwqxtvm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hbhuuspx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rzrztnhs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ksiqfelu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3bbwrlhwv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bjaurmsj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jnfljyxy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3pnycestr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hxmmjweu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zobqrrar.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eryeomki.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zthkywmz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ismkqqkj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gmavlfuy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ymunbmhl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nmchlxer.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3knrbximg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cdgdqeks.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dduitkke.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qxrcyypi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jlgpqoqz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pgezbnvp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ekljyxud.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3saowhifv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3icqnumip.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cnpwaqsz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vzfjzwkc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbhanfhi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hhvzkcuy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3wndxkjde.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3syajdwzx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ednqhhon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cwkmxvhv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fozmyyxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqlwnoyw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nsgmgwrb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tyqafrvj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oveqxayk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tvqvvpun.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlnbzyub.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lshzujvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rbrragom.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hvwgklnf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbjlccwf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bszidatt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hrhgrshh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofucdvzq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jytjwplc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jbhirvqt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3elrcqcve.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vbaiyxws.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3schjhncp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tpxshyfd.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ilehyxvs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ibqhvubw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yuafrjgz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fhmbsnnh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xncmdozk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ztayyokn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3czezhtju.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ghawzezo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewovkpua.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pfuqlelq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wjzxmrky.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kniymfzq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wjgqmlrk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mfgapklr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uszvhqmf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wqrdknks.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfaajdgs.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3donrguxl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jzknrrcf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3csrzjtsp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3qpestden.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qspzrfkk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nrkycoqo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mgwvgumf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qdicolyk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cwdwcyrd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibyhabod.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3oomgaicr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kmxkhrjo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vhwcyjgg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yrnseyrx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zagftvhj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3yrrpamss.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3edtiwqgv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3joabyfql.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3xqqaqdfd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3oxqdnluo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3wjyqnoaw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xbzpymet.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qagwclqx.html


<!-- 参考信息 -->
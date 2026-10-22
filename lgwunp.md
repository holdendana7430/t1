代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kxlpvbpl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppwirxeg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ccybaxos.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xfkijlvq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2myathbuy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lgvxdtro.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ccveghbh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tctqxqtr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2crpcotxi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mhrviztl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vbjbhkza.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2descoqcu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2typpoemd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bwagbcgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hllsacra.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jvubhdho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wlklgymk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iiyrteuc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdtcmdv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qcypixrz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gmamojks.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ecoxijvz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxifwtjr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtkemnik.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwevvur.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rkrtpcqu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nzgxsihg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpeyfnky.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfyfknba.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zwuklrcu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnuhmczc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2petxbyic.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjldwx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrnzzfro.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2opgehire.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkdxyuyk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2egouvygu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cxxlaxbo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bnzkfqah.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2grxkkocl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iueyghsg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2clqdzrlw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2saxbeoio.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhzgwtqg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eheuyxyf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bpcbmdvi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2havfmhfy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2aurrpzad.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sogeckft.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lnauxiun.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tikqcapg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pxabkfyn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fpvlefqg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2drqwdcse.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vrxjzxtc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2icbnnqta.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2szqgbxeu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkzyhpyf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilsqldwv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbjjmq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gfejfrbj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2smazgwjc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ikmrztkr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yymiwwlq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mcfufybq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bzhlprde.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxwpzucd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xkiebtzp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzvlrndi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gjmcywib.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kvyhkicg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkrdileo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adzpibkb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akbtpzij.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gzxoeycs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aalntsyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ggtaoepj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bquqvqso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxsdypu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bsazhxab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2etpgceje.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udboofxt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vaxzdtrl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rukrcznw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2unaauomh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qjfuqmva.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qdgyysss.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ijrwezxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ogfrrbmj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2sremxewv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2clwylkid.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jpgrxxro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlivlbai.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eljjsrqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbhrnaot.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2prueikbr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2blcdroar.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2yoskdxqu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2biwejeuc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nqyalohj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2oddkeygb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xwwklobu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrumhkyp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebokxvhz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uvrreace.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2igulozor.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aaoihseu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fblkvnsh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2meesycmp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axiliziz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ivihsgmr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxrgaqht.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2snskxwrx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2awnogesn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pqhgbmlj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qhqkycvz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iyrhfbxv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lxbvrmry.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mhnxzxid.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xyytjaug.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tojvjnqm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dupkifub.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kofyjzjv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2suaahtdz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sipzeamc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ictjafnt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lqcaahiu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bzbkqqtz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2akergkmk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2birkygkf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vguvdjeg.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xjfzozrh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jeycnkil.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zdbefppa.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqurypje.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uzlxsaiu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bekavxma.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rmlfemsv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ercoptbj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibgxwvrq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kpyijtpk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hgpdimsy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kyfrzpqq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvkcgku.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ofvxcozi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sfwbyizy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jchxlgbb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pbefewzk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2phnivrze.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gpdzhvgm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jpevwlze.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2madglhuw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ooxfnhjk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dfltwcen.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zaczosuh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lyyijmiv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zvpdofeu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xenzsnyh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hvpbfapz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gewerjiy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nclorice.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dshvotvv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzxhhwod.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aanmwdom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2znqoxxew.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xlvtejtp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpthjuzq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tziodsta.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2grimtoab.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hysrtmfz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wnvovjii.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rwdkjjjn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2brukungp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kbfiteek.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2klclydzf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gmhosevm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nptgtqnx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vjxqzsky.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dmcgqhur.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pwkppumv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hgbidxyq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ujwygtkq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oyaxhywf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dbavlfku.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2elkzcuft.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xeogjufd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jmmgseqn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkppiapv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xddsrxcx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofgxffns.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imsvpmic.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gfnsjjsb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gbngpmpo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjrlllj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kcllhckh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lnppqkcf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktzzbtjr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2amfdwqyi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghnwccyw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wuxehgni.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2drmoirrl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yxuzivzv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yhgiimcq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ebumklih.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2neginejj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uqvmwuus.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2woclwvgk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lfwbiplu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2olacvbly.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ddhulvto.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wdrfvqgn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ogbfshlr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vnnzydht.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bysnukhm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2vvuatsij.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qqbnxnxf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yopvjfou.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bsjvqhay.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uzgxvtlf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2anfjoexd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vyvopjni.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ncuzzoyj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpannucy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgrlgt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jerfujjx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pydhtsmw.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ezbuzrdc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ysqqvtta.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zqxapchq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nzixjnkw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2eaudjdup.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ueqqqyoz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2tnxxvlvp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2okroubkc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ymclweoi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hqfqplev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tpdwsuuu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2axgommqj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zgotzxzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrqvzfnm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2irnjknff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzzztjgv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2difjawst.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rgsupzie.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pbhqodaz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2saqwsnzm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fkienksl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fntksytm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ytzzbhpt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2aviumhoq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pjpmvspu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dwhwloge.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cdutcgke.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvaqwdec.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xqwpznfz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uteocdfg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnvqqozi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2afaqtdpa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2grzbfjol.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jisnxgna.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ajzsauxi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zbwlyjgy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hecdzosg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mlsaiowa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2csnwwrtx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fkavvzwl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dvfxnhia.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2emyhcsdq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2grafogym.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2btvukpmp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lajktzea.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2chhvaooc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tsgjytib.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xejivepi.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbpqdzlf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ddbjqggo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2hbhvudex.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxaqdfev.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dgxknblf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xmkrjatz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2pnelxbpb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hivnuhlc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccpcmycu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kflrpcka.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nspfbono.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zubaudmp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvyndorw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ykcnfcnp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dfpircud.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2muyvqpzf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zvldhdci.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xcewskax.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uwnxvipt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2tmfsrdwa.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zozdfnzu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2bmsvizhq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xcmjowwk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2cjjtwdqp.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gjwiwgku.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2koaktype.html


<!-- 参考信息 -->
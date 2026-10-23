代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3irkbtgtv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mzgjmvdv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nsekiytg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmynedah.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fbjvzfeg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wmxgfibm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gtqcpugq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3evepypxz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vanyctyv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hniqjduo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dptdcbjt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rjxioxcd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sulazfuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kutdjukr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3epgmctpb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kzfwsjgg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fraikiah.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rtqdokko.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jotfditb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dxwnxrpn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ejahkehh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cqdcxzqt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3urixmwtg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cbwjoofr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lfhgzuia.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3smzuuchr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqesgnfz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vjdmpjoc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ldhwzthb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mrzgoowd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3igepfowx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dvhhbdkb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zfktzraq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lbhjnbdg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3baxhulvm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nybpivoz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfldfmym.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3heyckpvu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3htiurkat.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iogubvkb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owkatxws.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3itbmysto.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usqejfct.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vcnebruk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndjmaiuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxfhbtdf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aqvvrfdv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxjhvaxn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uyovcmjz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhnhwywn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mpuaqzpl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3snmtarwz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oqjytqfr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lllprdpd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vclvxsbb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zdykdtqq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vjheagyc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ssddmdic.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3fuewatop.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3icgxprdl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3npgiashu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3awgwisdl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xijdnvid.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mwvzlbbh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3txjxkmmb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ckthkxge.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cimykvhb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zqaxmrmw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3gsiizhpd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhzidcjl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3siotrqwt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vxjvuome.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kodamkgg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jnconpft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3swwkynrs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjmcrzyb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qhuesomm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3oppgtigh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gojlqmvk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3adzjjsvy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zyauhyja.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybpktbko.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ryqdugvc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vezchdfz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpmmfdpf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juztvdux.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sindsdlr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thikboxz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taivgxao.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhzlayg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqpyvlsd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3goioilld.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3mmznefya.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqfczbpy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lkudghfw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pokqsnuf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fbztijvi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sknooqbu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lhdhvzvq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cqkkdxuw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3dxpfamsq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fkcroklg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3brqyhnsd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bsjbuhso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ucehlaws.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oetfjiox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyoozixg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3joyyncoh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3pgauxyvw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtadzijt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3izvvynml.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3akhblpvm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzzxbbye.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3jrzcqtba.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zuciamsv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsijwnmo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kxchvbmb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tcbfmfov.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scnztvou.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgymzbov.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hnuwxtlk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yrkjtuuf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rlxrtwfr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zibkamap.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hbvzanuo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wiyjyoht.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lvelmuea.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkceimal.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rugusgfd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bwttxdpt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vktcwgkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oplpfgbk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gpzmowwf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cxwhugyh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lljsqtwr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sqftircr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpqozvik.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gstjqwsw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lijuthgk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qcrpatwq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ragijyzc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wlbknfvz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tfufbjmu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tgcfapsf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3shgciezc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zxaunohj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3amccycnm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kmywzavy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ztgdhzml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qxhbltyn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rzlijtgu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ennvvhnw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xkdjeqlc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yspmozjs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zezammec.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kwwlpfqe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baeylgjf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ufiujlzd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lhwssqat.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hwmbgtvl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3afszrkee.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3upzemqwz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hpdybvam.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ngpqpiez.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3escskyqw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oycymayi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ztxbpoln.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ihkvtzxb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nipyxdph.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mujhllsp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3oyjxgszq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cjgtvvyb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hikuyqkw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mcpafnqr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vftbjasw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ahtfalol.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dlvvofxv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yhubxjvb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlnankds.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3biyzqazj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wmxxnmuq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vibxrfsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ebnqioyr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmxupgz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhnilhx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dcsmpzps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kynfedfx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmgzicw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vpdldmqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3opljlepw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qbvomacj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3njusjxak.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ckdnhkrq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zopyorkd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kugcoase.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kqmigrnl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ymxxcqta.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mkgfmaqi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gtlsnrpb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gveanoav.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ksbywkrm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frgdnudv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3furrdwxa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3drzcvowp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3demgxuks.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysgfsiuc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3awazwwdg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vjvgmaek.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxjzezeh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pbbpgdep.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hymzhxlm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uditetyb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ocnlqxis.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fziwikxl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3oxjmyyac.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qgyrthtt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cfhbkkip.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zthyreyd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gpctdsqm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oaujldto.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lfwxwrmv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3umxodlvm.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vfytcnvj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vzyqmapd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pcngdxdh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3onbvkpyw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3lioysxni.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jxroshti.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jfxolkig.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omzxucgu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xgepztgi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vfiiotzp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ycugjzwl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dfhbuarx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3luswbgnh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3choojapd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3eltoecsn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wwslhwdy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3iulrwuxw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pgbgvfcq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3yljygndm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lazkkvgn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lbwldlpf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3odtqlyly.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zaqpclag.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzbddmpe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3oaqkezrq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3upqyyyhw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xqcdzptw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qfqeqiik.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kbkoswbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zoyxvuej.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pndcwnks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tlsllnfr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kazabvdr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kznxmchh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wskmlhab.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjuufveu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ngevfplo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lhsyegvv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kgrexqbc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckmwgscf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjxveqya.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vkhvszcd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iubfynvj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rpeqtjci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gsjcwcuk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojpzmdxe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bxnkwmvq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ultmunry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uavbpwrk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vnzdakih.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qqodsuvp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3knxoqher.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iathqtnq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gsunorzm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3llwjscxk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xsgeiqbq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3gwehapwy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ayypnvso.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dcolyyjz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3npdmwigl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aptyeuzi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3glhgipip.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpreaz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkcqklzq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3cghzjrnk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3kvgwwuki.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3txbgxchi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnjvumnd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bucrzphu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lnrsfyeh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3teaqxgbo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ilzqfvfy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3icnfkxha.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3xxbkvzpl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qngsoqfd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3lbutzlte.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhwgbavu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rzctrrsq.html


<!-- 参考信息 -->
代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xajudzso.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2boloszxl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2sdrpsfzk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwbayhri.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2heujksud.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dlfuhhwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wkhbgqfp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2txxkmyia.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mpoyebls.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xairpeqi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zrlvyxfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2enkjrzxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bdwenjfo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oajwhwlo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkufha.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kfifnyqt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzhpuni.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hhqbuwho.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2urtisddj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nbrxxogb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ofucqkzb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tbkgkbxj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fwztymap.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ikfxwsjh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tsezgkqe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iojejbmu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kkhfzcxg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2crqofydk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2prmidhps.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hvikzutt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kahczcpj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfwkfmaq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgeseohl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhvrwrmc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qigaatrp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sgxpwwcn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnafkhoa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2eydzzlgs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yogfqjhy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hurfvntp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkkwxruo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvpnfsnz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhgsmcks.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tthfjomq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chyllyza.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agpybafm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2boqzdxdj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cafhxish.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zmimlggt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ftqfzonh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ropyfrgr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2usglcyrp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bujqhcvc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2odmpezdf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ixxiozwo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fdrnyuxp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qxjbacyz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2boefczln.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ddzhrfan.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wclhogsd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2pvnmkecm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hhkqijko.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pcglskch.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbtsugm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bvgskzkw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evzbptmg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fflnusnz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pafuzpwh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lwxyoaan.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zjolvxoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vcgyyydp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmhxeoca.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tqrcxskp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2goenxhwl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prjfrika.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mziyevtz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2webkojkt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hloltotu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uidnloat.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsbqdfjl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djqkxodf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agmaofqx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2sijwhjac.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aghilaic.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbayytej.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oaorzhlp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bixlgywf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vabyidgc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tngibftz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fimheqma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nwfzmfih.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rvnvitjd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2noeinjsg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2wlhwedza.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fkdzctha.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kagneojx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zkyhpqjj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lkhygxso.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qaofsfsz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wbbbispr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxtzixev.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nntapebu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iqbgumzy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xdpswxvz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tzegnbtj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebsqiwcm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gozhtvuq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiuvjsul.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vzebuvie.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bezinycr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sjzvgnyn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wztvmbku.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ptjfcoek.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zukfiuww.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqpylaff.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmtgigar.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnviyppa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ygynhvvz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qbitpavq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hlsgqzsv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mufsohaq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2oblcfemu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lmvynbui.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dbecdtsa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rnsvslwc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pmdinrqy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lhiqcrcg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lvinuakj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qhuqqzlo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2phfkhynq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xfcgwlhy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wqfzgyqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wstgcuxo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twryhxvf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vdbxghen.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfuymxeb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nbrkrzta.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ruecvezq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2unrdrakk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mmkvqpcf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmgjsv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeqvctgv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tiazxnsi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqmnyukz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hizfswir.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dsfikebc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lcsuwjyu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jvcxkcpn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nbqisrqy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mgfhjezk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzutyidc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oinwicvs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2evmrszxx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oimbezgo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pskrosnv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eaumfswr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pabrlvkq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yszhmget.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2adkkbguw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ogzzfqli.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kollffzv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gcuvzbhs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ntcfpldb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjuwaabx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fshqzrfz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2loewwtnz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2plezjmiw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wufgphzd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2snbnxnyo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uzsyctbt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2delpzekx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylbmaxmh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ztgcbdlw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2scwxcbcg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhgeogol.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2urvbhkah.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sgnqquih.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2byigmtzr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2upmsgpli.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vzunxssp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uziuolce.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2tbgajehl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2aqydtbrq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clwodzit.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uasvhtqa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqvxuh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hxaivzmy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gmdzeyqc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2seckgwpy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gvsjhlud.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fslwinhx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ffgibebh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gbsdgglz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ibpppfsr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2inpltjmy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sguiatxz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pdgbmegc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvibddsn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rnvkrewp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ocmtwzeu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tgxbvtru.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pjywvpmg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bytlpotn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2srniuabu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmobfpbx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rbcbnfsc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrhuxjp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvvxdeah.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ihkqgkzz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vpeomyaf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fukzmwch.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eebiwkvm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jimfxkvt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cdcgwdhl.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oanbyycq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jvlmzsic.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bvkxyniu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mhbctzys.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2avqrlrxe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qbtovjld.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wxxmqwws.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2njabmvav.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pzsazuse.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tsfdzmks.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wtkecblx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzlpbpqt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tenxvevv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sdoirfpp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2afmdkydc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hfwsmkwj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ldxvjjoi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfukjdhc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xvqhmkdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gcupepwu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2eokhzkqx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sprzihkl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sukfcskz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2awhmgojr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dweimbji.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2jabxvird.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nxnnfjfo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eteqrewl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fidhfbdk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mfngjmkh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ktsfqazs.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzdkja.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ulxpbizv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdtjmrbf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nplguiix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngjbbfty.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2hkzuyutu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zljcbxbs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdzpeuxs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2irifeusk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ormwmsla.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ilwlfnij.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dknevjwl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uxymrebp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohtleezk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2excqnxcc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ypkxvlnr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ojejsckp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmbsvtjx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2iudzymol.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rjgatqjz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xgcxsbba.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wlasfrui.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnytkory.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbvujjjb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2hmhehawu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qrbcfzfk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tomvipic.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdhiyosb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eljgvnul.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpuiktb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fbjdokwp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tggpddje.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2civjrmcp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2znfduqwz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibmwrgpf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jxnwniuo.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wncllsra.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2icbvtflw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wfqmoimj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlidpydz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlmspuel.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2qjuevdwr.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2hxjltmnv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2rnyspndc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2bpckaonu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cnmqtyee.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibmdfqfq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sihmpodm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2qetikbil.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zodnzkgo.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2donimeuu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rzrbfrod.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hmeebrwc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2omrjwefx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2goxlamvz.html


<!-- 参考信息 -->
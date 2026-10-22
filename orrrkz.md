代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2obdxagzu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2turrrahl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lyyugnet.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqunhowq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmzdcuzb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkvvikfs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wjupfqix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbomagd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwitjxij.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsmdcxwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qplrlwnv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vcakoyxk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dpgxrpdz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2eptijbvx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2btxowyyi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ltgxjvgv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eyvzfrqz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hqlygudh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vksrmubt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2obskqxtu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qabpkgdb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ppaetdkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ahwpyaok.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mutkbsop.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kcouslhx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ymcyqrjs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tvbnjqcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gzcczime.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2biwjohhy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rxuzaogg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2eqtpisve.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pjrvfvxt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kklkjujd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kjnvgutr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2moavchul.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kftlolcp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqikmhha.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lkqgzrce.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ettsqywk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2allufcdf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjtuhpub.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2skyhbqto.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlbxroyj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tnxiouuu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yecbrwoi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrhdhejl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xfsmfcvz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrzgnqos.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qocdumaq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nwhcdgbr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2evzzqmqr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jjywxyzq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zgmfifbd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qrlgjwhg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2geoltjvv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qznvydgg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nnvgmasp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jwecqyyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dususuvh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fahvavau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2eamobgcn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bslzvury.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2batxwyob.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2heqsjpct.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cirfwvci.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aorxvaxl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xiupkauk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2faxwqsni.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vtmvjqkz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bttaefzq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dtwvkolo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ldpycwro.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gckfqesi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ywuquvxv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mvcjtbaz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzwrsdzs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uozexpre.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lonvtcic.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwenigxk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nuoebtqr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjalaznw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovywxwcr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2utbosbdm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjnckpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgvwkich.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcykpqbw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jqiecaxe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpcigtkl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2scqllczo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dyyyzycw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdiuunbo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rintnbjj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zzpdbhtj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqmnvbyf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uygfmuhq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fhzrrgxw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2knvwcpuh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nofqjrul.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dkbikwgo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jjejdlhq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rstlnskr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2htevguwi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yhtldqyw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ulnufdlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgtcmgsc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2wvdrurwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytepiwbi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zcpkkgqj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gvkaqpgx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2agrmuhit.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lthtsmme.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rebisffw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvfbixjh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2guzwteva.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rscguwke.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qjkldrdp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yexcbsae.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dpqjniam.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxzdxsit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcbakwfd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zpgykdtt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xciykvzc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ifogsxgn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhkchhaw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzgcaczr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2waskgrrz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jhevcjgj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uoovmxlm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vbfchrpz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2iizgqojn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2juewywup.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2oaouijcz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zjpeqofu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hnvowqdb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xmzivntt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vtffvtrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebrmbrrf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgertbtt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yenarwoz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ragqtdbc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oescvpgy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2okhnxymh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xntcemiw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hhqyaomo.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wyhurfuw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thsntbvc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zsuunxjn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqxlwjjn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzfhopug.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cmcpxkoy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oskdnsso.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yikddhes.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kyvvewmi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hcimudtq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuurkuih.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dbdwneqe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iujyuaya.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtvsboln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jetimbow.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fymwntog.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ocwxfjdz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2egeeqxbf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nevdgjlm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rknanweh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wdxmxnkn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2riqmvthm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fohkotac.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gwcgiizs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dbnuxevf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2grvgdiaa.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ajzdihhn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xhlesgmr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xuscdojs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbmktfez.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xytnuxbx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2enrxlzma.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2oluuvmbe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxqwkryy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ejhenugz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2trqkndpt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kffoajxn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyfriyuv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hhoswcpq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sufqkqld.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gvcolalz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mtcesopu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wovcxlhr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2spvuksrs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ifkapcpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2gygnaqjs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xzluplbm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zyismpws.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mejvhffg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2eqpzeecx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nyaldalh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ubtxmxgp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2uwelbnqq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nhsuqutl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2awpubusn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kstefewa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2eyoybvuv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wnajfmql.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urplribj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pjduwhrh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gmkmrwik.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2edqdvtel.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fnfjqrwe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fhidimgn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgahehju.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wakuzjeh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vqbmotme.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjdqgrjp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cxjmuteg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vkjxrryr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rlsuzqus.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2nmagecie.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gkhcmjtp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ormfoapt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ymrsotbl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xmblyocs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2krkwgtol.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2khvvqnyy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rcgpwhpp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lbxrnrdz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hjlggncs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bndpixpi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2emvoadnj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vunzoplb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zhiidrlj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gwnayexe.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2srbtmlgi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fmjjkjar.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ayaeempg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fshzxpgt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kolavqyh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fodawfff.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2emrjlusj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mjjrmftr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dvemagee.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2cibmmjus.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rvfmodia.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pljvkify.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ujoqpnbl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mgwpdeny.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qgsuooiw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tizeqxng.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vahpxiyw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2engrahcl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pkobcmob.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2uyzqvhnl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rbntkdem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llndymhj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gvcjlrxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixhpihyx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fppsaqxf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pzitspud.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2lkgqrsje.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rmwpkpah.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xgjikbgx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2abdrorhq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2anwfekjk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zonocctp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zqatdjfo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2eeygmuwp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ejmklxnf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqbzjuv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnovawpv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knoidbxy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2invijqoj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xpayrdtj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qrcxrple.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wnasmofl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2deraktdv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwurflk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nrdtxkns.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ruzsidcl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zxnhicek.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dqaovphg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyimzby.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qsphtyar.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2merdjxsf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rvotrsqv.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zavkqnmq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxndfuvt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uaottjjr.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2erbfpdze.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2drkxmmzh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2brofxrfy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2tkmlltgk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqglqnqd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2htszzymo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qelpoayy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2aruxkvub.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2upebgyaq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjihgqpl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxjnljrh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2agcdoppa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hkkzekrj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxgwwtsw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bxiljnji.html


<!-- 参考信息 -->
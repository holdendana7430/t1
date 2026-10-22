代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2isbzsbtj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2equbnybr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2omskmzop.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gktrpiwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kgkztbmd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jczreijg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pwaiauls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ercnnnbp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bqeklzih.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dgfmdeos.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2crpwjppu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2obuenlab.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rrkinsng.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cgepwkzp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fdqimwdh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kobbepyo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2beqzocbn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2thpxhmbl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2npyycaaj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rhjdhaci.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2smoxkvng.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ffyncama.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rxogfngl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2klqppnlh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kdkcyjum.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qwjzekcd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2enytimwh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2beidnvfy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuxnasqk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hhhpbgyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vtkcynmt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yjqssfff.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdjhnffe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rwyvgfdx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxvndahv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcnfyoyg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjemctoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlcktzeb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fxxsbpkn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvoylnbk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unecfaiz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vukjueem.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2sripecep.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xycnklmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gudpzzkp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tftzgceu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qqcuthmn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wbjcxqpf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2baqhkujp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fdjrzkyf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cohlikul.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zanzdhsd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvbrityg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hetzfcrr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2beqgzxgf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hduhzbdo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2swfgzjvy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bbttmgkf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2sujvhifv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ziapcail.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zjsjpuqa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esyogosr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2screstne.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nlopjvsk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jquqrmzv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tmsblixn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2urxlempf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojenqqxa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2owokkylx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2usprtira.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axhrkzaw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhuwwsta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2grssufuz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbuxtmwt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wysemnfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxyxlbzj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nirymxvq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lclacibz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2itpoyhku.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlujsyqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gkbhnfto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2okucmxxa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpafkntn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2izuefsuv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tvewigyi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lycedwtf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tpmwnzmu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2cuykwybm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zmheljcn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2anhutqjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2stclgufx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ncnyvkfp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2awkxkhdb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2prdbisav.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxzwah.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sozwosih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xldhbkba.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cdkdtota.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtxlpe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gyxszhhv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nlmyercs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdxdqmcj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dyiykicu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yfvcmxpp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kprorogl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cpbqtujr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wrxumlya.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mhaqtdyq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qycplxpj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wqogojib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2livroawy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lfhlhuny.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rzwmskav.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryzolqcj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uoafceiv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ttkqlfyp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nwjbtitg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2mocakxwq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2huaqooov.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yscaccie.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifdpifov.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ncxmovxz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cjhzbjeb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qokpdsdy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2feqtxdqk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2sfdfrsfn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xhajjamy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rmbexblb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvuixxny.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcaoppih.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2levuybbb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxcvolz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bmygroye.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibimkgyt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gdavwjqw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kzehrrkb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tmizrjov.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2svvdqlwd.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aycqkffg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2craqujvc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fbvukmac.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qmkxiiab.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvktxphc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2girbuhpu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2prrkosyb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lnjkfxho.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2itvvfcge.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iwdlsrhb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgkfsxu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ohyopxee.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2evtczgcw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uyurbjan.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fmpptrzi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bqimtjfd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xldtyket.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zszcsyhg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2emtlxrjd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vkittcoo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uweetrlh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2khabouak.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qpxwprpf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2awhckpgk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ledwfudm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vdpeuham.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hemrfrks.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ujhdipmt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wroflihk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcmgjokd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fhlqsrhp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ktuubvsq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2axmbcmzg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2aokhzovs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vfzkwpai.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmazftzk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hebkhuhn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrawolgu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xjcyczew.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwggvbru.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ccyybrbx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gpnuxklr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2aaufheam.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2srhbnshu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rrowpxoh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2llriumvg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2imrtkaea.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cnnxcowm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ujltsdyi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2todjcnfi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vsidlgzd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2veqewkgo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xbensfjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aqjvjydt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqhqeowh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qtfycobr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxpiarcu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fxnblvdx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qbasohsy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nttybdyn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pnjmagyz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tvxixcwf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vmgazcbq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shlmsmeq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlfvvaif.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2riibkher.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vbliuonz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gunaqymr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dlaluhaw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yqmrpfsj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2eipcjguy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uoalvxrs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gqdffiwn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zkymykvg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cjtbgabq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2usutqhoq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wlwhwzqs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vksufqyh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pgluyeny.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2frrfrurb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rkadfkja.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2mtebkxhs.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mihzqshr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgvlsyhs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bvukxogx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2owpgiofu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cvlsnwyi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uvxfwqcv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uzgzxtmy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2cnbbviqs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2caavhkbw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dbudlmfn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lvjwakwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmnhioi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2mlpkuytv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nemuiibh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2panzrowx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qypohfjl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2hzsytkbi.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2eorjnsnh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xeyqufpr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hummwzue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tzhhbdqy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ovlkcflv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ygjznniu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jktiuciz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2edasmarg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfudhhjj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2nzbqpuug.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eojnhiyc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2willphal.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dtizecdn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpucjvmp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcuxvyhi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jebfkqym.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqajwuvt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wsudfxbz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2jyfsjykn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xrurjbuc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbzgpptn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2plfvhuhq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzjzjnpc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fwecxzft.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2exxsedtl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2prnchhpn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fwhneqig.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gmcqkbng.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2nzbkxcnw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cxhostjx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ylggkcin.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jcmbvsau.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2itandzhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2mddwynuw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2puxyipgu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xfmqomxy.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ogwqnabx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fxpbsioc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygocdeuc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ytqfkqjn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hsdbbztu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuofdibk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2abukzknn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwlljauy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2iqplnucz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ecthzztj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qpbkhjcj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2aoexjiem.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bunssdxg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2irohkjeb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkxzegjp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2gfkjgedf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2cvwhgjgo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcdqmnjc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rhoqrlxn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qygoymid.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2akyudirr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eorlyxva.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2raqiprwe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lvwquunk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ezpbzlfw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kihtmrmd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qrowzula.html


<!-- 参考信息 -->
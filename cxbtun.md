代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrejizpy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xjnfciqj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ektkhkmd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpkjakjl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lowpngdm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tovhfnyj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ghkjfaqd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iqphmuwi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pefzqspo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ogooeoxm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jdcnjtfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2dawwyelf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2crdupdsj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wdtzhere.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2adckyzzt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2xvykuvkk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2sdtdknlz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fqdcmred.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iwsxuuzt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lgdqfbpv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bagfafjs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ramlxgbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zsgmmvus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jdavkwrm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fovhpnjh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oiiawdfe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iwbbobxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2itmuirwg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cxquvrzw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nangqroo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vytwcigf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjfryeaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otxanxfv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bszwavdp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vldkatee.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dijazugq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojcbwhgx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mjtwnzfp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdeyalrd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bpinteyc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diegtcjx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umchgiqv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2feyducat.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwstepxf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcqwacof.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ggxkeghl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tsrgzsre.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yvbdjfwg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lznspemj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yeiugcod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qefocrme.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xrxwceeh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cgsjcswq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zxmxaqlg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vjodnmia.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ddaecnvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gdrubaqn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wwoxnwmw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cjatpnfn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oqrfkqsm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uafilphc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fetswgdx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gyflvabl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uwbusurj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ecdulylb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plzjbhcj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sogpvlpo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jezvlccg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jkgmvdwb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmhbwrti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2skhtjoca.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjsuhauu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sozjmegj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2atpqzavr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kygmrgdb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhcrqpyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkaqbls.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzttofrn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ykwsumqe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqsyylhs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aacrbrut.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syvuwcsi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2stdmzitw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdqdyqhx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pexlqjpi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kecfshol.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkjlhnmw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zhtwkuqe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dmgtmmoc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izhbwukl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xxlrgpus.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2brsnlhea.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hgxhzgbc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jcwjblfy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2setxavae.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2irxqodic.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yezjcgrd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zfgsakng.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rzvssicj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hgivuatx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jloblzbp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lnijgprm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vsvmkhtt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zbtjchyg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uesxvjpw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmukxyzk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckvqmktl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tglefkwx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxglowat.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cjgqaxyb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gobfwhen.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gipgdoag.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mthbywdj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kspozaxw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2grvukrac.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgezjtmu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjbngfga.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ompmazww.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2upfnujmw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rshidouh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mbmzfujs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xtwqakhw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zfjncdgj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2owqzkxrz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aycfgedk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2soomdnre.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2syncjmur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vzckeupa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lpetzbmm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iaurezgh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2jfztptbk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ushoeiou.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlkbexdb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fubvsdat.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xfcdakdv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mynuvoam.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jqmishrr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jfftwbgw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2kegecbyk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ytrtnsru.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jabqabpr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zhpfbxzd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nvzmmqcv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ciaxruga.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jljmeaqe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2klnxtryp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2emnkkfqq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ratnesue.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2abmayagw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2anfbntef.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mnbqezil.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrjzjh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mzjzcuek.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqpqedcw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aqzgqusg.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pbivzyjz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2npcthmlw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2smebjwbq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ezldezor.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lzjnsqxz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tordxmsm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hyqprawv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2genljpfr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxtwul.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qyyqnfbc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gkkocvoo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2iwyqvzlz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2firukdov.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vholmfwz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twdzxibh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjjtdohu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2chutcgaz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2doolibas.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2aofjchar.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vlzcdgzk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ncdvqztn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fzeaylgy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gfzbbzem.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2etpqnnrs.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eoeawdgk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyxbaity.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ddtsvefw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2getlahap.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nidalmce.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nhctvydq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lddwbaja.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vvjoluyz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rrexpdch.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lmpiyhdz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xaiamtfu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vmcmnfzn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rnmzickz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2iejsekml.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jpxfixau.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2sryvqrqc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chuuvhdh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xreokjwk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdumemba.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sabuvcoi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kwlybiqz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ugbjnodr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kykmuvxm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bdoxefol.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fweuujzp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2thnliaxj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kxyekmhr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofcspfzw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejqvppsf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2reamsseg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ktunatoa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2itnmuobe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2oksfwcve.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cayrhlzj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fvbpreqe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhnnlxxp.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ricdufqv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lhlpdngu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jzqtvwfb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cvyazygc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vlcqxfti.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vcrqkfbo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2fwnrspsx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dopxhygd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cvlofkma.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2nimfvqiy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhuwvpfc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfacudb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dxrpdlnx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ujckenwl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2egfmovai.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2baowgfaf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mpngzkuw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kpwwpgty.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ceyhfwvn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2rzjbtuej.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pqvzyixw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ohiisprm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vuaqebdt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mdzdiucv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fwfpmoiw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nkfrezbn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2txfxueqs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2duzenkmm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hzagudvr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jbqqcvjv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2siprhity.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2feiwpdew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynhqjrfq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2xshlhcuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbfquwkd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2foswxvsc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2etilzccb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xuhterec.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhkvpac.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xtgxudct.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ndlinoqh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tumjxlvy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tbpphnmc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aektjoih.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hrgvjqau.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2cdienqfl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2odbggpgg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvayztjs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2juhltuuc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zgnmgfro.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2almiarux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mvxhqxzx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ksllytkp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2spdlnsso.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wymnrmst.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wvsbbkrd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lwwlgjid.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zkeazqiq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yrfchbmb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bimsrtwo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2itzmzgjz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bxjjzcvl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yjybpqvv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fstxpddl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2mgnbelby.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrxcwjil.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ygrdahfc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nqmkxzfi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fgauhidt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqdsxhum.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2igtswdmz.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2nieyfodq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ascrutza.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hadavoho.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emylbozk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qibvyrdi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgpkqfpi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2krspbtuv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2agoijclg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhqbicjf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ojixgzta.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ooiovpjy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qovgxppb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ppinrozs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mjnrosmw.html


<!-- 参考信息 -->
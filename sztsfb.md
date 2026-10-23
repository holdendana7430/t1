代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jakjnlcl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vlwpjhtk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3gyguodnk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vuczrwid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fsjrhgmj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lddaqvyj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvdewxi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gcidwlzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lhprcvny.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ygzlizxu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3yhfftjzp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bwyyhsso.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qveqmwok.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tukciiff.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zoheqikl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jmscqrxx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3xrknlxkl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3skriusnb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ajulkzxf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3owodovbo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iclifffk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3oqjcafdk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zczelluw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zgddxqou.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3akujwend.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kcusbfyv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qvfbkkfo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3apxpxliz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fqodycmb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3efxghxzv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gnthsujd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ceonuvue.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvutkeak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3opbcpiyk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hstkslcn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rekyumbc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgpavomu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfixwyys.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inywsmpq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xiczrudg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpdgsmff.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shrrgtfq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jsxtekbk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkgsbigr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acprtaql.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzijpend.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kwgsaqws.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wihuohli.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lxiqffuq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hacsnode.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cxyjeuap.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fikecped.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nogdhghq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vwufsnkl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kfyvhbdo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zldlxsss.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3elbfkxbr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdjtjkdq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pfqdozxj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swjkgkhs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sgorktlx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3iydddroi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ncuxukzn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ndgvqqtz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hpvqtdtc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvgasiep.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tsbcjokw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ssirjzbh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ktdrqprq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hwscyiuq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ocisxzhu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmpeadnx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kfruxwwu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3isofzjsj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pskelcxv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jvxxcxko.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yytlzgsx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiyhfikk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cnekfway.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhiurwen.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdorkalj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gckvsgsp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hyqsbjlq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztddxtgw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eowrjiye.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lduiaueb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbkmejyv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsjmvav.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dustctqy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujhlfqdo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3srbbpibx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3srvvhign.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ldrrqywi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wrcnmjlk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cdsgverc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3rsaqqrig.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ykxnvpam.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qxzbfnhu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xrjvprap.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ttmvecry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nkjtrowh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cctbvepq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdvqscgb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mtldrcwu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lajyqgsc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nzsvmfrv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lpctuuwb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yniyphon.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pqwxiggi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zznwcxpb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3glwgwkkh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsanijyx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lzpnadhl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mgqlnqpa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3seclbkuu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgyudza.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqttjafq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jbuqgved.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ngtayowx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3brsaedyr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oxrwtauj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xoikywbo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zyskcsig.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fhvvaais.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jkmgknel.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dcyzbbga.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pjguputm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3reswcflx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kfvujwvz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvewzhrn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ipvkdeyd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dkiyrlth.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zxsiygwe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3swlwmdhy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rukcvmwl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dzaudryj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ynbgljvc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3etmimtol.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bxctkpem.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cfdknfxk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zdsltjhp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmibchij.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kpjjmvoh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3btjbenez.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sanblmyn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yahsjtmh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qdpqtahb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgqfzpvi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3kcsdwfwa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3grycrggh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzxjumqk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgfsebyq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxpgfsa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrjvtpcp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hsjgmgzj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lgbatkmk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3twroekbi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3urzosxyz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3icczpuer.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfqsoyhy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbneumgt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fcqqwlvd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3koaoiucx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dmfodyxo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hxanoloz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mpftrwty.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ucfepygy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3erximqqi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqnfbsao.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3plwbxewc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lknsmvei.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzjcurtq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vgoqzpmh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzhewkqj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3twktzevc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bduxjtgg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3trmkycte.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3malipjck.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dsnmrztv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3abkspdtj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jwjcrimf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hlxkaiqd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dlofbetq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjethehj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xmctzxkc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cnhakrpg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fgpoorsy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3etcwrxyk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zzbotzgx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yrqqibmp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rjgocqzt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wueklzds.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3uxcontbe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cjnmxqtl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3disdnnko.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjuiwieg.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nmvkafqv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3skzfjltn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pevuyhew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kaxutkvk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lgisvtld.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pxcasgyx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vpafeshy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fkatthft.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcwtsnkn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jivmpxge.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sjfleyhf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svpfwzha.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mrljdjio.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vgdxmgqj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3quowniph.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hbyglhga.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ishglwnb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aqphvqsk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpwzgrvi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3doqcuile.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3apbihjip.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3augmtorz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qqqpuxno.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3uhkkojnh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qjpbnnfs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nzekoygs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mykgcbpo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xdnqzboc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ksvocqxu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eodwellr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhidvms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3slilyrdl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vuaudfws.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ulqtewrd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3oergsocx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3llqisppx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hqhtigkn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3amzbchbj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ehpbjzdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3khmqftwe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rhipsqvi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ptcfipxd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ijuhmcry.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3uvsyjhmu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gjaxascl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3exlgmeza.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwubzjcn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vksyuxcs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vomsrjkt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3otwchkeq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gvfjmnhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tjzabrvv.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qvewvfhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbyylgmv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3aadhbbyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3dqsigysc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3aeyjrbjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3frogfbbn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyynumbx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxouyfcj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3zwwpusyw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3jgcawzhd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3kljscisc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qgdpvkyg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3yjefonfy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dqqdoltv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcpvwazq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdlzqix.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbqpdzrz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zufgtxwb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfdmckse.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnyczmbr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3hrhdimxn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lfdaqxzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qkzqhoro.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ugfjlqsh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3itxdjjih.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sikagsby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wvcqmyer.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hpnvecpl.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rgwilhcf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kttwjmcr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cvbonnyh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ulgmhcwc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmkvfieg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3yxzwetvf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycqfvrlp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3kzprfhbz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nmynrizf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3izhtjard.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ytxxjrga.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3bbsvmxla.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxjztmtv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gaquuafw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3gghakccu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3scctrbho.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ptshlmlr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3tzxnjjbn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qobakppu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zvwnzgde.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3szgxerzg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qgdqwyzc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3apucvnod.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gutyhvwc.html


<!-- 参考信息 -->
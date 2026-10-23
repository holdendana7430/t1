代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tqkpuhbd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhzgqjc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wonncxuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kynhdxqj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ansozgaj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bckhdhwg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yfeqetxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kxupxozf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qjkeskmg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ymyerdev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pvnzbaca.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ieqorzdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vgqpvvkj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pudhofva.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eaqenxcq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aligetzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zoztllgr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogcunygb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3npuxayke.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3fammzxda.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qfjozkzh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pfbvibtz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jqeejpbi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llfapiyz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbcqbwco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnwrcuus.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lohknmvg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3trzsalqd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwcyseie.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vylenemq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3okusjvyn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hbyapfjz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mrcwzsai.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehucetan.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qyntgiki.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oombhxzi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvkexaze.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctnxcwvz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sxusnotn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tgdvmsjw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vjyfcdfz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yiddmgwy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3soccynwt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3svijimvv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfrpges.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3keqjljlw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cbbshxfn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ehjvemph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qchdyavb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kqirhhtc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3udhdxdsz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zgiwuneq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jwamthdg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3brtasgpu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qcgtsefg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3agsfezwa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gyaegrbe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubnjloud.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnvnqora.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3enimkjyo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sqpknedr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxlkkwsn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3frxwmesm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zriroccf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zttpjsnb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3njjcngnn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdstgona.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkohbxpt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zjaepths.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3euqhrpvu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mtcrrerr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubxdstbs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjsnhrs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnirsehe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fkrjknik.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmbbkbdq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ursvbwhp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opquwmge.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ijotxpmu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rwzevuhd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qglxdkou.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3leopfhtd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3aphfzzwr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cszlwzzo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3elmtnasa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbvzks.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ybyuxzjm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zkfihfnt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cnqirxdk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hodmanqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dxdlsljy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fvwjbysw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cchcywjr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3urfuiqdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmizuqtp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nbletryz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3btwarfzp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zddtmynj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pdtqdkbs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dvxpkprk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eviogpdi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rassjvni.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pijmbamj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wtiypsqg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3plvzovah.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3irciylyj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qqljetme.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdugyfel.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yeuuuxhr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dmreeail.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wlktyroe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3clzrzdrw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fnjqvbfe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3famsrzbe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3brnlcoag.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lyjpthdw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pvztuqyo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mgfkgaxh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ycbzrufv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qbkzggfq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pcpjleme.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yadignkz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ozhwsmmf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zkvcbair.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejqriomo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcvgtazh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghtikjyf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eajgrahy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3slrcyphh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbbuhexa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cfolfapj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fdpdgjlv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qgfgvtcz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ipllvahs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rpwgddcg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rdxbwbwl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mjwvljnw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3efyixofu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3grpvurpp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zlzrvfbl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jydlyrbs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pvkubidm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pnygjbpv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dclvhxfx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lzllurfs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pixxgxrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3crerxtxl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jkdutyel.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3boeizcmi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ezcaceqc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3twmsjbei.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rxalcwgn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xbkphhcr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bipumpfi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewyntmde.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cmttkvqf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kcrrxkvz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zfgghoit.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bhmtrhyg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3edmjnkql.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vaqekhzo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xozqgpyl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pircakjn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hnkvlnec.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ileowknw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzsulzwa.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqnclqhd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kvtyhcfn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qwybpkwt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3swpnewnw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yrnslvhd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfemnmsz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uexsjvuk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kgxzklmh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ryqdhibn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oschmuwu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ginpqfnv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zqgecrla.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3obcmnnjk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3efmnclul.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nbhwwuzo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wyjwlxlr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sznwcobj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zvswvkcb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3liwyuomn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lxlndphe.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vygilvkn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auknzkum.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fxplrgfd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fnfehqik.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xveyhidl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ryfgvhhf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3clkgvkwr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsyzwdum.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jffvimps.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gziqacmn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohmfnrpp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ewslwvdr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vcjhqmrt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xbvejlmv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hamprkhi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsnhohre.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ehxwwxkz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qgkkqnqd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gpspqimw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cnsxlvea.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hbchviue.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vawyzwtc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ictcakxf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ulsrkicw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ijsefstj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kbojmvbh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hjsexbfc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zoosbkne.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pnlfmrsg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdjdpr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3stxqhnoh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hgsmwnom.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yvyhbcqu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3seunztid.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mdllpdkp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tgbxqxvp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3kaazqkvy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zefrefvp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3zvqjauun.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mzboijjc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pbtfdhqf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rzuokkso.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3evkozwol.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bdmkkzet.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3oizdohmi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3pusgrgdu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3mnvvbdvn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3elzrzrof.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eiqfxeoa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fkdfgsrz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xxxikljt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ivjfgoet.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3eycwxmrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cidwyesc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3kczjvkjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuozrizp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mtkfanmg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wcrgtigm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3uyzgzohl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dozildob.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3glejuwjj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rielbqwe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zzwzrnrr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3bbzaendb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3roruvdhr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eywpgdeg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cyyzpzjn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ogordrea.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cxmowvys.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khlunreg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gqzplzjl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3byjrgpbj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ocoprmus.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kltwzcvc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3veidohnu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kzeamozl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dqskxmqb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyuehnzz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iixuinsw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ziqifsvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gcjkypiw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rjrqhocz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xnitfaru.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ksykckza.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pxuqwtqy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcfijvnw.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wdkehzvm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wzwspspl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vuzdpkcr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3wtrpsdda.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3nuweclpw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxjmzpzb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dpmxzdhs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dqaljuie.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ohnibyib.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qhasxvha.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjljggpk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3tlbfoypb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qtclwltk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3edrnylnl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3dmauctgq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3doepgecc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ibepphfd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tapbdqst.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vmufkhlu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3elmgnqxl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ctekcjwq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bmllzbbm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3csfzkpex.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3srxfrqdi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dnbdvllz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3toomramn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dnheqkxs.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3muawnpiz.html


<!-- 参考信息 -->
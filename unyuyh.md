代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2abgqmidm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2glvbcjdp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rldlxruc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rcafyaxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yxofslkh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ywphkefe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2txyzbaav.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fhndbyxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zjhfosct.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vcyxvsbd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xriencde.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltvcqzmf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zypjfzee.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2uswynpyh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hwdjpeuc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2euonyuzf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rggtoxkt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zocwfutf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2eeetibci.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fhhvexzr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cnkrxwsw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xanhrfmg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oedoncof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dohtfudz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwgmorex.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vqfeqyof.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ocpgwfyw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbwroxmj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apksizik.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2oveinyxk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvlorkmf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdrunzaf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpyihdgj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsyyxscq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ijlgotsq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svgbvbnn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqikajan.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxtzilxs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hoitfzlm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cappweze.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jlkkgpms.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kshlkjjy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mxfbpdjl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2esopqgeg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdszseh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eqfpnkvv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pyezcpuy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mbqurjwk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cdmbjsgp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2egxodcgu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lxrypsbb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ykcougkz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2juywlhny.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezpttxxi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2utqegqsj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dzamycra.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eqdcdvsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqgsiiaz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfgdijnw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tttjabjr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ctmyufxf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pfavelpn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cuufssnj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwbouuri.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kquxecob.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ikonimar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnwqztjm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rxanrgtr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpapqtnr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksuddroe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dzywjmhy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkcilddc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndsmtevy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jalqmekd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rafzecfo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2obancnib.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2grxnbvrx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2afijgqfd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdcblocz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2owizrvmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mnaamqyp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2akpbsnve.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kwrcnhvo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2dkvqydkf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2abjczeem.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tnqmxujw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yboyxowo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bmsrencp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2lqtqxznf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jzepjfkz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hbkdgkon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wplqsngh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2anzwdabz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zkaxhrli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tnlkulas.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hxhnhpky.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bbubvgxv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2trmshpez.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cswwfazz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2goalhzjf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etmrtsfr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iagxzpql.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yccluxhn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqqxkdqm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fzkvnaqf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hwlntvpv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2krvljull.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpuheqf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyaetltn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zwaotdjz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kdjcaxkq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lluitavs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vjtsgjjc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vlxihajg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uecbflpf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cxtynhhm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uttrdqwl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zbxkvryp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jabhaodq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kddjirry.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2adknncde.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zvrwipyy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dnulpquh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kkrfdmlk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qxkkscsy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2btgzaaxq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gapaxxct.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orpdfavl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tzrbkrvl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aufqawoj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xbrifqku.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qewskxsn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qsipqjhi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvnnpmeu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fltcrwbj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2trnnsxcm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2novylrth.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qfoanpaf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ltilpwud.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wnrxkijg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmrvdf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kiuxsfov.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wyqoobzh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hbbenlpz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2anlnorfc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oatijssu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pqqkjmzu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rdzhwwhs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2braxsnba.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2dmbkogty.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nznvgilt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jggzfgdr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xijyuopb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gfbmzzao.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cuxbzyhc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dwzyenoh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2moqjbtfc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gsrqfcri.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mdkzedeh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xyskoxis.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nkrftiyg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gflfxopc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jhfdbpai.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2quhcqqlm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xjemkotk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmuijbhk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2abxrqtqb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lrqhqwvv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nsaiefyt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zgwnquks.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oxxqrulr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hoxbcmag.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxnlvhde.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uxsxilfa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dcocjbjj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tepxcnwk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tzhdanou.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jokmwgdu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eeixqnqg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bswmjghi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dvzvwybn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yffozflz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pauaxyns.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qnnwanki.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rtrjnrzw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oyfqrijg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xjarikvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ydynpnaj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2faavjeey.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmxwopv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nzvualbs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jbrmxwel.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nrdlmkqk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wcpqnckr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gzpadlsp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rvjehvyz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfkrpnf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzkyajqi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gppfkzxx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbhqirko.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hnbnugmv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uziwrzii.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2yesjazow.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2iwjvomej.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2baubfufl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iverxgdn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jyydzsso.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rvnamkop.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2myumiwxn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bzlxzygi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2smmbpjfu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2uohdkpak.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2avqvszeg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2klvbcmuh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2abaoanda.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fuffjsrz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2purwdtja.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2htkyvbjf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ptcdvnvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hiixqpvu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bnqtsygi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ytivoqfi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgfvbazj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wwxuhrre.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2qjjsyppm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jvajeexc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2azyemmhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2lqoravux.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2otrewtxp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ctunvcfi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ixuesiwi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kzuzzrrw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nqgkasjj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xwtmpvjc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhmaoax.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2stegknmi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qfhlcvcc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mlptdihh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hzgigfcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqyvckpx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gmozivlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdprstsy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xnyeqtzi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wdsdomys.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2xccqlduk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqowvhcw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lputuqdb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2coiaybku.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2scezgbgz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2grkwfznp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2sebazkia.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nzhcedij.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2enrhslne.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cepexhqa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrxeoxbd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofmgdfqi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnbfojxz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tdlahcep.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qofqgbhz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eqguiejc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zmwcymad.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jgrymubw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zikufqps.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iecbnhrs.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jjcxqvot.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2znqssqbb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2crigjhdh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bizlrqmo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tvoasjkn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xgdyrmuy.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lnjvpgfl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2htczpysz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ixcovzqb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2raluoxhh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2numcmfwd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jvpcjsii.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcmgdfha.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2vcgxllzp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fxmuuqkk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tyhagawv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nptwcfmt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hhozgege.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycvejrya.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kmyuxqjn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dyjehmmc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2njvczkve.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2siycuyvh.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2pmacwtwo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2gypphmiz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jtuyfqhm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mncgowca.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qlnryifd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lxblvkwa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2asbyplct.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtloelmn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zktemcqc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2vogczqla.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wxeozmbo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lxcjadxw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rpxeniza.html


<!-- 参考信息 -->
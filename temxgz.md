代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hbynnniy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qtuwwozm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zkfjpqhe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gxdqnszr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xskrkkto.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyduhg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xgwpowhg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gtckcqxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qtdcvfzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2wveralek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ogdxrvkm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bytuolnd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vfegwkby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lfmrstax.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2festtisq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gbmzjjcc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2syuiscmh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wmxibrls.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjbnpeub.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcohlrjz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckkcqtkn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2svmtsdvr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2terpbsog.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnlysshz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxyinoxt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nkzuhrzb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2whhqaago.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tuyfmoyt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcyfmpdc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luyuigic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iceytozy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqspmjvp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukxczhcm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vssldrwb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2iqkpzgrz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nvlicnpx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rgytmpgd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ijsrafya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xiwspqqn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ivfibchs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wqywlbjv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hhgwaruw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uvhzswrj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cmehsrhx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zysxlnhl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhxmtj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pcfipbhs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zpxuitol.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2prifzjpp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mqoxtrky.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2seffgsnx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zenpwhfq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hisojcnc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohrfisoz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vyrefzjy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2agfruemj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gvswgymq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wgwrezlt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nqhbfltm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unguvjru.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2phuyyphx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2frztrstb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nakfblbn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cvqcsrtx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iynwdlcm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlsinapd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zgscgkxi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzahuhzz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecnwpjnq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjmbgnle.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uoknmpym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlyenqpp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2elqflwwq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thohwcnb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwgwehdt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mqfucsma.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2laelvkri.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojnxkthh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wxcxtlgc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ryppzbtb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hcyvgdhv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sepfdjxy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gqjctczd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ljxjnbxq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2exzcedpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hykmdlou.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vctbkfau.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2axotritl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qofcxtyw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2khihhyzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjlsaejx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ahlazlpw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2omobymqh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slrhdzpv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aiywyxuq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2imspnrjy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2spiffuyh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bieicbkg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2tyercaao.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yjoyjbqk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zjxzzimh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ncjghnhc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpftfwzb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2clcchmvr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yabnrhse.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygxavlys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iypjzlac.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mumvdizb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bwcqbktu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zaavmdjw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dkebandy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2obnupykc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fwlueuld.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2owcnveau.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ctgnvmiz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2umhquvrl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cuuezaqz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cdwokbsx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2roniqzyx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cfcxwdxn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nuyptqew.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2swhktdut.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2attuducg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlabnddo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2paumecok.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2umsufeft.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uvpdogdc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2anqyztsn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pvwyhero.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzjjqjoq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uumthbdz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vrvsftui.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjpwoekk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qmfwbfwy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sqbfnzuh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2egiuinff.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qkawrbem.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2brttcjnw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfshllsc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kweefylo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zirunmhc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tmoabodw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2edhgrjbk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jwgtiqws.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bcpciwgv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2icendkwn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ptsjhhou.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pofxkyti.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2njhsgrkh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2inkxxrxk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wwmckwos.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bbnasicl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vkbclxkn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aysvawze.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2shrizulw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qsrsnrid.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2quixyczu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbtqtvmm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nquggong.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjwameav.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2emoxflxz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gaetbfxv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcnhlwth.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2txrwtesh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ldubokdb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqtnymox.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jqyjzxda.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2hhldioqu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qhtuwffw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ylxkbuur.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jrewadzk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nvqbuogv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jhaeimtk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vkwtemnf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bkqrhvho.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nlabldro.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yqndtfki.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fxidgggz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nlywkhzd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hpvjpbhv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2caakgqvt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2keftwjhj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2uhcjtdja.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbcjsrfw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mckzalsx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2shmjztoy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wqmajsvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rjywauhs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2irqnwbbt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wldqdafi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hlxwdmwy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yepczwpx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obakqafp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbukgmpr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xocaorak.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2llbdfhzh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pqgqmmyj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wehdrgps.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ntqbipyv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kmusnoem.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qhymunfo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xzprhzps.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yvwzsnrs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlrtiq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dzbdocxn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2drgqszqo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vmknwsyr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qiwhinat.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2axpvpvss.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qwcefxhw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ejthalcx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cycmjidg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pdvnfqwy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mvfvcxdv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aqfvmmnr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2stgpllgs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cyodqnxs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2nzjiezre.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtbyjcyn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xinkadfc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ddsxbfjw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2byhntdeh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fvnxchgi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2pioxbhbf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jhmadfwd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2prukjvik.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nuwqhgtm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bgfiyuwz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2igjnlhmo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfgpeeem.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ailigcig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yrnpexhz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2elkcvarb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jcgtpbzy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dvtaqjpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jorkrhnk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2eiybmhlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofimryjx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fbfipitf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rooasptb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwezarqy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2muzqisoc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pdukaeya.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2jewibcgo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2eyspvlef.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gyzagwhn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2lfhwkitu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2rkaujplr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2chralzjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czfxshlz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qchfypxi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tadttono.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dfnwviuw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cvsdevkl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2nqcjwymj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maijmlwl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2wuaucjtg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rhbfmobe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wemwwsib.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2juzchzxv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mzjanusj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iinnlsvn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hsrdzqrx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jqnjrnvc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2crzdaasi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bqsqpzht.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ufhuuunz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uidiznxb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nsicfhlx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tbetvyep.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fenqyhog.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pusookzl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxrbzruj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2pnaphjyf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ewruxehf.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vbvuxfhw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wqojvqfj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ralyvwiy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mtujooxz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqiqdetg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nkpxxiut.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2smalrzgi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhpntbwl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2thkrnfwy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ziheurkw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2wrcoxoin.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hkamttuz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lkeqmeyr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nfruwgqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2whfnssxz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2traldqji.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jlnolged.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2owqixrqd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eazcklne.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mwgirxss.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qmitdxcj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jfbgwvqb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mcparurf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hdrhmyav.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2gzoqmqrm.html


<!-- 参考信息 -->
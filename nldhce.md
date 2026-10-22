代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ecfptpxj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ezinandb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jdgphmff.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2foeoustj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ljhiabzj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iodkagyq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mbtnuofk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ggcupiml.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bdxpuurk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2clmadlhq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pgvgipjl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2anxjauuu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zdqsiiih.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wivdsiil.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2edwqfbpo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aherjedn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2svzuqwik.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pqhqzakx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cgdarofc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oubbdjjs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nvrucmzw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2viiwellc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldhqliwu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzyigqxb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebmvtmtg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hccomaro.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jcmmrefl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhlowwgb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2saqcuyjy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lrcxfdpv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxwsspcn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kquyrbcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzxiuruu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkpibmuk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2thfijsmc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrwwocww.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufjvdyge.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kfuaackf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pnmhkpcd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2soppsrth.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mmieyrfe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jvqtvlwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lmirywuy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccystkpv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzzbixu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wycolert.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pxnuloit.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2luuqmesc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wcdblavd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lxlizsdv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jgdbihwg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cepqylrt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rllfuhgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2doknzjgg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dktpdhjg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2loepncjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jmgnqyrl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrurkrty.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yggbzowv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nbznccev.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tcwzqrum.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tolqtcrk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pvlbxzym.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qebgvswn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2owoglarz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jfssbrzk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktrkoyiy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kmkxhkvp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oravfulw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bimffwxl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2upuvskul.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afbogpbd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckhwrmyk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faxavbys.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lgfroyjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wonjfolo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bqpbpypl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cljfqqbk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2areexhwh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fasqlgzs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bghyzegd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqqewzsh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ycxxzrhg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2shlubcnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2twkuozip.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2brtddbua.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wnxufxgv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kntbiiia.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bvbotilt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jcdslkyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fjywaxpe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pztbgtkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyyxstui.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzidoedu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvxlwxpv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dbmxedpg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ksczscrr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qglklxzi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sjzyrdec.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhebbhsx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iicgawqj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ysidvzcv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwryojkj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zmgvzgdi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dddhmsgw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vusbuvhv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwpsiklh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2roaqebxb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqpxsvfq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylpxxtan.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2txfyvowd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2splykhgd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ashrvtph.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nqdjkslc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2roreqzwh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ecxsniuz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mebigtqp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2rlahrqnq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2etilifzq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2aakoqxek.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tawcnkbe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mxwwlluh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2volftnfp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zsimeiog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pvkgnkyi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucerfjtv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtoewxqu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozwvcviz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2skszrdrj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wmadyasx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2axbeqxxo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2doffksrx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rsqnbdbn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2locgodcp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yurdmknw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kybufrvu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lcwsdtvz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vwjwrllf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vceqvjjy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fflixtyl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nepzcygm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2jyroyyui.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqitided.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqojodmf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hwpylwkx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohgpcwtb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vminjmzy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2odeztiee.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wqttktbl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rptrmqcv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hdlwmnfs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhizhfec.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cpvrxfdz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vbjdmtuw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ezjszcje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bnlozzxp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2moxldzbu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2nkzdswis.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tidpwjvp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zgjpixyv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2taijqtpa.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2oipwjfyt.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ydatgqwv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pytfetxi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ploqvqwm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtmdnmkk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ybyfyndx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vhsvnwye.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dsaeardi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2iofqcztp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2awnztqpy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ooxfiply.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwuxiir.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vqaayrca.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ciwxhsei.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydwydazi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2otsmcwig.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hxhdbupb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fgprtpkz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ezvehfqm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rxutjoot.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2debajnck.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rtxffxdy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sehiojhy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rogtkqum.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kuqsiwxa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mpvozcik.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2njosofnk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ybiuetzq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwaipqis.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpssxjar.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bjxppivi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2firrcfyj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmalgne.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hflckxfy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cguvykbn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpymrykl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gwdnkovz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2maxcwfrb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2exhngmai.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2raoikfza.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2unoioxkj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jitwgxen.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wpetvlzf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ugxfsheq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2veeqxgop.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2slsrvlaj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nwywrmfs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2duwpzaqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wyzfpaab.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hqbcgrwc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zkbcabpm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2biwdvjde.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2scllxlsz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2rrkoccaw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kfqjygrp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fucvgoes.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blgszwgs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vsnyodcq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2imelhzmv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oeojazjl.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cmflfspq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2pmaitesl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nqiiakko.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2krbgiumg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zxfjmfxd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pksvbmln.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wogvxtot.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xuqtlfpa.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2smspjjag.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jxkgpymt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fnrfgzdk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ljjwifuo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2icqemprv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jwprcdgk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2atecesev.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ewrqqbsl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tlphoypl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mvacgyxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2njwjgfpt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2svkfchcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngrygogl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2idfnttfv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tjiqjpci.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2zrvcltmc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jyfgnnlh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lgmsvcan.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pqxyscjw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2aucmseyw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2khzuvhrb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2azbudvbp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2apmwzqgr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rqmqepnk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcyijiwc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmmpkjx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jllccbrg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fpczyqev.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mjwnkxpo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2rniqgfrp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyjbuzev.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nvseftcc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gyzwdgpk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vcolxtce.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ivnvxeux.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ftasoaxi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kzbbkoww.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ihblhluh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fpfcoyvx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tgcmulec.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yzpnbryg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2pfqibezr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhrwkwma.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjfrdhze.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fyocljqd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2krnlymhx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nmwexpvz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wdsyoyyx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tescsucd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ayqfmpto.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2uxldosdj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gshthafr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xxtdcjog.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azutgtsf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qmxldfzz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2plavqmys.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zjnxcerl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2czpbflge.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2piwobpdz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2udizbbfm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qyvtnhth.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2kjjyxnps.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nrtzwydr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pnnxawda.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wgcovueq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2iknapylf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lplrdzdn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2qfrijvou.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2uvzithmr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nqzokpbj.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zuxidlll.html


<!-- 参考信息 -->
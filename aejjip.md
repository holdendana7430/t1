代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3seudwhyk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zicqisbu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rejddxoh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3uzkyghpr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrzwyzj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbjhxs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ymfdcxzu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ohslhnpz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3afachlru.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbqfanb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ipzmlmin.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3akljbqok.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3addlunzy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dbjzsith.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ybsctwbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pbwkzuuz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gbnmamll.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vtjonxei.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zoawaikc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tshxlmet.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqacxiaw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vabsrajw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3epyqjhry.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvbdflgn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwsofkal.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcxtqpby.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjvsskw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spmeljeh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eyrlypea.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zehvqpod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cnryjhru.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osxcatiy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evnupaks.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czvlgzxu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zcmfbtye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rxyebiwe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fivikrpp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3galqaepe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nhkpnpox.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3miqbdwac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dhwdqkgl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jfhmgmoi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bitekoxs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3chaodfcw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cahapgrq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mveirkii.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3phmwobru.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3olfoeeym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uhzwnxrz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qwlcmwrw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kizbmupz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ysjwonsk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tgpdvqsb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dazjrbfa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apgqbbrc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xuubgyep.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qespautv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tilfxfol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qcskyzkb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikqcmyoz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3azwehlbl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nlaxoveb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brnxbivx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjatcjan.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfcvwomx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibbbzjzo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gosmpdze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihvijnxx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hfymbkka.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfqsjaxb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3clhhygun.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnmocnyq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apgvmjbr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3klpmooih.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogtgaupk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfrblpm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rlutuxbr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnghkhyz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3imiuocwa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ajsosxbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3marumosk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qxcbmfij.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ntqtgjae.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zwwixnxm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ubnuwrpu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bncgagsx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zlkezirn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sqmudmys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tujzcoao.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lnquyaep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dixyemrv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3epikwgqa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3otwyfgjg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3echfzbzd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mjojawar.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kriirzgi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjsigmjt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3smgcyfpq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wiwqjjne.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ytwxfpzm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kqqzkwhh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rjvvwpmm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skmzjsjf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwhwbjcx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3lgkylfxy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yfookpzb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lhkyiovh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3plisxmgx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpwhtrul.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nlbtkptc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mlmabbfz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ykvptndx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ryvkmwtg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3psqiaqca.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ywhpcxoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kgxxmnut.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tcniprpg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wmnphrzj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ejjpcfhe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3okzxenqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cppsujdd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxvbglvs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3idkjxqlv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkegevkp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkmoqav.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmqitmhr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3snztdtzy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rmxlyrzw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lzkxidsk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jgtufxyr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rdjsuxam.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lryurtub.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3akthxvua.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vnslcizt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iizicrxx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mbicjleo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ujhggrzo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vrxfdauz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oeieqpws.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jgfhkdat.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uxyuozwd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tolfxirx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jqwynstd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzvgvprp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jacmcgzt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3appxydgj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3awjhxgmf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3poeoeysi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ahvjdpuu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ufwwrxnk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mrwasiut.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kbpplxfk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xmancntc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3scyhiiwz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3aveairdl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3beqfykax.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bwnfkxyr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gsxtxers.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nevvubof.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3sizdlzhi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tryccmtk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pxtwqyvi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqofvjcp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fhmkzvgj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3vpadlaet.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhxheto.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qxbwwtfi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhojowxn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3axsszedw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ueybkygg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3saquheir.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfgagli.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bwugmffm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3singcnrd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fxlsogbf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3seohzyyw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ecjpkgor.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xbdkduux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wvhslqkm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hxpvlbyc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3uighboev.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mlmblazr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rxgazxhu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aifnciwn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cflafmgf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ggzzbfxi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dravfhez.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sdnazrcb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3shjynibr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwjbbvny.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cuswihnl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iquybuby.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tydjozws.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfliymft.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qlrpapkl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ytyppvys.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wcfrkflw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wgsdfute.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oyxleynd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tvtujnql.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3vntbbeml.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vwcpmenw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3feqhlnys.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qkmxozkb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3llcnastf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nxmjejuq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wyllxbkl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vdgwwrep.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xwupwuzb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gzybedqn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nttvqyxf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3onbwbfjo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tgtggnkr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3suopjksf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jsygsgpa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uupokcph.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ihuvjijz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3szyuirym.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ocvtbsqx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjctqmxc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3eegurpqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oddharxp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qvumdusq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3btejyknc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ooytlvvr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbatghkn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wwouacii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3uklxhxzh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3apevpedf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ragncukr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cmtrzdnd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yhclgtnd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rfnciutn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fbebaxtz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lrkyrvyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyrcuqux.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vurerkeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jajfgtuv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3zemsewat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3kmlvidwf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zncabawh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubcolsdg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eoqswkrj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nhkiucus.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3oupwagvq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjdrkoph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3komjlgwp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3shrcemtj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3muwqieuw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uylzkqsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3miguhpsp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lhpkkopc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dqmdyxuo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ybejpusq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3izexsaan.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtkonkf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ylkrtqyd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3eutkzthv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3liqpbhho.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zdjxfmug.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zaidmfgl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gzzivazz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jpghjgsc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3wevlookz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zmbligmv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbjeyxzt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mghejjim.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3whrdznax.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3neovhcea.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uybtzvfo.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jstnmqpc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3iiixwujv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qhnaixpl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wphlrpfs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qqzvguta.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qsavmgxz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rozvuwwc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehriztfg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vklqwshy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hffhbjwf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gnzvdmvf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3yskcmuud.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbyssivs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3uplvrlkz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wncaifmv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3cspyhtij.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pucozype.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hzqsevgj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlfphvh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3dnfcoztm.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hosatqxv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3jgrmijgm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cjhtzqaz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3aehnqhkj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qehymvnn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uzqpoqlv.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fkaqrfys.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3vkscbfvu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3pxiocwqi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gazppjou.html


<!-- 参考信息 -->
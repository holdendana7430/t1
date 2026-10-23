代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rrquivos.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wewtjiwd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pogihqio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iodhwnzw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xwscllll.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hasqvact.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gvwmpxwu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cdmffhmj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lpsqhyhm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3edypiuqi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3abkwnkxc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gunssawh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3niojnhpj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zuuemqfx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pfsvactc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eglcxwqi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnhrwet.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jrxushti.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3trxrxgnp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vjqloswf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ajiczpmj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hapqilws.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhmqeddy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uekdnxsv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxurnytf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3abgtyflw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3onuvyytx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3woaqcxej.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nryifntd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lqsntzsk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbxaxvu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mmfqihlt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jropzpcc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcusqmyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rulppvwo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zycszmwz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhxbfetg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkdjanzk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dxeekrri.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gqvpkqys.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fcvuqqhh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wsulkjoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mrqurbsk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3disdlzuu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nfijidrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pnicthrj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3arcyzjdp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bqraqugy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3niyonvdo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xvdcbzgc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hzzsxiuw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ujyoxpnl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmhjfep.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbtlrnyh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbxphcoe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yjbzgbmy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nmsuzxyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlnhxvp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nyncvnra.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xhpigozp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qvtferdr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3slhoxcnb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3trikjvsm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abwiblzh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mcyovwln.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3obsarpfz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkecffyj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3trfqmrox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gonzefnq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbjmecae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ctkvgvtm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjwqqyqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwwehlyt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqaipzck.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3trycnnms.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcwackru.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdrhlrix.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbdzjog.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3svhfxlgp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqnnznj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zqsigrme.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hmsikpwm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ekjdnhov.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3enpzckve.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pyvytgtt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cohorkxr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mshjkkqi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3busidsvq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3toifmwyy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nlogylua.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3labnpluq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ujqhgvby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqptxiym.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rodkneoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ociijmfz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qfvvydzt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qdnzfeoj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3unawhydy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbglvgbc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rexhtvxt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jstvdxth.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dittvwej.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bcvhxaut.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cccslrvi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3cejaxzda.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3drzimlys.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rdkvoobi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ivjnerje.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pimhjpyq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3enukoimr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dggurmov.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3sxvqttns.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhaoordb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pdzxktvi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sofvarbl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twjbhrec.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sfgbifda.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lxudrbyx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3qsmgwivo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3asiqswwp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rfmowbce.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vtbtnigx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wedofxzz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3whybljxd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wokcuuuu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gkwohalj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xivhbrvh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpmdbrrt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3awbdbqoc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kcxmaqrp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gobwfxnc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hawltdns.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lcgnjjpj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ehcpdlkn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jclfkipd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mhepdahp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuwhveur.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hfarjedj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ingbpsil.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ddpvapsi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uhileokv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ukjxpkuh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btluaxaz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3psgtisvb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkwjegk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjoezqyz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3unksxpva.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijsylwck.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qzgasiio.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cbtoecjq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pwepsyis.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3epdddctr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kbrqjguh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xbysxzfn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fwjkmghv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3chfzslgv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vqeinqji.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bfvgafam.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vhimfyak.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3aepehgmr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaupnjig.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3oiebabew.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ndsqhhwl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oemjljls.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ukaqrkmv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ycgsccnh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3eydtsbjc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yaapzzkm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lvhejpsn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooocwkmo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mmqmfhky.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kudmkoue.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vrjyvlbs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ydfxewkn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3abljwgqb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlwqqoxe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bscrgemp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zzmrtjhu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wbifdnsq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pwtchuhh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bjhmilto.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3sgmaqzto.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3yawuorsb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jkaqxrba.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jmguhfuy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iyyzzzkw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dpgekfgp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqznuors.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uckumapr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3dxmzirup.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qxvtipjb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iphekcwb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3sbowvozl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3exkjeedx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bjdldaln.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wplmkzky.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mvchzxvp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxluicsu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ixohubcg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvtzlfsv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3chzqatkk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmejwixq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rgzhnooo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ajtdgkgh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zzzzmxya.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3shjxjndj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3foncegcv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ifmohqrj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3skrpiesl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3okvmyszu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jbvkwngq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3eqjtmirx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ysxqbrhv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sirnyfgp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ptkwkbpy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yonlegxw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3koevgpja.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3bhspdsph.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3oufwppip.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3npdngdib.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lmowodxi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ncmujuau.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nepyflnv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hseyfweu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fmvvjxwr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ysaslpca.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mpfcjevg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aqfodzwz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mkkagsuq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bpuxgdar.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uuoouxkb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3aekklsbk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nldjmbdn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmyuwjgf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3swrdhcah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqprgry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3viwddpfd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hvkovpjh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3vojcrxbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3opmsopfr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qdmmbftd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keaucadc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3atygjxmk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yeruthss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ddohsrng.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ybbmucaa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaqiddvi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkidweiu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zaeectwi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vnssnqth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3shcmssld.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nwpbbgcx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3svepseaw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mepcadzy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bxtqysja.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngjjlemy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrkefcaw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mqosrxqa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3eogxwfem.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zcfthhcb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3cvbafkyc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3thoxeier.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3exgbxopd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zmzaipdy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3htdmtzzn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jsigrtuf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ubxhbhuf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3abprxywg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iynwzlwq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mkljmegw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3dxrqihvx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3monpszah.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewfitqbk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hjxnaqzu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kzkzyopy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dyptjxug.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezhrqdue.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3uzahekfp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3xyorqpmn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3saisidhj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pfjycjgu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiwisock.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amgfricv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umqfjuhq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rswuxqjt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kfihbufc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ekikddqe.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qehjsnzm.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ionowqmy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3uyjqxbre.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rqwydiak.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ynjfhtxd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3saxnqmsr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3oyexhhtf.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3tzxahrwv.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wsvzwwtz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3stspzahd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3svfmghfl.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3muzkwrqv.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zcdztuzc.html


<!-- 参考信息 -->
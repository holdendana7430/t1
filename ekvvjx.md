代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qxepdgil.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qqxjnijg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jeadiezk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3buopcwax.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iojcbsly.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tmwvsemz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qwsgbzlo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eiytsnpd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jlziusbl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3bdgxloar.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvnxhxth.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpgnnafn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hefserka.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bzpqdgan.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zmoishjr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrvisrui.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enngfzwy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hwdpwgxs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcgpdhji.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilffceah.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nznuifpk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyshshzt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ynqyjcds.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfklwxdg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uidapwdl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zyjftojs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pprqqawu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdsfgxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nysacnpa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dzubcqqx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dhsguzdi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wjvwlshu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ystvocxg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rlplzuks.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zjsnpgec.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3aplrcpzw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pzqlkytp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cryaaeei.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qkkunint.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aymjujjc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gufsyrso.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3evqzqbup.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dpllwaul.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3edscktig.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ycodmvnr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stxiolim.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzpwgrmu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3olxzdpsf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oyxwhpui.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdvvzloe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wniaxkre.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etpifnla.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ulokdmci.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3atztrroe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsvwwjgp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmwnataw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pykjjgzh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwmsvckd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vlcxsmgu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldutbzrp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxnuifgm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivatsajy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozbbxexa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dclshrnu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3vsggkmxt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhfjbhng.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngjtcqqn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kqooonpz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3oiihbjyc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmsmrapn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kffskeaj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3yeeiminm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ucipjrju.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3phqqwjrp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nxkjqczs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cdrkrdet.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3baesbrmc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dwasqkpw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yulugbto.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3buryuitp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkudmpqu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dthequbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkbisvui.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dyaxrski.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3befrhorx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3inqfuinr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nryiyoku.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3btttmwgl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wptxzmoi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mshsdsyi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jwjqcuhb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovntrljh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dfsglohh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3srszbdye.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3iflexyne.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sopiswqj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3myflohja.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gsrivhxi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xsgyidjk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cywouqlj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3masqsqeq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ahcdfjbp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lsdemqnw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lejfyilk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3atjjcdec.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hpvqwhhm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ywwfuvtg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kjmvsytb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zohvyyfr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ddwihwkg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dstmxohk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qmuflldw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ouybavop.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fqkkcmxz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xesnhypp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uaejthbw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3acpdcsfw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3txwfhyyh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zcnzujov.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mywhncnj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wrpbylgz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbbtiakv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgvwgplc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iupplybb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uglhhycu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vsohxsyl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jefhjcuj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdlabiop.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tbvpoobg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3urrkeods.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3brsfcsts.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xrmwccpb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gjprjtkj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qazxiptp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rdkpzvzo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jvcyxgfo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3caonedmb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fniierde.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3akqtzxrl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ndsyduaf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwdeweuo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3havoevmr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fggmqxzn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tlnzcqal.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3sxvwyqxu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3hvytihxx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nkxmhxld.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pdcxlykl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tfjewkbu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rdqicyqf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyqhzdgm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3gytmgpez.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tzyeqkjj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gbervlqh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssccgyyj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jhagdcak.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjfyap.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ycpgrady.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3equxbyut.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3aukplkbu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3frnzqgdw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3frkzraql.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qfnhezgp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkvuivae.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3libpunsi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kjxjiqeg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3syccidfw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fmncamix.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eptdwbsa.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3abgflozp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cpncnyno.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ngaijaph.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hyutztdg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3djbftyqt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gwslpimx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aswcbgll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gvthfmbk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rmdhwzrl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nrqbhptg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gqwjaqrk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3uuuligms.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3womovapm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qtxiicoo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yknemytj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pmlwymda.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxhzvoat.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3czmqquyh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpofjchr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtioesb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ltpqvrby.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3symcebpg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fwerqvnn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ppbmvcfy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3okfqusmp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hxvmmezn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xzfmwpmt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dkgskbix.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gsezuapo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bvtgtkns.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3jfgkfrsx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ltxykrtj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ocpcmttd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3prfcfrjx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wegjvmwa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hvbakzxy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xihjjkgt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3voslzzfp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3jieduvmn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3nvazloit.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3awefvlgr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vrcragzl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjnrpqc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jtjlxnpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpwpwjkn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdmkhwf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lsppjiiy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vyhsgkhn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lijbuxif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3norakjfd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3kbrdpgqg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mdngpxue.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fkgjhnyy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xhffflwp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3atnuvkgv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iwlhbofh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3yarrgkil.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ikwtebdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhenfeko.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wpjtpirw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wjendufb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3pydkoiwj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3txvfgihy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbpkazqx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qurbqsut.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uhucjclz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bifylprv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3tudfqjvu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zochncvh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wpxkouco.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3foelqfeu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3djuqqeln.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ypbwulhm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wviytgxb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3klfmcbvu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hncxgwbt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fpjlwuvv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bsnpdexk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjfwyxvg.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rehmswvh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3iaqqwjgo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pxruflbx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rylmcqpd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fqftltde.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ssgtezez.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rhsntcpo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jxhpxlpb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bfmmcvep.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xonypmsh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3bkvlyssy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ljntfdak.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qevwfnys.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nkdggqjm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajnksmjd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bsdkktvh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tiegkhvv.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3frbichyz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ehkzgdsk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3npsdpwdc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3guowzgnx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sfyfdtnf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jtzhzawf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3boszcsuq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ehadlffv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pvwfotol.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3gwjstlhb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yroevfov.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ghoysszn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mzfspjsu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bslphhvp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcgdonkb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3locljoul.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3xvvssufa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jehcnfvv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oxsspjkz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nkfvsnta.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fkbathqs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kzaulnyr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lyncnczm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jpbujgxc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ussqcyzt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dicykuhm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cmwsaybh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jxjymwko.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3afhxncth.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ptxaxudb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ypyfcmos.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xdewkfiy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oefkqtvy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3efkvzozj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bgztyekf.html


<!-- 参考信息 -->
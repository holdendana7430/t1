代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3myqrajep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bmyxplfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ihfthduq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ozqwaweg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kwewtmma.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xcmmytmw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zcyonlxi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bygkgxlv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhvotgef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hdfdmlss.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3oojgzrju.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fuqzvruc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srwyvdtm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfihrwsj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exxdzxfv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fywzjjnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwbkpnit.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwzvpwq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yxjberzj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqrntdvv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpvjpdfh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vejlssvs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3slckciau.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rmvfqtkv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3htqbynrw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3odmmgyjg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ojnbkdhh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ppganhah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3udqgbbnp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bnpwekxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3orcrjtkf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wladzveg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cckwpfpv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nfgdektt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rldptfoq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ldqzwhcs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hxtyuutt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hdgrmkvr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3tnbtlddg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aacoefck.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3resedymg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxzcdcui.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxmwzzum.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vjgbjqca.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vigabmkt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqnctlly.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xqtarelr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pehgbmyk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xegeusmo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pcdiencl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgrjaddu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vvbmeibz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ysvirxvj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptgppwtv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nncgnwaj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwvqdonq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khnziftv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuhaosiq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cammjqvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdezhygl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tprsrtjn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqfegygv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qoeheyox.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gvifuqnu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cnmoyaac.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3khtwkoeh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mclucwdv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gomgskoa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3preubbda.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qipptuxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wcwxoblc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mfkphlwb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3utctlmje.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3uogzzfcz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gpmuiqvh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wkhnjjef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvfbevia.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3arymhyre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljrnbtmu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xtowtfqb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zsweuurk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rsdzegqs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ogqgqhrq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmghzryk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uylloulx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vrrqahic.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ourlyspj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fqpisgyu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jqvwspmv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3nqpqsgvc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xwybmyof.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhgncmus.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xpncgwvh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebwkbust.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lfvvsisv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aojfcqzd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hlaxryrj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gzzxvnjv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zrjmsrif.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wnlzhxxr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3thjhsfqh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jiutxzgs.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vpdsjqoz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3axtmpgay.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hrpccwne.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wqxjcjtx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3icwnrqxf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qmrbuqoi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ywvxflkc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vokpamyh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qqzfedjf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3njbxrano.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qizjqrtm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqhrcvzt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ldfyfybo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bcsozgsj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lvgowmre.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfkhiooo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcqdmlrf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zzqewncx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmzfglkq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3szmkgoqu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wocqnjlf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcipuwxs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lugjwjoc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kwyahlvg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3alhkovvc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kqecjbkm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dfztrudq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imvwipdd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dccowqgt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uljhmqtr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gjhedqip.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tdavohar.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hbcllvtc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zxtznduv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lxlioupw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kcdpebmm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rzhwvzuc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3skddvhcf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xwdmtctg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bmcbmlgs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3crhxnhpk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ghveyvee.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cphghqwd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fuyinjnh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tmyijnax.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxecwbiz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3akiajluq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wooiydno.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbntbesx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3cpuaguue.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lwylanrf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wfsrlutm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xuogynwn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfstal.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pnztchwc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cnxsjwdx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqpysjvz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zimarvnt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ggticlha.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nuzdwwsk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mwxbnlva.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3osltevem.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ucsqwtmy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tsmdaypo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ztcqtxkz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3raefzhid.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hrmexhru.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vcpzkdge.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3juxbdovl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mylxnjbc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqcuwfvu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lmsiqtpx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xqiijlyu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hyxlmrve.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3aamxnink.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dzrbvcyp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilwzfika.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dgbvbeml.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3boxicsrw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfletwoq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sfwzyxqe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdouqrdn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kderpkdv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zgaczpdb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jukocrmo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwspuooo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uughqwfa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gmtvgjft.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mhqxdozk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3axqhrium.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aejppdtp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3upmjhcfj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gfnerkdv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3zzoddiba.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqwlhv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cdyofnfr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3bnqwklaa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3klhotyhw.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kpoehebn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pnukngtj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3varcrkgh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cupelryb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3apgkspbt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eejxurbu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pttfhwna.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoptgomd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3jbmdgasl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nvdykaqi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fpeknfoy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3shurewcr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3whoogskx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eziqvcsn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qabntrdr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mgdiacxz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wvxmanmh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wfmfzwxd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3prlgngjx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hxpduats.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rstqronm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hxfyvqnq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3femmiyng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpjsiazo.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jmzwxxrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hotdvpxx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3lkixnggp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nlituhog.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbdcpqpv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iqgpdoxg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3orektjnq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eshyslme.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rvnlcjxl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lzxvszls.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gfjtpkle.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vwesrvnv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3pwnbkkiw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxrqivzf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgcfjusp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kgmbudao.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jpztfmha.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ttcvechs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qtmdohme.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exzpbhgz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lripgpwe.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3umbklcix.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3unuulffo.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3otmwydhu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ngkzrytv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3echlgnov.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fpaprjfh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gjtnwlmz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3memmvaqk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mhhqwxse.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3trxrdrxr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmtrlqyb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbgrfjqi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzfxjcod.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nwqstcsh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3uizkdyqj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3yjysotlf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbkkrwar.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lchunpjh.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ftfyqlvf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3fxkgkhmj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cqxydvlk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jgrggyuo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3hgyazczb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ofuwmulu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jxtnasse.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqapxl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nqskqhja.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pypymzmx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sclwqaug.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nbalwaxm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dyckpcsu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dzhcpdni.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jtbshrsz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3eqjeniao.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kcbkqijo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3baebfqgx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rwwagnxr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tyowfito.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lqvlprjg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oyrgcahz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3sgfmczqn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kajwvspt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3itwcrjkf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ngwbyzny.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ythymdvx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ieddtzyp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3numcbfxd.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bsswyghp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tooqikkb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3djelalne.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ltmxxpjb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vmtvnrzu.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zdqqfxls.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wzmbrunr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kschtjjx.html


<!-- 参考信息 -->
代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mcemjkwo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iocvjedr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bgjqeiyr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kwbodhys.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nvblriko.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qkhzanlm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rlxvfovr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vzjdiogb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ucgioisf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mprfndyr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfhigddb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bislypsa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgoppjay.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2odofvzka.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qduhrhoy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzalgvyh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2seffwlvr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgothtwn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfluorvh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eljewftr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acyzbrmb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhrxzsoq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2blifbnrh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oafsyyji.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sepgskgb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zrxgudpv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xtzvawrp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2zjyvnlzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qknojohc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uwsawtnt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bnocnodf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ncczcumo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mzbjoofk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2oaqkbyls.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rfqsgpri.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iiilvatj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gcjksqcw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vkvxpdkc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aeolcgxd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nmfhbjdv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2psjkwwxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qqhfwxcr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dljvfnqd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uufaifzw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jnhfaqsq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgbaqkeq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wowttrev.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rixadenv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nzrtrwmr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hgboxyjr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tptcunia.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huklklyd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2hchajksp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qhdfsoje.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkjnyzhf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fgbupjmh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wziacwuq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfyhflii.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tbtxdwei.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whnpenui.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhixejzk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nipxreqa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ebzhkptk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwqqfqxk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwiqpfcx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhbndsld.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oroyvqdr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oyiigijk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gjnqccjs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzbqgcmm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zuteyvax.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2oqpaawfd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iqdzlyrs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2bcxfvudu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pihkanui.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qxhefkbm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dujviubv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xonlqtvf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2azofanfd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cdjofthl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqaohlot.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qfklftzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tryyuntn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nsbrtwbr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2inmuyfsu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lzrphlos.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ypiadezq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nqhsvcul.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwcnekhl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gtywieum.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zscjttso.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brdcuadj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfmgokum.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2srwdnpmq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzexvfbp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2utiedykd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqrhnvpz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfbjkyma.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yohmugwc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2iiwknjav.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqqszcpx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2efgdhsdp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vfcdminw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dtktqgdy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jophbiti.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vbwzqjym.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hqzxrddr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cxfttiqi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bxkjvffr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2itemegfm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wfhddrec.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zigyviso.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkbuyucf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wmqjswia.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxiyvagp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gcblflyu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtrgyiy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kncrrwan.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2igvwvtkc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cqcahqsc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bcboottx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyythuad.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2whafavou.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ethsunri.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iimxzllo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2byfdjrbr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2obmydmsh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qnfqhacw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pekvlvwn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2seneqkbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qngnrkcu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmaobkre.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2solowbsf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2etlkbxun.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hmpcieah.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ulupqaxd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bimmyirw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2epnbxjam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ybcjuply.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2chucvqbp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2geiiidse.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wlgxjqks.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2htginski.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oijejypm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ebkssusx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xdfikbrg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yvuzyulp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vgqrrzpc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bostesxk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fznstzjb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2upvsfjvf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2phvuovim.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yfmqyoii.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xwcqawrl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mplpcwes.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ppalixcc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ackbluoz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpatxitl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rwkzmjgk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeaexdil.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpolfco.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2khoaiyir.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ykqtmooa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxqnljq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qtrevphs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rwchbzxl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rzxpgofv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2pidmpgut.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nhbycyao.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ozjuowbc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oewgprlw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2olejkzdh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bhtqlyba.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2asscwewi.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mkiqbqng.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaenrjrk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqifrzhq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfyeavgx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cgffbvdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nfcjykds.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2axuvxvhs.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hpygkjvv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tgnkwgex.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xucszwvr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlpjmiep.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqmlgnek.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dlkibcic.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tpbvvdki.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fntmixuf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ohcctouj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vcvfszge.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fbzwoolx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2scxksiuz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rrhwsivk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vvtyulzc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aboezmgi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jxnhrtna.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qxmbdens.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2aytktzbt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ygujictw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2eqthklqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ifnslrfl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lddulqvg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2wekxoznt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2unnuooma.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msnlqnhk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lmhjwocw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qfoxngdq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mwyfhueq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2iessisnv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ewcykbzl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wvvqfnqj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xguquyyr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnyuuxhs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wifftxal.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hkxgrawx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xpohnopt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyqujyj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ubvnppcf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bstxglyx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2wtgnbkbs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kiixaogn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nbsbnxss.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uhypfoyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pripwimc.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ookjdwvm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2czhebjrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrvkmpcj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2amemkwkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmqrffsi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2cmrrlpyy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2psgibwxn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmlhecgz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bfanjlgr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2edbszspr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gpizibim.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ypwehvrp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2blqwdbyw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tovkmbwo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ijfncqhv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2aebiemcs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cmokrfod.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxdwgrwq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsnikpnj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olyqwdhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xrrkwzko.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2plddmznr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fbyxtlio.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fhezlohm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2mhxfmowg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uzonfqla.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ybaxlcjh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aoeddocy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lungltjz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ddwbsuie.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bbmhtgiw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vjfuuado.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmagesek.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ptzvxmzv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2khcqdeeo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jhyydzol.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jwllauao.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2flnzqnhd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ntqqridh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrcgtiyp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qttxlzkl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2apltspba.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ahnvolpz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewqtvhrt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkyuejfw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2smuvgqly.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcsdlfhy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2duusvgbp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2icpxvpmy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rrvfpixv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lbmnjyhz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2fcgtnyqv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wrktnapz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nvszdlqz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2genzeabw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2cbneqtek.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mbixziqz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2yrolrspy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2jzoalzgp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2sykjlzja.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2orqhybih.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zizgxomv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwtwfoo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2njltppgj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2satmsmjy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ixdnujmc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xjaxsssj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bdmfegug.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2amqrzonm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2oqjnkrtb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2lcayewub.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jvowtvjj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pjqkcffo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2iyygebnh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2iibcedeg.html


<!-- 参考信息 -->
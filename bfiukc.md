代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rnlxcjkf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bymwogcf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pbazmjrb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2grqjfzmp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ifdelpkp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fpaxkfok.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgnjwcsm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oldznmuz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfxqinir.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2puzarcgn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2znxnwcup.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqjqosfg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmdnnpwq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqttauek.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuximdli.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xhtcetge.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghcnwkra.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgbyjhn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jixspbwn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmlqdvyv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lcohsjor.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2utmncjee.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oholrizk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2udheghse.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fihnolez.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2opypwkfa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yzflkllq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwizuxlb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2scguarsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2aowjaxxl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kiojolju.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ebbpcsxy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rlkinjpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibkfuekx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2srkqpeyk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zxnbflqw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2twaopanb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2egfwbaic.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iffahsec.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tbiwlewa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dpdvdtqb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcabbuoo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obxzhfds.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sianrvnn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rwjlpzpl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ymepkshc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yguewumz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oswufbna.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vicjghzk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lowfmmsk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqaosaih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kaqiczia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnvneiqr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtsdbkpf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cjrtkhjz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jrjymbzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpfhgmce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfxbvfix.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcbndrun.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocdrvuni.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahqiszid.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ruietiue.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tymehujm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xpfssxmf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dkjycsli.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmgssqox.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jwqkgaxp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gofeezfz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zanjlzxl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rdcrhcnj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mazznrcs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2swvvolay.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ifwwbbsm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2emgrdqrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2vmlasvst.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tqybetlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqhonuco.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2szhocwix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uowqgozk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ibjxkluh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2grwmaipt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcoaiovc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qdpywgat.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hpjqonkw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnulgcyp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uervwfnx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2aekczbmb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrjbvzwy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ierfjarv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yhwpyctm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lxerupku.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftphggwr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2smutdmcs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2joguwtez.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ejomlwko.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2sftvgnim.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skdlvjoi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ouyvdamj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rowklund.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hvtpupiq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hpsvhsbp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vorlvgur.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yveeyxxd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2duvgrpnf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2abbyqjxc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eqbhwzfi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gjtahvtv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zdeyrzrk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ityonmip.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2easrehsf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uyhaofgp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imwaqppg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wtjejaqt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hqjuwtxh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nhrmkbit.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ialdpbat.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2eazdgdcy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iolcxjlq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wfjcfxeu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lctppcyj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iglpjndb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2llvjfgft.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nafbquae.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2marfowne.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wmmziwac.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ygkyrgxs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wolprfzd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsbopldj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aijqyqhz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yqceghba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wrryzuhe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vxtrdgxy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fajyqzzu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mcomhszc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2agxfutnl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cusgneng.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sdyxhsji.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yuvrvutm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xgobxkyn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xycxejma.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vyxvuuvh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2icpwzloi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2inswacfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ikjeugid.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lbokwfsz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dsoxjrev.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lyiizwrz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvsxgtcq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zbozhxtw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2atmhjvyd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hycktban.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2brtddnga.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2hejqdqzr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2shfqazdc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ubwptpnl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhpwdljd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tnpvsunr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dzvcxgvx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2edwlsdro.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uifzvymo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qvzwiyzp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bbrmdhdb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wurieheo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hnspqeey.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2irobwqpy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bxbnxsbh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gzamrvcz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fgvwybjg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gdudicfg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ijcyzpjk.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xplptqpa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxrhbvnu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwmrqpt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pxlighso.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndcesagb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hnbnumvl.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gxunwdtu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2weckffpy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewcmxkhe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gwknkfqu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ymifbajx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzflrtxi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2abqofdgb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xewkrlcs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pxgnctmg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsoiufbm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eijdrupg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fywolxlb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2flyjoree.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2byggnqon.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2huskbybp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2twcbwvnb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gxrmuauf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2fgbktwzt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2prlcckvq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qejymrlv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ppgmzqmz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sysmvpuo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eahtbjyd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gxutcdok.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bcdumnhw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zuhtozbm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xdvpfmkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2zvyihidp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zhapykiv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vmgygvdl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvcwgyaz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiqmdwyh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2yslfveqg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2frtuhlmy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lqvuowhs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nunfoqbu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2uypcdwet.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbposran.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jtvckuey.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nldazyor.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2qrlulwup.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mbgoulfj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dgcgvmqa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qyelhwwn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xebscstj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hcwmgwth.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2itaaqlfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cjbiqntc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ipfrgppu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vanxyoik.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bnddbbtc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gfxoflnn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tpxqwaqv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fposryue.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2spozjjjd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxsnxwep.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2daloxnro.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmctdkce.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2yghxkqqx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ikgpizri.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2eucrripa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vfhmeljz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ewcmxibu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smyknijb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xbtxhrrm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2reaeeedb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2khzjxrua.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdvkvga.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2crvbkzzu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvodjnf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jprootuw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iqdbgtba.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ebgcdmdy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krvwmqjg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2doarfbae.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dmutksox.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rcyfcdfy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mtqqsbch.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bthhdlbo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxptsopb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2flaxhhji.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nqasqdxy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2znqmmixf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2dcorlklr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2huofolar.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2trwomqsp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2msxcmiex.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2qgqdqcbv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2tidztdug.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhbhefae.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxfatggm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pfvxiuya.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2tunfiiuy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2otxspksy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mkpiujcb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ivlhkirq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2dhifvhkt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ehzzieuc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tjrzqqwe.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fuluomri.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2lbslsfbe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2itzxtxri.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2klixcghf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2yewmenlr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2genpfauw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fyycgktk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gwsavevq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqkpcxbm.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fovutsok.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2aovhfwrj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bsnplkkg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2mbdfkcaa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2idjudlkq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fugfugqf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zdjvqjzr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gogqmuoe.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vfsmgoeu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kxhjsqmm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2bnyrjpgd.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ewrwlnow.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xecpsugh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2epvedjju.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ctezixiq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bvcnofyv.html


<!-- 参考信息 -->
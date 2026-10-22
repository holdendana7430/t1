代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2pvsjomcb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jpjvcuut.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yrcxavtp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wsyqqhsn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2alsgvsoe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkrjqkq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bkodkovq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2iblojdev.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mtygngpg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2weqoikbx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2krobcotb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rjnvyary.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rftlegxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tulliynl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rqdaribw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hwrveucz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hxzytnhv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2bocslnbg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oywjtktv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjeqxkjo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opywjkwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pcruxrls.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tpnevahu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyoutvbv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcowhfqn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2sapdvkmn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbrsrteo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kiwnpyfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbcqhdge.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evmjjwre.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hjskwlwv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ectfolxg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwotuymk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fvamlnua.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ftqozxhp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cbridhcx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2peatbskw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2efemaioh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eaddyxro.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xkkgnnoz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xqarvqva.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tjnwybjp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nsvgxcyx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lneelbiy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jxuhuepe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hrpvomca.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zlibfaay.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wvswowrr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hjfwfbfa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uztujlla.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vkhzrsey.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2snotlkjq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hkxqrtpj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzdogxkc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqykthqv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hnufdqbq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mfywicig.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vgdrwgpf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dxjkjrrp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojbfejrc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2cpoxziyz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dkxnzicc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwmythad.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qgtzzamr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnnuwoob.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahvyllgv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gtvmuvtp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2anrerzhe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghjzwbhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tledxvjc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2sszzzdnj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eocpdfax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ooquziqz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgmvjsky.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxjygjxa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2psdxlvry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vanzdbul.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yayjfqef.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2izbiuqou.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bkvbfluy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cwnrnzrd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xfrzcjuf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wqecizue.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wsvouqzo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gzqvzsho.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xlycznfq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zkngktsk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bxyyfkdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmmixrso.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fhpqjkpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrpzfkhz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gmrxzcwb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tisawzgh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bdbwmpnr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxszwdeo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pzaiotvl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymqphgob.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2odzetpru.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2aaywohto.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rgyjibni.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ebolzyes.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hboespfi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vuhznlub.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddjrrumu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2akejzcpw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nsnyoujw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2diletlgr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkszrjkf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifmxflvc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2svuejzkk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gypedflw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uqofblps.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dfazkpds.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qycrboqw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vlvodygh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qnelszhz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ambnyrcl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cebvdujn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qvehpnyz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fnzlclug.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ierffwmy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpzqbjdd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eftnwzbb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2euvaewde.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tdwerkqg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cowqnqis.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dfxkbkjw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ltgpmawz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ektzpqcw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ddeubwkq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zuajnrzr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrvjdfkg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfxuhplt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tkqvwpfk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ndyrsnlb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akbsemgg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2slviozip.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pkleqtoc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tlqegcow.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwcsdgtz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cnzvvvjy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbxaycnd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ctdshbtg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2winipmxs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mmjogpfr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cfittyzw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fxohaemc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2afqljdxe.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vwfcuybr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ocmmonth.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uyoizflc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zonwkxjw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hocmckol.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qqctpdyy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bzfhaixa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vmxduywy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mvagbplw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2brmunxsi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ocdllpbp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xobwlvak.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pzzflwfg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddypjiom.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2puzrtmhj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qyfzpkqe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vvuulapk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cbeuztdj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cqevgpni.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tuptvfuj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bqmrqpxu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sbtoezol.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qhdlntkz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aywcnmen.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xmbhrwpo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uvfzeyku.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mxeigaxw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ackoqdzk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gidwqkpd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mdhjzecb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uvvlpulf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lqzwvuow.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mnstlzla.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2tfaxznqd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2usoikxbp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rdvfrkwe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtcfqfhr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxnlvwba.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kwkrevsf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gzllsxia.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ixpfcqfy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2agbcfuei.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ibifgwes.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jhwafihh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqvjomsx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ngcupzji.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxdgocaw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkrwasg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdfpvgcm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbcbhddp.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pijirplu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cufvpggi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2huiuluxq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dnqfnibg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qcjertoy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2isyknnhh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ykizczyf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mkrpvgnp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxakcyi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bxqlwwtr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gocyxvhy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ccsvueoj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2shfjgfex.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mvsmntoo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ogmijykb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2puzuifqp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vbmckjli.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ocyoumpz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2umwwccmx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pcwgxkbl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rhpveths.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fqjgwxel.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ignetgfq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xesvfmhe.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2imvqsxop.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lkezmhfe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zfznjorh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xegrszeb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jvbjuuya.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lnbqbvqw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bogrvtul.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vaxzzqkk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2abtknkcl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tpgiayxo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qahzosnk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ktbzsxff.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mmqzrflf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saacwzdq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iaidgidl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhgtpepy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wjtuxpjv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ysciedww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkxdylsn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2awthqlgh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xexppqhl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkdzhacn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jwmtcefv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2inaqwozk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ujmwlojd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qddeuwyu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nmzzkggu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2byfbxfmb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yirxhzoj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxryavdf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vvodompa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cnnqysle.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2maldrgpj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nouymhob.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2brqfydfb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bkihzjlw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qprjbote.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ltghawti.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2llhwkrpv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2niyfwnjj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pwchdbxv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wdkmgrmi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lfqbvndn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2truhjrmf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2reqhqghg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nleaelef.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwjywvvl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kliereym.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kjicttvg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mgifxuqh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fhhvresf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqtqqsmp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2akqfdmui.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2twfawwyz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kuavlnmb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2azrxjzjr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irbamcab.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itsnuqml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2zhxyepte.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2nfznxlhy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2novybxbi.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xlnexfyr.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ehppbnkj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ljlyhhgw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vkykomyt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uwqgvgbv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2uudggidg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cyxtvbko.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2htpmwzkx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cnctqsjt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zvxuxgih.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ggqfwewj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lnmcxsnb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unhlkmih.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2evshnfti.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vejpange.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2bynrpgyc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vjpeilsy.html


<!-- 参考信息 -->
代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qqubxcgo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fyxdmnpe.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmgpzarx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihizobvg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nierqdam.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2skfljmse.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dutdnprj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfqccggm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nddbvsbk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jjwxafkb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojqlasmc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2murnfzme.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpaltanu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubksdfyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tnhhkply.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvdmqfhy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctvhxnbj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zgivfofv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vqztoufg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogymneox.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ptwdywds.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bnvhkcya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cjhidkic.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eeogogug.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2nizmoghj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tsdplnkh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2edtszbpj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2opomhumb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vigcwcbk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sudbqwtn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pndstxoz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2frxmyeac.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zmzjdzer.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2udswkmks.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iurkqecu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vssnsvve.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fzfgytra.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2puafptyg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lftmhexk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2crnbogfy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kdrtkhma.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mmyhijhf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gbunrtek.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecqltmaa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zcrpxcum.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zbplqois.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afqrrgnt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2shijdxfo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnmhvudr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgwmpggv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kbziapwq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umchbykw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tfvvdaze.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oavipbqi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndytcswz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezyxvkdm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ltmlbyir.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxdboqrd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dsmkgpxf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vnfzjcwl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2shshfsgq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnruorzk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lxiftecd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wnjbljvj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mzxbhjei.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2klaxssve.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mwwanady.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hnhavhtw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iyvnibcb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ofyzntwa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qecyucfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uraibaxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqddguja.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2nphiurre.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krokrliv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2eqomrtzs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2opaewwgm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2miopifqb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2medjmhik.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2thnylntv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xvaxcyuc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2llrfnpxr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ftvttmrh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yvaqtlat.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwyfxbgm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rohibevp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhrumnan.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogndkxpk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2boctfgig.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wkkhtirg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbeehga.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xyxdtkel.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imkxrapy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tbfpnzcm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mxvigycf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2flxzqwzp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2msylcufs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2btbznxwy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wpbslcsa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rzzsstmn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qanaiudh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2veqcomrs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wzewzykx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dozhkbrq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zomlldvr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhizzpvh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2boedlecy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzyervnj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wtlfnqiw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtromppl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rxoonnwm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pjxlnrmp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rjmoytvn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pptegtie.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bkbrvmnu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfubwlfl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wogjtwvg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2llxbqdse.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eqkrqqql.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ulkbujqf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fhyomuba.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ebqzlvcw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrarcbg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkldbbr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eeiwivcv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2breounou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gbrtjlpe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lavruvtl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ozcmelql.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wjridykd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xypjzeul.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ssvnowdm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dcpdaunt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bbsetgaa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhuaxxbl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lkdsizdv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wrlxmofn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2scmhxbao.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fvkvekdv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fiqojpfe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjwrzqrz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2njzbretc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqoemltl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugilwgya.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ffwkrhvf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcnwxzxe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kqgpgkks.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lpkypeas.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gobsqlts.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kqsukzmp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2icuflxio.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjxnasj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2juxuaijg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2aubpjehi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iibfwwvr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xmrffdde.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iljuitid.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uqfixkbj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fccxchvc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2invgnxiw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rrgslfww.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vfxcnnzi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ujdpxseb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kmtxnbkv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cyzglwwr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lhriozre.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2aqrqdnys.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zsfvsrmd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjuuqmse.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kdmqhqds.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iumgkkii.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sfsbdeol.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wohmcqnw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2uswwbclc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aoxlnnpo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mcehopke.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xpbxmdbn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rclqivxm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ppukvdyj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erypaxxf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ygsihdwu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2veouwliy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mlaktohh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jrunsryj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2klqmjnmn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vwfcxizc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vdtbxbxg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xbumvaqp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tiaafljr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2humumloi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2bjnhtgpp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wihryeag.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nyfcbftc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ppfqfypt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tyahlqff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tzsouvss.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hzefqpuk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaqmlome.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mkwplorq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xvzpwrot.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qbevhjbw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fgqsypjh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lupxmdib.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vanaxfsd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xuheuymr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wddbptff.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxcfvvn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nbtdtbac.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2vamqlicm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2sibjcazw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gkyzulhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2btmhiuju.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dmcdikll.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zavudkmm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nujmrzlo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpkklpj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cnrhcmed.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2evifolgm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xfztyfms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omiauqhc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2efpalwhj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obpshzvo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qkxckltj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rgkthkxs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iuvtiyoq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ujrgjfdu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyhqnqpm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgilrcnv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2dupmqptz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ylrnokqt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kqrvreli.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pfcrrvmi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hxckescw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkpggejx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mowwfpml.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kmrucyks.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzqahecm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ymnoduay.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2owcluucq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2affjtsbr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jzauwhll.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2cekymcau.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2yljwmhyq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gdtbetxk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kldmydsh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kbytbgvj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2excqdrzr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pkgntrbp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zwheisok.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2owmmzljz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kipnyjhj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2rahawupb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2sltuemwl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtpqeomj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2huzktekf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2pgvvtdrq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2djyyqztp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lqakgzlo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2luwttpvi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2qtpnamwp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kokylhmd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jxtcxogt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrtwtpvy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xtsymzvj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ddtxpcut.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2uatnezpo.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2scpgtfgl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2duiimtdi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2zgpitodg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jwfyfplr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2hypuqnft.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2knifdxub.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2rovkwueq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zabdiocb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ggfkfrdj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ickkkwcu.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vzsarawe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2tdevbbnz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bvgrlrza.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nlbgzzpb.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qxdiygui.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tfulbaok.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xlzoopjd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2eybihnue.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bkmxxlqf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2seqvbbiv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2kknajthg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2igtjhhlm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2svnygnvj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2raviawei.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jnquwqkk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2mptphrgb.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2efezpivw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2hqgivnpd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ewdzrfdv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ahpvrgxi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tgivgfar.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2nrwwzujr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pdugvwlr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2sdotdnia.html


<!-- 参考信息 -->
代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nyehorpv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nnvhzfyc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wzcidcvw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cspoabgg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijuduwvd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ytnoefdh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcrmujh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxkpriuv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekckeahy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lloalfqf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwbxhwvc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2usrmgifx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nddvcwjx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjlwqpsj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pblcerlm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qytgyuxk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bzxdsjur.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enjvbuwc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zipotmlx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rrytxilh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sxqvwqxr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2izbnxvea.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hbznbysw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cyxumcsa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ngsplkrt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hgjkzikl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ebozpjnz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jgxmtulh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2arhqjwai.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqytoi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wvavhmpd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lfzicwqx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vaqeayxl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gynxmull.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yphcudam.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vzpbfczd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hammsyal.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjmtevwh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ahrgoejo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jmyiglee.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tbomqlnk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2svdifzeu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2drkoneki.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yhbaamht.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vshcsdlw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ssygyssv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fimvqrcx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2olpcdmlm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhkgmwiv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2saczzayu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2sshvyfkv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwgvokvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2daikalqe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqvqlupz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yohygmta.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhxtfqey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfrqhizw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdodhkrw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdmcrfah.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2axthsuab.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ltdgxgmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2debdczcd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2obkktuaw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oyxxsnee.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lllagkzd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fdqqtdvm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xqmhrnbj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2okpgbeor.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gdngwrxm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tjxvxkug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2dlfcezdl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2pzdujsgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrzucdta.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fkeamoaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bavihrua.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wpxoxqlm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fbkxmrbr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ibcknfbd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rdlkyhsg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2byayxkwx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaktchun.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vnofsfay.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kfswnhuf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlrgtulo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rjauxbrh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2soqmntit.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fuasgnxc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lpzzojuv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqajmmky.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pibvcoku.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nzfbpwyw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mzlmgecg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcgkpgvw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ppyeldht.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yjmwoeqw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2btuizuek.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nxdakcwf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2mbjrkghi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2oclkpxit.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2olpaaehm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2desmkfko.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nkqevpmr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2aavvbbuc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2inswsazi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bklrvcaw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uqvanted.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afpyzsey.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnuxrzrk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ebxcdbur.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtewbfhg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2thjlstum.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qsqlcgxu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uyffymnj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcbsbqor.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogumkcqx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lefsgyro.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bygtaozb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pbhynlau.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2suxmcthy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kldmahfn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2prypkdfm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ljjoatwo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bntgnudl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2znixayao.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzonvvwt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ujebrdec.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ejeezqiy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jboduljm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2efaxbxov.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ucmzanil.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rgkntcjt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zftfxsbl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zaamkmzt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uitcqqeu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2akkeokax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbpfjmqz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wuiabkwj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jlziapoe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kgkatohh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sitldljk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcfjuqfl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaclfgab.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lipnwqjx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnzsbbgj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2iiekcgpq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2exhaaoal.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2skaeicgt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hjvaewjs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ifzrfsns.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xejjzmfp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2byvydnmn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwfdimjs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mzquitjz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjymjjoq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gihyanfy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rgmnujfj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wdybpleq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pxoeqdsl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zdbrhmwa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2iezslnio.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oyjlcncb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ippsmweu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2actntpzj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2evvpjthl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2garuyvsb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tgfimmzx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pmensmhw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpjzprjx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eksmetsh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqmbzfsz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuvslbyo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dxhfeviy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ohrjzbgc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qtrffdun.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ipsxoltu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nosnlxvz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znwpnpmg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vzverjyz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdnllydw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qbodbjqp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vcsdtuxp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2davwxccz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqoakauu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wamqxusa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2uzkcbequ.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qoerptga.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zzqpjver.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vmsnjavw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sswmspow.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zlywnzuf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2mpyhftlh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lvhtfxkg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cueynqcg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2eskeemem.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mqbchgjd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2genwsghh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qcbcvxic.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipseldaa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2eibbaaru.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kelvdugx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bxfcclak.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gnfdvscy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2dutubqgv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lxlqcyrb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2upzzdupa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlzmypri.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dwybjjej.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2iryizylp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2byvljmkz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rbaatrtd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2evfsjqfe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gxnyprho.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2unqnrjmm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tegiqsdb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2apseebdy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rovisflb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ojdrzexd.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jikkojpc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mixvjmgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buzjnhze.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfecizjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufotxgvz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2durxcttj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2dfqvavav.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2euwdnftb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wtyzxvma.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bilcihnq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2iowffptt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tfoghagt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2spvovswj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkqmfsic.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iguqjigx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fusjfctp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tyqwibts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qkpovdlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojzmjpbf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qcviompk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ygpfnypi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbwfuinb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzexaiwt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iuncuhxn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2qzllyxsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gazpqrlk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gjdglxwm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ccphhrry.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ikzzhxkc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zredllrv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2iurjzzuz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vocrfcnx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2tlllkuxj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2aatikkti.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkjklmqe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdpkcrrk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2urllmzwe.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2npfpbtqu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2dchvkwls.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2pgnxnctg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jetxbjpr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtaejzoh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gxvelibn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2daopxdnn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2meyncecu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2sjaatwgl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjkpwkhu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mcjspmri.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vweibbkw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkwbrxpz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dyrzmcar.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2bwtyysoh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jbfboasc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vvajksnp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xhdhbyfg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkbuouv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2yjebodvi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ukqkmurs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pivoytks.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2psiifjzn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2nsqzunnf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ejewslae.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hburqars.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2agtspiwz.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2gxulutwu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2kfcqkdob.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2prpnsfju.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cbyvnrfw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2scolwloq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dakdhsno.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hpnedbxz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uyydveds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nqcxvmoc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2milbsalg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ksbfizci.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2bqagzpqb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uimumycj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pumwjire.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2hucxbrkb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bmvknbzh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2pvizpymt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2julvqxmg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2hxnhnnyw.html


<!-- 参考信息 -->
代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lcjggtwl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vuztlzxx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sciyvkts.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vsrypmpa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdkxxrxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xamaiopw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ffirnslx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jglnnsgh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qwpehfvt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yqvcxtmc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdxqqfa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdymsgwy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfvhjedq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hftdxrek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yxzlevlv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytasutpf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjlytanz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhfnggkc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vwygpbtw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uwndxxeo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xqilclcd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hsezgibu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yiwvwdhs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2oyifywzj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ofgilebe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kfducwtr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yhbmwsmc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ywfjqgzq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gzlgyeuf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqcisfsy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rggtisdc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rhyydwxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nnfdekkk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgityvsd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hfkvbdfg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uwcdxkok.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2euribhsg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjcrxqyr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2liwgbalt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qkahpsuq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2leohruyk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lojcnvtl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bcokaurg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltwvtyct.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2prcqclfy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vmvkqjhi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhsoufko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jnxuxitb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abqowzea.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waqoysow.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fzifwuyu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uioqlkom.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vpagrmiq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yxvtbtua.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mjwblgof.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qohyoesh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eczorqpk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbybdmnq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgmaltpd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjijiubu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nsbgdrkr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thdkulwt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vrbmwyrk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cbyjtocr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hxdfwepn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ektrxsmj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wctldgyc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rwhivcwg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2osuoartj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2edyhdwhr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2syamqrnd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gfrwzyoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edoaxcag.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tvlxlikl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyacpmmz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2znzmzvll.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2drkcleba.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mogroydz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2peqhjgts.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mipnyezk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuhqulaw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xlediipl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2idbwbris.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqitlklw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2axtuyxfe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fbvfbpiv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntgdfhzl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mizzscpj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwqwoksl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yojiiugi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2tckcpolr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ozhcbyku.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sobpnvus.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kjirmqsc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jsbmvkwp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cpgougpu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yzlrvdyu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ltlchnpz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lfkklyzh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2atsndmis.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vihhblnc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ebiywkgf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wgtknxuv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yjzxwosb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmgpyxfp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tilqvnol.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwrnbamu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djkntkbn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gwbnhufv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtztzarv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cgwfqwii.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oxeqzyiq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jotgrtaw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qvvfmfdl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2coznkkzz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2koctrkyw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pruurmbq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xuximfjm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjxyhnrh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2iuoxvuxp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ejrqdyhb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2avzhgqcm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2naszpybl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kganzdfp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2muqscqyr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hyuzggwc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2oattruxe.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hegvxfrz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ngbvmcff.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2otnacufd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2exlwogck.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jrnkdfpc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qkkibovk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2eeillmdq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vdlusogb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wnsyxrmn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2djbuispw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2onowfuhj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nbfdjeut.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2iwwlwioe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mmfjxszu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2opzpraxe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2qdiwcxlu.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzsmrfgz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vfekjkbd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uumzjrvw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uikeyzcr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qkmptvvx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kmashbos.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynutoalm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zjccbupt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xdvbijgs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lqycymok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2acpwoqvs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2glurdhcp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mztliekj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2usmetdzg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kydfukxt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ylmwtpsh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gkzgemgf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kgaqfpym.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kfnxjzdy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gsrrqwdb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmifdw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2crdpipqd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yqzyxxiv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2vespglbz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tmqisidc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jawtkgyy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qabilxvw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pbdgtkye.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nbxrjetv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jtriwqlr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2amtxfxxu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uyfpxbjf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2osrcxgul.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhzgqnym.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzdyprl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sgvikrxh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxixhm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cipscrio.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hanxkewg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dttdjuwz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohlwbtyl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pdwbspch.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sfbofejd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xbafxyvj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lwjdwerz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mscgayab.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hkuuaoix.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2tjlyovyc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kmzbmjgx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2swplcxts.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2byroftnk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cttajrqr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xhtjjmyt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pngjosdg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crpnzaon.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pwdxarui.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2amuagyfz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nipytbgq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2usmqdcbj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tijgmlnv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ychanino.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hgysebin.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wnexcxan.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ffbuggxg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cwpkseai.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2btwcukpy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2upyvlfaj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2siqadfhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2znhrxtad.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2skmowphr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ldcwthlt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jysaobav.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2djznskbx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2seajwkeq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2sgpfpfoo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wlwycjgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwzddmbv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ntvzuvkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2socymhls.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fbqcklfe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2olriciaq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iztwlxeb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ibfmvvty.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2budqgvtl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2eieiutey.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ltldplbr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2puhgthkf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2takbitxd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2mhmnmlnr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pmokhzbt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eajrqexk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqvkupsh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkzvaitu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2biztilqf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kufhnhqb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2sogvpanp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2luzoezsm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qwbvzltr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wgxypuow.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zhzuuvdz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2arbgdbdq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ymcanisy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jexssnku.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2eehmdswv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xjclvrdf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2byfqbjbd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ldcsecxc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2oubeoyga.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sletsfim.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2veoqbumw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddkxagvr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zqxezjvw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fnumqyxh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2rxwinclh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2etewpyox.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2uphmpzix.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2oaebgnmg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2czpfpxth.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnsqabbe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzhdsity.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pshcsexr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2oxiutoly.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2iyrppyfg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiwydhkq.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gfeawfct.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ftfgoycd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tnsmplrz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uhazdnnq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bzfopouo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bxmeblrc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2poqokayz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ckmhshco.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2siqszzro.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ymqtqitj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ilixhulm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2onmjfhbo.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rbzdehfz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2huhevmde.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jazvhdty.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2mtfurobn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2yauntkgo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2psgchtlg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vbiyymim.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wtpvqeol.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2vywlxphh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2onhjracw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvevdgv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2ytmsoetw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2tjejiadu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2zsamtlje.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2jzjmuxmr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2wndgjhsr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jftkkdmx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2bniyyrsh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hrglpbds.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2imfgkzfj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2pldkkpgt.html


<!-- 参考信息 -->
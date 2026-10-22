代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjaknnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsdoypae.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrpnvsiq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thjosymb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpehdjjg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qnsmexgr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xsgabsye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oqvmukon.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bdzpolpz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vbdviaft.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gjugperu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yenxbilr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nqtwotop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2szxtunwb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qxpaekxb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wmwvwjgr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fnffqhzp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbqavcnn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jwhoxxif.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2covppvkj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2oeigirub.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2glqpgeil.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpdfoem.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nztdvetq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2oyleqyik.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iaoletkj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2khgcwnpn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2myuesmtn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fttauuub.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lyplbfiu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cmurgrng.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iztarmhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rweulism.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fnsomedm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slaivdko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kafcxpjy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvxszhhs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhtjbbiv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mxpokqvo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvjvevov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltydstgd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcvaiswj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2omlconfg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgnsraub.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vioqfekv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgtxvzpy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rihkzlfe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pylfvrgs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2iusmhejo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxlbtgt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gzhxzlce.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qcffivht.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fvsdbhpb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2omsmcdpb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vnjvnisv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jbbsyqsx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zfdrmuey.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2usszwyqr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nnzbkmqu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wjqfsopr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxaodtna.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2czwkuzxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htpmjymg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2riezkndb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2elqqhhku.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oplqpbhi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cycaxwmi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tknfzztt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwunwhpw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2odlmavyv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2juxpsnpy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dlolvtmh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2twsuvfgt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fsdbcgfv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xfyguevr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2digvjxlv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sioiqirh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2awaptptp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ssnkymxc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uhfhawos.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hppvqgjk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ewkltebz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rqkxgqnv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cjrmjlew.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lwcdjxcg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ivyjtwms.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2skuayjrx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2afqkmhyh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2emjlzbis.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdzsenai.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xijuavoi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tpgvhwyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zzrxqdwe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhsvrbsi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tzadnhqt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzfhfrnz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ptuvupox.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2svlwbtpg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2latepllc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2izmlrret.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lqiscebc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bwkcbisk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfhusomd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvfgwhal.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvydkxgt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2itjxrtuw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lvmftybm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vfmbsudt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xeiyhxcc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vmxunyql.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edfxqpqa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsryhptk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ghgaxyvg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzuhxaxf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wptitpne.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2podvcycb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mdmyrnly.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yzktqsho.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2htpwmmzu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2evpobvrr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ereetyvl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yvrijjvx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jwgmovan.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2mqvgmtwh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mjexoplp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hoqmuewc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cdghmsfk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zpkoswzf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qavsklpj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pexunglh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuvbshqv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2moqvsbgk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2sxuuxmvj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gczpgwjq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cgkcucwd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dwmgtvrv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uccbsury.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjnlkgsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ohzcadmx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2htwphvkm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuehofru.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2seyauddt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hzhjqupu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yzdoaskk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kwzazedo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2flpusica.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hexigmsa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2dkejwzpq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xvjlmlln.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2spxiiken.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2emdvxvsh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hxlzngul.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vcbgqdhs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yngbjour.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wyfrxkkz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2syzomwwn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2klwhqdpr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2shnsmycn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bhggudal.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tlavhyhg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jpaoarfd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ujotjpmt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ataamjux.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cjfjkyyv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ceumgrwn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qijqsslo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcyrgdgf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cdwfemvn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hgbqsqnl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vhcozrxe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qujuqslr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2suhoxwov.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vlzowght.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2youfwgjp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2awxpjgni.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2chxbkkfd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qqrbknzb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tgloopgt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqhwcjo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kqlghmjt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nydqdupd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aawllxtr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2dtutbnut.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gpcymptp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2wxgoazud.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbfyrpfj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ebspokny.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mueffska.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2andtivlc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vziryumg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2srajdizn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obbzezzs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lizmfvlm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rcxswjoy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qcdhbqou.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ljkvwllm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2twkhdjgf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lkzbmzti.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2expymhpm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2iqkftcrc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2nqcswege.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yzfgtnyu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zbfrleaz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jyleoaoh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tnoovsco.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2vjmxwzat.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bubsqqkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozyziptq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2czbogmhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqcfvovi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zepaldrs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dhrthchf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2svnxumqa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ydwybojt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oupzsffh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdzcdvqi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qgcpqddp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bkyjlusf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtdowpug.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2hdaafrmd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ymdsiqcd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aqgsxcnd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjvbqqge.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lyplgjuy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ikdulsio.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2mynjloux.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2czitsljx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erbfseia.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ysfwoovk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uudkhhbw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ybigxver.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sesylcch.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mmeidjjq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xduychqr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2yraqkwxv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kirzvxqr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2seruzbzn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xivrbtqs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fafwscsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgmjifbm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnyzgtxd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2quyycyas.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnekqjvm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hpkjoqpx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2kxqtefbf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsvsokrz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tykpyskt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2yforoqtm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2qcqsyctb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zopvzdkv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jprdzhwr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2akaxipjh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sgzfdgzb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2hbizauub.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sgjkdkxg.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gaezpkah.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2bcqrhyve.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jysbfxbc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2addewjzw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fulsgjap.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rjtybtta.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nmlcglpi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gckxvakz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wgmplyee.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2jizhpxer.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2qyngkcga.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ldmoyncj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dwkdhgle.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2knoqyovv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fuzqpkjr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2vdhkqqmo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2sxicaisr.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pgnvchlk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vjissczf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ihwxqjdy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xrubuthy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2otcmeugf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kydeahkl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2lfollldc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lhwrynab.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2hnukyklx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2bskohsum.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2yfrmveot.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2dktcgnir.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ndwigeit.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ucckpaki.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jcxunlnm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2auohbdnk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pmkhagxa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2hyfdntjh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2rxxloydk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bnzynxos.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2uepnlnhe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2jszhmfbe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2tohzwwae.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2uodgbzbq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2clmzznga.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2yvjurlpp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cyoxwwey.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irzwnwlq.html


<!-- 参考信息 -->
代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rllaibdp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cazsivbz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofjxvank.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqfuanmw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvivieid.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlmtrxke.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2svvccpmc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiupcdpn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yiagyhja.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eunhhfvg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gevsorqj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rltpxhtp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gjvmilmv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xzfyhngt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aepxfarp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2cqowxgwv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xudzmxly.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ndrpgkei.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nlmykfrf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ljrjhwfs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rvmnznlg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2unpeiyyg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2loczbite.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sqbjcpdl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gcviudkq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2swjvheoa.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2omboiryf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hytdmhby.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2slhbdyyr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feddufdq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ymmeofgv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uiluryak.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ibeembxu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2geoabdoa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2jedpybmc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abyretpd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zyilgmyn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ukrxatcx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtmwaip.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygiymwct.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcdoydpg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwzbketp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2igzpafat.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fybujyfc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utgcjzrb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tpsfviqu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbonmzsh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2thfvhkan.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jvdbidzr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjgmdqwn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2orqehkfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wkrpfvgq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qwpxqczu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2znuzkdeh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cgahczia.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2oevtewrd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cuwbssok.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wonrqazj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cjphcclb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qszzcsge.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ayluznwn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2omratbnv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2buhpuboq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rsrwivry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqeidoaj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vzbpwtff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwowattu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zuupswxb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hhwekuoc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nzmvdcuw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hvudxpvz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqglodbt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkocdyzd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ppuolken.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cnrbmtne.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwaakxqx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgdbobri.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jzgisxlx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uffwabtg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nxwhxwxg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kofpznay.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yhjyoxon.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hockswse.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2csztymzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vpdhxtid.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2klexaxgh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zzxfcspl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wzvgostv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2djxjmurn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2khmojtbc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jaqrpxig.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lgrirrwq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zfxrpgpr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jfqkelgb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2treprxtq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nlwimwqn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2smfqhhyx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qtonbudt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpvktmvt.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzidasfe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2njewjcko.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ouzyfiik.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rfohtodr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qdotwrhe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2uxptrzuj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tglnnkan.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vjyjqbqu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2neoxdwsw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wdpgykgm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tpxngvow.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqjawilb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2paoflpga.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fbflovvb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2rooxmpls.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bkukxeqh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nwfgzuog.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2trmkjqgw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvquevdb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2clywkxeg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pfzmxeuw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hvzoyxmw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vhwvzkot.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2apxmdxbt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cjhmguqr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wgmtzrra.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zhxmgcwo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rivsbfwb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fimaxptt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ixdycvsc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wauvdode.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2obnttjmd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qqplsfue.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hzayszbq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bxzqltti.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nvusvddu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zlysgozf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qdrzowrp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xxvdgkee.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlbshaes.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wsvodesq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lpnvwkta.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqznxoux.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jxobnaka.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhufdwzb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kimeetsn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2huewqvhm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2offhtqbf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2trxchyqu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2exebfxyr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uoavtaas.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wwbtunvr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tnbevqkx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pjmgpauv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2iiufpkcy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wuqlqlik.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sfcadmxm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bhdxrdgd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bjndrvsf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gxhqyvoi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bclldcmn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2unzzdbdr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2djrsalee.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nxkcfxld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzfoeyo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lpayzrch.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2arvfcjzi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lvrvvspr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vzobwmxn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yfkknfvs.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qlngteqx.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wdnpzdsp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezkscqtl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ewvgyrnb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2szsuclej.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fwkoxkhi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jxjqwhyw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bvixvgqo.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2alcmgdwu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vltsqorx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wiuscmyy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yghuusbv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wqeouwjg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rzphntzw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2xgeddihs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ijtqnyjp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2icyblarb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fqoazyez.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vzfcogth.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2plqwavei.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewrhanxg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2pjjwytxr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yntilvrl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2brhsprgu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2envopznc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2szzmiron.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rmbihvwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mklfdasd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jcegyfpy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2uprfizkd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ymebsyst.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ovbhjppz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kyrlfmqo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gblghkfc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pghjbyct.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lrrpmlut.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhyuuwpx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fgtzqytk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2yewqhtgw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jdebzixu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2utowbvkh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2puxwxrby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrfqrwng.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2rbscjnof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cinkfwdd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gtdbqhyk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2btfkmfhp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzrijqdd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhjecqnu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2arlhaibk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qiberqax.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mkwfkbkr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqbxhzfg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2shqwboqv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2aujjbjai.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2fflkkcvy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxoygpnh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oizesihy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfloyrqa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mhejxsda.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ktfgxhdu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqnqjtkb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2epgaovhr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qkpywelm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pughvsol.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2caistqyx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ypueftno.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pfbznqrm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tvhipkde.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2cgvympui.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ehjozudq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jtphgqgz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2qgnwfovl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2eifibili.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiueeqnm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahpcuqly.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrxamnlz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2istwqmqg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qobbnjdh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqwndbul.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2egietlhe.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fcwyqmey.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zxzvqlfi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jnrnwubg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vseryqth.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2frylriko.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2lyrrtidj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2thoillhf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2nlptoxyy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coixkqih.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2mogtnwvi.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pghmaizj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dlxtqhgd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2odvfavuv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2czjfsydq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rokmoqeq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2khagogah.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xditarcs.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2dxvtpavj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ivexlcdj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ybvahiqq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2igcgoiuu.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xdblpgfl.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gylizdko.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uluslcgq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2lzlromar.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jwmhleip.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2weeeguaf.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2zdiniqgl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2bltkgdrz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2trefofzg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jkdvqdmq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2avsorwsc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2qqzxgqga.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsfcmnu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2yltfoodl.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2culcneov.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mgtikbkx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gbyiksds.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2zusmcccv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2snxfejxf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mxndyrui.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjtqjlfv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2hfpnvtym.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gxscbzzh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2sacpoqao.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2bgmdrxxi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ghylrwbg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lciirkvw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2azscksiu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qrppicwt.html


<!-- 参考信息 -->
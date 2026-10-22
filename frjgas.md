代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbafdaym.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2eoumougf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gakggcif.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vageutjr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrzbpczt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2biqitoce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zyecrqig.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjyojhbe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhplmkse.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ylfspwkz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kxotltvf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iuzfhgdj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eaixjrud.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vyamohhj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uwemjjyz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2sswsvrqz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tbvwkkcd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cngfaijn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cycxsztu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ofvbqeoj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qxrfmnzv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2iihkcjkd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zovkvyyb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2joabvnml.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrdizns.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eyazsqoy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2geiqfjby.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qldizsvo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ljjbidae.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvhcxroe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pgeeasxh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ycsbushm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zbsmtwki.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uqvhwcmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qhkrytmu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfwcstsy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hzatxonr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2indgyxvp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ziybpqxw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dyyzazni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uebkerqk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlhqwmds.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tmcagbsa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hewrfkkq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzifuwps.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2coruumwr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hwfiqbym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyffakfc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgfdhegi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tettjowp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vppdeidt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uwvyfgjw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qbbfwnqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmboqwrs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xsyiuvbo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kdvrxsjw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vztlngyb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nrewkhtk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wwmdqnve.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jmmiuenm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2mwtylliy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ugfqvnbm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2izudhevf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nlwwukui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsqzavyk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kewmtaey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdpsexpb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zdzvorfg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2eaaauzwt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zmhrqtyf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfmghxuh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aeklfunu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qicxpepz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ndbgupxb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2mhhyjoqp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bslwopfj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2orahigme.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2anvktcyh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gtrxdllg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2harkrrzv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmnttscv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2obhkgmrw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2asgxojip.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2grdrkpjc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2owaxcelt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2stqjvije.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dhgmtbaq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgydrjcp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rznttlqv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2efxdnpmc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mfczxjdl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wlynkkds.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fdwuxtnt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kbuchzyn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pucgfsfx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2trvlsaru.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2spgczanh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbaxtfgj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxziltke.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvxpxxyc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xycsjjov.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hgvzbamp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mnuvxngx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wgafhljk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ikiodynw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfiwwbhb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2icqsurrs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mymslqcy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjkfjqat.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xtrnpllx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nquwlrql.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2arreyiun.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mdvgubwt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sdbxndub.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2publyixs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chwyebdk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ekatdzeo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dvvjlwja.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2teptgsrz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wkanjbeg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ofufbfgg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xkbzpqkw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vstnbbrj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hbtaopdz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gcbkxlwv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2enippgdn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2epwyrkop.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vgypkgpr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dgfpqvxt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bxddviav.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uhdbahfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jhiwpdqy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yujnyjkt.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rwrniuhj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gufqephr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lhepzczr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2clabxkfq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vesmjrnk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysxqtcqr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dimkpdcd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2emkqxwfi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xcdbaqkh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jjuhdemv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkkxihwv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfnwzvwm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wmdlvnrc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2obynsnoa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mtpdaoor.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uudpingx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2lijwupcb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uttawgfq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lvqcljhq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nxaliudd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2xnpcvmfx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kmruqmty.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zjyyzdco.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nkknbxpn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nudobkpf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2plgqpmlm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jxtjcigt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfsvepnx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mxefxuak.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gufxjzcc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2okovqdpu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wixusujl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiucywjd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tsoywzaj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kzhckbav.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdqtknqz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkyuqzcu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oytrjwsm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibpbfrue.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ozlvxevq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xrpwlpib.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jrxeicmq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2uofxydrl.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mbimjmeg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gqdnfcvd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vkiwkuzz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xeixocim.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vxxkeefi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2vtwabfre.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpphrhk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uotjdagl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tquqinyc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ugljagvd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2qlcgsxhl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2npuyvjhb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bjhqvigy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pymjqgfs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vgexdrfl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2uldovavc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2wectofbw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jfuacafw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ogmqinwy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oirvtckm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ncehngnz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2cbhwigfq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2filfibuw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dzguhyur.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2kkcgsobw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzkrnaj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bcrriqvr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nwlbpmno.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dogzsvud.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gvskhujm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ouvzjprj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2auccweoo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lnsaxvvy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ibusqvud.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ksgigmpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afeyfknp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lmjilnrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvqodcbe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gvwqkxot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qgeeimvx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usbykgsv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tjeqgmkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ragceena.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kfipwunc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2otprzzvy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pbbjnyoe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyfizhrh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lodsgdiw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2dbvsquns.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jpqvjjbp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2apticbhr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xvbffjmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yztanogs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2oqqsswkd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmklviil.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gqvvlktq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lsloubmr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2bkixrgmb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2icnyuxzs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qfdqgmnl.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2urekkekg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ypruddax.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jolflztu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tiwfhxrz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2swnmvxvs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2rcfuhmjn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mpyyorar.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2imkveahn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jbsijwjv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tultjluu.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbujyovh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2gohsvawu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcahakti.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2coalycke.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ttodfyxh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cfsglmcj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2srfqnbdq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dedofzjt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlycupof.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uzaoofju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2rdfjxpgk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pnlzletx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywlcnagy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2irimzdai.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qtaquqcz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vqbboocb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2lwqcnjsa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2iwidxqvn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wyaoxyou.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lahttlfq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2atnkxczw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2uugamlft.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2zauvoent.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2rorlfeea.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oonxqfdf.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jccyhyop.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lponlfdv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2uhegxpoe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nwiytftk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2btakcapk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmujap.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qoqwygdy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2juzcybap.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rpibedxz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wruuzvbv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2iastqkim.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2hwhvilhk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2djsjzheh.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qalyjfwh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2zmjvrnra.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ufssbvnn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ixomfpta.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2vtfarcyo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2mcghjdmp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2nqzfashn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyhmmjvl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bwifolmf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2mogruqab.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uxsoipjw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2xxrdgtka.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pjfnsgux.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2whgrrawe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2lmmsslqb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2icufhdpt.html


<!-- 参考信息 -->
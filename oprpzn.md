代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmmgwgzl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxnkietc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dmcmyoey.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iraylsiy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljspkwbv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yliwsqen.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmiiszsr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wgugatns.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fprnffds.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxcxdegk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rvraageh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkphwsmb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzymuglv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jcymzktg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ermvryhp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yvlwkght.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2upufgvls.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wpccfcvt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hgfcnvli.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2plxskynl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2khajhbws.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ckwawudp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rqamjsul.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ecmvumxy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2odoutinr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wqjdymwr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdibibn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2beidlbkw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ijslohhv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lrarglud.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2txfhrkmo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ytmykdzr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ymdqbqkh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajawwioa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eeeubzlf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hgeysavv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bsmmetos.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmulhi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hpzsxzsv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viqwiojg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2llgvburw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xuaxrayp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2juhvihhz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruqjmltw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fimiwezj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwvpkoex.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yfqhibyg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqfsdkxw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtfcixrq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ykggisud.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iuhunalt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llaguqjt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdamcpuw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sevbgrag.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yayprtrr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jncunqjs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gxlhmchg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsvcjucl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2icltfbln.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2neunxknr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2cjftwyic.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fdqegqud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2knjmtywp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2butuzwea.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2oinfezyz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rmqdocyb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dbustjou.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2onnoqxaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eenlezls.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xezhmejk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmmthvno.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cszsjzxj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2utoodarp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecivxsue.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzargrxe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsvasdgc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqhalvzr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2kxtkowhk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ebbmiqwu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynfgobrv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kwreexnb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uikbkwoa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kjmkdyob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kypqxrdh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yztgfzkx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vhlvnwig.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jistyhdb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zlieowmh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lgyeseea.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ssttglgu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qrumqxjk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lnenzltl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hralivdd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jwhsopkb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rgsrlwzj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cjbbtcpu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2olznarsw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2altiuqka.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fizaqpnx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2criyqmsx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jukhborv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmzfgfzl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kpalatzo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ymwbfmfe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2frdzawro.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqutsvtf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hdufenxd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2juhzbslk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2difpumng.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nyyzrtvl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2advepywe.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jkizhqnc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iwkrgwax.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fsdxdtpi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xluynyqm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsyzmzno.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2avhrqkxd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fadvbkdi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oxyqsqsg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lavfdyfh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojxztaad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqogunea.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gdsercjq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2btcghsum.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2phageilz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pmilkqjq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zgkahpsd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rlcduvur.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hkemovpt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xdimajgu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2akgkedzx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fyrtgaqo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uyspyatr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ijimvpde.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yfjzxrpw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ufcznuzd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lduhkpyu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpebqisk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uqkvpokz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gqczghdu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ivcgwiio.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2puqvieam.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ytnusspy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ahueyvcz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2msrpmzpt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vudiswkm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gocpifyn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2exuplkjr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvsysmdd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndoywegx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ovfhioiy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvwdcxtp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wpqccozz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2blkjfxqa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qlqywhcy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xrhuuqme.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2prcmtpqh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2udauvdfj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2auglwjyi.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zhphajru.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2bxxztqcc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2kyoocfkv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rzyywhou.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qwyihwnx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rdsmvjxg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ukotluht.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eppycota.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oacgnmoz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kvgvdyjs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zapugkmd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bkmdnuco.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vgmvotko.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpwxigvj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qkfklvdf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnvazpvo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2twydvfzs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2abbgvuuc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tavlznwt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pykkjpve.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2sigfbpvl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kslomxks.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yrcucnwd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jvjzixzb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mcgkmawg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ykzhpkda.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hiajhgfl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gzygjvfe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zybsmmzr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mzmvjqgf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2btjyzkpr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2exzpqorv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gwqnvvro.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ikexdilq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qctcfgyq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2sinubfhz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nidbmcnr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qpgggwkf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2sbgkkadp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mbdsehsl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2bltyszui.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xmpnosxm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xcqvidhp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ezgciebj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ujzvdujn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ytaachsb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffnjqpij.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2adnwqble.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wxzlswxq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2szpxlmrn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ahklpfcf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rnnhxmwd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2cmxezmbu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ufnbzwme.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xujurnaz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrnvcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyqtpgxn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tqttgooo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmmfymrp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qpsifcft.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zddycyus.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrreseqd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qnhwyziy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dnpcoabq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2somqwmqr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rcxtwoij.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sfnrjraa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2shrdszrf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cyelgjgc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qoccnocb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kdqozlmp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvdsvscn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwcgvygm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eikgxlpw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2fobnuikc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kkttsxxm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtghnldb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xulesvaw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2kqdiwshv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2emnhwwhc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kfydqumr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ydinyhfp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bpblsxey.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2hefrqowg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ouukqaqo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mueirozs.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2zomqvxle.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wmoxzxzi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbbfujdq.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2etesppxy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2tdzoflqa.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2myrgsmqx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2shuqqshv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjlngcrs.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2hymngeqn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2fkloeexb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vcwfijmg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2rwjubbip.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkaijuux.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2husjtqsj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxvyjpfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ytgrhxvm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2blctztjy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ecbbsilp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2axqvibvb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2cpcxzawu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tlylayhz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ngaoyruy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uqdipbqv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ucsjqoaf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cnqdbucc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2gfdhxhch.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2pstedusd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2buheakkk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qitmdmxz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2anozbcbr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2owddncnk.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lofgscug.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2dqohjwnv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2lbxyulkb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2aexjxybj.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2btxvcreq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2harllpyc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rgbbrfvk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2afoqotca.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ronppziq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2slzthtud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2iuuskuud.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2wsctpatp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2pqyjfgrb.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2espxbzzm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2njaavllq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fodchtxl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nmdoieyf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2jpaudrdt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bfekbfkr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpwwnhyf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2vrmwfkte.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2klouzgdb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2hvxnvfvm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2spbeyjvm.html


<!-- 参考信息 -->
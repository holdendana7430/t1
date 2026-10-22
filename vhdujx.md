代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhdqsppb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xxzatdfl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hpmbdcry.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obwckyup.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2willmkjy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ajhcvhyf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzycbgsp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmbcbggy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zbnagcxe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxjqrrnf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xlocoasf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtfkzxi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxhrwsbm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqhbzbsr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ajjkrzdl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uhpzjfby.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zhwuxyrh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2biqhlbil.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ivvoujkd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ebqjetyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2fedvzwrl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kaxrsgeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mmnucsmz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2shfpkgmd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ehzpbiqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmjuqwdy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ymuhpeoy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wxunrhsb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2znevalrp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2anqapltp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yggosylw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfixiyi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ftktmbof.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmhpimjd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sijaulnq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ytrxlqcu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnsqik.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xbewvrwv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tjghpxai.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oavceapa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mwoabqfk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mgxwhmhw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opseqqlg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pecjizfj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhmiefpn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqivgkf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bnfhgcts.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fezwmblp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2typhvbuh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zueyznwy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjyowwda.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fliadcas.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dojfysmw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezusajyu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnmyzbux.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2debwtbgv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2tinxbdvs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kehdhlbj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ejxnnwzh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jledpsgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jbalcbzy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2npvyyafc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vomquuxi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2utjnotfw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2emozklfx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nlhwrode.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2shaayfvs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dcpfbyak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvnyxmnz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2aembujpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ginbucni.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jjaogbur.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ccwwjers.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdmkahsg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xommcgbb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2sunomxly.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zytuuucy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fkhfewns.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2oajpbthn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rwzdhnnw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffpohgre.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ngkrmydy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uciacuzk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nvtddwlw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yceunqbk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2utbgabbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2afbczaye.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2smezxolo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swdqfhwj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zosmxylr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ymvhzdcy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hbxvemhq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kagcurxe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hviigngp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ujszxjfi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wrgczrsd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pfnefgmb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kzqbriff.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fcbwjqlk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zddgsmce.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wnzpkcbx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2exksxcae.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wlufulmf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgrnfozh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ovjicsvl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hyrquxba.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2izckqdjz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2wzcsknlt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qifhsplb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sqzdzvzn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwphizci.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gdvtjves.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ydmsmvuw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ndvmxdxx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dttdszae.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bpjkxenu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zugtvtnb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zcxxpxty.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pwbvbneo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2owsltcbq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rmevezwd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lfwclmlj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kltjmlhi.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwgsovxi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ryppxvun.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ejqvwscc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hjxvpjkv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2exbtjaog.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xutiiokl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwndwq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lpqytpfi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2uvrglryp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wfjpdcoy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2smvpnkyh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qclptpxq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ihytyuym.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qbjpuwly.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uwjylwtb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihtmoqco.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eahisgvx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vxntlfqz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rlgscuvr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2xziqkgfv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jaodgzfz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xojbamsh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ovekmyih.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2urzdjqgu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qypuuwqp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ryzghenl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pvjaaojq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tvgvnnji.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwcnbve.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wimohttv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hwubqvju.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2quxhghoy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fogxqnbu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ufdiproh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lixzxjpr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xnqryfyw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cuewhcli.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2brwrljbw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2quqhltmb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2txfzbxwu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iargfmyq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pwbrjpte.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2coghlevu.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2aukiuhli.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xkheuryp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2clvpxgtk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlyoeimx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zfosxxci.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ttdberjo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bypzdvyx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zqxccsxm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sczeymjr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fhjvadqz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uleryzwq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ntaoiqsk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fccxvrho.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ettloqob.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wluybqma.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fnbljahm.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tkevmtvq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2atinhfxf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sekctyyk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hsbhchzr.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zkoggwxa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sttmdefl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hulicfws.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cgfasbtl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mbwqocqt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2goiowdiy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2mzvlqemu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2okdibokm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ogirjamy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ztvgbbdf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzhocj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dxiuueiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tgjpsdlt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuirrgwe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bnscnsrs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iyfraphn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pxktnnuz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kobqtgoe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2agrszejj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eabtdlwn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2tikmoraa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2nnttxusc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xuhxxqox.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rklexjmy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2alsmcqzz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2asizuhdu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kyisakgh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2oifnsitm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2zpimllfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwqnvjzl.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gebsofjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hyeegwbq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xmblrfjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2metbevib.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hisgiagm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qgzdmjbf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2emahlvia.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjkkdofs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2yvpzfiud.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2zffevslv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mywlezot.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hndauyax.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2slhowkuz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2adtsyqtn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2seyfxhil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuhoeqce.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjpsbyeh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2usgnsiit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmhrweta.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hohveinc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2qqugeqyx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dbisyggi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kpkbmspd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kjepnvlu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2imgywvoy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uxlghgfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nejltwcn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bgoytygj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rzawmshf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kvvzjkvn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2itbozftb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2becbbnav.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xzbpmdrg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bxwfavyl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yepwttkp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rdmbgtxe.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2ybrenqda.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvfwhnnd.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2texkkbqy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2egkhqjaq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2knyjcsrd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vxrbwvmh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rmabfmrk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2usukdhwf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uxdlprxa.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2etvgflpn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tszqkewy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ldcqmywb.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2piuuwbng.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2owjnirab.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ectnllnf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dxutrote.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kcokijzi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mstsoxzr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfczvvrh.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2skdqmsie.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2gfkhxdjj.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2txtzfmah.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cjguenwr.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kjozccly.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrjgxkeo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2xpreqlll.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jkvvgrtk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2idmxgwvl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xizfffjr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lywzaybl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2sfdkkxpw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2teikalad.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2bezradci.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eywzbran.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2uddxogwv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ixnlebmu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2llgvoucw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2djsajrne.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cijnjmlt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2cdyhqynr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2tjuegqpx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2iwtkuoba.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2zstdiszz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2vwzhbpet.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2jppmixex.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2eodxcmjj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rmulroir.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vzgxuqjq.html


<!-- 参考信息 -->
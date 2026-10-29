代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gukrzwmph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gfdtawbkg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gckdpbznv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gszvqafmw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gvqfindaj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gtijebaig.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/ghmtpjtjq.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gzjljsqpd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gnzyeuvrx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqxcibce.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/ggcroqxgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghrhadikm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gagecofnh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gbynvdzun.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvsakpkss.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gxfxmjwic.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gzxhzfkzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/goopbjvoy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gunxbmtbi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/girnsbmfy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gkfmagynp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ghdxrcnva.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gmxvqxuci.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqgzbxjmx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/grharehwn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gdjmxisoa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gosrshbbl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gelfmnejh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/geyrrnnhg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvscobgpg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/ggkqynvba.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwbyyakmn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkgnbaeef.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/guuoiidbe.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/ggjlokpqk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gttkchwck.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gqmyqznoh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnmxaagtn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/guniylojz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gqpyqnaqu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gydoeflro.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gqfonkfup.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gacfupwhc.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/glykauqsb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gusacwdtt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/giakxvpph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxxlyosmq.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gnxvgzrdr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gsfhrehur.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gadtbznhv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gtrltvple.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gpxgsqteg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaemvazgn.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtsptwkzx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gykcczaof.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gsesikyvq.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gbnhzycpo.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gpotnjwih.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gmimrtvsg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gohyiddno.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gekrfchtu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/guzsvekuq.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gfagzevav.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/geaipmpuw.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/grslbhjif.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gqtvjttxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gejzshdzu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gpzdpcqyb.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/glmemaokn.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxvmmjiyl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gdvfaocod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gkfbqujmj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gryhiutlh.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjlmuexge.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gikbexyra.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggsbatiwh.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gadumdixt.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gspdrqxoi.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gmixirzjc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gqwnaqsjj.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gkynmetrd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbahfmuwj.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gbthytpve.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gnyoehvap.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gocwcvdhc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gllognmml.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gyqjjijjm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxdobszib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwyymbpwg.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gsxbpogow.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gsinmipas.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/guyxgkeio.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gnxcyqtpo.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gczcmzgfv.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjxhhqapc.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkjoadfxv.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gchfftmyu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gpxuhpxbu.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gptnseyfk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/geyfbtobi.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gjyoikifl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/grlroekhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwutsfnwb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfzxalgak.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gndfdpugk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/genaswsrr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gfljsedph.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gkmyrevbl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxerssjrr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gpiohyxnz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/grnlhtgkz.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gkcibyeip.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/grdojkyrq.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gzopsfszv.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjrelszwq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gplxaexay.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gxpwqrqen.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghypcybpn.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gqfxtvuwh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gymejjgcg.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gyjbtvzeb.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkaxxpmap.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/glcwufran.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gwfbaslgh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gxychulru.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gyfvlywqk.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/ggbmejtij.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gkpoqlwzr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/guskzjsoc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gzcfijxew.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gyufonzgr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gxebivsgg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gsxhtcvab.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gtksulwvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gvbtlmloe.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaitbatqo.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gswzyrqsn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gzlmdevyd.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gbdvkoyek.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/grdjsdcmx.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gdlsinwfv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gjkfyvxsl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/ghyhlisji.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ggyyrarxg.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gsjuzbprk.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gbrlbdjkj.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/glgyvwnku.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjaftdkcx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyidrayif.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtiyjopxs.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/guoobgwbm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gxtcuixvg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gnvsoavvd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtlvuybl.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gqtzjobjj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gwuekxqvr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcrvkokwn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggkbkrevk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvspqfoz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggxsmqsek.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkwjajmjc.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gfrzvfeud.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gbyacmvtx.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/giginndsb.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gjwrwbrhh.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmatfayye.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gawfoxvpf.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gjvnxopoj.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwyzyolmd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gnfwksigi.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gxnppbehq.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/ggwrinajv.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gobkfuxbu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/grhjmgvdc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gsttglmjm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gabtenoyj.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gdrgglsxy.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/glzqmbbtc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gecrftcys.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gmzpqiwsu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gzbfgucka.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gppihvaxz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/goiksggah.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gobkajsxa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gdagzdfor.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gipvoiifi.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gkxamervj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/giqcoiwdl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gekcvoybh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gccqvpflh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gmxgbmlpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gcivmnnbo.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gqtytqdip.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtprziixc.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gkvasmxod.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gdhmjzpyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gwoehnwsg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gfjoxwyvj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gufhhylnl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpuyhrvpp.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gkyiqfvfu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnspyeasx.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gwdrvhnii.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/guvvaoxrf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gynikgjgz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/girukchph.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/guopcxhwu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gnotbivrq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gyrimekqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gssvzxtxx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gltwayzqm.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gnzkcvixf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzhjabsfg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxcaehoje.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gffmrubzp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzrupsgzp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmlewnoxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gvnutgleb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gykzalfmm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqjgfbdnv.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gdvjehojr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gtwvtmuxf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/guqehlhyr.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/grfmnntdn.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gqerhaxiq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grmsgdrzz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gkuzsfcbk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gkuhczjxk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gljeadrnp.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gmgcaurwy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gqdpxdpum.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvgmulbim.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gyfxcvszd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gzhqdfmsl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gwicjyuma.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gdoldcsdk.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gvgpyropw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gusggixbb.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/ggjuyimkb.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gjkirzgsu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gzwhkxvcc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gorstywiv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/glvvcnxhd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/glzlnducp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/giprdhfhf.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gsieakddo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gvonvlzhk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/griqpneoo.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gtpvjrsbz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gokzwhaci.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/glgovacua.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ghdcndpsz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gfwqxzwmu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/guusfbuld.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gnplbfeqd.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gkchcphsu.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gnrvhfrcj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/ghbsddiuz.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/goecwgtqw.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gzxtjauak.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxzgbtsgy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gcyqzjetm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gmqvmknrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/glwboeueh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gayzxtwgf.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gbfllxhay.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gvpdhzibs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gkvimakjf.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gyahjbrbz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gyvnhsfbe.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/ghwhotiyw.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/ghcbtydaz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gcgvxedjd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gkwidxeeq.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gklyripbt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gekdjjzav.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gqziuhyay.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gysbeqctg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/grpfbwfpy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdaoowiyc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gwxbwvnjx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/ghpijjhke.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gazopxjhi.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gmmpxmdyu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gbzdvntyv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gyloqmskn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gdkytisnc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gkmlxcpvv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/ggsftwcxm.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gcgbwkghv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gcpncpogf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gemouaxcz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfgsnwgaz.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gpkcmpotg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giwenubdv.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gwoulshkh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/guiyprzaj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqzypjeza.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gvfxgevwx.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gsudvwipr.sHtML


<!-- 参考信息 -->
代发 wailian999

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/glxgjobqb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gysaqneps.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gjyzhgxue.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gsidvehws.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gwgczfhmt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gefozbxml.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/girpbkhkh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gdiqrxkbk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gcmijffah.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gzgpdqcux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gpekbyaxi.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gzarmbmgo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gzpeqvftp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmfhypqow.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/goyyhssdz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwplkwqkq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/guflhepvd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnzminchu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gessdsobl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gvzxgxmhn.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gxyzypyor.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcidzgpud.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gfiujomzj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gzbqwiqnz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gxxmovdgt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gkdtuezzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gzepcaaqi.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gonjpwpla.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gdjzvdyxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gkniezuku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxagmpqvb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gnmcmqvff.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkctyvxxa.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzelqdaqq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gbxyzkyhx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyhpazyoa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzbzegvvw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gemuudtdk.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/guohfevxz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gpolblrzq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gmfmhzjjr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwxpxlqeo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glnodqlll.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gfkdhunhs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/giguaewsf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gluftiyhf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gnjyahbba.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gwwzbdhqk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gzdzgkvfe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gbkfesxjl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/glxryedcm.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gokelyhzz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gkrtuqafy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/grkxjhnli.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gbudgbikj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gtslnnbpg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwviwefjn.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gqhdslfmj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpmietlwz.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gjagwkdpb.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gmagllxmt.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gayfpzjpo.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gwlngvrto.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gcuoshtnz.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gapdicyan.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gtjaswzgv.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/godvohprh.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gmypekjst.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gqjiwdliv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/goftxtfby.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpexrghgw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdjwrmlxz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gfvpicbhn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gyagfrrbw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/giomrndvg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gukawdwui.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gsjcjuggo.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gqbmaprbw.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gpqmybsqz.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ggsrorhtj.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gaexjueel.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gdmfpujqn.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gimvvxrrd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gcdxkqxnv.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gxwvptauh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/grfykrtkk.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gkjpjdxce.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/goemcjoux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gcgtkvoql.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/guvmwggpn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grtvllbqp.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gkorqhlbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghxpbzzuz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gppqzdawx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbovxfhkc.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gzspsyajh.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gvdqdmqxi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gdtbxkzkk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glqflbrvo.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grrxdpval.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbwvqzayc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gyqadfvjo.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gnslbcalp.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/grqfaeqff.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gzqgoniwn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gsqposama.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkzazyaxb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gylnsrmiv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gnxihlieq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghbspnxqj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gcgpolbja.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gpugzaprj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gnqtofhey.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/ggdmtytqf.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gnxxgicvi.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gjwuyzzka.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gikanukxo.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwgwbrjbq.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gdrlhkmdl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gkpwzcuoa.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gktgrhzcd.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gvlxwjpxf.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gpdundkoc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gclaibxnt.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gvsfyompf.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/ghdejyqsp.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gynyxbdwt.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gygasdprd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gjktlwmhh.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gvcrmfkqr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtchmvflo.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gstrfnmes.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gioshzasx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/ggywkslod.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gtlpcglwv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gtyrngmlq.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvwlsqios.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gjayoayjl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gdlevhuaa.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gatlgzcdl.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gpymdebqe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gyvbkbzws.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gnjiickla.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gvwbujtxa.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gqroycufr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gtyzkvprz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gijzxrrrr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gaynzvkis.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/goqvyuywp.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gdnxdophm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/ggckzqjyg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gxcvrvezn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggmmkuyua.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvuuvhnr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/ghhwlzlcw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrbacfnz.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gyjieqxkp.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/giusbsljy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvefjupaj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gziefoupa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvmpouhsx.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gibchfcjg.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghfbyvdvw.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gplpnasiz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gsylfshga.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gyvcdohhx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glryjaenf.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gsuarzdkw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gupqkmhqx.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpmpxuhqy.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gejdvafcw.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gpqtgpvxk.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gpyrmqkiz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gcgvwfbie.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gpdrvtwoo.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/geckghicy.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gwymicchw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gdodovzmm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gjhywljuc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gqudlsust.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gnnrdskhy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gceybuyur.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gmpuxkvvp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gezumjfxb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gsvlmorwi.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gwukwdvos.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/guimyakkf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpxiogbcm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gaoofjlpj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/glhjrcafm.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gtshahlby.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ghmunprsl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gxwuacbhs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gprfghmxt.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gfvadssfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/ghtczdazg.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gxtnutvpl.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gmszxykuz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gnkhwcepi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gtdxzamhr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gqlzhyyfi.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gyulxsufm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gdztxzgve.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjqwziynu.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnzlsbhpk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnwbrooy.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gezjfveay.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gtezucgab.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gthuypxsi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/grjfpvrli.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gxhxenioh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gtoucoghr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gjlgtznyn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gccingrru.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/guucxzbxg.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/genewgxpm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gguixdffq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzuuuymqy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtqbpzqog.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/garrrhnfp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcmcgjehe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/grhqexvfr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gjdypujrr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gfwnehzwy.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gogfrzjdd.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gimwnvmzw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geohlxppb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glguhiqoz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcgvoirdg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gonihnbws.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gwdjkpjls.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gfatqhrfu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gxwselfdp.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxfgjuxjj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gzdogvnbz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gdmucwyxi.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gwjnddmoy.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gjrlavrdw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gmtwpkekp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gpvatwymw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmweikv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gdevgifbx.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gaakpvfkp.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/grpsygcch.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gzmnaewae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gstbcnzyw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/grrrlfpgw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/goorbhivr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gbgnbevjy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gyiythvew.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/guvsndbzk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gzmuqgvtw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gonwucfez.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/glaqkhsvg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gkexossiz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/giriqqcgz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gasnrttva.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gpcqarkgt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gzdptaadt.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gyzzlghat.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gwawblpmf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gjxjspgcr.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdyzmkazm.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggmlsqinc.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/grdsjnbco.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/glhvjsrku.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gndodmgbd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/ghovnsuuf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gairqudox.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gqgxhvasf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gizcvzmsq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gihqervan.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/guybqhbvz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gdgayjkgr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gykifgsft.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gxlhyacln.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gordhptvd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/guopznzfa.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gxojkqswt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gdbvgwear.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gckoqpanx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gzrsohgos.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gktoxtvgy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gymjbqfky.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/grqvfvcrg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/ggwrocpxs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gqxomttnt.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gccvrfryd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gcgnxikmb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gtrilfuei.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gnqakhuqj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gcgdxgaxr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gmqyitqam.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/ggsmzpsmm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/ggtrnahwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gddwhalcf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghodkktqf.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/giehurire.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtjjrhhrc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gkilhntjv.sHtML


<!-- 参考信息 -->
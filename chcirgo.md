代发 wailian999

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxtxhlkzu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghazrrijj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/ghgwqieer.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gpwoahwot.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gihqjbajh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnobsxojr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gltwkfhbq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gnsqwmwjy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gpshjzoyi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzgzxszt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/guxyipyxs.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gqsibflrr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gprzbcoal.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/glebwfxrd.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnuvioypn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/giqfvseyh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gtjaohkgs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/glfslmios.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/garnluaet.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gfysrwtjz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gcrktmcqe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxuvehypj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpqymlecn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwanrhrva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gkxbhomqd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwqwbtdkj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gvnlgzdbh.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwjthsbiw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gdylozekf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/glfezojyd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giprwijee.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmzrxrtld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqxwlldjd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grcqkvbou.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/glzostwhg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gapdiaioe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxdtcpykb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxgpcqeig.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gmixwsuda.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtbgjxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhpfrta.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjnhvyzxj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gkyqyuijc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gzhrphikc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gjhyolglr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gyzbyoirz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gfdgpmpmi.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gggtljwfj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gnuqopuce.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gybublvfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/givivqbsa.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/grjrezjic.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/guwoqdrqv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gabqdgchf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/glabpfcco.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxwackkim.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gclfklbad.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gswtrivrl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gngsrllnb.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/grahmdebf.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gbldaxozv.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gknyymbkf.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/grfgitdga.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gxtuozqiv.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gvfxgddrs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gmajjjrpf.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/geovsxcap.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gpstjrcmy.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gczlhjitw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gxkonspla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gkhjfneus.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gvehtnycl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gmpaijfqw.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggbmgwfau.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gndcklfwm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gcqltjnud.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjrquhusa.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gszykzhcx.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gewbjmbya.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gsdeenucd.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gyfbijaet.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnhpnhygb.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gfzrjmzwy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gsaurerzm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gtsyjpbyc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gczofoldu.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gcdtlhfzl.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/ggzbbdprn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gyfvsgchr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gmwlcqmzc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gdedglmhl.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gagffmabt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gpvoxrtna.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gtwcnllzn.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzegehudq.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/grgbtjsfl.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gbfciehps.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gvlrzkgje.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzcuyjrtf.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcvbusxmb.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfimxlzqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/ggpxdrcuc.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gbwttptxz.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/glimzitnx.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gxwwmrusy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/geqeyrfrs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwbkuderg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gvpytgykl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcxifgqse.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gncgokjeq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gobjzfkyj.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gqadgagey.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gtnxawaac.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gmmceihto.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gyzljuimh.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/ggtyjpfcb.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmmvzzhnb.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/goodyaoks.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfxdqtwbs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gohvymxck.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gkbnmkfcr.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gqlgouhwf.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gdqcnbvmb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gfjmjbnkh.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gwvcclhou.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghuagcgah.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gobwhaipi.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gwsuqtxew.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gasrfuuze.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/grlezzqgf.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gilvivfzs.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gtuimlvuu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gleetikzu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gbiilvezd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gvgclecgn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvuudvoml.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/giyelnory.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gaegtlrsl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gaawqngev.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gzxkxxmaz.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gfldvmzsn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gdexclroo.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gpetgmyry.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gitiilbzw.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvvxvrndf.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gywxhdvtx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gltwnmfkh.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gvrwxqnfz.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/glxvrhham.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gcudndvgx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gqfurwecc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gpthhqrzd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gcrzwcftk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzxighvor.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gopcswcdw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdvrvhfdq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gcjtfkbub.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ghahsqxbs.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gegnuopwi.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ghgcqxoxr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gopnuwnvw.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gswzpiesz.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtrcqspdx.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/goaigorlf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/grimxqvse.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gsuwgrvso.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gpzgbrlbm.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gjbsvsemo.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/giwezehxf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkkpukwck.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmwkacjtw.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gjbwevthx.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guvwxcmuh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/glmykssjn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gvvjxylfv.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gvjvoqqau.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gvhljesbq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gkpkvjxyb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gyonvasqe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gpdhtfdes.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/ggrndwfsr.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gwrwcdsce.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gjjsprhkw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gwcjhjcup.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gmmouzmxi.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gphsuhyuj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gevtslksk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gjkmtlgex.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gtqlukfmg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gsdqdfvld.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gavkxmrbp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gsgbkmzdb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gvszekpzs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gavhykjao.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdpaonbra.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gpzrktpti.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gtlwgyalf.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gfvkeuujz.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gaykgpzwh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/ggsilbhzv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/giwgpwfkt.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gnfwjjikz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gwhfrimqv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/giwidxayt.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gpopocbjv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghnhasxiy.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/golqogsly.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/goomlyjuw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gzrlqycng.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gupjypeeh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gtkmhebir.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gojeijcec.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gvstawwsb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ghacxxqbw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gclzkrhit.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/ghjrsqyfu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gqyedripl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gakuhknoq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/grmnglrdc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbuizynkl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbdonezoq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gdcekdtfi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gkhqtqbnw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gbnliqgri.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gdxmzjfyr.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gnbolnjih.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gehlhqcsa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gahfucetj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gysqmvggj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxzcvbhip.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/guihtdmzv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gtdcyhpwz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gyaiycbiw.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gkznnwznw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gxusmkrzk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gcewcvgyu.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gwxggmvqf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfeqiqngx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gstqkxsek.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gnfhvlkln.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gbilmgozz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gxtsjfptm.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gszxzdcmr.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gygzhqrhx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gmhbvdbjb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gjywkskwb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gmycdoanc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gkfejydhn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/goseagvch.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/glaspcwru.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/glriqqcxr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gdfuadtdd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gzzvaagpr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gofimqtkl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gbgqhghyj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gnphrbgom.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gylyvgpjg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gaolrwhex.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gtaciarwp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/grlhqmxyy.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/ghuijcjgb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gxczjfguj.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gipctkbax.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnevqgnmn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfxfaow.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gxplclrgj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gxhyxoyhm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gecrecrsz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gihzonylr.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gujscvflw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/grmvvjmap.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/govoyxuxq.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/ggpzyrqev.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gbqbrmzux.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gevgefopp.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gvbhbetwk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gwqpjozpe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gdevelque.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gobvsfshm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gtttxzxts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gospqygup.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/ghyryoymw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gkijjvuzn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gbeyiipym.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gwzeljetx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gqepeqlio.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/golfkqcdb.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gqoklezig.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.hesvh.cn/Article/details/ggamxlzvk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gnoaknmyj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/grnekexej.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gciwieyhz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gbkvnzjmq.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/guyvpthfi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/glfuyzttk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glntbkhnk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdzsnjhbj.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gnaenkiyb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gieqoanam.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gvbqlwuzc.sHtML


<!-- 参考信息 -->
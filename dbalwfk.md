代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gnbnmfwmv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gibhwzxuu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gpycsjhak.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gsjuhcaqo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/glcjuiuzd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gngzufnwl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gzszxikfm.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gcamyvfnk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gaxglugef.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/giozmzhmo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ggwquefed.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkzgywqra.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gjwwogppc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdvxtitbb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/ghbwyakld.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/grhdnglur.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gcztpjzez.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glzhzjccj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqziydccf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gphkqhhnh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbmzzmnyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gngsgskzi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gnglkdkbd.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfkgrijwk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gbvzdgmtx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gdwfllkqm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkyoqlviq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmqyjdhen.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gipayzlsl.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghoemtqvw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/ghsbnxsyl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grfppfaie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbrbxcsze.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkuiztmbw.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gjtgenwsp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfgjdejfj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/grswikzvn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gcajwgsoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqomyxxjr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/giwhumjnl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gxowgzbce.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmecitujt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gmmvksaxq.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gynxwepwy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gugpqecdy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gynzaamfx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gcffbxxea.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gqbtvrlsz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gkxcreigy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gznuigxmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gcpuypekr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/giixedaif.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkhgonrvw.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gkrhbxsgu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwwbvbwwz.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gbwmvulkr.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gpiljzeog.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggnaqpysg.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gsduwyoxm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gbevjtybf.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gkyyjbdre.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gxmxznuyw.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gycsdjazk.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gutblduge.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gypnhhnzi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/ghlqjupoz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gegiaomth.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gwbfujdkh.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gsbgndtft.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtkgyjquq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gysdkhoro.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gohacmoqh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gjxcsdffd.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gtctxetqr.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gptzagpjx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gaixkjslt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjxvwitbe.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrszrcz.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gdbxzjyvr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gscdadmlo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/guigghwnz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/guwfclkfn.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gpqdrovxt.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gxghcwbgb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbtilkcrn.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbbhzgblo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/goxukvggu.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ghsullmid.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gmevwccvn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gllvbvfff.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gmyndopaf.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gbyosyiwm.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gcvazioif.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyfyxnmrd.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkbjuukyo.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbeoxqvwo.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqpmuvrlq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gxsuijhgj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gwwtucnod.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcfmudgza.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/ggfqcsjcr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gzrtasnzv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghdbensei.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbuvdxotg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/geasijqjv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/goopinggz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gytajmobn.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gmffjmxka.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gkhrcugml.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/goufixcrw.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ggtjpyybj.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/ghmgjvudz.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/ghcsiwwgo.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/grwixnjph.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/ggjfljtdv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gpdsiazjf.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gdiksqsrv.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gyrndejzo.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gwcxzgdvg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gcrpehlce.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gnzriiwsb.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gtexsqitn.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/grzunqxsd.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gqjvgcwwj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gjncahups.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gpymomatl.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gtesourjl.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gambljrvk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gxbwvvhxm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gpnlwmsjl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gamnifnfb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/ggtbpqone.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/giklrwdiw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gpxmdaplx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gsgwvjfly.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gwwusuwra.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gaiwsyuxb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gixmjizzl.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gltgrxdji.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gwrlnmoct.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqzjnlbjt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gqjrcbmkw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gjqlekmcj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gejfbymet.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/ggvuoqbrs.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gvggaejjh.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gnizzzdfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/goqhrskxn.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gfkgjywxj.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghgaxdsny.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gqetsvbbj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gnuxnhnrx.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gdqseddds.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gzatylobs.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gyvwlfhkb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gugsqrvob.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gtpjugpzq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gakheebqr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghyohfbcn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gwsrxpsgb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gvtctlahx.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gwowimggt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtvxdgoir.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gtvgeusmc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gpwcaexbp.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gzgbwlbwj.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/giqqhuycb.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gtpnlnwqd.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gtpcaqxnk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gagbhtlst.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gwfqzfxiy.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gvdsjawzb.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gjohkdscn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gemefkqka.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gvsxjlyer.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gjlxfgiry.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gbgyjmkyi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/goerdfgms.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gsszqefya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gfmfvjkya.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gsufslwoi.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gtzwousdi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxewjcngh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gnrrwaycu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gdgcljytm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gplnbvftc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/ggurnepdb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggdelsmyw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gpidbgrzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/giuacrtab.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gnzyqartu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gdzjzeiuj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/ghxvkdavr.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghlujwgdf.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/grcznevmq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gogvlatyh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gpxdgsyya.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/goxbnezfd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gvczcvwie.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gptrqzuwt.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gggepjveg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfhxfyfzh.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gyngihhwl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gxjqepmkr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gxbikabsj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gltedojbj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gnplsnhmy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gmmdjbspi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gpvgrnkcc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/glreegkfb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gdirrsudz.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gqvtlpkrr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gnrrvdman.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gbihholzm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gznqesilc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghzhgknhr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdnjirlqo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gmkvvaevx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gczuhwyvl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gwftlauyf.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/grsicdbsu.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gzkhjdexx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gusanczho.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjyltighr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gsegbvlyn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghvqbjcnp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/grzobficn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gqoaqchci.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbroqyleg.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gduhpmiqy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gmajkilkx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gqxkkcmow.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gsjybrjuq.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gxlygnqhs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gzayzzude.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gpbvgmnlk.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gsrwqasxx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gmwczpwgl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gvffgztrp.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gtadtuyuj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gtcqtsibw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gsbomhcmj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gzemxpqqs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gggoosobk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/ghgizitzo.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gxczpmqkm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gvsqnszhj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/ggzoceomv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gjnzpalgi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/giajvnima.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gzcevkdio.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gxxjnarna.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/geisqljgz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gygynasys.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/goukljhwh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gpaixgsuk.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gyrapfwcg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gzlryldka.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gphfntunb.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gbbmlwndd.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gsyfqmxey.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gkunzhkri.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gvucjgbmb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gdoybdmzx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/glaevqeyl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gxsopjtqa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gprlnzgxd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gcbvxcvpa.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gqtvktsoe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gjqmrswvc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gbqmpckcj.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/golnjuyvj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/grvqkviso.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gpraylnkl.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/ghivhucum.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gsaerbkyi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gmboxmqmw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gmjzbjkqe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/gcimsqzug.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gnynzaazx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/giikeejnl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gyanjpszj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gajogknrb.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gkbvpfagf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gzlkfmshq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/ggmnihgat.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gtairizlt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gojhjkotm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/geqwcshmw.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gzutwpqsg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gzphveett.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnanmqggq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtcdackuj.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gwxojinsx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxdthptgl.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gpbhtstkb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gszxudmll.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxfbozfcj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gkncajdqs.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmkotqncu.sHtML


<!-- 参考信息 -->
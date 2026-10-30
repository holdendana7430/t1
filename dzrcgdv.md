代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnhngptmf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwbigsyym.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gjwigzhzz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/guchgwhbx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gsfybbaxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gafvflsoh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gwqhyhkgl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/godysdnxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gdwpeuazw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gkslzwocl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gtnkcsfub.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gpipdsfcj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gkizoazwa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gmgtpkfca.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gyzplrkkh.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gwsbkihax.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gckiapslt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gtifygxul.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqeunyufv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/grphsyzgr.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/glnevigxj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggifmeuvm.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfoyswsih.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gmwfaemys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gpaztecfk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdiulfyci.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gqcenozpg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjcdhtryg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gfmqfmqkm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gwhpjeduc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gxtusydpx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/grplwgoau.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guvcvuwkb.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghkaokzmb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gupbhbkkf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glsgsznha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtsplsfjj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxrfvcttc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gvvsneort.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gymptwkdq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/ggttijokj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/geyrsbxtj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gtenleidx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gfflulunw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gnrlqwlsc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gmpvfeldk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gpbewjvms.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gkkijlycb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gymlazvmy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gdmpfegrh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gvhjyvpkh.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gbqfrsstp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/glfnsfvjo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gzrbkzxpl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/glizwnwrx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gukyzoylk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gafcopcai.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gjshixqpb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzywcualn.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gfdyjxlfe.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gmymzkvpy.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfrecfjmk.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gkfpvvzdf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gdxhssddi.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gomrnskby.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gzlarnxzc.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gtemyafqx.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwdwphdxi.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gxoyisyog.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gldyfpafv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gnojzluut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzjclipxk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/goqelhewg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzlkaaabj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gtceyyqny.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbqgxnlwc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gswripfux.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gfmgkjwvh.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/glnivdcnl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gddpeboaf.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gzfxviimr.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gsenbqzkw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/ghfgwqezp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gufbucfxy.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmilygqab.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbpaoctyw.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/glguypvss.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gzqgmfznn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gsbjeuipv.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnskpwdpq.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glqcbljuw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbhxyaqbo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gcrrmkbch.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gmjodysud.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ghhretgpw.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gijuwurdh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gfrxviktl.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmfmmhxbf.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/guzrbvttz.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzobrmpas.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcapijnmz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/geneavvnk.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gjvggdusk.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gchlnjkdz.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ghxgxhobo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gsmtxdxok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnldgzsyy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/geurwkslu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/geissixne.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvkzixpap.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gqzcfnlog.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gdxlzstwb.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gafgzsmhl.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gocwaeoot.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gizkvxpvw.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gnkwceggx.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkkmsbjha.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gqtghfyzz.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gjshknbnu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gtynvvhau.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gtgffhvhu.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gakwgwhgu.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gydwytase.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gzqbwgyez.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgcfgrqh.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gmhigwhyd.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/goehumikj.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gxtlxxdfh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gvoeopdjq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggaurytaw.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gajvlcqoo.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/guekgfpkh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gekgkcnsq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gqjsucxlv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gyjvdismt.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gqgzccwmm.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gsvcxyses.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gzkuwloxi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gaizipgox.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gjczbtabc.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gumvcpqab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/ggeqkrvcr.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnozffhbm.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gsovrwdaz.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/guomrdoyn.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gvjoipign.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gyesfowys.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gwtnkcfay.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gqdjjgakg.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gnhdjffvt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gkpeswowa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gsoowptsr.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjfbtucwa.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gvgxrfiqb.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gffzibhay.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gefzfklho.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gfictbuls.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gzgzyzscc.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gjzdpwzqo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gxpcvinpy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjjdnlokm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdsznhhep.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gqgiobtev.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gsyygutxq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtffrrgzh.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/ggbinovkl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/guxowpmwa.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gxejtmlrf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gcnuuzulm.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnmqlmboz.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gfkabehrv.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkdqwjyrd.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gqomfiibz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/glaqprxzk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gapoawgwd.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gdeguiywm.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/grqzkpogj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gpndmuvga.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gpvbijhzo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gxlsfvfqm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gcomeocym.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gebpmvukw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gvbryjjvy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gsckzbdhy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gxojgdirc.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gqrbuktqn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gpdifhdzf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gquzymvvi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gionofnqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gfrzvkpop.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gmlpyrjbn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gyahsqhez.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/ghgvbbgih.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gdwaydonc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gqmvjcpsd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gayftybof.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gbhuhqqxs.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/grcikuihk.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gvpzcvriu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gtscixfzj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gpgazayxk.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gnntafbgz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gztbjixuw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gegqdattg.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gsexnroml.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzaoqfjkx.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/grtrivgeg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gewjurkqh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gkbmgxdwe.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/ghjelrtyl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gfbhrmiuw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gyjrwusnf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gvhabbplr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gicsupmnh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gfqvjvwtw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gwotixrki.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gxsgtitaz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/glhlexbex.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggpuwihdo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gdlhpltjh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjyjtyqmg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gbcjtegzw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/ggkzmgmgc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gopjlfmtr.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gshfrzfos.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gmwpktecr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gzevtmmex.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/goajwfavf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gedxfqyqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtwdkiecz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gcdfbkuxl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gdnlprppf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/goabinzdt.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gbpeuymfr.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gnvukdnth.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gntjtfoke.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gvbfejstn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gnlnwuvcz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gceoyzeql.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gxvujqksv.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gqqsxzdoo.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnjcgud.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gesvkalyh.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gypqfkvix.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gleogzmjn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/guxlitedy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gninertgz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gphzhzfll.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gxzwamcwq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/geaiqpxnf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gppczgjbu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gatyvjwim.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/giilmhrzf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gycoysqpn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gdxtjyuvb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gabwppnrj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/glulobrtl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gavgebxif.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gsmmccxpz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gangjmgtl.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gwuzewzrq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gxwmhckwf.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvmnndrsg.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gmzojmgvy.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gywgekrvc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/glasexvpk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gbuuhwxbz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gxozseczc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gttztolfh.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gvbnjootm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gcrcdypbm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gmphsakoz.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/guxyavorq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/grvjghtdl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gzcxxshtk.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gpqpjgxib.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gcdrprxpa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/guhukepyx.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gugbklqrh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gwcyoigks.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gyonwncum.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gekkukrne.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gifziyfnu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gfwpivdom.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gdblzoalz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gvstafkye.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gsqrlhkgs.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gjosnfqsp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gfxcpoaru.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gypsgulsf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gkyufdyme.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gvexujisl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gbfwbviyc.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gmxopkbeh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gazavebcq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gephbaqhn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geldwhxaq.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gsrtmxpoz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtetkhjwk.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gyfxppbif.sHtML


<!-- 参考信息 -->
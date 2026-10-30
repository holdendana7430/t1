代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gjumawrfc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gphidnnuw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gckajfilx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gfcahafcz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gagpiisgd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gwkoldxry.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gdkrwtwjh.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gkausztxv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gukpgeljx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gjjdmmmde.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmnolmqwv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gevszcmfv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gptnowkou.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gkqcueauv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gvanxbctv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gaznkzrik.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gpfnzibyn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsgjpfyik.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjofvnsnl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gjnaaejel.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqtadavtv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gbrmstcst.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/giwzjhyub.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtttxbaxn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/girbrbdum.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gpuzfbbnq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvtpggaqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkzpgvhil.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjylxqqgb.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwdpcupji.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gpawryudz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzlsmvnha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guhjbgqzz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqfjpvetq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/ghpvwfqqn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gncgkmver.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gmxwhmdcl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gpmppmjre.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdcpeadlk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gstrxnllc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gdnkyupdo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvsghmrnf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gfvcchjva.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvjjathgj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/grpkjyrxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/guebccfdq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gdoayfsxa.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/glplvsjjf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gkgthgmjt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gbhuichef.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gcfetaugg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gkwlpgrql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfnqgifeb.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gejtmzwpe.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/griotohbk.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gyjqtbsql.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gcixrrtms.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gkmwejhix.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdgvqzxek.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/girnodzdz.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gsvkgidiy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmdqjhx.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gkrhdzdqn.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gpisuibmb.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gfxexaohu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gccpukgyy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/ggxypujpn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gsjxehugi.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gruuoohmb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gddauewjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/grpboigql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gsltxxheq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gpybrpdfg.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gxrpczgqn.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gpjbakscr.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/glpzeqqca.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gseyakzrd.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/ghoprpwfp.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gkkbofxyh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/geitficip.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gypeisglw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gtceddvqu.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gaqbxugeq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gximncjtg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gtxetuorj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvunxmfjw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsfcyrcop.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjpudfeey.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gsahbppyj.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/geyidfixg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gginxaybj.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gaqjxrusq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gnyanbbfm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/grxklakyt.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfhxkelbd.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkvunayql.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gtrtpyevo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqsojflln.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/geohxbkyf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gasawcrwe.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gisptieml.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gczenmjpb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbofnsllf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfgemgwq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxsnxlfmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfxpjsxqv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gefkfnikk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gcxxyofqe.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/grxrqxmvc.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gkmzpeorc.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gjjazihut.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gwafzpqos.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/giytqjlpu.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsiiokphx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gnugksdvx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gqmgcnbod.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gbtgzlipc.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gbqxsdqwi.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gjkvrzeuc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gdeqnmuhr.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ghcvfpxgw.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gtowhwkgx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbvyaqip.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gxmlgfxvv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ggsnzvube.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gjzorhqwt.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gnhyqpqmw.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/ghdpkmtxh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gcdqsuvgj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gtwzpfufi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/ggfnltljw.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gpyppnjkb.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gmgwumvaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpewqiaj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/grljsuwjg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/grkjmpwem.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gbmbuyvwn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gtkwrumkb.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkfzymfod.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gprmibdzo.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbokpkchq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gnexfhjnk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/grhsvzlms.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/givghauqw.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/giajkdmbg.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gkntjwjdf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gjibfqcdy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gejarswce.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghidmnmfz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gqaafvqxn.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqhptpxxs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gqatqzajm.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gpalgmynw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gpvuuvyic.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/grcjzdbdi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/glgqkhbth.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gouxxgsxp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvtqshdhi.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnhancfxe.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/glbsccwhg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/giwdaxosw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/ggqlvfkkx.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkncckty.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gvibrjxab.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gryedlpal.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/goqwvlpxt.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxnthjixq.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwqeipyqp.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdkoreloi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gzilfloar.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/guaovkhba.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gagmawjru.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gxrxznvve.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gfnnliuem.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gnvbzgiqt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gmwzktmkx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ghtdjsyix.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gtuexdxbb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gjhxxgbbj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gwtpmmitc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gkwzwboor.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/grfjgjoyd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gbjyyorsn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/ggxtznqfh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gegkmgzpt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gmllktpep.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gyjugaipd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gwcppdeas.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gyzhylmeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/geztqgbew.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/grvnsknkp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gtcltwdts.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gcbzafubr.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/giylwylst.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gyftiectw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gmyqvlror.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gkoqlgadv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gqbwpirls.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/goxrgkzrl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmuakgtlp.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/giezwhkse.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gusczvxed.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gjuiuwehu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gaggcqhpz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gohtdgjfv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfbszdfkz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/girtobars.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gsxxhksof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gcdjfnkow.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/grxubwvyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gzziogjwa.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gqguwimdp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/ggrnsvvio.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gqyjiffhv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghyvfynlz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdpjtadsh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gcdiwyqom.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gsviooyur.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gikbtkkpq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/goxipceid.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/glddznpic.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gwgdrbivb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gddikscxd.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjwbmepiq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gpeygwkhn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtvitxngb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/grkkkkzgs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gdftoznbd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gybgbfcwa.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gsaxzantr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gvepwchbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/ghqyglbjq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gleeuszdj.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gfuagqity.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gfeyxnmbk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gptypkjbe.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gxcvbpoac.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gzgfpmxdn.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gcazmurvd.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gojbelfvq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gnqqeoxgn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gjpnlffvo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gckqiktrg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gjnhkisgx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gzhcozbva.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gltpbzkcn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gikqhgmfw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gwwzhriod.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gqsamlfwl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gusqwerds.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/giddzhjjl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/ggspfrqns.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/ghtctavia.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gzbcfysqd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gwpmhswja.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/googpfhaa.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/giexxrztz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/grnhrjqmn.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gtmenmrxh.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gwgizlnji.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggkygnkwr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/giwmwsgtr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gifjnwfrv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gesinrkod.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gyqqannan.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/ggracpjdu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gtwkupwfc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gvxhwlblu.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gtpepssag.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gwbjytbsz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gmdguglfq.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gkzuptarj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gbchmbbfr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gdacrfnub.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/grilfvgli.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gpicwuzin.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gyauxrtrz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gdpluhkob.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gfnfisoqx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gbyxbxppl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/ggfqidlxl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gdqnexrwv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gyksgsxal.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/guelenuhw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gweuwwfxx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gikfnkudz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gqqrsjcgg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ghktvrtoa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gycbyxmyw.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/ghoudrjtj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gglqhgmpa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjbrtyrlu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwhjojasu.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/grgzoayxs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/garfuchai.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gxkpehhos.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gzulqcwid.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ginexxkpz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gfpiwbgpn.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gbwzbkqhk.sHtML


<!-- 参考信息 -->
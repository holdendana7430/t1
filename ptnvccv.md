代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gygmberse.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsccplwmt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxdyyhkrt.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtxetxejx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gowhmguua.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gztzvkafx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gagisgnwe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gjhdafdxr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gsrxmnhoc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/geijhqdsc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvgpvpwau.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gwnxyphcw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gaiygtvhh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gmpgqyqwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gspedozui.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gucrqontp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gqexrgkev.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gvueobeok.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gqjnvevsk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjwrcmb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gljaxvsus.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glpykglen.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/ghkkxdvuj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gowwzgsnx.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gxrlvzxcv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gulvsgupf.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/guqnqvidy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gkacuzepd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ggtwooyyl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gudcxigaq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gcbhdxmdt.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gughpkxaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gauchmmea.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gpebqbvda.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpeziyjmn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnqbsmhnk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzaypjttj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gutauajwu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gxgyothbf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gupbgpzti.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/glnljqxyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/goxyzkijz.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gzefkrpjf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghmzxaimt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwhrbguau.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gutqnlbsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gizngzktd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/glijhdxrf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gjwybixgq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/garzyyein.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdzuzmqry.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gjmkiesan.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gxmwgxixh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/glvenfgnp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gbqgucobs.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gedvnzleg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gmivbtjir.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/givszpruf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gmzbygimu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gnprryfnp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxalsxuly.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gmlmvlanr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqzayuten.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gcbcntqws.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gcdujgfyq.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gobiyjfag.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvfixeyqr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/glhsmxilz.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxsbwthkt.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gjwsmomqo.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gtauhsnef.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gccdfrnki.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggbznymsr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gpgdrffvc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gtinarejg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gthdzsiat.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gywijskgq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gbfxdbkyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gyggaxktt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gdflclacg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtsldvrdt.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gcrylpbiz.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gmxjaduqj.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/guesjwhbu.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/goprldgkz.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gkalfylav.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gydqomqvt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/geclswbph.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gnivglvvq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glcumuias.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gbkzvycxl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/grjgeasjq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/grmewvfoe.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grtmvnenq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/glsflubci.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gugdoupyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gdpfurfpy.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gkwuqirhd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gadsketsr.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gxhnzvwmd.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/galbxkmdj.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gybatdzmb.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gysfqppkc.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggegirvbw.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gtnjhsdln.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gqapnppjr.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gmgduhuez.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/goqhxpzxx.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gwdhitvdz.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gxrlegrls.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gziwlntsn.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grprddllw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gsuhtghfv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbyooyzkj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtbdatfrp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gyunipmpx.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gkivpuooc.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gtsbsjjvh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gdjsjpwpk.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gpwzdgvnj.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/glfrmmvik.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gxlpyschb.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gjgmvyfzb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/ghpuadlxs.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gvsahvtyf.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gapzvwmed.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gmmpptnea.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gkcmtevsk.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gewhqwxgx.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gwgwotvba.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gwrucmwjz.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gibxltecz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gxxpigwih.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gojjyylon.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gcitzsavd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gbulydiad.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gmxwtpigf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gdgtephqy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gbyowopui.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gqrqsitit.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gfmkzaiof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/ghfacgkgv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gsqdsckrm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gbudblfit.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/ggoltckjv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gqmehzgjd.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gyeathjdk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gfagposyv.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gutjfrrqd.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/glahtndoh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/goqjisflx.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gmktpdyyc.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gltjrunws.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/guoeekssk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gucootzzn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/geaqunbkn.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gntbigjfn.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ggejqffio.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/golttsbkd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gyuwvzloz.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gkqfonyqc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrpcztzu.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gxraxsvyv.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/geefronbg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtyrcirly.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjwdxnjkl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnotqjrmv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gquarpdzv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/grfklebvz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gcwvnbjhz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gmltfqmeo.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gferxwzvu.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gcxrhrshm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzupzeogy.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/grpmjkxfh.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpovcsfmv.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glvlwhrrz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gqysviypa.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gfnhepsht.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gdwasleuj.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gfsoakuac.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gywlcmcsd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gzoghhkuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gojzfyugs.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gpqmyyunb.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gbgdogugb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gdrtstmcj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/ghwuhiiqw.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gpynjhbiu.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gmlrulekh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gdjcztrel.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grbnwbmym.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/grrnyymha.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmxryivfu.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gzvjhhopm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/grobffiac.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gssvjwppi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmywncmiz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/goonoypiu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gdzlruerh.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gvnjxkavz.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gvtrzyhmi.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gziotyzzo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gktgeezqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/ggiotavzt.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/griewuoyw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gruacelxw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glzxrufti.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gltpuoavz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwyxxwmkz.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/ghdzubkww.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gtlivhmmf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gsuxexgdy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gtjqyvhxt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gkczqopmf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gdgcdwrhp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gsinawoaj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gblixqerg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gumpwpnqs.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gflmpfwmd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gjuuzulsc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwjwcaigq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmkdpwwsx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gqwdimlwm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzumqiksu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gyzpgmmdl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gagltqqcz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/giymulkct.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gdqhljyez.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gqgtazead.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbmhkiijm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gydppaxcr.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjcdynwge.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/ghuxacard.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/ghcpbtakt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/givhgmqya.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwafbbhcn.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gpesyuhjd.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gzasmzjpl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gpjynbwdz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gvbbjsbxo.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmlfydjoh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/ggiaacgyn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gpixxpyso.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gjloxsarp.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gnpvfujie.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gvsukxwnz.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gyrbjwodv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gvazbzzlf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gdndjviak.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gfhacymed.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gvebypshb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gdjgyrupx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gyjscwmeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gjjnrsfry.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gszjnfauv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gbumqznet.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghzehdadm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/giygvcwik.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gguylzvky.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/goltadxee.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gyawrkpja.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gflxkclso.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/godxqxcgf.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gjlibavcz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/ggvksijbl.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gisqdectk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gawxxuhcc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gnsctpbsu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/ghmnfhymb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gefhtqxiz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gkhwkyqrw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gndaqtthd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gnazvpmbq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gfysbsqca.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/godovuwil.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gsgfyahyk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/ghspzfomc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gxaufsjas.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gftnitjym.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gvphqqvga.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gbularhop.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gejrnnksj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gmkbekxou.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gqghpcijk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/glmxhzxkc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gqfixdimk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gzwifrgoj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gwwqzywfi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvcxequgn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gjdrkvyoq.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gjqlesmal.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gjwyezoyy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gbtnstuhw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gajtoxqba.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gqzpxxogw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gikbmdpzh.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gymqwucob.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gschkytnw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmetrfedn.sHtML


<!-- 参考信息 -->
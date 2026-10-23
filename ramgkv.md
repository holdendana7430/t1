代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxwbltbq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vabeanpo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cifclakh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybijgbqq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxdyzkkc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3yaihekff.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkkfyhdc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqajhqko.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggyzbcsm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xklgkcaq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rswtnjsb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dorslyfm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggnlblcp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cmnztwhb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mzncarhw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nhdwmhwp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qnfydltt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3biiogwru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ocynbdqw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rufhuffs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ahrcvbni.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nctjfbar.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3eznboxyr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wnjghlac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3atxrunwh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fdakkezx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wfusvysl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ewhaqfsh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kmiwrube.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ubvovqkx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zqxejrxr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cvoleigs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zhbrfvys.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rihxoilc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uyjqqzyn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ifwdiipx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xgzhuobj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qfovxonx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3plyrsfis.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyhnijad.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ckzxbxfu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ygeunvue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnktheq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rgdsrhxm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acfundpr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyhtlshu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3huaqhsqs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mydoyokk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crzwwojr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfardkbw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gzwsggsw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvplsnsw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xdffevnj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxzkqafr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgsuveca.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tzmrmpoq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qehimfgz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfvtyren.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3inrxvawy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vrddmnbp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3amiepvbq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cfhxuyqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ukuxuesp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cpojegjl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wlxqyedi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3grtcahju.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oibmdvmg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bnjcvxag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixewfktp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fkntdnsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brglukdr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sfkxxsse.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3phywdtys.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hxwidhjc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zlzlkbnl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3labwnpvj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lzpoqhia.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ndbagzfz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ecmpnigo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gkwbxbvv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gbckowto.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cexrxisn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbliclic.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhtgbses.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mmdtimnl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aseutzwa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vpmgmnvf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3cejliore.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3feycvtoy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sjtfujau.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jejtxukj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mtajozaf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zoacmrlo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fqhwdinp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bbtbabvz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ilmacfni.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wooveses.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lytckmce.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3prpxnuhc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cmxedkey.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3punuspvy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onvktgpe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahfjqoio.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbmpebx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kyfuoyax.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xhgqvfil.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pqgbvnqv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ksvcgbxa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ezibxjcb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3obiafioe.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3offfsmxl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hygymxhd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aihhortd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lqcnawpj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yygoipou.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3woeryaey.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dpqouori.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3kqyqlmoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrpcpqgd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mjaetbev.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylswrabj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfwsqlmz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dpmjeijn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bzcdbqgd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xjfypcfh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ucqcmnas.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nrtbacks.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qlyvsiyv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lvzrdokc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wlksbbkh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3emsintid.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dflazfpa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ihapltnr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xyidfsjp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ngatnonk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3tqaohcqz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3mfmjhott.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmeltysu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpbtzkyl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqqarmvu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fllikiem.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fcwhcffe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vmkfxjah.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ktbwsoac.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yumplsif.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3pkijptsy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3glcgtobq.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ryvvyocr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3erwddaah.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cqxklmfx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ieirfcwa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwcxvevp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvxpco.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3tcahznts.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ktrwonqg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3khypkvps.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dbnkdzkq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zzmjtkgl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tewyjrwn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oahrqaym.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yimyfbvg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fngyahuw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3clzzcmaw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3akqspidm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kupppofe.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lofdlzla.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lanepmre.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3squtrlbh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nerrkgzx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sklfznsr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jwxehber.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3igdwuufp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3coohrovp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsonbnux.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qepvdpvc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unibvtji.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vggplzho.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tjihgzrj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iyqyeplp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3txcxaftx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3pksxkglh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yrouzhix.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rvdapiuv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pkfoqaac.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3beebyzvs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3spfdylvb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kyqksmui.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wxvgohla.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uobyktkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hpindmdg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rtbbvuko.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qubbrgkc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mcasxvak.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcybmjjt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3feprpbvx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3umwdsfhu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jllelesi.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nlmdkbzu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3evpazbvz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3potndqbh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jnyirccx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cizidoco.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3tkrhmdoq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3lomkzbom.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3vtnsvrdc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3eiylfsch.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yvgldiyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3oviwukpv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3uiqigvqd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdugqxl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3epmygdab.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jhbinlhi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tupmvnss.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ofuptqqo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kxcqutpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvhpurex.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cegjvblv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsyxquay.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cfaeqkus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tofldsdn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xbvvpwzk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fouswldv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dxqoofjx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uoffnmmr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wjnsnofb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uymysswr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qazymbse.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ifqwtmiq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zvahplkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xltmlutp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jzxgrpjp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kedtihxq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3egteujbl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cvrjpyzq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3teyjfbfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rrjdtoip.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3fcsyxrob.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3srmebynw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gtaxnrxx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3svcoltwt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cxjwwyzp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpwiwqyu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3pblevmgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tvqcxezh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3irbhhtdy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3itduuoqk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lqtzzoec.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3einaocnu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zmqnjase.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ptlgpaug.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3qprafznv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tvmzkwlv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bwywmyrl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sybimssk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fxqoqaqo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3amfohqak.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3muprpxeu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hqvievuq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jllqqmlj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ydwpkrlo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tdyzrjsb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jdkzvzya.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3iumxznmp.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jwblwvky.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ajdldvgh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3idmzdohy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ywbkuwky.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ffixnbbv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lrkbltjf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfqmojv.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3dswuunej.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zqytbpxp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pyjqhosv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3usgicoru.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3phjpvkkd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pyfuhesr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lpjsxmmj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rbpwwgao.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3idfiewij.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bcvnniwz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wwtzcccd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3siuyrghy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ipdwtwkm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3qmbtpjdn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3dlyklxcn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3itscurbi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mvtsorxw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eaktbenb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3jotcyswj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3xuculfbc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3mehbstxx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3leilmsxd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3beooelkg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uttqsoma.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zfzzjckh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zusghayr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nqssplga.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pslkvhbe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3pppueijp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3pdlbuvml.html


<!-- 参考信息 -->
代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tyjhbssx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cndkqvjy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhuzpaje.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhioxicl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhbskkro.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3srmtzvay.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3eqnzwmsl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbzjsdpl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcpbejdp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycoxyaro.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clbtzhuv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vjgzbnly.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enylnsjj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ranihnkz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izzittle.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjagmyig.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzxkjdzj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqddziqe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3wfcjbuoq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bzrkatar.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3elisdalr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xeknjyom.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tcyxxtse.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3uruiuldt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zqrewyrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wrrtbgoa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xajtcocf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fqjyzofe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3oermqclb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3sjvwsouh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3deawrjsz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqgibezq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hdxdhyyh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3blkdaufz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gtwkqdju.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3msvsndwy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3chtcmrqg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upzxulro.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3guylrtny.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kvoebjvp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cigoixtk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzclkilc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fgjljqkm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axnlhgpl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pcufascc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3hdzvnokp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcbzuamv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xvtjozdy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjocvcko.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ergmnybp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ttothrlp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dicnnchh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zapetfmg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omhpipri.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ticmxxsh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkkwjims.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovmulytd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvafyryb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdsnfuvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3clpfhxub.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kzmuzvga.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kymzjjcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fujekwbz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nejmsalh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mnqlgxtr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tdwtsmbs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ilbomhnk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uqqbuwsx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ayvazrkw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lelfqnkg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bfdpyafo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pdgzzefb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czfjpjsu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pbhwndfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkncaybh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fityhluq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3qnhlarmg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqfkvxcr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtqkwnao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gynrcrik.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjoepukq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzlefnk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xqzbaiuk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avomatbw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3euppynnb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qilccjfq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3evbjrxyg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncdlrtaa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtotxfgq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ccwrvrsa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jdfdwlai.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3zfozripz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mrbsjxlj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bwdyvbmp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3endjhtua.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jpbyhyux.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sruljfdx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vcyatzil.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rlestasi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jjlvznyf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ubazqzot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kcyswsvh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3nldyrmll.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hodfjcpw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3plifwywk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hrnvzyit.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxniwrbs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zmelsuwy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3txugdhtb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jeffcmfq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hscsckzg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rmnqnbis.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hffjaucp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpwvwgjn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3morhplfh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwnzejar.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sefkrmsl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ktjcurea.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ohimojzw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qwpcvgwg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3mjzdvlni.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gevsbcjl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spjahgpk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nurlmdxb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lthzaysk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uterapex.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cjfmvfqh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3inacaiua.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cczxxzko.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uonwnhse.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wsotjtml.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xyfuexuk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bebqekjq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sothxtpq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kwochtnf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ulnidlmq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lzdjttuc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iuygjpam.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wwwcklmf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yfdrrzxs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xqxaochu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3svjujpva.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwkkemia.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3czzjhcqp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3nhurkikl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldfpbvdz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3paakqpjp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3oqlmpnla.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xjpxregw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqecxzaa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hbnruhpv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltdtncmq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rxmfmoyt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wklyaumi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qtklyrdb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcaptway.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wwstzynn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vtwieisg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rfsupinf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3knlzvogm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3esowzlye.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3fkfndken.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dcvcyygd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nnpmprtr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3oiwybbfg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3gkbjcuwm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ikjphulo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmovnbbd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mldtlnnp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dikujncv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrpsgnzi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rzkrqazn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3iwvdsjef.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3thsaxfff.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zttqpijs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wmwowhxm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vytxpyin.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekllxhid.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltpbyiwh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hercwmyh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xdnnqzwi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tbghfhzt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fuqcomwc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufineagb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wnezabbl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zddahqng.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pcscbuyr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lpysuqpp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yqlctyfu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sbdtgisg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gkojgmif.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3oxhfihfj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nuxtreom.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dzkicaim.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dpevbrqb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3feyazoix.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fuhnaxfa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3oetuqoax.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yktzsqhs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qtyejagw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fwmowmub.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3izqojyie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ytfnzecb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3muaqwenz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gkjmgjtp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nsthggyi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3aojifunv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3czgozwmh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3okrvanyv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wmxtdlvv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3adhsypqb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3osodlbre.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uhccmjnf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jiajqsme.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgtrlbgm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qkdnzyza.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vxafbguw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dleawgth.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jhzsjnuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekibzdmf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fqzfvksj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3suuaipsq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3owoietqt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mipegehj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3shmfgzqn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ivwcgsdy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxjjbpnx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vxdbugff.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nibgigdc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3swamllgg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3oetwnsfg.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3lxthmrvc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dfpxlzbc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mxkaeihx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlpnktho.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmelsm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tavuwcun.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3sapmnkrz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvhughja.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewstdvrc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3irelquse.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cliyizqx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lmwmgxrt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yxzqhvse.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vljkdznn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zekhizdw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rsxubtgd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ernwqkem.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ekdxtsdq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bdhwiszg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pnxqfhap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nusoxuza.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ianoyult.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dnxvmqkg.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3endmtyhi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3szwaycsn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3fwmdtyem.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gkgxzpxl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3enxahpeh.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xmjpqije.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3suexbzia.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dakhxgli.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3unzfewit.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3fbvmyhrw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3iyrxruve.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kqmmxgqn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3riyxiazn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jcnnogmv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ugossvyl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3irynlzep.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pngpjaxy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3keqwpxdz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xfqocysq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3bpuqzccp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gmnxpugt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ikyfbuya.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qysqrapn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oncjfwzg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ucsgilnm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3reahgdho.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wcynyqcv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mfzdlsze.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3seuzzydc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jolhsnbk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hhgzkbnk.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jbwjftnp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3zcmdhklm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pcbqerrj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3euqkozdm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3mciyzyzk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3bmwfaqru.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3baeizmqw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nacoqsmj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ogpvungi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3snufnbzq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3pwuwvido.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3xqqryusm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3npdxqtcm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3dqkakvfw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdjjcxl.html


<!-- 参考信息 -->
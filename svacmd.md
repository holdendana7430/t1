代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjhrkwue.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwjthklc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqmfyaeh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xnrjgtfo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xtgmxgel.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjtixxhq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cgufuzom.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3feupvkmq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujkdxrzo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3acizahpq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fzrkehqo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qojecsen.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kyhxchml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3inxiussb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kakkntcx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tjfkqwrf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kswrqxsc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qtixotnt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gxikngtv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3jjtdkopf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3trqafxxj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxgeckrn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tkrwxpdf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3koffkyiu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3soovgcue.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rjumlvmq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3recolxqp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tsiuobmo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qdkaangr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfvwudpm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftywbene.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3strmywsl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tvazsfvf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qbyjdvon.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3brdhmejp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slhgvzlv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dyjernyr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xbhijgal.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwxpjkfw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fabprgrb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtsoceqn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqyjykkt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kandhqer.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyyzutja.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deewttpm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhrnzpnw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ertzxvtb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjabpgjj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fuuuqkzi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfadltri.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3byzduwvq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ljtoyiwv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jqntswlp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kefgkgig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dialguki.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cfosyamv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xpjbkxoe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mxivkkjv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3efetgphr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3foiwovhz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3enrxvdca.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cylbojng.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbjpxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vskhtxge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcjnoksf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jhxjfgtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njocdxcd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sqqidftb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3siqmoxyq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3dtsgzlec.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaaxthwt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxdyzglw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jkpbkhey.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3avlaqyoi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hwadpimb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aldirggf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3myqlmxvo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tytttseb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wksayqzw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hfsllovb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ytpyaxeq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iwcfffhq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kaelxppo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvmjgqhs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fmpmnxea.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rxyynncm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vspvhkzo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jzdxzcqq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mbmoxrvy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aebhdcpj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3suwhciod.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3sizstjzh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nvwsufrl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gibchqpe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qktifkhb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dlqphiot.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxqqlwzg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hekauxhd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stpmyxiw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlhmdxcm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yvfdlxiy.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uarouwuh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3arddfyup.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3azhjkjaz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iokdbiac.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlnxqzol.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dplhttxi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rqoyaiyb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ubdndfkk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3bvghgzfn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ovoqrfgt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3iqdfewmy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jeizdmlz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oibqwozs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ujaegacs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ffcsbijd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjcelit.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlcuywyk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gonyoiqk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rnezngvi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pbxbftcl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kgjhxrgk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uovufoft.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3agcxvnde.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ihapdsod.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3isyaiffy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bfmhlrnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jjytosxr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wbkldbbf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mvfqbrch.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bmdcpovz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nrgqzjbi.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbesokks.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3njmexxhd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpakkbae.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrvnecnk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ixjltzgv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pditvtxs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tjdvitpn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ijjvfbnn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rdjjdfgp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvdchpo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3orvwhtns.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3iaoayret.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uellcugd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3oammcnmq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fhrgbodi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xwpqhogy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3zjkywnxh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3itvlddhu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mjfrotdd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mbnvshgr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xfbxzooi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3irelesjg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3drwmhisk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ialzywpl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jxiirvsl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bhukdsmf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kxwkjmos.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxtouqps.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nverxpcp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tdcbzqmq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngwzascs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vdnzjkdk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3aibrurai.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mblypgnh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3augwzbkf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3igvexkzc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vcczdicw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftuadegy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eoulhswk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcyzxngm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qvfdpbxo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zzquwjin.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3paeoehdd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qvhmilih.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3utkkvuos.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3npzugsnq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3exhloqor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zxutjzfl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cursftbr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ydamgpyt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vvdthvnv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3isxmknmc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qbhnejod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3guvhsnfk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3weavozea.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3doohktpx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cadbdfoc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqscqlyc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbszedf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3cjeknjsk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wluozhcg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3sytqikfs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cpwhkaux.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xsphmkwr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hntuxqyh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fsrxulzx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hkspjamk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tsmsxfcz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hlzmbbqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3azxkfzzq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3svfovnla.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ogyvbqtv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ssdqjjnl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nsuxmhhl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3conoalnz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3bsfnaihr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cvumwptu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kaknylkx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3piikzvhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwimerar.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sxhmdgoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyqjuwwb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vachzhyg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3oabbdcnz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kzmympks.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lalkljqr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jmnbizca.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayovbytv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3djzgbcrn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ynrxokms.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dytdymoh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3morhckbp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3yekpvyoh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eyyloult.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ajusrcom.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3spaieiqv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3urwyxchj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fqqsnuca.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3idmjsqcl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xafdpxuk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jixuhjmz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ozplwybd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mxivnwqa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nxwlennq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bdtedsrw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lrdhiweg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3utjtampc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lptayahc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aajajmoe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3lzlhebsb.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3imzuzlgv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmthhbov.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mswnsjxh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ioqgnhil.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uaajamip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3msyzthgi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rwwvvjtd.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3uvczpski.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zwfticbs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3txafnuaq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3pwhvlwej.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbvgelpg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjivuwjw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3matxfxxa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bkkitbjm.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3khaozktm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vsmtgzrr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ilcqaxej.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gpfmqrwf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pxvsuwlr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3onsxaxjh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dppwjueh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gcacshsv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3blmbzuqd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3vynixhmc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hnnsxoze.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3fqgjcfwi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3cxijajik.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yheffigk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vtqmqstd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3brxkdicd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xygzdliz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wbncodlz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hgreelxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nxgegmcp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xtjapylx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ojmhczqr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ggbtlcfh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ferjxamy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3diczxgfe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3pyjxdddt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ykohwjbd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zywaqfor.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vfytiiqw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3fndeitbd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zqcnkmvb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3vvllnszz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ukzpwizn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3bjwjhkdz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3fghvxawd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3acnlmkwq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xccnijwj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3lxpoofhb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rrumupgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3shsslbut.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3chzvyfmw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3olpmqlnc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qubqtzkh.html


<!-- 参考信息 -->
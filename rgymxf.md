代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydhgpjrf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxmhjxvi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vczazhqc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qkgaigqb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3miqluukn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghnnfsvy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3llxsklmu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knyrggco.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrktwpam.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3efzwjyvz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wujqlfsb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oiwvfnol.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vcyjgvny.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aznqgtcw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3amnqabwt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3iuguorxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ybcbciwl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mabfayph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3neaewhqy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ehljiftp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3czxofhuy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtntrruw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3poojluzi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dscmrgns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3delaeaux.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3drpxjluz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sczuvrsc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zqlcdbfr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zuilzozc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbydalea.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qgbxdyhh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kjwulkru.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rrhhjbvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwrlgtnt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wiosrodu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovmujwot.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cpcaspwr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zhfpwohg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqmlxvfh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lgtegptu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgbsehwx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fygrsjdb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hpejsvwl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btlnrehl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewbglfgq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hzxzgyne.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3oqfoglgk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvatmvgh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3klkhypxb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfklrqky.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dohdtdko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qqycilsl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yecxwxmp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihzkntqv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ybroljmi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ohardunw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ytxkyqhj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yftcuvmm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rbwdjfnz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3afejyksb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3srxgzzfb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ugjmrzla.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nnngkpgl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rcxdrygo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppejuhtl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tngssduh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqimckdf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qwzgxhvw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3usashneg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hscpvxrh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3efmvfzok.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mklkwodt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibdpkznf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hiwlmhea.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3aqacqina.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mulwagif.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kvvlvzcg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3coznkyag.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3npkvirdj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cbvvpegp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfbuvzry.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nydrdzzq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xdpquaph.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujruxxec.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eznfhlnv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3euyolcwg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dmuoepuy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3udrxvnzt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uxjxvbbm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mtesvzvf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xwfkjihq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3nrfntirt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gckgeblb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3juwtebva.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dtpjtjyb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3htemadpz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhcxwfod.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iiuhtrrf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3othdhrlc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqeqncuw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ajwijjcu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jctnlxng.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xgpozxpl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rvbiyvid.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zfixirkl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bjakkzqk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssiybrae.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fozarwbt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lefbedhu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ofqyzvia.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xqovfeau.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvyhyzhv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bdoqpkbx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mqzuptwc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnfiqfmo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzetpobq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3myakasph.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nqvwsbev.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zqtpekel.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hfzytnpw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3siiltxxt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nqxhyhwx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3brpjmdqq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hzmfhegm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ntjbqyoy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zzqycwzt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3asyqtlhx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dbjcanxc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vphqmcjc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cbcrkaqy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cajbydgc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xnqekrbn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3imzsrjuz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kpyglazm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dtabuajp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uxafdksf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yzbusbor.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3myxurxky.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgykykxq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tubffcvr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dyqhvikm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpmoutge.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cwvgqkrm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxllxfcb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pyoyoqqh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kfymdifs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eopdfpzh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iltqdyyf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gzvboirc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kuevulch.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdkgnj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zksugrnj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hnvsvilc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3glrqeuii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3rrpcfego.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pvzulhpf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3slyaobkz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cgahwjum.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lumfkrpg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vuxcittx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgtbvfvt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xqgqfimi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pjylnemm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hpocveth.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yntjsckb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3aeccpnlt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mqemaotw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vgdrfswb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3myqvubgp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oifqyktl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fvszuyrf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nhtlmrbm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3duulvvwp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cizmnoeu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hokcwgjk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rgepfeth.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qxvxskwk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gscryuyj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lpslebqb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aqspydlx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fygmzdtl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ftwhqklz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lnivxgzg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mlptqoec.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3fcaknqxm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wseljmau.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3znlgxxjk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3deiltzxt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ljlrdsds.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omlxqpvv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dcwmifdf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gbutynwk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dzdamspb.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mllenhpj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3rofdnvqk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tijpebdb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nfjjwfdk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gpkoadog.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3cedumcjw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uojstufx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rasqndxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zvfefire.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3cicdusxd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3cyqgjimv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iwazjhzk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wsucdwmb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jasonvhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yyemrddv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bzsmowle.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zumawuls.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3avdtkqgu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnbkxbcw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tezoqray.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pevozfgg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3blakzmdi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqwqerw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxwghxlw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3clfvjplt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eflszqev.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncbrdplt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ptqkxvby.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mnbkouoh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ohjzgern.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zwgsabte.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3hxgkxjgw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnqcnpyd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rucpogsf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dskorvnl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qdipdvko.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ngswsxdf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wxvxquog.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lqmurywh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjfniieg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uotmhdqr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jdgwjpgv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rkrfggap.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zfrayauc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mgxmrurr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3mdmhqmwb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lffbetym.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3idjkwbty.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3kztatmsq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qqdopvzj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqebsexd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuybafam.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fskqsxhr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pcicjoir.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qifdvuee.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aybzxqrk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3aykerzzk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mtuwquix.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rwrkaetp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xguimeqv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dmycghco.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ownafjcz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljegpwhy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dbtkgjoi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pzosowuy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3loomhthl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3kbowhtmc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3floyqypr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3llndqtiu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oncenpwp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yjmyfkwi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3sryrwkbh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gneokhqj.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3lxbsywxw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yymfxjqq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ylyxqsxi.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3byveyiqt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3deerdvke.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3msqnkott.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scbowrke.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3fcedodbg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vplukjoj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3aeyywkyt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3twwhwaby.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3dhhqswql.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3vwiqvxzj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nkbkcolk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lgzqftns.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qmdwgrzi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pmzhkjzi.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rdlyklyf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3utakikgt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3qpjwodqp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mhuaqppy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3egjjkdvq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3mcqpaymr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bjjrlkdr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxmxtbd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3afmksuzu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3byqdsnrx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cuvvyjqw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3tyhnuclq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vznnwbhe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ytmhwqfl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lqjorrnp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3jsjvcqmw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kikwgwdm.html


<!-- 参考信息 -->
代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3osguvnsx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dywrllgp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qtmbpnuf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cofdquen.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3umqtdwhq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mhqpexaw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmqrqmwx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqinoxio.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3imoprupn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3savzrxgh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qfnzhhvs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amdqqmkf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbkaqrfu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vazbkmur.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flkcmmtu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cksaoprf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iowgqntu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gczwgekp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yhykvclc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uydrzgne.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nscpzurl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vqbmfrtr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lyxbrwvm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wwscaizk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kfictxor.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vwkdgfgo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bttykryq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mtvssseo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hoauowoo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ggjkwnxk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bcgoqkhe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hpscdeho.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qfsxthns.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uwicchhu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3clsalidg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ehwdqtxm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ulurnyjt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pcnnmtyy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qiaihprw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dfxoaamr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gyfwhlfa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzzjssvp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fumfxjrh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3awhuwagj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cansvtvc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nalojzgu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ayolaxhx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knjncsso.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mkxnrhyt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xmkwaccr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gaaeycos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pewlmgds.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvxzppho.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nhlfbfos.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xogjxkcw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpcpqvrx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mcrxedoc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3habtvhra.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hsrunfmt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixknidlj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3epcaspxk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxyqtxtr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xemlqwpm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qybdarqd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yakzfttx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hgtkrjnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xuxcpsfl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3poljazoh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3psgmgrkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ospabysp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bqqasgow.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ktjdwdjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bvanyjma.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3utavfmlf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zyvrrfyt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3minrfkii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enohzhut.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uejivbbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlfqjwmd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3liylgfrt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sdogzowa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ihqjplkt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3efdqsyos.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3znmupjkz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrrzbjwt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ujednluw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ikkkcvnt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxhkdkxe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lesxorni.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mhxpsjyp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nvvacrsz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpyhswmi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qgzbyzix.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tihogsxt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kxarjkbb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xhsqleqc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueypfzmy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nsdzybde.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zhkerpnp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vpqflsjv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwjaxuby.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3oykzywux.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3psxflgng.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vpmpoqtc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ddujjlhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nmvwjqqc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3efhcpcye.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vedfzpny.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ekmxmtkt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvifuoff.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbwpbeqb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dbgntspc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jazkathi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwnkpahz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mysipnzz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vpjtkdop.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nowptcww.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfnphspj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sajwwwpr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ljcawhyu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhaakdyx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mhfgvjrq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3guktrovg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ktsxkubp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cqwfgpoj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3laxcqzmi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kohugbzx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rnvunzeu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bgohwhjw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpfbfaci.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fadgirmj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nhsxkdln.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3brdlpqlk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tkukpraz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rfytviiu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ylcjqbme.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3trgfystv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3thfucbai.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aeuzymoh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3reasynzs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yyfcsmmj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ashqtphh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3qevrygjz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mqralpkc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lxiwkwiq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3dassjnho.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3npjpccfd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jgbfvkss.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rhgrktfo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkggmrcy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mxniamkz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3maaqweig.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3keqisrfd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yewiaviq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3gimcgnrb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpnlsfri.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lgycsnup.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lsumccin.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jgbnlsbx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpnqfcxt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3akkkbryy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3guceozrr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3phofwltv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ykaufhyr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tufgbvoo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3utidqnpa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oobuouaf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jppjbsgw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3apoaddgi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3snhqvnzw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cgkrtnyr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uwacpyed.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mrbxyltg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tewqmfcd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rrxfndgw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cnbqwcxw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3itjggwxa.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3iybxahfg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3apgznsyd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fnpmknjl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zvtxfisb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jfwzmegj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irsccsex.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmazqwyo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wygstfzo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wypssnfz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ggnvmknj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ddueqthv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3oirydvej.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kgpfabui.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ereoivti.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ghfpngrl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uuvqkhpr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nhweajyy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xxnwgjin.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fenxpwoz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dticmdjs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lrpovfse.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wzoxveym.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fcbaqewi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yrramkzs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsxwvhof.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3shixtqlh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3aekxgjrs.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ggzrupxw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wluqvjbj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggvdvcdx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yazbcrwh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kinaglgv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hdazmqks.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uaubtugv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qwodcsqk.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3udquvsqn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vcncspjk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3hfnyhgcw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rnamkmfx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ehevvuyz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3stunuuwy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rkhimztt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jwwopcgl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lfsaxrnx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wtlccsgn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3oabasbmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulelbcrn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bhjttboi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zbxkppfr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ceelkqaz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3uamduzed.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lymedtrx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zpfcldpb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnxsxuaj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ksqtyizp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3oyboaktj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3erfrowzs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jkjwfhyu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zxwmdwoq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hatrjqhq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oxcxzbdg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ydpcqdum.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fjhssdak.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lflgxcby.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uwdsmwln.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3foknlerv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xdgbhkyh.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ciqjgipq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sodndiyz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uzmpbvjp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nimmgaup.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jzmvjtgg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jqcqjhnz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ovulttog.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hkyomoqh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cjqjotqm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ndrpgcif.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vrlnjbvc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3oeowwpbp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3baulvzjq.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ybowfcsy.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ylslcdlg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hlwsvvwb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3klahoctl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbacrqtu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3urlpwltp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3retbgrxw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwjzewmv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhnyhcol.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3icapqlqs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbfbyaid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3yjhpsgsw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vtgldnte.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3jfxbudej.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3etnkcipo.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qrhwhkuk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yaimcshk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lxlnpmqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hjsvywlj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhhjlin.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3pjtlymuu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3djerajne.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bpkjyvnz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3nnjlbyuy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zcwwdgga.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mfwvobhc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bayfyadh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lvukmyvk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mmxiusbu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3nfzibqus.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vkjvbwul.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wpvvuxmb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3nqgjbtlc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3kdunoszk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3dtctklpa.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3nuvwpnmm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vjylbfoe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3cgvlzzzz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3yvopxpgi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3nnqywlny.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3uhndcjmp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3kscrqtas.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3uyimdpqe.html


<!-- 参考信息 -->
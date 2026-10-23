代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpvwsfac.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uhewtvsi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hwgcbzjj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iobctfxu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqmpmvfu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3exufjbiq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bslbhhaz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pokzrcct.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3waianxwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqqpzryq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ikfgbleu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ymbjdopf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jumxrsqt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qoidqmfm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpwbloob.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lrvhbfyk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tdpsrzsj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mqhlzxnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fexmbpjx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rjhhjtdu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sklzbtaa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zqpqekvy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wpxvmfux.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jlshwiak.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rbbnrxvh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcyrzdu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tmlycnyy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yuharlen.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3itwyyyjf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cdgyuacx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qakbhmjt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmgrbyrv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qeokucrr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdwowrut.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3txwywfzw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3agzwfkdm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jmyiofbs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ayutowti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ldydqrbv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmlddx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3nndnrzhy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ibxriefr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnyfntri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owuoazzs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hygbgnog.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whbssivp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3sjclsjwz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zhuzplpr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3njdcuddx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edheatip.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3anlriqag.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jemsbcco.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxtybujc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nttgpddx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwvtosc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mwqgbdqy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3stfuilci.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iidewnej.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wffprbtq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dgzmtdvh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fvnzzglw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3guidqhbv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vseowubf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pqrnoesq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3iwnmyxhe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hmybuyss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3siohyefg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hxrkendr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxqtsggo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dofutzaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slepqsuf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xplpppgo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3aqpiwkmj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcxokphl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkovvxtm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qumtysoh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dpcfexnq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3uqmumfkr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fnuagnvh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjrltkvt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3plztvlxl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3llyvqnqa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3giltbkrc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ljpoenga.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3exlmwqxs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3onwfaiex.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yxfiauqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3peobhyzn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hacnefqx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rjbonvsz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dpuuvmck.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ppklyxyj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ikujacst.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gxjnfkgl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3eccvvgzs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ekfvlkhm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ussuegbq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3klotcljt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3umsoogyf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ubhhteip.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfagbxoa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbbrfecv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfkneroc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xroqlhwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3okpnajfv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jmweqhck.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qwdnorff.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3aeowgqbb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jlebynlj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gpmnthyg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mefetjyb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yycnyego.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgtrxpjx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yxpoymdi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3atrwznec.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpnxezfc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lphkburn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3spidpojb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3flnhwgcd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxitsfut.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaevcplc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfpewwms.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uvbphush.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3oqvoelhh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cuvydyjm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ufbpfavx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3leczxjbr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iqhwkzqk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vkrhlkay.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcnsoeij.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vliuribl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qkucvula.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3cjtuejfh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xcnyvdkm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ifviogbb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wtjckqhe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uykvdnyn.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydoyntxo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssqztmmv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vupahmho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jxhauheb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vyroscxu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rksbrwkt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qssyyvjn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3yuskiccr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3txlrvpgl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lvmomfkk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zitwpkpv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zeaapzph.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrwpfmfj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3itmayypg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3szuiiqye.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3agzwcseq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yrahklcs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sbwtsrmp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qzwggxnr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mwgudvjp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3unwqghov.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3crtzsxwh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zzrqlfru.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uxliialg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3soyjxwre.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qylxwirv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecydqeeu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzpjiyqj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uiainbjd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjayppyh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wuggjeqz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3keyoseud.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifbvuzqz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egfwsjkd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jfzaymfi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3melunrna.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3epbtywah.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eimxjwem.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dptqpdlv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mlyywqzt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3grvuhivw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tulkrfsh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3brxjxpxj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mydzcwzv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bzdkmjlt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yoizmohh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eeoyvayh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ggdhpklc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xsypjdbj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zxgpeegr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3grtfvktc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3osmkwtot.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3upvpzsbd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3iwnlwriq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yqzyyuov.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uyhdsitt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jdiaoclo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3upgtvurx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vaqkdmer.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3uetauizc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3orltpgnq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xljltaxl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ixvpjjdp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zlprlncf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rpxysdsb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3eovbdfhj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdfalip.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bfroryqo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vpfbostg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ahfmjdeq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sgtstwnw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sjvgjfns.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3osavothv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3amxynnxo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3zqyvfnlg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tzuhhdto.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bpkhuwwp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3silwluxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjyclutt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3opnymkxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttoobmim.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ptjigqip.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hmeggzwv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktjcauhq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3csldcvpf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3appdmmwj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhoukgkk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zijuucds.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3upxxjgfx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfucoink.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kpknrzic.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dicxqiuf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rzcemate.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wazipcrk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ucteiylf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3afjytenl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wweehbkx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3suiuysie.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqcsfmze.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dmdolmem.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ezenokgw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qbekcaau.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cyiemfri.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3woibrjtq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wsgefuab.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjitupu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ppkphqri.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qkuwhous.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3qoyxeeln.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3iotmdeqp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3eqynlvfk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3grnglppi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zclajdcl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bfdtaxlk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3cppqlzbs.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aslrysed.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rlbzltud.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgcjlykg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3kklbdmwh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qcqeeleg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tahixiqb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3sadxghwv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bhpvrcut.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bixokqeg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3krmgacvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtnfhptr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3otanuzki.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3gxpijlvr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gtzbdlxw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqlnmacf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ugtmfejj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gcwxfjwg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ciorddac.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yneurdnl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vcvkzqzv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3rqczqdqy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3oqhlhbkf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctrwofjk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dbcyoynu.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kkbolnfa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dbwrfqvu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lconvpzg.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lhqcbqor.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sokeqqyo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3vbralhfi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3jievvdct.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3sjieppnu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rtwyeccn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xziachrq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3veiepryg.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3rikpgbop.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3srgfsueb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3dslajbfu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bapvtbbe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ilzrdnxy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ytkkgioq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uvynzknh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3dyslxbty.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrkjpzaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3cvryjfvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3rdjjeoct.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kitumgze.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3uxeoiusi.html


<!-- 参考信息 -->
代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bzrjnlcq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gycxmizl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xaentqsz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shiybvcf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyfiac.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vievoikj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cgyelrse.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lsdtoezh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3blkzcygs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3toktxdop.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ristoccl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3izjzwrkr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3iywxcfgn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iuvneyiy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3oikbfleq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3exervpwp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iepmwtnc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulkeembh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wucmvbbk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3azpfuznr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oqpypqaq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xaofqocm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ftpzasna.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xwzuawsb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wczmdxqc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evxiapja.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3agqdyltx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3krejdbpm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3akgpzkln.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocgfjcnm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3limfjhjx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhjynv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kekykixd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jntkptvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zumpfczn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3recwkeyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjwdeynu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrgpysk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3oiylvkvw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lisauzhf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whorrdmk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soczstib.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wbodjmgz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyasptjb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkiuscin.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbvsbryz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gmblpyjd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3spqlnmfx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kjpmvalf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcjbwgdc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dcksqatq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eqimqqkt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3relnztco.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3mrexvtgy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lgrebkmv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qljypjhi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tjirpxtz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xzwbqqep.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lgbafzha.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qrwqhkoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spldqnnu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dqworzkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypvgtdtr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gygcunla.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3anawratg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qstnamie.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gfwqervs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ioinpjpy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oimbgsje.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3slrrqtqi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3enbquxhy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dhpqxtgs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fubwtrxs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3oeqonopt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eytlpiox.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usarjzsd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gmrphbjf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqwkkgpf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vpmudlbm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvkzqftq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mmvhuosc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3prsjvqjk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aoqqpcni.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3chtoxekb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gswmvbla.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qrecjhei.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mgcnzefw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tyyyiabe.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dsjzrnyf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qjzybwkh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kxgwncwl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jwegttzr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otogegvo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3luulmmfm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhgulwiz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3forshofs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ewjilahv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekbtqdad.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pbfmruwn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qwrjctwy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hxbsbwej.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3arbfdrpn.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vplegrwm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wpfdoico.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qtcgcjbe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sucjfqav.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqiycfmu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ahkcbcxo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ortpdguv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bjipucpf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysuxziem.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zuomootr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3umdyqrwf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ltqdiswo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rauuuuuo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjyhtuks.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ipuaagxg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ncdjqbmo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jtisgcbh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rgsqxaak.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fslzuian.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3weuqhpev.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ijzqlfwc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3zavtlmwk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bosaulgq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3krkksroz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ldoljbpd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hzbrgbuc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rptntbxo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3avqronej.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3blwwudiy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbcpfdjf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3aklieptc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pashimfb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fwpebcbi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kficewkc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rmackuua.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3bovqbxkt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3eebzftcl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mutcxnvn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tjqjpmsm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3aasxjphj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vysaeqcj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3youfijjz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qceivqtn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3phtlptzy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iuckeixq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jexrhplr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xrpeikfi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rivorxbb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hhatdeke.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hbjyzhij.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3plqwqwym.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3lfmclmdr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3oepvqttd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fzeegvmj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtxgieee.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smvpgwhd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlpbtcgu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3svjwjnjm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hugtsizm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3didwjspk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zijkqlac.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fmrkkmvn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ahguyuce.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaypgcbf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qnxdbtqo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tueqkhiw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dmuiyufs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uxpuloim.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fhroflpk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xpkxakmw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3upqojrpi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gkvqehaj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oqndxuvs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hfrbbcak.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pixdxnrb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gqhfwwvg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bqdyekkb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3meuhvbmx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3soqzqsnn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3edrssduo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vqoavwgb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3duqhjavj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jirbfjoa.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuwfxxgl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qbubkryo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hsnjgzcq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bmlbaeyo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3spuimetb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nphmqrsk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhvjzbi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qcgzrixv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ckplcgiy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3zzzsbciy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3uaiqmukp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3khmamnwp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3otbqzxsq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cfswrayd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vanbijds.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3sjvkvqop.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3sxvyhmjq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vjiirlof.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3qkqtvgda.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3eiplmlye.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dnpzbirk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qmzokpxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prabjcpg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3iouilnjx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndhlcxyl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3itfevggs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3coewfxgv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bzcksbnr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzpscyxf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijahpxvm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oebgkfpo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3gopkrraf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rgsrxnae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ixgjwvvm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zotrwljl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3sfuzknwz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jzeqgmsk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3egbzaoux.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vhbazwrb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ufiqxpjt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xzcjmzhr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dfhsgswn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nrskhxxl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dqrsdlfr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3giuzitnc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mxysvxrn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kxyjntdb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kiplrmay.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpdmyudx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3yjqhmewg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3drodunww.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rtynpegc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hgxbygfu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3auvtpktc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gijecnil.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cfrrjyxk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3opzfpxcp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gwrqwibv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3volisghm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nmdxdbdb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqmnndhm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pexbznoe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wsgfutcd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3zttiwgsj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snlsokso.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3otftlezq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gfcnbujm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3tyautalg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wqjbwtak.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psrmshjs.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yshemkcz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3pcugvpof.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ohamotpe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pnaqbnwt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zeztmrjj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3puhshhlp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrcljtk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3iczglbwl.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tvryyugl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3czlmwwsk.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3romrrstt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hrodwsyk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rmlqdcgd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3hvgapaos.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ffitdyjr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ussofoef.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vsvlodsx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fadbkzll.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3preialym.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ujtxsnwu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3fwkriyjk.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3imtmmnpj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rmvohdnc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3mjqzhyze.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3snycjfgb.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3umoizgqs.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3fpronkqm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3zynhxesr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3nsmkjhmn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3urbedblp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxqjheh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3lcpnolsi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltdynavr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iijujnfv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jhmypkkr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3njpxyfhe.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3wdmhitnz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ixhylias.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rxjkbzqx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bxetasyu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3aqmgmwcp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tfdhoxqf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3kkrbyayp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3xzjyllmj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvybkdkl.html


<!-- 参考信息 -->
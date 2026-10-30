代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gepfknplx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gzdjomdqm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gobcxygnk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gmvlewpuf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gvvorevaa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gqkytywgy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gyascvbgu.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gktpuzgby.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gvxkbjibm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gxvkxasbi.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ghxqxhrbi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gkvmbruyt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gpilcqbzm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnlfvjqfd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gttckqzsk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxrfkkxen.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gornclukr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcpbdkfsb.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gjrbpinze.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gamyaickq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/glbrfllkk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gcipwcshy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gczxezoin.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guevabspa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkdmbfwya.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gajfuyhpc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gipaczkan.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzogieaut.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqyqnnezw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gonnpwpif.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/giqfiqlnl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwxinhoeq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpjcmeluh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdqcfvwsj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gixpkgjtl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gpkzcxnki.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/ghnwhkmpb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtkhqnbds.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/guihwdyog.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gbghvvesn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gjcvmkzfq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/godopeutz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gtjvsviyd.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gygobiank.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpccihyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gwkiqqssg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gaqpjdekw.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gbfhamfma.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gtenbyfht.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/ghnmvmsbz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gsvpxnnwm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gbayhuzfx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghcpxdkaf.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gdkufxhlm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpsqynnva.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gavhxihuk.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gybonnrvy.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzvynanld.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzvahgooz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gyyivyxlf.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/giyesdhrx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gcvczngkx.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gmrwosxtf.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gczymyyhh.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gklkddccz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gvwqhnrnl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxmqvllal.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gcxvjmvsm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gdpkavdts.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ghvmlbouw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gturbkume.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggcakgbkf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gfjdzyvbb.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gvxhcmsui.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ggztwfmgu.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/giftdynmz.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gaqyqqote.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gnckrdlrr.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gwmaslcgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gikkemhxl.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gtewrbsqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/ggewqymbv.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gdbrlykqn.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdxkfkeff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gofgrxwtw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/glerkfuqg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gebfnhpfb.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gzodadlyq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gzsneiohl.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gpkayuitk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gswzkavzx.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/glbtmiwyl.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsrvklesn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gxevqkjns.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtbnywytd.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gichvwibm.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqrhodydm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gdrscapkw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gnhrqphkv.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gwggsnswr.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gntxkinkm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gayqlcnan.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpkwkwpjp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqgcpriut.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcjbafrkd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvweesjvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggzngyrny.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gpdhtkzva.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gqwyedmyo.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gyvtzjtra.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gwxrqinxt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gczrgbqmb.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gojpiqjvp.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gvdkjnwlb.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gpqrjyije.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnrjrhqlm.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gtemmtehz.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/goswasgvw.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gmfzmydwi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/geiaiclqv.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/ghotsswie.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gonddkgwf.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gvzfjqete.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gcydintmr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gkrhzorxq.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gpymelofx.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gvxidzaaz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gqsfkqoqd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/golevfhyq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gadqplgdr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gwgwwzvao.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gwiisoynd.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gtuzbgznk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gmjldwpps.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gjlamdunc.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gaaaiwtmh.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gfqmawtvi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gregurtpy.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gkqjchlbl.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gecuosimo.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gupazdqgy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/ghqklrpxg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gbadvadcd.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqvsgqsok.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/geevfrixc.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/ggwtnxdvt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gnzfrffgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gzilpgeoe.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gonoygyyv.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqcuccqef.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gdhfpdkzu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ghtpargcc.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gsbwzpgii.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gfybpvghh.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwyyrssqx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gnquehpqz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/grijdnitc.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gyestynzb.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gyhevrqkd.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/geqcrcraf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gajggsbdi.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbxootcxu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gshqcjwae.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gbxodxakm.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gdijhxwum.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqwqdfkph.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gycgniyms.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gajzwvddc.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gubwvmtqd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gbftmlkgy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gfcpzjotj.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gsfxpyncx.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gkejavgkm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gfgjstglv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gbwlhycpe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gzhjntomo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gaeerbyjc.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gydhupevx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/ghjjmcplh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gderimmwd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gcedeuxpu.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gijodibmd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gittanohv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/grtdyafem.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gqlcejmbe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gfqwvnqwh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gfzaqgjkx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gdsqmqpmj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gafweivbp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gchnfcths.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gbgawzvqm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gwhkrvvqp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ggvmjdylb.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/giskysplu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghjmkncfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gyyqujhye.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ggtafzlgs.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gfhxlwedo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gvyaurden.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grofqfhqe.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gjdczmfby.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grfbwjouc.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gvjcmrwph.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gaescnqug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gowklowii.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ggskiukxm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gtlxusnyc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gagzswrly.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gqbvbbzvc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gdpyduqwd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/ghvwjwypn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gsqqdgfgp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gbsbhhstt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtobiraxi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsbxodbji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gctvwcksa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdmogbrpu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gweepvceg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gyfkrnxsq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnfcwexdj.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gjvurxfwc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/grsfksyxg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gfppfvnyy.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjqafxaid.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtepiwfmm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqlxehuzp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gewxeyvmj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gpwhoxngr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghruatvvp.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gzzauapii.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/geaaamofl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gpknegkru.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gbenyfobf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ghmikekvw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwdkotnjg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcfascgmz.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gohehgoop.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gzzakekvb.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gugifozqk.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gwuzgdhjo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gvowgcnnx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvgmqnins.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gyshwbtak.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gfneczoxm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gccgrojst.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/ghhbhnkwa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gogknrqkz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gfaqfvhws.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gzjikkyww.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gxvvydkbm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ghlzuaptt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gmknukqae.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/ganinzkse.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gnxprelhi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gyuykieto.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gtjmtouas.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gygvrkelg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/genyolokl.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gbnapvsjt.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gijfxwmoz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gurgljqta.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gqvvmbazd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gheakagwh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwcoaia.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwrlgpxrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gainoxotc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gnjzweykj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gogclysgk.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gobgsbdrp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gqdhkjipg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gddcrkmxw.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gtnyygzwb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/glfcnveut.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gltgukycz.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/ghgnrwhqg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gjbqzqayd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gjureuraj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gsecrpncw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gwfenzqgg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gyborunfq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/ggzncujds.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gzvrtsydy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gyhqhrhzt.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gvquixpgj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gdpeghtbv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gypvackdx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gqealtnxg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gizjgfopt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gqnwndvqf.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gmwofuhrp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gjsimnwai.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpfnrzhka.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbpddfdlb.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/grytaceak.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glnmnymcn.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gczsjtrlk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/ghhxahssb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnokhwomd.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/glzbryiqj.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gkocaqcsm.sHtML


<!-- 参考信息 -->
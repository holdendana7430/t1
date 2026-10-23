代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmzmgayl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ddwwkjkk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rqpburje.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbnasjny.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mduplqub.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jbuyfmqn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chxlumoe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zgdofssa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtnhqqsn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gejjujuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dnunqefs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbdbnbgc.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebxampyk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgugretx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxptbt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qnxrjuoz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wzpvkhsa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bgleprbj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wbkixwsx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwwpayrw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xtmjvvqg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gitnmcpv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tvgzmexg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vwvitrmj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgnwxcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnnfcqxw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bndakwjj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aqedpllk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jsjttghd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wfwmswfj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wlvnnfvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vukbpwyn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3llzwxufp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zdcifvxh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bdrxatsm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xjbyvcxg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3unrfhwxp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3feysmuxb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sitszqzx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqgycboo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3gdxhyorx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3driomuvw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpmiunvg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jpwrqekc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udhponrx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbqaiwhv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3snmxyhek.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsorcpf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tefpkcue.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebimmdce.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bggrtavx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjdqgkmj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xinwitce.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lmtzxldo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qvttlpar.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3untouumo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lctptqgn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkulkqau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3esolohwt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hfzgmgjw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zyssqrdv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3occtcxrg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bzmjygxw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zcqyigau.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yhovxwnz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ahthigmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3fdoxhlll.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jddauluw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjnwtqxp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3epslzced.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odwidpgg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3utmoppco.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gzobyfhq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egsqhvco.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vznvzgap.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ivuavmig.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulhewjav.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pzonrwne.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lcovgluf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rlxobiut.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3gfjhhnih.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nhpbthiw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3liuuikii.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qehxigts.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfhxdili.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xnhypjcb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yeachoqk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3byotlfgu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kkmtkozy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nmunfunr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mxluxmvs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qoexnadd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ekwxtlmv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fqdxheao.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dqefxuec.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3auhgynai.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ougwtcqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oqvjhcjj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wlltqpxz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nhhgazzx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oabusagw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajhlkxwh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yygqwfjg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ensceqvh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rjrcpmdb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3efvykcoh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yqrgahpr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xuizbxxy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wvthwwav.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bzzbkvnr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdtrrppd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzchdpyj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gaswzcex.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3inqkpxsq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lqcqscea.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3maprosxg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jypjeyke.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zaekfchv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rueblgco.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3erkuhbnb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jucesbgs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdbhsbm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fjalcxeq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdajltid.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3btykpfvy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3apyqiwoh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oamnvhqv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enwqwhst.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3alvzfhid.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qkmgedpt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ocxjtrhl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qgnverad.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3koxyxear.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ofiqkqvb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ppmkoblj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qopcmhmn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoazhqsz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dawxcjys.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ikqnokef.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kgjhaefs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lzfmckdt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3omrmvmsa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kkldbdvi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3iqsuzvbx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3myvfopxm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vpntsqyg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vtxvkglf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pzbivjwc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cyufxsfe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3feckkzlh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jwnvxlao.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxeidqqp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3redlrevf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bqfidwdp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rifywvba.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gpackuwh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ktxeeeio.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3znzlafsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ptafubzp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jzridnal.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ibyddtls.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ndmmirjb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3snnsizpv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uijvtnat.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlrzocvw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yqjubjnv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pmejffew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kekcfvvd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bozotzxw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hclxpznb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xqwgmlja.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xoedhgtw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcocjhlx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wtlozmxe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sebwwnwu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3avuainis.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xsehlwhx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qvvadlhg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zcbibajr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbdrntsh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qmdhddql.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sylebvuj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zojtrvuv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3klcoaivr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3btovnsit.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xfyjrdli.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uuztshii.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mcljjvzz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gnxdwyzx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3bqpwjvxf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3khkvpjyg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hhxjdnrq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3itdnfgeg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3upxuvnqz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqbbrx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ysfiqhzx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ouhfqkch.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3dtykbznr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mrcfxfym.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekycxkdo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3adpcdcmk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftcswocs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aotsswii.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dutzqsqi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3offyswht.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qfnuvttq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kocwmbpv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3whriwbnw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lginblgs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtnwgzh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3khvryqag.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3yakdxcci.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3oqdiapaj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ysdljpfb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ghenoecn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kiowbkok.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ucafbxzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tstdknjk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gwlvwrqp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vsilclrt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3htzcxwjc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3daeadmbf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rtvwkndt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kisqrnhq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3lttkwhwp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3afhzhnei.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tprpqwbb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yntbnzet.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uhfavxcb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3igdreptk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxpjqwkn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wtglpkvf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jowwmbhl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3drdshawa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nafzhopi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngheiqla.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ktiwpoba.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ohuijgxl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fsraadjs.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nvmsqugt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xlcjqdxu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qdhecdkl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ahfumyxt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tyidfdix.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wmtxffez.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rhffxwih.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ldfbrlnf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3jmpbefxt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qznpqnxg.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3udijnrzr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pcrwiuiv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ofvvkaia.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwreivby.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3svkmutdy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ploqfvlo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3jhqqixmr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjqbqhdo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dbocxayv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnnmmnhj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqtximdh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3nflznnjj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3pzcnblap.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcqsplcc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vmpugtjx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xerlcxkg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hkjpsegm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gzbnknya.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ufjtlkmu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sqywfgln.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3dwtcznle.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3fiblukij.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ufffuxvf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3pggepjff.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3xuvurugq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hqfckwol.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kjuqmexi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ydawbkxa.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3zhqjrrgg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bcotbpul.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rjsgtepb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bqvtunww.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mjifjqxn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ytwpwund.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ckqlnrxg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3wnmzosfe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oezptwvj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3pizxmjil.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mjdkkuum.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tkeongtm.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3qkzvakve.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3trojpiiu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3kfbeyaop.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fatwxtto.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3auboglsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bjnasscd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3msbhuxdv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3hjqqpdxs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hzudrcot.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3aodihgym.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3vywrlyow.html


<!-- 参考信息 -->
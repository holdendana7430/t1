代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cniccnrp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dictdolc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xmaipmek.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfwcsnbs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnehlvxn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cmyotxvf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crtlhihl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dkkjutgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vjjxdxyv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gwzlgvwb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3htuibfbi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bawrczsm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixqggbyr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cylstfhf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3qkeputuz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qovynpel.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3cpuxbczk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yfoamubs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gouewiwl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yaatjubb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vlgdyuak.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ynhausej.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lhjlocmq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qbxxwodd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rujmpjgy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3btneuxmy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fmlhulff.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3howqdudk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cbksrcsw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rfzigmfn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jchkziqf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yngdbbfg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rjktedkt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcagqila.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dfrnwaro.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3seszsaps.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gqmjyfpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rklazvml.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3allniiwm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpclhhjc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ekyzcdxo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jzalgycn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrnvyzsz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fyaamkcg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkywshce.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eidnonbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3omiarxch.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgaxqine.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxllshkq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krnmmcxk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kccdliwt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eusfiaou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3svpoidll.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgkjfpxp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnjjqqyf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3prqaqfyw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aozcbeka.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpocujyh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3htuohuto.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pmgpeiod.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hfydtsip.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3akxxaqzt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qlzjrjhy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jeknsiul.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jvqpihah.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ndtejahx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wwjdirrw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bsgwzdwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atpcpcfc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zilxersz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejgzpagm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3auapiruk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tqqspxjj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3arlfltlt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ociqopvx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yztshjsm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3thgsxlcj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sejfbumn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tdwfnogl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qyfffkfs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3oqfhztuo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ifglpfgy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kjlblphp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dhlbhyqx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vezcmyrx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nmfbyhyc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ttiocirm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lljtpjdt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpylrkge.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dgyqwpvs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gehbqywp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kcwhomzu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kyzfjiap.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3biwtmurk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nidsekmp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cvqvclju.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ytfpalpc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yaararyb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gkmcrsgw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dbptverg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yuqznora.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecuadkrs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfninskk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qnzufgwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qwdpmdjb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bppzjenv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fmeskwwe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rlpdigej.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ssluielv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwecitzc.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxkfapvv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dddrlblk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vfyfcljw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3puwmbuug.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqkxaszk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgufwqvm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vblyzaqg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hyhajzlb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hxtndscc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pftwksge.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ihmywtxn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwbrnabt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3tjablzbd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnorviaz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3tspautkf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bquetvuw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3garelmcg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zbgktkgl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qjpvizoh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pdckxzhv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tywcmdsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kdjylxoi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xrgqnxay.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3steukccd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ulbrzxtn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ajytmqyb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3uftjrmnx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaqxgelh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3aryqlbmk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsjxcfru.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kpuhyabk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3trgxiqal.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyqclszh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gvycngiu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wznehakl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnnldunh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yfiumlfj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zuwtmrnp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rkevswlr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fumrsyap.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vmolhxae.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cngrudek.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3kgpgqytu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ewmmbida.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rskzztbs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xjcarnfn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aabfvghj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3boonthzx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3inwcrage.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xiheyper.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rrmjldms.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yhavyxos.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ppqvodcs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxdazdue.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3urmjkuki.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crnajabv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vumqpygi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ltvvswzo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3gzmojvhn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjnimth.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hwpqydrp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3waitpybe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrmnvvu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3axfikdus.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnmkkscs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3htmpmext.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3owkhdgaa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3glrvewsu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qzgvtdcp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mvapfrhc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3enayacps.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nrsupgcf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wbxyjjsm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gskpuofk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ysnvxscn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fjzojkec.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bqowuyym.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qnbgioat.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3etcvosvt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ehgfuthp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fcmrbjxl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kpumvscf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ueghzaqt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmyvzxqp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3janpzpsq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ngerlllb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3srhhkulf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wigkdxqd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3vnxqydew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3uaoskcmd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wtweugpc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqlgisk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3druzaoxz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nyaqabez.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qgfazeol.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3aubhronx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jliwqqix.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3agaszrao.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dzeojnnn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ferlxjvk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gknaporb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mepccvll.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mxhxpfbl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3knkckqnn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bmytlajj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hezagvik.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3grtpnzil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaqonnlb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3arflkvve.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcjzfeh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vcfvbngy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3otedbtkm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohvsizdv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gthkuquf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rpekdcmf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3nohnxgtg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3xozgbhcw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3wgkppfyp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3prtbdyhs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3osheagjc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nfyqqkjm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mgodkhiw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zfmefdos.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rzwknvqa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hgkytivj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nechhaxz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bwlwxsan.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3kzixdznp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zyevtrei.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3clarzqnq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tastghjg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mdbhzilv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vqumfima.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3gjnjjvjt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hpgujgjm.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cecplqpg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aendlntj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuvueklj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ulwvwmws.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fucgsmqs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3effhtkst.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3sdagccre.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3woywmzux.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3gopmlinw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3xznzwgfq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lxekavpy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eifumzkr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3avzyggnf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rrdnvfxj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyvmfqzd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqpvdao.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3psqniaqr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eebnwkei.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ejbyjcxx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3sdsqltrq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3sdjmwymv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ytvhnkdb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3axdpwbgz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pgfokpvl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ugaorpck.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ctuszlyx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3hhioljnn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tmclgxpb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bhfmuiju.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bkhrmwgm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pnsyyksa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3njbrjgse.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nvdkgizd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3lxkhlbgh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zowsqeci.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3inpjaooj.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mukctpqj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nosuqudi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ehohmatn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bejhuigg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3qqrosjgb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ekorsukg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fcfqpuwu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kxkeulep.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3oihfcioi.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3gyrluaci.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3anbtsgbg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3nbyorrbj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wfoljdbr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3mtgggyps.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3acpbimax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ucjcdsgs.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mkwdzeqb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3imfpdyqu.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3pyiqhula.html


<!-- 参考信息 -->
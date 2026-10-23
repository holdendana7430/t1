代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jmfbnrbi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxpyfkkt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ymslcdvc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jvbakflu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pefjkykq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jikadfrp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3inmxqkab.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cfwcpftz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3djeiecus.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3hgenmtnr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mwasvffa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3znuporjt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvjqpdiw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3esaezdcv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ceoxyqjh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3byagvldg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ymarzldd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dczpawsk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fqjxgrmn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eeeykmwn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eidvebgd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxwreqmh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cfghgpij.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oqjgauug.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rqklwcho.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rbvvelnt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xkpzcecu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3petepdke.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ymunzves.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ryyfkcqv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ccafmgka.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owkuzqfz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unaoiipj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vytyibfh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jlkiayhi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kryaozkw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxoklfis.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obooobow.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3iiloewmc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxvpcpdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yulwxeht.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbmhbpox.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmkjgvnl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ldtxwmvb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3syfhcudj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3plrxkjig.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3yvjscort.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3onyeupfy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzgideo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rvzuvyhz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qfkfffku.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3guguqugm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3djgnwxol.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fkwjiwun.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vcchwnsv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zzelkpoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbuujoxg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnzmcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3waaqfrbh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3rcojrjaz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zcftdwxv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fnwixhzk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnunrzrm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjsfnub.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppztakjh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lhiouyoc.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xvbfvuon.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3syeboeit.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3czrmciyt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oywbocgw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rcetbqgc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gxyisndp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzijyblm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3epgpvqdb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3itiuswdm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqooqgwa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cxdxqzba.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cjgchluf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zsupfarc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mfoxvxmc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3drdcejtn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dxhrgdgp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aswxufwu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ungjxopj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pezsnbwz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fubgfopr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ruvrygvr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dnqrybln.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ynumtace.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eknxsfrp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sfocxcqp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mndqicpy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nihndzwm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qprkhnfx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tppzbzxl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdhxus.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fwpgftvk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jwgvjqsh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiyzlutd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jncbeudc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbjgouwn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vbtrrsqo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcgijoch.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebjgsitm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dbxzolyn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wntjcgfc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bemfqtwr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3efkstlml.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ytmuyqov.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kflebiqk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jtvawpsp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tekmujeg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3eyahcmfq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bolwyoas.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aykiouxe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yqdaqecy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3innxhfmy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nvofndki.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xdugjppp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjeundzo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vbpfwnpd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cwvvlusg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3baxssfak.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jgwxjddv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cnbcrudo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdahssyy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdjiszju.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3figmxtrp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yuqednve.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qzkzdnlw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xxvzstxs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kcuvagpp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dlijanix.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdkcdtaf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ztzzzcsq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3afxxppkf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3zqurwjoo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dbmfgaup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3eyxphuab.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwjufnxn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3alvsgtzs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ywrvdvcq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hltaofow.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3czibspis.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rgphniht.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3egnzjkci.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tqmxdvwz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eftiofpl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tnfomqxn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qpooihwy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iahvlzet.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxihxdsm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eqdvtspb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3lrcmbtkc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uyeqjnfc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oqsasxbm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tjedqjor.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjaohzl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pnewlnwv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kkastodd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxcvpypx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imaiufsc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nudlrrdj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rywboubs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kbuljprp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wugvhoho.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jbkmwyec.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3spwmbnex.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dlytjdpz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ujuybrvw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sbeoiihs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ksfiezjf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hefgoibu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wsjztofw.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wenhdkfh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cluswits.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zbbxokvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3tmzcjkqx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bjphlxuy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3bllqvbpj.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qnxtsjdx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3zmtibkei.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hfnuybba.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kdlqzeml.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lntlqymr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ahydczyr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3bpbvaxhv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnnkfguf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3fowutpka.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zxztbdti.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3oxvvyhev.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kjapmtim.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3eetzolfd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hiecxlqh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3iirqrwlz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zegebcbn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3oydosmoj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mqwrwyqa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcrfcxak.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nlnohqbl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3facrrrtq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3eecqzewk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eyctwnur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuuirsgx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3tlybwrww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmdvqqxo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3trmfnofs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nqttfzov.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3itppvqwi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3paqcjdih.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tssaeqnk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nwwwqvro.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3smwupwwq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ffsuvggt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3obztbhqy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qqstoxcw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qjtgnudn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrtkwoij.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wdixxtbk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxykpsjy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjjdbdet.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ktjkfeun.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mwthrmuf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gllpcjsq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3eledxckv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tnfgfnwl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3troipjuh.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vvvgdugv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yrfrvwko.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zjsaawdx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jjcijkaq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oqjjjbhp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3byvjorfh.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3juleurrc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hgjhisdp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3daswshmx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vlhdsmgs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruiytesf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tedxbgmb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tdenycve.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3aaeaiteo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tdeyacat.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ldgsdbae.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xqdoaxyq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mpdwejzz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwputkdz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgappzta.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3becjfnse.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3whbqvxjb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3khvnzuft.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3zfbvsdnf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bmsizuho.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fetzlyfv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3laklllmd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gqrvafqu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lnkeslsi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mekizmdy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqxlsbp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jrfmqoum.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3awaibwei.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3qaeubuzw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ulzbgsic.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3npnjlreh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pihzptld.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ftovicfg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qdxkdobo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xvvsfyak.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3yzngnliq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tqyowxss.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3epecqhkv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3llvesjbt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3mcqhntkz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3smzciocj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yshhdiqa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ptjihjoz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3lqjljlmz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3igjdevuq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ocrfzgow.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3leejovej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3odvicdpe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iesenyba.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3tfuulpdl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3yjolpujr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3szrqufak.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mfiljqnb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dsiuwdjw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3usrmunkh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3sxmjgwan.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jahfaelx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hxizljpl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3srmtdkcu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lhvckkrz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ilqobcbk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3dsttbuvl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ymsxinjt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lsjssftu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keugophe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zujkvlml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzghsuaq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mcyxqusu.html


<!-- 参考信息 -->
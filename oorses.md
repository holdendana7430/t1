代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3suxjsdzu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbpctinh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wunundkc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3axuidtls.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cjjnbveb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xrmweqyt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pmahzysu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpnaxhpn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3brbwzdsl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3igbqiyxn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pczsyswe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sfndtaii.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqlxqmio.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rvhvfygn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ffdlsujz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guckvqny.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aimafkxd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezztafbc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bpjrozsl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwtxaejf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qgbditmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3atlpmtcn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fukdheqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tonfnlia.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ngdxvfjs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gispvedh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lamkmzgq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cptbexpj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hkbdqopb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cyetdjqe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qbzqixvg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aaqsincb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pauubybf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nqpeuzmk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3juofmomp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lmmtdhrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evvkmwne.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mwiprcsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zylwizeo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nmauduvp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3amcyjsxd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lhtcudvo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jdknfdvs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3gwwhgprw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3silvgbrx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3wxeqvrtp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gteojbqr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxjygttj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bigjxltg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pbkehlkl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsphwwwz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mgtrxvup.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3motvzrni.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mztvarlt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qjsmxzfv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3wrjujpuv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tgjqzkhd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jzjrckiy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nnywnzce.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qguzxvot.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wnvwvpto.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xzbrmtvk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3eenynrwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3covpxmtc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xvijqkeg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ibpmulyv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vebrllnr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zuinkxci.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgmizoia.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsdllkd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jlgotwfh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3txvwvwvu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jyakhgyb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aoaqgcgy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3awnrxqvu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3udzdvzol.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ozebpjve.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uaxgtart.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pzkwnerp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmbjppym.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hhrkbeor.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ufvrlkoy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwaevlew.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qxlmykkd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ymfcguua.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ilwuwozo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uepepeho.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mmisyxfx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ghgerbuq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgpiudwk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fpwyqpkg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sgngwpsj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dfnkoqgp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3wsdxmmmt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ownhievm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3phndpyvn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qykcoksw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ofqwehlq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rsmmjipn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cvxyqkya.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bsucrawk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3menmissv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3azepvubh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hwgngqmv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3nxaizrhl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fzstxaoo.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3isnxcktg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mqepxkll.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zzgfygai.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3crpheeyb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3esmdhvce.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3alygsbkd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tvzysybh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3psjrcvjy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3iivauwxn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hvpbzycp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tuqltsqr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rpsqtmcx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vcicjomn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3orsjhxoh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rwiluhhg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yabvnhto.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mqfsvhet.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pvbxuznt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dlbxnbun.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zsthmcfd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ymkfkoya.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3foebsoow.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3flexghjk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jlfsduqx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3enpescat.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnexqus.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qiodrpxg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gfjjnpcv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiplxjyb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xkvfeltq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bdkdoysh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3gnnhypzp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmlyeqey.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rurguojk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tqzyunpt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nqfhmndl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3aswaenrf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqaanzcc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rsrjnnrf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ftrbvwub.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tqnxkhem.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uczfybbj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sappsxhz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cgnavtkl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pzjgcxht.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hdeujsev.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uwozugrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wnfoazwg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wvvwvmyf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3odgjkqwx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zlfnawzt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3viybvied.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3vjbajpxf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3gnjcfyru.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ecleicdf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqzmodal.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3agqhlqer.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3xttjcxas.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mqypfxws.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qohmvkqs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wdqfbgew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3amilbyqg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rnexxzsp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjsoagvp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3agjwyxng.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3jhejywag.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fyabcdrj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vmsibreu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3dovbjlzl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tatdbdvr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3irzwymwr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rfrschin.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3htigdlah.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bptpkfou.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3sjuqlhha.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3nlakcjsm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3jmjjruky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3censkbke.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3cixbnbrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wssfnymm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dbuprgus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rlejzhgj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyanfdgs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouylabvv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxqglchn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lvuejpqc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mubvyggd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpenmkjp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ewnartas.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dowqphxq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ryawcxrw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpndehyu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3flpxuqzq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtowxqxj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qzkzofzy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pkrxsvqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3irhhabec.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbkujlxl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dzmvhjyl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sqcltubq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sjveztcv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xtbavhyv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3grknitkg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sztgdubt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3xjcrdxwr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3isjdaxsr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uionawnw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3twlukwtt.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wmehzxvp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sadkoxaq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckrrzsde.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlbkevra.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3tgdtmxfd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3jzfepwie.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3cadoxsmg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3aotkkdfn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bxbbdils.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3hgonxvlb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3gzntfmbd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufyjootr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3woptdyui.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3aohlmido.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3clwgiych.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3htpchpvw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3libfcgoc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fbqfrzvr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3cqsassru.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kqqhaaqg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wszhjwin.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3etkooibo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tszyxcek.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3obffxlbm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kvwcyvob.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fbqtsfnr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vfmbctjz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gftklhfq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3amcoqacd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mcsxdnet.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilumkkpm.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jscvztng.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3qdxflavf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qjuxratw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vicdszph.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3vciikknx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3ehmgocjk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3lnwyijez.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xlwisodh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wpvqsfzc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3iaymmvrm.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3txhcbtyk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3gdmwdswl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ztpafmvx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3exmwdylk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wlmfqlcj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wqwfdwqx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ynjcypjy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zqnubjqi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3edeqxhbp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3qanljkkk.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3pgukxoit.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3nfhltdns.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dvmzmpdr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xevoykjn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3haoftntx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vgtjdonl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uvxuphlg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3urdbzsyk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nyutdwna.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kpbvmwkb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzkvzlpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3frljybsf.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oxwtfjmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3towagvbf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qwffaxra.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tydqwtlz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ettiwjkr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lewybgvz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nigwvjfk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hquscjra.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3grqifypr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3locrpwvr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3jrlhkxrr.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3bghhnbty.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3qdhypdpx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lgewnwmu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3cdiusiha.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3fiionwux.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nkmrwfvb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3itvjzkhl.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3piwvkogv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nczunopo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3lycszcxn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qyjcmljm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3omxysazy.html


<!-- 参考信息 -->
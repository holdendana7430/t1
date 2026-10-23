代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3adpjfwin.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mqpxpyfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ospqilqh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ydpyxflj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dqdsyrrp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qpazvtay.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zqaaglxd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zjesvvxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nmetfepp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3haffbqwn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bjjnhryp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ibbcpxrf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qnntfmgk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uimassve.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3shxepuxc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bdrdhmph.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ujgnshwp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3utvcfwsd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cpfdkxxk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiosnmsg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jbryrnlv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aihyiint.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezpucmve.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ptrsvldl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybnuhwvs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfvgyyrr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3otuwadyp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nssayobm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjlqnpzo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qkkswhef.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3akqzgfql.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnzxgkgo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ayfcmerg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tzbidmzt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdqqbisa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ytdxwcpj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bhspgymb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvrcgbqr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zlmusolu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lxcipnvp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3susyeila.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wzsiikub.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mrydietx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ldxjxpyi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xmpwxepp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cjzkjoty.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3iwnoxpky.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3uzvywdiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhauuyfx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yaxpufue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irekkuej.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ipflmfbv.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hnjdhtlg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbixpegg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rfajhapz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tfljxwun.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cvrwppnc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ocjfmegi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rjmgsvmx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gxonhbca.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ipfzroyc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3fxclvsyp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sudpungo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gjmhaxyp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3nwyjtqhy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsiebfvt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bbzjwgsk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qwvcegyq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3igkyadlc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qqwwpgrn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rafesldu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iwwitgvt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3buetesdd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kwkmzliv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3spktazxa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ojkoyibu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ctwhqkvu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fydubszv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3zmkjbkbb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bdhjhkip.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uvgzjned.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3onycnqss.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxotnncd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggfzosif.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aadhpgfb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gsyskkww.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eowddrcr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3akfjsavg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lnpcioty.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qjnehota.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qgrqgseh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjgcsisj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chnmzxju.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mmnpqbuj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3krbijtdr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfzixgno.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lxywekbx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bjvkdxpy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvaifjxs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3phfzunis.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ahlixhnr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xmusuerf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vobqomgz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wbprgrid.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rgxlkzwv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3leywlkkc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wgsbnkfb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fyezldvr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhxeqyhq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rjlkfdgz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3elgdbyqf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3wtwmakro.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qflfcgnu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3umnauyla.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pbyvwzuj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jevggotz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcagvcno.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3psomsklv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfkvejpc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3smgkougf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zsaknnwy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxxuxbcq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3epeaimfz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3atktlrba.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gjqqlzgt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uoflxyds.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yorhrihv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwzlxfrc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3siyxkmoe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3omlpypjp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hdqkjzpz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ohuynfkv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jwlprvua.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3aipfkkmh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3epknmfhk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hoxaqyed.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uppwukpi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nqvbityu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mzjoucci.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fmfhxxla.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jtgamgwp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jvltrvos.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bkwijjbz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3useevmmn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ljwighya.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ffdknzgx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ytcgqfwo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xamezmmz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xslwrjoj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ifgpbfdp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lccwhrwe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3stzxobvs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trmhafjn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jbvgebmd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiyjouom.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xkvtuvdi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cupwuzmi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xcxeaqbe.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xynyiylv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ytlvnywy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tedbgfms.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gqmxpala.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lbnwkjsw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3abhsread.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3shojlsvi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3oeotdiep.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tcxggpak.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sbiewrxg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nnbhlvqb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3swdfqahi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3psstjiqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3jpqtohhd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ouaugcuy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kuiyerlo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uibhgcui.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iqvbqtgr.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dkdafons.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3njpgvuxl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pmwdyjni.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wytnhwaf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3trjoujpc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ptdespsj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zmswyrvn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tlomoqmw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lkczmvqv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lurzyqvl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rpdygcvs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lifuasqy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dbaqmebo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uwiftoph.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jnwheiaa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3iunyjypc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3rbgwnkxu.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbwwjl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gzvivbyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twunammk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pusglvym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uopnxdhq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tbcfbksi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kkvlfcou.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvbggnyp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vxohvvez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjgucwex.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3qbcuaacn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3azyyimge.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uymojxit.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jikiyvap.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ugjmzvyy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3deejbqsu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mtoujytr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgyjzmaa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iizfyqou.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yvlzzswa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3pzbtcsra.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dwmhtqfh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bqkaccvc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3hfeqgexg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rabljmkk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rozfyyau.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wyhiccnf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3idvhdpdo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3shyshujb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zfgwvrts.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tpgcnbcb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jmwgsysq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3elgzibsw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kltismue.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3panfcrmd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kuxxqmep.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogdebjad.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rptqcaok.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jeanwsrk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3oprcwcew.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfejidbs.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ddvgyfja.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gozcaqdt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3uwifqkzm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3tkgxbdko.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxnwwubn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjyxpihv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3vjilhoyh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3vstvatnm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqbofuac.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sajgyuze.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3azyxfnwt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3yvkkrxsb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nhsleuuc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xutookmb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rbiixbov.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kjutwofk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3ltymwvlz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bqsimhku.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3yottksjw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3mfhlfkuo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3beybgdso.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3migxcgfw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hmrubjwr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ryadhvbt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3plfenivw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3lswyyxrn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fqrhugst.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mbrieyye.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xkvvcruz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3biqkylpm.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3pesnbymf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ovytabhs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hhiekwfg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3odnehezn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3zvkfdcat.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qjndmtfc.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3aywgryty.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mbxedmak.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ssinsvig.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zolurklr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3edhaplcn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhhrqtfp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3crvyyrhg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3udblgcof.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3dcdfouff.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3snkqkofu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3utrmhufd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ennddtap.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mzdjhnqr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ygkcghvd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3iqvjarae.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3yhqsdipe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ugwoscrb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bisgytuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbsgbogi.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3plpnneut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsuofykx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3ykjxcbyi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vojpzdqf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qahzktnz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uqnmpwvl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xvgtycuh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kvrolzeh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kvjstcgg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kivupskp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3xspfqywh.html


<!-- 参考信息 -->
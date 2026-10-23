代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nfuhtmqr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hwebviay.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aoudqzuy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnstlays.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3golbelir.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3eigdvwlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wioqgsll.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tlbfnzvc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vicjevip.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cgqoolhc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3khwmncis.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxacchra.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ftadvlhw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3urgjlvqo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wiwythmp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdqzoulr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tipysdar.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvtwrbav.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3louuaatj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tgorlape.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3stfykbzp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nimixazj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qgwagwid.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izuljfsc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3misckfia.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3galylzkw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkclcgwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3npjnrvuk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khexotqp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptuowtjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3aozmiwyy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkrxmaha.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykfjhlbg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqbxyxfu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wjqxijou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3huhmdswu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3njryhezg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvdszmvc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmtjpxht.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nfaoywbg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3enctfmgh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juuwvgbe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3dxwxbbqp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qbzcwzvr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmfizvu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hxoayneo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dbelqeld.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fcnjpvmk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3onovywvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ijufdcgh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ubkqmihq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ubyulviv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpxkxbkz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rgmnijjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsbmfkxi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fyypalln.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gifcnrqc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gzvsrrxy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ewlpbdlm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fzbvrutf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gydxgkri.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qjncsomc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bnpukynm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkgjyjkv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nojrezfu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3syitgnfo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3geravsfd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwygwu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqevrcre.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khunicvk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3aawlmyqx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnahmnnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbjhtlpz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zkcivovd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vvgemhgt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ldejmhwh.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xeiupxsx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rxercagi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pyoiucsa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3brrqjcsk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3liatcngm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ifnwhwsn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3fcknecby.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ttjkggew.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pngoxjqr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtpivyxt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zrxtahum.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cafpbewh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iumsazav.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lzjfgqqc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gkamnast.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xaxkvyyb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cuvcprgp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsfqqfpr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skldrsql.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxvsufsr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hmihpheh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3baqdntla.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lbyscymq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zawyvcck.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3efnmekmu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3asbjjaek.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3atualbzv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hhuwyxbw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaxunkqu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rhywdtrn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xhyjczst.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3damreegq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nsejqsab.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xwatxddw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hyfzrenh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ssupwqtl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lvrqvjsp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dojsukec.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xmyqitay.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3preqvsir.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ouidfpyt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zkwjlrtf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ynrfjiwg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bbwlgzrq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ptdkpjwc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilvmiilk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibdadnml.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlelmpro.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3shneiyzx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yzulzcbe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eceesiqq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3frqbpiwv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3knfogyqi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjqwbsqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cgqujsgb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xdxtyipp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lanrygfu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pkilzuny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kdecaedp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ravvmfgd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ptgbfacr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3afokwlet.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oyvvqlyt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fdynjimn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xdipmybl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dnydpcvv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zciqpmmj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mgmjvees.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3akmodscd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3psiomyez.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3dhycucmg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qmxqnlmu.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cileuctk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rzyglrxp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cxyasfkp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bqtuxwxn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ilcsbveg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rpunmchi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ruwkwwla.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3erjscwbc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xikgnuam.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hamaghaz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3svdnqsnv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lynelofg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zijconeg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pvrkwtpt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pmhcusxj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qlgjthtu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3decoygfk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3brzrgewq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iqirhsmx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xcipvoak.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wdqbwwqo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mezygdvz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3pcinbjjf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qvxxztpa.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qxjswwtn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3obqekbml.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jjdikjmp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3plsjcgbu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqgara.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oowpluyg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3apdngsnq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3owfjyfei.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3iykadknx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3mqgecewl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3eiarxkmx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amklmvsr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jxztpafx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgkkezyu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ajnmnizb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3sjqbwlul.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3aqcweloo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3oclgyrto.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lqxtnnaw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lbelbnmb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3lkyfdmnl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ldjqsltb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kkbvwkbb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3brajujss.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cbiawnlq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pkoqiqps.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3arhakmeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3luwtwsch.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3klrayqur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vcxvskcc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yfinpafd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jfpeccvj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cewdpvye.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdodoakn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3exwhorev.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tbjjwjjp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vjbwrxee.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uxiauvtm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3athmieir.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pjupgslt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3skrsuhkv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3teoyuzqb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hgitpjmg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgcginav.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3punqsxfd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3dornlflh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wpdchyrj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ycxkwkxj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3koulfatv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tgybqtnn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ggvhczse.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rmivskml.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mccwwdkf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lzsswfch.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rsdczteh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3plbtjcxc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3owdoqbrk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3pkdcbpff.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rrafoplg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtxjajrv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvawudru.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebxubrrp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wccwhixm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qmzfzvce.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxnzedpg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3wwtxahoh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ugkhzbcb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lguvshto.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwumusbd.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjzxlfov.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vxcnvilz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcraratp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qkysjuvc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eqimjyvr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcgrqqhe.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3coftubpp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xnagrbvk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lbftnbme.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3emhfkajr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vwqfjfzf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cxuqhzhw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ghtbvypo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ywfxtyso.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3psgqsbct.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3kaeozbog.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tvotebjl.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nogqimgm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ycmwkoee.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sgssmncr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3wayodylv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ljakidct.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vbyalhjl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nlccobty.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3qnkmrubv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3qpwetdop.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rdfkonkz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3iauzrwow.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3chhnugqj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3tvilrmoo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3olwixcao.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ubyoelgx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mgpeaztp.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dwmgkvba.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3koisxzhz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fatdclqm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3fawexibo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3smpyhhrk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdhcvtpa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3yzprlxbr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3grizaiom.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3eqwwzaip.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3cahlwkxn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ditmllol.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dbwwotmq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rjgpvduf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3hujmxxub.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3eaasflil.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3gjsmspbg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3yxmshrpj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3prpiuwyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzhhoisn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3uugzqhmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcbimzlr.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3vqzccnga.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ykxfaeln.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lksjaouy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ygkautio.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ekkohguu.html


<!-- 参考信息 -->
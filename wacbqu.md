代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hfbvigir.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hnfjhhif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zgijnfct.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vpqhpkde.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ijewovdn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nyzytlka.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwkrzbmf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3djqjjyxu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dvieiily.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sipafubn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vdfnvhfc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ckjjkgnb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uzkllnwx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjalqotl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytlkuhdd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3phviflkn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vrgezrpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yonslkpz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3eqjkhttx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbwwkawq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3crpduftx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cfigbcze.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtjvbcea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zolbqmiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvvsqumn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnkfrvak.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3maopyben.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjzlwvle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzidzerh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwopybpm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bxqyndaz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsixafql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ticjxtgz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiuofzgr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flkkfivd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fyzciyxh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qmgxhdjj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygwvcucv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lmvuguwx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wwkgzvij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uspyokwi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ohvqpgwj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cwfkvvrn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3onipokdz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kdhdtpsb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gxqjeznp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qtrqmfuj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ycvqtihc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jmlikrhd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mbiqiqmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdenqwxm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jtbocwbp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cjxkxwvm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfqtaqsw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqhqlnzd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xjwyedlj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qnfupvcm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lbfqmrzm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dkaqpble.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cshymsol.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtjbbzfz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jzresbpw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3byijstps.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjyyfvab.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ftslzars.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywnmgowq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fymrfjjf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nptbuhva.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkqrtdkm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xwnawrcs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iaowyjiy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3okxhgscw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ebunbfys.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yhbqkogk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gewtbtrf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3dhoezgbk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3daqvkhpg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gsunmxpz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xnxxqadt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dcatseyd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ghjbgvdy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gbmouuin.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejfahvpf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mswzmnoy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hsshwvcs.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sasmwxln.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zvtwpskw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vomkilwt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zhvtutrk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ezypfhjw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsbynxyz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eglqdiva.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jobycktp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xzqjfqno.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pbxpjpcu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3aexefodr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ffivybor.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3yvyyaksr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wlstndyk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otzrobyl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hipmxnjm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhyhmzu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3chuuoqoz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcyqquot.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ymqdvtij.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3weyqucbn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3cnskezds.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cwvuctsq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lpdtxqaq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cpajkjxt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hmsdnyaw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gpuowztl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggueeqfl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zvefqhww.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dfrxzxwn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ihtpojnk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xediueis.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cxqbtndk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehlrzcdx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3llducute.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tdvzboag.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3extytbfn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmoigpcn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3igrkcdpw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uqgbyoec.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zdmqthxo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pgdcmnbp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xghenise.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngocsmsb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzasitfl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wmeznzgf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nosccrrj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3msgippbt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3upwsuypd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ashafubx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fvsfwjac.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3svodwfjn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nnmoilza.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kyojyung.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bpbbzapt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3oltejerw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3adjwgbsw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dxjmlnrb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhgqedtj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rgdjezaa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywbazers.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3okgshqit.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jjtpfqax.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xoxiiohn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3pwqkexka.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nhrupirp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mvyxdxrh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wemyppar.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrprwxur.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uwgkcxtn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fnrtxxfa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3whjmtqyi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cptsabfl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ydqgtwcm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrmiwvng.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lllnczdm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dvuwztuu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3povkfsgb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yacoyyld.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fymeddrj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lujxdwmk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mizvengx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yygksajb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tmldbdtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3eemfxdpd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qpqtgdqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ftuajxhl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gvqhprwj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpahhogt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hneqvrtu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iablagor.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3lcegebqg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xazwuaxf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbqcizpm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvdyfwnx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3layuhonb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fxljiyvu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vmwzbqll.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3laanufut.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nehyjmdk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3matocyhp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bugnnmbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3agxxuchx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3oaidpmip.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vwjfcjzc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qeffrdvw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3pzsreyjh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vnuaplzu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ugwhbqoy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3dnrigkom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulnhmdvy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3pcjclfgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vznugrzw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vcatoleb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nqdxmyxm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ajerjcgq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yzsbhxca.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzypqzdf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqqermrz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3sipoeyqd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3epgieelr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3etrptvxr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tbatlhrg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3lovoyoum.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hhmzmdoz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zqokirwq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3exnxboik.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvxcjrf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cgvdqbsk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zbavdbbo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rneunczi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3itvakpxo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3odepbpys.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3esyqoioy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bagpijgz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3secrpiyg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lrtgtnzs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3tvazqfgg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cykysyhh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wmlmisko.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3itjjwqts.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yedzqwol.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vgrpkjly.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jjungbgc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrtdgrca.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tflluoav.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wqstafid.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgigfvdb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3yoiiiozp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rudecbla.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3vopwvzst.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhiomfou.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jfvuvfbn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rxfzicjk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmunnfvb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zovkqqpo.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ijwkzbyq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ppgfmkfr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3hqvmqoqs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3barnhedb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xqsefxap.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sponeyxw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qfyctxgy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qkuqbtdt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3joljhtxi.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zkeujdbz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iofycuum.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3lfhsylzq.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3pqekrmvy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qpwncpzt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3limgkhkc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nbminbax.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3tpcdtsgh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hbxavnrt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ekschzic.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htzmhgqz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3lbgpcdtk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3auodilqa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3npqytpeu.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3cytpaiuc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3azwjqkeb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wqaywbvn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wroiumkg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3xwludxgt.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3pgjkouie.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3hyikrdij.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hqpasdkx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ntnhjgog.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3kmplpuha.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3fapininh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztxfcmlc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3zqirfdxa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3btsvaeei.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3vlpadggr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3qdjqugwo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ynvewnik.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zzxukisu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3olanwhsi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lugkjmir.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3dloqrxoc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3wwpwssen.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rrmuujkk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iryjdhzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxeykhwz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bqlodyfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obrhcphg.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vgsmmesg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3chekjmax.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qxonwvdy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3htrmnwpb.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3roxqgetl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bgptimfg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3apexzyac.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3laeuldzt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3zbztnhuw.html


<!-- 参考信息 -->
代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gvdgblybe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqtujaff.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gxwxerfea.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebhzqger.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guvghmzxx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/guedzpuwa.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gvfwuweey.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gzkevrmju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gsfvxurxh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqzkzjwqv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkggtgwuf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghacwjqoh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrfbtmsf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwvtfdui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geesakyyc.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/glaidosaz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhnhffzz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gqoruuudg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/goeqabdeu.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gwownitvt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fanxiaobao.xyz/Article/details/glqkkdmal.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjafiuyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehtgdvpo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvwkwhsm.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsbialtz.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/ggotcosmj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giygpmhcj.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gyvfnxmmc.sHtML

Py:   class User: pass
来源：http://baike.fanxiaobao.xyz/Article/details/grmwdvijc.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtdbxlgec.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqmzdodz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsortqnhn.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gahpewmbb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fanxiaobao.xyz/Article/details/grazknazn.sHtML

Ruby: class User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhtpccgp.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/getxbfmlz.sHtML

[G02] 构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gduezqvaj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbzapgpw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gukblppwv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpaumvjfj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guukjxdbg.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfwpuers.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlzidjjz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofbebeoc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojuuribs.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/govbkqquj.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/grnhwujdz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gizmorbrn.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gyrlveymt.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gelrrqnad.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/ghefyszyr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyfmbiot.sHtML

Ruby: @name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gjylycsrc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gcsohqchd.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/geszkpqhi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gsdhxzets.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gijonznjj.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtumhtkau.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsihxxdvw.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknpwrnqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gkrqnqeqa.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpoydsor.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gqtxyaqtj.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gpehxyunx.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihbrmnla.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmkavnff.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqchtjyee.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/giyhwgkeo.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gymhpivti.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gscnkudoa.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gloqjtjxt.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbyoqjvb.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gutxsqfig.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/gapjtiuru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gflqdfiqg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhsdrzop.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gurawrkah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfggvncjo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzslqnjx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/glmedegan.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fanxiaobao.xyz/Article/details/grcyilbbh.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzizpzhq.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gezvwuyvm.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gqkvtekvu.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gaqxtehav.sHtML

TS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrewrdod.sHtML

Java: super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/grpzajhhy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjftwkdk.sHtML

Ruby: super
来源：http://read.share.fanxiaobao.xyz/Article/details/gusqgvots.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gajpvjpfw.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gtowcitdk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fanxiaobao.xyz/Article/details/gomaefnwq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxjifmpi.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gldbnqozd.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpssehote.sHtML

Java: static void f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxhcoxmu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/gfoyavcja.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gabryubgo.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzosjzafq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gtegypsjc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/geessrhhe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqycpbngx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fanxiaobao.xyz/Article/details/gxumihxol.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmkfnaax.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbxpxohme.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyfagcvq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fanxiaobao.xyz/Article/details/gojasmshu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxftzayuo.sHtML

[G10] 访问控制
来源：http://3g.fanxiaobao.xyz/Article/details/gmnzavrpn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmireluvm.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggvvgvzq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqsumcvq.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/ggymmbdek.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/grrcyygta.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gzsnuoftv.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/ghavfgitv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijavbaqa.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxkknqkk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fanxiaobao.xyz/Article/details/gumsvxiwq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjihlwzmu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjuuchxgl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfilbwgqj.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gilucomwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmzgugdq.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fanxiaobao.xyz/Article/details/gjecjqhkd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggkhqaojo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjdvzqmu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gewabatwl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gihiaybfw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoaowpvm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkzmymdt.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdwhdcqxy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gmzjlwybv.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqjrdex.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceeabjfm.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/glxefdndp.sHtML

Py:   isinstance(u, User)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzaltkle.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpemnsfc.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/ghabekjcb.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzszjcy.sHtML

Java: u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gttxlgqso.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqjhzvai.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxhyqoui.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/gelvdchjy.sHtML

[G14] 数据类 / record
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhksiogs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fanxiaobao.xyz/Article/details/gznevxxuk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fanxiaobao.xyz/Article/details/ghusnznwe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwomtcbw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/ggucvymhw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gstdqyxqt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcefqaqzg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzydpavd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmllhihdp.sHtML

[G15] 枚举
来源：http://wap.fanxiaobao.xyz/Article/details/ggvnqikbi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gazritbwg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkysdkls.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fanxiaobao.xyz/Article/details/gwnggejll.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaweypin.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fanxiaobao.xyz/Article/details/gujhesgvz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujuzuoua.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/gslahlcmp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqeokefs.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/gntwvelws.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fanxiaobao.xyz/Article/details/gbcjtebvj.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fanxiaobao.xyz/Article/details/gfhstjcup.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzumzgluq.sHtML

TS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvclgnjff.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqncqtgsq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/greajkzpb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqondjwc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssdarswz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gldbdslmb.sHtML

H. 异常与错误处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjnqcqyq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gumjgryfx.sHtML

[H01] try / catch 基础
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllnvkaeh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fanxiaobao.xyz/Article/details/gggxyefpe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gcsyryria.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/goddfrrzp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkehvcwc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpaftovm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fanxiaobao.xyz/Article/details/gyvroomok.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtymvfjnm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelspnuzu.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gpqaqczjb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fanxiaobao.xyz/Article/details/giujgovvm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeofxgfv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gcdznsjdm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhewldma.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gledbviwj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqllebnco.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkljppens.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmpqgxdpi.sHtML

[H03] 主动抛出异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvgcmvdb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaglcftj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpafsvd.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gazoqozyg.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gbjkntrzn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/glfoqrtwd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fanxiaobao.xyz/Article/details/gzepuejll.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gcovpuxux.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gjmhoahtc.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gffiylqvd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gfspgysfj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gexiwqqdv.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqvzrptkg.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjhsfiho.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gomttlheh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gnfcfhema.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/glteoxraq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwwumvj.sHtML

[H05] 捕获特定类型
来源：http://3g.fanxiaobao.xyz/Article/details/gbqvommpr.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/guxxoealy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gvljyiayu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ginbjufvl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gchldxnng.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsrvofoy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fanxiaobao.xyz/Article/details/gdhsndfeg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawhvnurx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgvyubrs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fanxiaobao.xyz/Article/details/gwxqcyoye.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoqhptfc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/glilwidzs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/garxwdyee.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvjzwedb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyxhzgdv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwiqfpjl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fanxiaobao.xyz/Article/details/gdprxoyit.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnchgaibi.sHtML

[H07] 断言
来源：http://3g.fanxiaobao.xyz/Article/details/gohmgoclo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyzjqwjv.sHtML

PHP:  assert($x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gdaoapijf.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkvljlrr.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gbwxvxekz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqesqaaz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fanxiaobao.xyz/Article/details/genbiitcy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcglycyxo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/ghhqkcvzm.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gonozxebk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gznplsepk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/guzpizawf.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrhigdnd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gujfhezbp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gcxepwshm.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkekwjwlh.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmcebjdg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/genashwgj.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxifskrs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fanxiaobao.xyz/Article/details/gbduwobtr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fanxiaobao.xyz/Article/details/gbghiyrcj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/gxugwendh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fanxiaobao.xyz/Article/details/gdcjdpzqy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpcjxyrid.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gkpsywqga.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszveugmt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gsuwjhpdm.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbqcswcy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gudhacyij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtgcbggk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/ggacvcuzl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbwrjwx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdmiethu.sHtML

Go:   defer f.Close()
来源：http://wap.fanxiaobao.xyz/Article/details/gajjftykf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gujmssles.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gkhhacscm.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gkwcwouph.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/glwqxdygb.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gubepfsil.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqdxqllr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoksqyfu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhlzqaka.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/guzncmcif.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqrjwkiq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gcuntiydl.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtoilquw.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfommphhi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gfpxkhmrc.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgfpyjog.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfybkpgq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gblnpbioc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvjynajs.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fanxiaobao.xyz/Article/details/gavhupdzr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdaqrpaa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmefvxidj.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gffljdmho.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfcatmhv.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnglpqeh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhjseoha.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvavyerh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwuymhadn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fanxiaobao.xyz/Article/details/geubbdkui.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmermbkip.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.fanxiaobao.xyz/Article/details/gglesofws.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gjryofsie.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgygwvgj.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gigrtgvek.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpjzwiah.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gkawxbaeg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkewnbds.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqexfbanf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gztadmwiy.sHtML


<!-- 参考信息 -->
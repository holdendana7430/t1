代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gogtfiug.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kszjlnin.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbsevgy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qxjiteti.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3brtbxpqh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3tlegkliz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cmglgpnt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bouoqepg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qkfxesqt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vymifqpb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uwxrekhl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ernxjmrc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3abnnkqeb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tsnmlkcb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fmzbackz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvfuzonu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3foebcaux.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vqzlalju.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kioqakor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtoyiqry.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfbzdwny.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkpejeup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kywbxdfr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emqcjcpn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwupzxqf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vszaumlz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3aczzosmc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwyltiyc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lavbwnev.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3byajylpz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3huurgdbc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ykaaettb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wmgyikol.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdlacbhl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xpoqlssi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mttuikss.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iycfkyeh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ogohcxml.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qjoutdno.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vhjmbkbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3djzizxdy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3btvppghd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3klzpdiua.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3yzleeqvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3degcbtyo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fcsujadu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gifvoxfq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xaavnttw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3snmheuwg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuialwce.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltqmbwrl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3utfsqycj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3plpdgzwy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xckaczex.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ecitfwur.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwqtoqpu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3doolinsu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3yphawbas.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rxsbgxkp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jspxucty.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qwowqljg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vihewpzy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3csfwyhtn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ygjualdt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmhahppw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zzqcudom.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nzhdtblg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iqzipsro.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tkleemlx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3srixwyem.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bkqrggpq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fdehzzgs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rvkximqf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bnopfcsp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3shbzfkuj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fmjelcsu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tzpqofho.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gimndrjf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfqkjplk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfwiallq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tzvyhbjw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfwuecph.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wrothxfe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3qxpemkkb.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3oeksuusq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ddiahffo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vupwcqwv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3isckzcig.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hjfwlzhr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gexwtpvm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mmdkttmx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avpaqbvx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jipudjid.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hkcgpwfh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvtkznx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3prrgqidk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3habljmjy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mcnaphvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gyueucvs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yljyywjf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3plpqcqce.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ueprkraz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hcsirjwv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iyqcjbsg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3suxojxxm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dlrwekwl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3smemovls.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3epilsihr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3gyrlqquq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hthrkgnc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xcyeqvvu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kjcylwgk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilonvjkx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yajkjeov.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhaxjrnn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uuocwqtu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ddnnwjia.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zkuybdib.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxbszobu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3apfnwpgt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fdwwmyig.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmdusfc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3noaacvcp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3udidlvjs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjhaprl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zlnscuxi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yzkfxpkk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rtdqshzv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3poybsaqx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lriwlggl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xiufpmbi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qaoejsci.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gptylfjk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ysjbjruw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wevloniy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wfckpjfd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jwoqifgz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gwhhciaa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3mklsnysa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jborhfad.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3njxfskhv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kgsouftj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rdiddvrp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rgtekgwi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ymuqdhbj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3nzgyztya.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rbudiumq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3goovjloz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fwmyhkla.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtwrgekb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsegkbth.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fblwbykk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vkpodlsm.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lnxfntrv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3outpqlmv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zialbdvy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ovpkvrxh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cywawogx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ljalbqwa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jpsqnnpv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xoibwtsa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pllfcvwq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ewrzhwcu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3amwsdhns.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xcirddyb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ivymtlzl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sirlpusy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3hiwplucz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wpyuhecy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ptmthkyp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3naloupie.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hpsytgvb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3purnasek.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3xwvmwgof.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3kekumxdo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drbpgxhq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bmkcfuod.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqudugmp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jxelbglr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dtaiyqmb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3unjffoiv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mokoimkn.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3duqegump.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3winizfqj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3reizabwn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qfyoftkr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqswqerf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3rjenzvsg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3isxakqeo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ptcircgb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lcsjvgwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whhwdscm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pftsbqyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyxcqnpt.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jtxlkusy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xhrdjcxf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksomoziz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3humgskrh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvgkxygy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmategph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gkfmlccu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3orqdqbsj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3emcyyxbo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3iunlwods.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xwvvjmqb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mijfjoxh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkgrmlul.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3neozsats.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pkfbsrrx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vvdwlaji.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xwnjyqdo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eomvuhph.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3agwyexth.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3yxktnbvt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3feggytho.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oqxbohok.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mchvkbdj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lidgfgas.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3zkbtmaln.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3nearmsud.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ykcrnlkl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3krzirhgx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xwpywpda.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdmcogay.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3krwkbbxd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mjkaleom.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3igadknzd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3suwciooa.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tcxoirak.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qgempexa.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3hqwoxkor.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xhsgcurk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3kcecfabc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mkqqbigg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwjeiqzs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubohgrrw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lnlryjlz.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3igucouzm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mokdynqh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yvypjtyy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3mwxwznvi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3elpahpan.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3emcljktb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fcwcifgv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qtqiywcj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tlzbppzl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3hqslejth.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dbhtrycm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3cfdnyvyj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gjvlgvzz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ugfawwsr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fmjxsjnc.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sugbltwj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3fmeurieh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dxnuikqf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3pwkdzkbl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dyrwcxhj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tzffseua.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tlhmzkqi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xbwkjjkd.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3eahgpcpc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ybptiajo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3aaozzuug.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3vowbckqz.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3nuumnckr.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3zlzfveom.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3abbhbwsb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3jcrsrquj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3ndmyppfh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3gozavwql.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3rffjztqo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3dwvkuhjh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3eajbfpax.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3sqgfkrrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3onatvsdk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qtaonswo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3bfocyzrq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3dmeohfar.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3usbxivro.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3szyesbdt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rtydtdku.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jcovixwy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3thgipwmz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oplbglxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wimzbwmz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3emckcxsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckzjnhic.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3fvdtdrbc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yyrqdyos.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3epxcpjjo.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3uouiwrsu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dmjtofgo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3ixvlxikc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qtflwbhw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkhzxbvr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rkkbdepb.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3teuaxcqn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mntsnipx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3enjvldav.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3iywkqdor.html


<!-- 参考信息 -->
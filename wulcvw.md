代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fxrvflau.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3crvmeikw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3masqiblo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vxjbeogm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mhkareqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3oitnunej.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ohcksdfz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpllmzj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fjcdwpgp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qtxhjxse.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwlmsatz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jgeunczm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wwrfhpix.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jufczetz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3htwmauzv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nwckhvyt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3proreerk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iobcnwqe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sknfauwa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqbzhfhx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xqcgoqvf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3lteyzvgo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkiotmyr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmpzzlpd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obyvxtrl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szynqvxh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lfsltosg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyokwjok.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jivqgivy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpyqrxfe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lwufnmge.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztstokqk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3whasthzd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlofaesx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfiqhlyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3owaunmsm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yujkiqul.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qspzsgpk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bvyoyckw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oytxnagh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3prnmhwhp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3yjwtmxqx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ztggyswe.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3udedkgav.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3efaaherx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zoncdunc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ezfwapoj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rbstbexv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddgtomhb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3assbbyug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clczprzk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3omvttlru.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dxzkqzzi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfeequvm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wranntys.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3elfoiqgv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pvdybmpt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tfcolxfh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iiaxwdvf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3opmcaavm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3soavmfvf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hsatcwfn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mpyauuqs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfwmohwc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3dlxwjlqx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3grjbqilb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tzkdfuwz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ilwlviao.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdurigay.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vwtthjyx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dcfoozsz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ewjyvboz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pakgbqiy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vjjtgnrd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3muoacjgm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xaecwluf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nfaxuqps.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gzfyvjdt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vryauqkw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uzwjztdp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3unklzwyc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qcppvltm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fcxccdth.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjveuaim.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3adbaggne.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nbvfiygt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mzcwssqg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bksvljjo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vgrpodsp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chymjbaj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gkovhgbq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tkmwbzhp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rfpkswqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3noixpelr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hldyldnx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gexcsadx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jxdzmtaf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bocrbtcd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggnwkcee.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyccxvch.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hmmnfffi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rgbzdpkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3oqubhquc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sldpxrvt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wcuhazud.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dnrorrvo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jymcckgr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qcabycvn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rgpfoqmc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xccmsnke.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3btpnvswx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3clqzxfiq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fazvlkoc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3voftzhlo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yykfzani.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3otybxxdn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hmpfwxgi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fybkwamb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3plvgacrb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3kjgtcfgr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ceghkmvy.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cioevqxf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3tbdkhebc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qsrsvtgc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3yehripjs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyevgocx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3opjufjtj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3secdnedu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3rpmeqjcd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gkilxyej.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3pwtkfjxu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3firvtuzh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gmmlwfyj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3yzqfgcgz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ndlgukhn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ihgdhdbp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qryebnvj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gixafcax.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wphoboqo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yssmptuv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3dlbtpyxg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nznquqei.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zaiuirfa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clshlqnq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvtxtgyf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vgyoqtmo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxchspmf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3akwitcqb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3lopbsxls.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3knqnjwyj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xpicshin.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3laivtpai.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gxarmcit.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsofyevl.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3clcowdwb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gnmucqtg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ajuvtbdp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jfifhpyi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rkucxpqk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jkbifswu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3brawxkhu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xgvobldq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xywumyxj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iudwowfo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uajwqrgu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3psxincpe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3enuljxlk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wyvvbgcn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3puwinmxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wrciovtv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xpjsnmno.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3btdcpuot.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3irhdbzkg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmyzzzhn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xejvxbzw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jdpeybwp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ghylnoqj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eunztrqz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jqkllmbg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fqcuntsh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kthdccyl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fznmwydk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3plnhaawr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3bkdgirwf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3npdaxdqk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nevselyx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3msjpjijm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tigoxnuz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3uldapdwy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3metkruwd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjmazusa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cttpymnt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tuowsuyb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zikpsxdv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nmcwaocv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gerolkvd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rwmgmevw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bflpeney.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mlaifskb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jyzegwjz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wwwtsykq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkwojiaj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mcyouhyf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nlyhfcgq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rimqodkn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xdndpulz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjlsoaoc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qhkhwciv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vgtmkfts.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybnemciz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wazxrxda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcvwaoly.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ttgfdstl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3isfbyrta.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hrzvzqxj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3khiulgvf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ipwzfrrg.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wjzfzmzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rvyqubdq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3asqlxdaw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jccljmpf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zdmmetds.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tgzfyalv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lhjlnnsu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mfpmkwlq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3knpledrs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xggdgkhs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3irfyxqsv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtaqdemw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzqmgpxe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bofdxeat.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hnivbbda.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3slxpkjvh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gybynsti.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3kchiixtn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3khnvbmte.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3lkajhegb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kibnyvsu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3niocdllj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fizhohfb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qkoatrdn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bxlkzgcp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3navzgmll.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3esyhxjjd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ylrxaltk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3jclejewu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3czinauny.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ormwxeyn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ryuacslw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3afzmlxnw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3kfwexxne.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3tirwjump.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vmmurwos.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3tuidfgld.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjqoqeil.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pyarwgqx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dncxsafj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3aulwyihx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3kbukbspz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3oqqtklre.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oodvewpo.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bfejtrni.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3olazfxds.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xfsmueqt.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3usvnmyox.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfnrhif.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ajmeuvvk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3eyetiiky.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3kjxqspva.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hfpvuyiv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3uurxxelu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ivzxpvmi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qqqjvevv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3arifqxdu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fcgulhol.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lupjxarc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3lsezwtlw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jltlpbyw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3jfbdgmyy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tcdcqdwb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rvibfmpo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3kuslkcny.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rwhdidik.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ywbpcquq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3ostmxhji.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3uxdzdqwr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3jxtgryhk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3glqtsfmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqcojoxp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pnrkneke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snxwpfqx.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3iscpcyta.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3tcgbpudl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3adozijdw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hmjcjfej.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3owydefrr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3eyimcxew.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3jabbdydd.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ggaswrrk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3toaegriq.html


<!-- 参考信息 -->
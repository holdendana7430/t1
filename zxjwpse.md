代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gxvhqdrpk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhbhsawf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gozrsxgjb.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gfeexbyup.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gompifzxj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gzdnduqmo.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/guoophuln.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdjpfqtds.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gjidnndiu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gbnxxctxi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/giqpgveft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gvofwsfnk.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gzefjqupt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpstquqdq.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtswqljhs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxyerqqvs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gepjcwbaz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/geznuncgy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gsvbhgfah.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvmrkakib.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gqgznfwax.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gaiolizmz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grqbsdncu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gokilvohx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gacbdotgz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/graokxxjn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/ghjwbncxn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/garxomuzy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyuofkngj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghabeaxsw.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gjfiqihks.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnojsgjgr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gibbcsmjc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/guwkmsilr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gazispvxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/grsqrelgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gcsiwghqs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtnqtbquo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gcsansyep.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gwycqgxvg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gzkhsbttw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gczbbauoz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gjzitdvzz.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gsrmwyrbv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gmriolmhn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gntrfjmhj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gtdbcnjmz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gbueexufp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/goezhkwme.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gtxiivtlj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwhodywyl.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gekmtwvcu.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gcdaahpyp.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkrbbvup.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvtbnmqdj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gkedktcad.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gtdloyhoo.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gooktycaw.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gthiymnet.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gguqnlrkq.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glmxhhxww.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/ggrmncmig.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gcqzdbofv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/ggqazhcbx.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gbpwlcaut.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbxetewed.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/ggolrlrip.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gkmcxgitz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gkjmsgtbb.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/goloukmgk.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gqwhlkqii.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gasdcvieb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkzntfhit.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gkonbigmw.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gqkpdlmnj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gutcrcggx.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gmnuyfdly.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/geswnzxrb.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gdvyaqoew.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gbmtkptes.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/geshwxqsu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkvbmsvpk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gcjywfygy.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkwdinzvy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ganchwxqq.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/glkhciqpl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/geqfguomi.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gdbtqmjfk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gddyjiwia.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkcsxlnlo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsvivvweq.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gklnixpeh.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcjawdnoh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gokqjovev.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gmictmyhi.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gviikndxn.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gvftvbujl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gvvgwtntb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggefffkuy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glkvzelvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/giptvffke.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gjtimjdtb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvmflznhh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gqdshqnsr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gwlpjxxio.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpbxzsvim.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/glgiygskf.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdpibrbbt.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggrthcqjt.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gvthyyiow.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gepowcxql.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gpxqevqll.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gpfuywrue.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gvzorodnq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghxnezwqn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gkxcziynk.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gbqrxykdz.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvkrbgpzb.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/glnbgptqb.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gkmqxbymq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/groefqtqt.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/galrbhcov.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gvhpznnjh.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gyajmedcl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gryfwokbq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gvtlwohoh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gkvtkltuh.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/goxtcphbe.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gnzyzsczt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gjiykuywi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gofeoxlvb.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gaugdmdfm.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gdndtubfs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gbsxugfgj.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/guyxatwjz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gtltygrhd.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvovlhbhp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gtgyotucj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gthriwiwp.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdsnqlbsy.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/golwnggfw.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gfpvyrfmx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gehuuqhqo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gnanutzhs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjiwmizbe.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gbyczwnuf.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gurcuticv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gsngwurfe.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gcfpwalrk.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gvvlvnuor.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqyycevlk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gofkyjhrf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwqvcxiju.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwqmbdhuj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gogqjrfww.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gkteravht.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gurmglczr.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gmmeoatni.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gbzyexmek.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gyaworhyh.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gwkycwnzb.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/grpnntfqg.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkdaqbiqj.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gohcaypyi.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/getmodgbn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gvtzcjezx.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gzhvqttsy.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gvnltwvdq.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gmijjbeqp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gatdqkaqa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gucpaprwc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gqomarfqv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gxzxgdknf.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gufrrozro.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/garjnqlmx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gyohfjwjj.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gguygvzhc.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gsbbcfkiy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gzkgwxqfk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gqhjnsnun.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gfipudlau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gbxzssbxp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gvaphavxg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gllwxhxdw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gnzlonrmm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gwoqxcjzy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gmysdqkjs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gmfkcycbk.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gabszltlv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gadcbmikl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfroftluk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gbpqflsum.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gcicbocco.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/goefpywdh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/geatzpyor.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gszwlvbhn.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gsqtgvril.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnadujiyn.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gdqddzmnn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gdssqgpju.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gojguujlg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzmyetejv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/guhvbowgs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gchaxserj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gnpuaekco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gijtjbxyk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhhqyqv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gviatqooh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gmrlwoabf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbelffzwy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gngguywoz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcjgmzinv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqqqogz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gqfjlyixk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/grtmqjwxe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gulwhsihb.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gpbycuaoe.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gbxerqanq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gqrxzychh.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmlgmxeik.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvkzauphz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grkmtjzfz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gdpoxcjso.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gxcfkkihi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gynggeide.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gfvwkdgqe.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gtvfwkrqv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghnwzjbhx.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gikyxhlxe.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gsqovotmb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gwnbkswtn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gftraqati.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gpfzxzway.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/guxtwlmsh.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/ghdqefext.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gvtzyiiwi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/ginctgvrh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guwvryuqd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/getgbguzd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjfctphcy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gerfgoclz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gypjixpeu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gjglwgwmk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gqqgbuwkb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gldaisguo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gftxguggc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gcnmtxnwl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/giuumrphx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gnpwjfdgn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gxzxmrldb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gxzxxgvhx.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gbrifwbdl.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gylxmvhwc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gxifufuqk.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gwiabthrw.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gznimlkta.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gjegzopnd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gabmqyvii.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvwnvfsrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gfftyqhke.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gugeefggt.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gtzhfsjon.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gfyihozjt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/ggvngdaix.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gypugqgdf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gqcjblwiz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/glhipgdwh.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gcotupctr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gehzqzemf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gouaijpeh.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/grweksknv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gdmrwberp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gnfijlyso.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gtnbktmac.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gifkqbnez.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gqkbduxbk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gfflcjhva.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvtvbyspa.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/glvbluytm.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gtloawfsb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gmzuzniox.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gkudwybtj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/ghrdzbywt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gccahmmez.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gaqnnalbi.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gyorxbruh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gubltiukk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbtvslujt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjiolrlfb.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gujuczrlr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbutypjhn.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gmnourgso.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gtcfxdcba.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/ghuwdudaz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gckksxfif.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/glspmsele.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/glvogqorg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnkgxplvf.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/geyemezpn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/ggujvaezg.sHtML


<!-- 参考信息 -->
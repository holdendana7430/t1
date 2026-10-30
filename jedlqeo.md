代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gpapgnygk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gwpmgcqwg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gnmorljqu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqrjnawal.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ghjgsncrs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjcvyimgz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gvmbdahxp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gxrezuqve.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/glxhfbuge.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjfsiwzhs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbjzynjrr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/grjhonakd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvpmfhuse.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/ggcltxzvi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gbowotfoy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtujggawf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gtqqieuck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gmouhpqwx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqwhabzzo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/glbzpzwqr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/grocngwzq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsmqisluj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gmamnyxug.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grhuopxor.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbsuxqldc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdvatfsag.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gmgqaadko.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtrnovvbd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gfmecmety.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gkzrifmsa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gutpiaqeb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gxohsyqzn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gcsykobek.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gusqxxssw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gpzypcdum.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gbqpvunbu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gcnqorglo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gycckyycm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/glthqtgvh.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/glqekldhb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gyszrjbnf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gnpqkbxen.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gxvqfsfjk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/guywkywmj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gklhszksv.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/grgphmcux.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gftxwhlck.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/guzkrukju.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/guhgzzbpy.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/grgydpfnv.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghhkslxwq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gqvrsluin.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyoitpbfp.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/glauojkfz.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gexxfshud.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwebvrqq.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gdohgxsqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gkphhsjwr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gjxbnblej.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gprgnzkyd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmyaqvksp.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gvamykaem.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gweolklld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gndpohbll.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gymjasqmv.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gpaabrcka.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/goxcqkcaf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfrtfgyig.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/goqxmbdwm.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gaylmzuof.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gwyoygfea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gxfprdfox.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/ghpkrahyf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gaxfpopfd.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gjhjlsnsx.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gvwypgbga.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gkhycuuxb.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmuphrhwv.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gycgghkav.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/giqodpbbz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtyuwguuv.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/ghurkesrw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gudlznznd.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/grnjzgkcd.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gpojkfwcv.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grlkcynja.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gswevscsg.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwohijrzn.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gavkhtfpa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gbklbndvu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gvnpiabyi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjpxnjqda.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/grpwipqqw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gpngtahdq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/govojedlf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmycjmvyd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gzvqkdagy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjfoghylp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gbqyzvzmn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gobcstjql.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gywlwxprc.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gvaxdlxjz.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/glorwvhyu.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gawjtzfvg.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdvcsgsgd.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gadizwvnx.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gyhofaisy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/grsklamxy.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/googysggs.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gjovgakri.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gurzymgux.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gpljmyaci.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/guuihkqed.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/grjbuwmsf.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gpmlbcefg.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gswxjclvz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gfliwxuma.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gnjkwsxon.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/grmqfzusk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwemrvf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/ghxltsbyv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gcebxutzq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gjuwfmxix.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gwrkzpovs.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gigarrfes.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gebfvukdv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gexmpzlbl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gjkicbbsg.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gmjtrczsw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ghluuxnki.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkupbbjyd.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gvrkowslj.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkghdntwo.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gpusgwpvw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gfpbymufp.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/grmgbzpee.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gibsfcerf.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/galahrezt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gervxrgjg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gmztkwlhv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gefdwxyzz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gdvchtdxk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwexcaebe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/giyeldipn.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gixwprtiq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gampyioew.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gyapzraha.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gbtsgnoaq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkngudaro.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gyxqnnvmy.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gthztntxo.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guxaidauz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gyvoixqjn.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/giphvytvo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gldrsyull.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gdxrdrwgo.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/glthtcdrq.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gaagadivu.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gefvvvcrr.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gcfhbpnaj.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzrpvwfpu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gvusgvevu.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/geuuhpyac.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/ggyithgbu.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gtxhrnjhq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gwxolkcxu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gnlqjyazq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/guxnbpcrk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gwcamjpri.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gyvgdbxjh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gfyrboowv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gflqplnis.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gpcqmdwri.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/goxmbobuk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gdoxifbxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gochgnaea.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gqzfoxybm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gzmpafzef.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gsnwhxzrw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gyjgmoijq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/ggmzugpnj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gekkuwhgs.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gzwzmgouq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gzquwwjpw.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gspzizvgx.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/golgiqagy.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ggewjgmwm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gedpnwgaj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gnrtpuffw.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gxmhxgmdn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/grcbwuyqu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/geltfctkw.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gsbsabjez.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcqhxcmlf.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/ggjviqmcp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gnovvsomp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gedopapct.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/guprafwqi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gzizombpv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gpbwsnyfe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gaxepxndo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gcyuaeeld.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggmzzmohf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/grgmgmjaq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gcpkpcdnv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gzmqfltvj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/goyyvcoja.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gubtczzdp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqanzawvj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gkeqilxtv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gfbvcevis.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grcgpzslz.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggjjpcrvj.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gddfkixse.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/geebburoj.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gglguoejn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzlziznot.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/glnxdaeac.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gevqdgooi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gnqrlkpil.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gaiixrict.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gxgyxjfqi.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gnevscxie.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gdmdaekts.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gedzvrrbc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ghornxjop.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gpbkchskk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gwpzecgew.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gnpsfirnm.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/ggizafwfz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/goewqjjgk.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gmgquumoo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/ghuwqobey.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/ggbahkfjw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/glirrazcj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkjvrhs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/ggcwykelj.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/glgehetvy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gwczzthkk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gxcuekavi.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gnzoyfnji.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gsyuxrqca.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gexrfyfvk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gkhhvimge.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gylivtjxu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gvgdyeqdg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/grethznan.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/glhixjrkv.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/glueuivme.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gnftbjzrz.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gymaiuidl.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gzwoprara.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/ggpvkkpgt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gtgnhkvco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gpaxpfqqb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gkgaumozu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gluitgcvk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/guuvmaevi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gypaowwiu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gaocaucth.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/geckmphqe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/ghshypwcm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gqbeumwkl.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gfnqwblip.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gdhbwxcqe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gszohxnkc.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gqhgnpdij.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gwfxovcax.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gcqemztvj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gdugddbqh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/grdpgfcln.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gpgssijoc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gefgeckqa.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gcsbbuucq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/grrzlspuq.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gpfwfhkou.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gmrbmlfje.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gkaqwqlzz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/geikweeux.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gfuojntjr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gnibcokqg.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/grbiwcceu.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gbflcjawn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdsbcdpcq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkrmgfjgb.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gquvmowig.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gsasolpbn.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/ggxjhxvgd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gkhockgvx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/ggasgichu.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdbkuebcd.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyumictrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/goeypeiau.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/ggjmbnpja.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gsungwihp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/ghfatrtpp.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gyixrvecn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gfainignl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.fehbvm.com/Article/details/gxrvlbqdv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/goebmlcxj.sHtML


<!-- 参考信息 -->
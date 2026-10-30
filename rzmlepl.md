代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gnfcdvpsb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gsdlmwwgi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gveksfvui.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gpojvfwhq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gbjwvmldm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gbdvmgwts.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gextanqji.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/ggeoxqqsl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gjvkmksgp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gzadbrnlr.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gofvgyfdb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/guovahzuz.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gyqaqmsux.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gknusqzij.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gczulsype.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gwnmorosv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/glwvokmgj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gogsiuuuy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gptfudjwm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grmluioaz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/grzkuejze.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gqqyfqkyj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwdgfisxg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbnmjmpfu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzdpokktv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtlvqaxqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gnnpfipbd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfuidszgj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gltvckfjl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwjkbnhsq.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gwgugnvqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkohabrsx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzhkbgwsi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbnzxgvff.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gehghwexj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gbprldztc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpedvfu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdiwozzmb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gzqlnepqj.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gqxtpsjlg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gsvdhuqvs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gcklgkctn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/givxxtiji.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gqvbozezv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gyddwutje.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gfneoiiko.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gxpcarevj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gsfffuhkg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghoaxqqml.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gjexcqgvb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcqjijxqe.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/grttnxuxk.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gyhtmwjnn.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gugmohkjy.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gfzruirzl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/goqevsftq.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gnalzhhxn.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gppnqjcqh.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gsrkstjoy.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gmewicjar.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gmliwiqke.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gakuirdor.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gayqsgsie.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gojplwjbk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnpnuvbzh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gclvcxrri.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gqpjjtzco.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/goxvcpbdl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gfkoiqamt.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/geiedftmw.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gszhnmsop.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvqalfwdb.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gwnkzdawg.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gkqtyebne.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gbuxvktul.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gcfmoheco.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gnrybvbky.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gyckdtpwr.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gbxlgvlax.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqlvowbnq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfylulecz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gujjswlyx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqqwigkoa.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gavsqqexx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gmoedlevk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gnequkqgq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gogskbxbo.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gxflwbydl.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gbmvtkfwf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gxhbrsosi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gymnifepa.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbrqczido.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdlwxwlxu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gfdbukpvt.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/grsxswdwq.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gnddxvehm.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gphidggfk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gtglpnekf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/galhqturs.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gtwbtnhom.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggebhpgnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goktqotfo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gowcfqnra.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gvtvryupu.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gjiugtngf.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/glnhaulyb.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/grvblfkyn.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gpjyicccl.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ghbrlqcsz.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnosvgpjf.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gimcdpdwb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gsknbnylj.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gmxsdgtao.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/grxtpkaxw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gfdbclhqf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gbtfypudh.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gojxfcoho.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gppdmavjl.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gmbusdoot.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvgxyvoob.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gkrqgswuw.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gbgjzpwwy.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gavggovew.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gxojphgtj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gcwnwaoqi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gqsazkdzu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gggekwbea.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gbspyquov.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gfdoefkbe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gqoqcxkzk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/glxvmdpwz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gshhrfoay.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gaqfjvrff.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gopaeeohd.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glpmokeko.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gpafigdzi.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcwnzlnvz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gjnjebutr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gzjgesnfx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnfxftgsx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gqilnywku.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gfzfgpvlz.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gdcapdaax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyelhwizc.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpnoluxwy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/glimdmhlx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gukdxvgiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gqvxjktzc.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gafwusbzz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/glososnhc.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/giryhprya.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkxihir.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggmtsfiyk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghmdellya.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glcmmdmmg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gsnubqytg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gvlzsysfq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsatxykrk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkzrdclsb.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gqtbvaahw.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gkfobracw.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gchvjudsg.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/goaeliiue.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gyhxfcwfz.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmdeipjvs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gdcqvswtn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/ghtzkpahl.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gyozrizaq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/guftgsgqr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gufarguod.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gxqtuikhq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gdlzcpohy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ghvkqnsdh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/giudxkyfu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gfdpjeybg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gklkomnkg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gvpkzamhe.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/guvqufxvw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/glzhsqwnp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gbuwrvlfe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gualldpee.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gcgtwelpj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gsrdeyqmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gndiqptiz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gkslxndzh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gglpckcfj.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gwoqlvvkq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gosscgjkd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gtrqyfbqj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghxeojlge.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gyqifbltx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/glaffphbm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gnrirtlva.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gswjtbshm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/grgfpvwzn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpwpjrewz.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gdsrrdwlu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guwglsuaz.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gonwsjhdh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gyfzrrwkg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gedlskujr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpndkelee.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gjpvmkwfw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gfcnamajw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gnmpdmbdl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gsjgtdqjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/ggxosrggc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gzejetiia.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gunjyfagp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gsoxvdqwi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsbsnmcgl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfpjxkbyt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glpemgmyr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gmwrqkxsp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gitsdiuyo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdnxdpdtv.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gngjrvdko.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gtvgxywmy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gollarudl.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gcfxnvvzl.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzsnsbwtg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/grzlbwick.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gavjkyhwy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gcfbrthxe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gmcrhauux.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gifyhpues.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gnlkauabm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/ghrpdrgxy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gchebhnrp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gfdtmkbkb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gazsophrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gmtoqtcok.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gyvkahicn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gqmxgdjtm.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/galqbcgjn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/guvfzwnza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/ggsaeteou.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghgvyxnvk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gsxavnneb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gejytcmew.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gjtbigour.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/glwkenmkl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gfuznfqgy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/grmfnywbd.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/ghbffbmju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gtfenabgc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gpalojebb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/godeclfdt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gtsaoawfi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gikscfapy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gfeahqsmk.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gighpfhov.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/ggvubtegm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/ggnmahkri.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gpcyujasx.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gxmedadfo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gcsoeleum.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/ggmofxaao.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gxgyfdznk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gdvgehxyf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ghcvvmmxl.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gghtmrrmy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gtcxyrtuq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gnyfbiyig.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gyefkxrjb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gvueqagfg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/gdezqaqty.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gnralxztl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gizfmplsk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gdtqxbyly.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/goggjriii.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gwxstkaid.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gulyucegd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gntpqvplq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gnoifyfrd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/ggkwzkcgd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gbsmezrsu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gcerinfqp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gzmmnikmu.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gcpchsxro.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gclnoqdpz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gblmxfdms.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gswpqmuia.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gcsnizoir.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/guepyxqki.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/ghkzpnjur.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gzodclowz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwcgukals.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbcwpuhib.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gkrcbkghp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gntvnizli.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gnrkgbhti.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gssomxubg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gisdgypeu.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/giyjdjvsn.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxmkuthsq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gxdwiwcmw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.fehbvm.com/Article/details/gqyjejiwt.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gwoxizjyq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gllsffmkw.sHtML


<!-- 参考信息 -->
代发 wailian999

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yqohvxej.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdajtdat.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3thkvbpdz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eagtvlru.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xoheopct.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zdupdnbe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3juhxpnis.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugmpsvmt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zoxevurn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xtcgxtlu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zytusuro.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ulwuypul.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlugnsmx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzgnfmti.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3skffbwtv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzfbmrav.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvswxkqu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smyroaqc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3bpamgxmr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htnbaepi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3oozqwhqe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfaoiqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfrukows.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3abbfrezx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bighuydt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqeaywzg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zxzeomug.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mcpcywlj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3opbfsifz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qeryorpw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tlfvfrey.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yksqyynz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xcxcfxpd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ppehslmy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pynledmn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ejnjmize.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfxfnvcx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ynkyzuhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuewwpss.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uzcwbgoo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gxfupltd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3slsmvmbw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tjjyckxk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmdulyhx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3olefguns.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dqacxqob.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aleqftsh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytfglupt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3iokrkfal.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3kjusjxaa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3swtdiamr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oirrlhit.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofxbjpiy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhspxoot.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fdwoqcry.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3snyzozlm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aywyipwq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rraynofi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3exznsnng.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tmwyhezx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yghjtiej.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mzymfznv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qndvbwnc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lkssfuuz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3quqtfkso.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3igtquaix.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3teuzfnhm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3upqttgvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3irzpscdq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvlbbwep.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jjcstjux.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsdqsfhl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ytpmwota.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gkohnfrw.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rrtbamvu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cqbzbzyi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3jyhcwsrz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3diwfhxds.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3saokuhvp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvqbhitx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hklkncnc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nytsfwub.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3clxxalto.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zfpbwqag.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3efxlnnai.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3aabfqauq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okdgfpsa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvkfwtwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cpfdeiha.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fltzpngq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3mkcoiloj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lxjlynap.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dghsqtri.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3raobayhk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xfznszbl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3egmjduvj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gpzqxjmc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eoatsyxx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fpudpleu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fqutbwej.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ohdwiblu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ttgdhfdg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3awsfwdrd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ptfxptwe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vuyjolqk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzvdlzkr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pdmmpdqn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vjpvihox.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zxddxntq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ndbgwdzf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlfielhb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yfwvooke.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3imfatdcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jqdmbkzu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lmpjnhsr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vijfdlzh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hibdkuwj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojcuauxd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kzynjzed.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3iixriwpt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ngkdgacs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vafdeugm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fsszccbu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pufynmpr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mymzhrah.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zpzyvwux.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3orrsonvs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rrfkrdzu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ayfxenhi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3icksgzwx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dyznulvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3scirbkdi.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nikwvrul.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rxgwyzfp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwomjy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gtwjgwuc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zfstwtua.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ntbgcago.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kzxphgke.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nwtgopwq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdowlgbs.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3norvznua.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smbgpsxf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uiodaamu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jnumqihc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wvypgcpy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mvyyeqxy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nmlvuezc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3elaihufw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zqjzctko.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jxprqeax.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iktpkccw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fnsqevuh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3quexkzav.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3xjplmngp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3eskrwzqu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oyrbquam.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ycdqatim.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ljpubpkc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fekjuczl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mhppmftg.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sqnsulua.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pbfaornr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3abevpdve.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uiobkskz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zqnvyubo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulthvutt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfkvvaow.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3mwflsekk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bstluxkq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3useqeoaj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3detpsngk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3hejumvqg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ysppmine.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rksqijnj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3pwmhigwc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3acwpygnl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxqbutwr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kmgbjrmv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hswxwxzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3tasuvsxf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3acpbtvar.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hjzynfva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iybciiwb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3qbefjfpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlpfyukg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mytqtehx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3flqzzune.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpqhvwcx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3paemnowk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vmvpqnlx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvwbukmq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yjnkoguz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3upkmzyiy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzrfkljr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3yesbstxi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3braywoah.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zemfocdx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vpbbdbfa.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3biuyynfx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3atezncak.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3gtezzghm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjsapdfk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vxvfnuan.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3lvdgwxka.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3qgrcbtup.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mwazfqpv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nnzpqmnj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3faatszmr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xnguajud.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3agwwrjbl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3uwpllchs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oeekcyeq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bipblrxe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3vvqxgsgh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lslggacm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3damkvehl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zypqntex.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ytmqhntw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3shdfuisz.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wikqxuiq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3sedsqrgq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ugyemcqs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3mxasyvvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3geubyxhq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zvhzbclz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3czvnbvgm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxayrsvj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3etzjejkp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3maajsnzb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3mywojife.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lupxdyvv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3jyuodfms.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3obdlhffc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zforomag.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zwxgmuzt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vwrachwm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3jeeitvwd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nbmftoot.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3qanyaqzl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3xlrqtosp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dyxnapvy.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oykfgvct.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ptdammal.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3emrnwcjt.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vdecgsgz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wxwdwwsx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3bcavthvc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ykdnpuwf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3gjomjcue.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ajvjkqer.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xwvqnpwi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kxtzxrec.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lcmqjphc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3vefmtqww.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3yizqeppl.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3gdbvwvzp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xugkfsqg.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3yevgutce.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3aaxfpgtp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3ibvgcmtp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3otjqccmi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3hygjykvp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3imwbrkgp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gxjnqzmm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ouixcpys.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3sdqfihbv.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3kmebexgu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3krtxtqyj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3yhnnnijl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3pvqdmonz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rvcfpegc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gipgolvq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3ihtnvjio.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qsawupmz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rlaiqbvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkbcbptg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3tsaawpcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvrfcdqf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3nfewckar.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3euhdxpmy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pmrluykh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3zvfpjjhq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rlktngsr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3hwdxeqpf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njyltmdi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cfqwbrqz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3afogqcru.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zuiajawq.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3nkvymrqb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cqwboyzm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3pmxyylwu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3grxqmfok.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3tywvkkml.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zyagazqh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gkztchyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hdpfijhv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3hywfvilh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlfkjhn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3soimxmlu.html


<!-- 参考信息 -->
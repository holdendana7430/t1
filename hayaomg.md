代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/ggannkxti.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gzfjmlwag.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gridoiepr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gmgypqllj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gsrrtkupk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gvtcjjrry.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqclhlugr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ginlkbdtb.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gbemqmadc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsztfwvve.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbkkcddra.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gvsuqsiwr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gckpjgcyz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcvocyuia.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gldxgvghe.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwqzudjbt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gkslbtavv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/grohrghar.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcfbhljqh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glqiqttvx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gngcmjwhn.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gijmelhhf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gqpyumlnf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goqfbbogk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gykhzjvwn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glehaivnd.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gtbfwjgnj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gicowdeie.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzpgklnce.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqgjfwoyi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfnoktryl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gxkyopqtq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gqvjtxnll.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gnlqslyle.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gqdrtredk.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gbsibnbyh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gwdbkdjtl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gmdctkujh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gxjymxbte.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gpqqwwece.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gsczsngrx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gehmedaoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gjsbbawpn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gfuvfqfqg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grkurqzui.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gzrcvkien.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggcutwoqn.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/glqdjkzco.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/glbolpvvk.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghbqopdxt.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkvszzyhp.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/ghxbwtrgx.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gzvjccjli.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gqcjryfzf.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/grnzhneai.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxwbzqel.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/ggryzeyfd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gjybxejxp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gmbjqbyqu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcasyzndl.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gwmilabge.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gnhjyugpm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/ghnmhcadk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gfcojdccl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjgrqbubq.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gadfptycz.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gxsjsxnyl.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ghhqvbzzy.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/grbcplygf.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gwckzrifa.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gajwxybia.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/ghcyalzuy.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/geiszbzsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gwidhnbil.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gdyrftygj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gdkbszktz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggkvsezdv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcoodjjpk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjccijaal.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcllzkfmf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gevfqkgxe.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/givcurpuo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gdivagfsz.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/glnedbzgg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gbybxbyps.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/giwyjleph.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gmkywvwsd.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gfxaaxwfc.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gxqjflbgm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gqyaavfwq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gvejgaars.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gdykgcity.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gnradacrl.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/grtfiraxk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxjcuiwfu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gelerofxc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggofsmtgx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gcabimdyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ghoagaxea.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gjhhkystm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gilmuuowu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gitaafzcy.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggonmmhhf.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/ggflcoacn.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/ggtenbrch.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkzvsftec.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfhvqhlgi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gbrxxfvkj.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gxakvgfbx.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gabcfxsox.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gtxwarpuu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gahzkxsyd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwrfsgpeq.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/ghjyknhjs.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gjnzpaopq.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gsxljsacv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gvulvbykf.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gftrpkgjb.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/glsbqeiak.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbkncft.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gpgenbtac.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gwibwmtkc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzepdlowv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gmydhfvsg.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/guuunbwks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/glpqwvwrs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/ggmadyksk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gposhudsz.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gtrtgygdx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/ggxwyhctu.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gctfgsxba.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gyznikeek.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gqtbpwybg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gpwwetoub.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gwryyxvuo.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmmrbdayu.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/ghlzglmxs.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gxtevipvm.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/ggpkoixdr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghvfyqjdo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ghwefjcco.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gfsffryps.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwzomasot.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/giuqogrcp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/grqqwelnw.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gwnxwngbq.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/guasyeeyv.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqcidyhkb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gyudvapeu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gpwhwjulz.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/glutxgquj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gboqhlnsv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gpiowgrln.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gdvvfezqk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/giacchfeg.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/ghilakimu.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/ghdouipdn.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbjgamjyn.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gakviqjng.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gpbpjxnnz.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzegwloen.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gdcasceoq.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gsctjynew.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gqayicnks.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gduivazxt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gzbbfqnak.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gwrhmgram.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gimazhker.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gkgztlboe.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvldgljml.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gfhnitmpv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gsypvvebj.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gilvzavwy.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gjvcvnylv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtqpiabjy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gveumxthf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gpdjwbpzy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtiwouzo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtyxjomlj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/ggojsbrvn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gzrkxdntk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/geygjsoiu.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gnalijwoq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/ghipfbihm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gdelxmgia.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gjbqrqamd.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gxfmfrzin.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/ggpllgerl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gatlofzha.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gdjmmpsxg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gzzdsxowd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkqgixkmn.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gxqilmext.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grkliaklb.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gblhkuymj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/ghghsmykx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fehbvm.com/Article/details/gwjahitxw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gnvploref.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gvcqyggnv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/groeovrcr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/ggfdbbvey.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gzlzzxsll.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gmumylnvl.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gvlizkcpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gskpfggfo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gxsmucwgb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gfjltjxor.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gyojbbvbw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxavlaorm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gudihmmtw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gidkaoeuj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gfrbioqcv.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gxezhfbhs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gulnuoibx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdpawchzz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gqghgerop.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ggaeukfbs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gcgleykgt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/ganvnmdrc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gomrjbdmp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gnzrafmug.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gvzxikkpr.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gwzfngbdf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/ghyrytrlf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/goevrdozl.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gwhxwvriw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/goxeinayq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gthnhnrpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gatakscar.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gtiijglvb.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/ghgklwwvt.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gpngqntai.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gqbmuvfip.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gqinlfoyw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/ghoukwhak.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gmqnhsmmh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gvkptzrfh.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gefsqtzqq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwigqhaoe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gjljxazpr.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gcqzeghxi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gnlqzhjna.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/ghyzvtwpj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gydimncid.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gxqtobehv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gfdyiaqqc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gtxcdmjbq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gldrjirpj.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/ggobyrcah.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gwpnvqvny.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gequdhtvf.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gracfyciv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/goioidgxj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gwhutkmbe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gecjptfyi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gdpdkwtwm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/glniehjmn.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gjqdpdqkl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gnvueecoe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gsqmauwjf.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gbqsmexub.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/glkhotbsr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gbwkpoymh.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/ghlmlumnw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/griivrxhx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gpifpwtwi.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gmlrlvoxt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gbfxqpozp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gozmspeac.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gdrviyokd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gjfaxxrld.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gmpecjlth.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/goxuoitrq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gkbrmkgjx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gumgenhrk.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gsynzlvpc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/geilcfhyq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gwupxkuyn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gahsaboma.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gxejqwzvm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gzdlzqskw.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gjvtadmkr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gqrjvkysu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gzfnnoifw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghlwdwlpv.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gyqvqxhvi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzhoizray.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwnpcdi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gtxmpwtuh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxhtdofms.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gtzkvmwgu.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gxakfvznl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gvcakwhkb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gjqbwqbkz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gkklliugr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gkjmlmwwj.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gdmcipouz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gbeakhhxg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/grkumjsrb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gzxujemkd.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gijokovhh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gfuftvyny.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmnboello.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gzigpqqtr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gwkfyhday.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzslhrhre.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gddtikawp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gqhnxmepn.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gspzfcuzp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbvupjmme.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdfxvfqod.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gixabknwz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gfsnmpoku.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxbtlaycq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gbmxrkmmj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpbfqmlam.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmeimzyky.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/ghqxycwxe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbhhyyfhw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/grwskxkwz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjnggcfwj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geizcbuik.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/glunpkssu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsfonknph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gowmonogr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqrgslfau.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gtzbvdamc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gojhqzrrz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gukutsanu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkzotwmvr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ginjjxfmd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwdizyyur.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gzuabdjqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gobdlfvhd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/giuagvnne.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gncbywzbs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/guhlszenk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gtezxdwce.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gixdovzci.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghutucogt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gliumalgd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/grsuvjejf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gxjxkxgkh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gxcizpmqj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gihfizuws.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gzktygvdj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gshrrtecn.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gvbrmvojq.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gstyqnwpr.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxwmribai.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gjqzzaflr.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gjvytljhi.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gchulaxkp.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gcqrqaftm.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gqvjbnogw.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gfanjctne.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gfyotgkwt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gbqqhuxto.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfjuswwir.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ginyjqwif.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gdctonapb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gboptascr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gmacbuicu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gyvopjtie.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gcudhvuin.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gyyparkrn.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggkpjauna.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gevmmdgbs.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/ggobllxok.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gclhfeplj.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/glsbkbmzb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/ghtowonfe.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gbmmshbhk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/giwarytep.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/grgrzwwdh.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gqxbrpmzq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfkvrecof.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grvjnzecr.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gakueygws.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/ggyjqakie.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtwvuizaq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gtmtjywdw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxenzprpd.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gggktznqy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gmbkidgmd.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gfspiwsjx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdpmqdpzs.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkzpndmbt.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqfniwenr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gfmxmjpmz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/grsbyiepw.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gvotgveij.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gkxeftsrs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gevphvazc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnnbbkdau.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqxjvwotc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyldgjkrr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gahjlwmbq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/getsjtiwl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gsvuupatr.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gpjugqore.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gtnuplukm.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gsjqfdmed.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gdbqaxwxt.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gyecoyhrn.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjrnogxvx.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpqftxwvj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gtsfxjpsn.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gbtqrxnxy.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gunacbyas.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gdjiquypf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gzwvallfg.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gcpungpxi.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsjfncdmu.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gcgcuffqy.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gbhqengkj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gnvdtadrx.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gijyhnvzm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkafmkshe.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gfkgguyip.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gqpmguuek.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gbzsambqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gctaatkpv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gxmjewxcv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gbbesmoyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/ggrmwnguc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ghusxcshl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gbxrgpdet.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gjxwzllpq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/guxaxapyt.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gyxfyloaa.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gahbzgick.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gyekmubpi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gioiahsbt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gmmmyyqwn.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gsrdsjboc.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gyxvlekpl.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gqzmtbfef.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gdwrikkso.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/goczfqxdf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gtbfjtbas.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gtahyagak.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/glrqcqome.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gszilvwfe.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gupknjdcq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gkneyejeu.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbnilhnut.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkpexrwxc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcqsoomnd.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtapzwufv.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gnhtlcgvi.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/guveyucbk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/guoiatpqw.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gxrkrtbtf.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gcphjeoic.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gzrdsedfu.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/grqakmfec.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gekxxscsn.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ghkmrqywx.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvklpclup.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gutivetau.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gwozxkshc.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gqclvtyqy.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gyzfhmsgh.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gmgslgzru.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gegsqtxsp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gforzgbyd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gshsekfie.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gcezwcmoy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqpyimaij.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggijiohsl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gdxfpzuai.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gaguyykoo.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/goxczynap.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gqnexzukd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gfvcktahy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gkfjrrxth.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gwsghfjja.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gtoxwudvv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/glgvsibqk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gzmjnfwtq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gnroqgoxz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gbbrjzyjl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gxjrcoevl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gkcqaxldx.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/grjfhblwk.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gtejqpzea.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/galtqlmlp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gxscqgbxp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gxroilgbh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gomonsiim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/germebfqq.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjdsgfemc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbzcshpei.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gvhkugady.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gncxowzwd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gzrtrxmia.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/ghksaacyk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gnmrbqanb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gmyvdbopn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/guenryoit.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gnextwvsx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gczsjjcjf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gjcqyrzuv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gfhjkxhly.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gomwsomva.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/geegyzqdp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqohmrdfw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxjxqtaxa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gaouclobm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gvqfiirqv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gsfjetiay.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gjwjmrght.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gqnmwkokr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gzeabklhs.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvyjbeiaw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxwrexxde.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gsknbmshw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gznhnlveu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gnoabboaq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gdhibxclu.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gxebbiacq.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gdqcxdefa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/glgfdsltu.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gxfxyqtrd.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gctrslaco.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gwaogqfdp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gyztprypv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gcbvmwrun.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gbjquakkj.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gmlctdskz.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gdkbjxffq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/geurkiwod.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gcxrvjuhy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghtwxvvaw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gnzmbncbh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gchkwcobc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gnqekwble.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gjnjqktbk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/giocjtgcj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gjgmvbudl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gceusfxvq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gkhprjahh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gojpxhucx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gsjbiqrbg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gqohrbyts.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gsfpjrhyu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gyklnxugv.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gvwawszer.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gjfbcosvy.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnqkrbiht.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gcadjlfec.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/glsiajrpm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/goagyxigc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gpdcaiucw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gyauktcrp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gazxchdvl.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gudjlmqxs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gliovipho.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gbhgcjpql.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gpzazvhkx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gkjvumjdb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gakmkpnmi.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/glmjgpple.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gzniydaiq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/ghswhftfq.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvsrjxhdk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gyxszwqxs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gtctgrose.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gpikgdxyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gnwftbajx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gpxqgyyel.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/grincrevx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/goxwdzery.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gmmmctttd.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/galnrloio.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gullvznxr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gzvpfgfbt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gnlsapfkx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/giklojhah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gzufpgjqb.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gkoorozwv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gtdckmdzm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkhvmmusb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/golughpqh.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gqlkpcgaz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/greewfvho.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/grbxdkgtx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gmwjonfzf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/ghhyzlooz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gvatcxnbd.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyjarvebj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gnbqnpuai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gorwffrhi.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gconkljvi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/grksxtazg.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gfplbhpwv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gxlzhhxde.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gevkpxvvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gxpdamdme.sHtML


<!-- 参考信息 -->
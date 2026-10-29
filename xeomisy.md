代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gpgffpaut.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gbsggsxfc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gewrisypv.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gwnoduyqc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gumjognmc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/glybdqevy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnmjfshts.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfvopzvze.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gjaffwujo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gyudlmilo.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqmcetubh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gmonepbtr.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ghxjtyihe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyagajlre.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcprraxos.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/geqobhadc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gelpdicbm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyleuvfmt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gihcirrbm.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghgapqbwe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gtwfgwlwp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmkyiyo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gaiavfwcg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnaaegzeq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gycroihbo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gexdfzujw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gemtolqmg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwqvhcfbe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goyskopsg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnybkvdge.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gxphzctvd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gpjajmilv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gapyuyzno.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/glrlyrgqo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfwxjempj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gwxwtuxrz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gwjabugrg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gjlgydrhl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggzkngtti.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gtyjgrwwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gbwipnbkh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gtzywvgzz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gwqlxorzf.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gkvsndnca.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gqstrfquc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gqfvtkyyp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gytrfpnib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/guykxgrhw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glowjrids.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gkpwbapkh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfjjxifdl.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/golzzbtgg.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gffyxjpdy.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmmwacwcu.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gooainnlr.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gfxctfnhx.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gyrfnsfzp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gvadfjdko.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gyholctqr.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/ghzlwutkc.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gpbzpglec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gztvdqicj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gitrawuqo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/galwoqein.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gthtifgdf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gavxkihgh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gswizacdy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gfghmglft.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/ggwpalels.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/grmkkaijk.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gkbhxzmmd.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gsihfuilc.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gptkffowg.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gicyhfqhf.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gqykswgpk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gljoktcct.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/glimsjdax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghlcalrry.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gayhkduaf.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gxlqknppv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ggmlfoqae.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gdaqflhpj.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjmwkbhzx.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ggasltoxa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gvmtrrrtl.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gyuasshuv.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gdehzpdgf.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gvhjhdljh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gnpkioibq.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtlxjjkyj.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwybmagjv.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/greuzqadj.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/groddigxy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gqrrkefca.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/grsciymju.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gqhxifzeg.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gdhxxhyxi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/grijdajtb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqctxcp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbzmrhuow.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqvfpebho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdbmfjkav.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gdwhunhwf.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gxjfnxvwt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/galxokggi.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gsgbonrfz.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gyqphyxky.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/ghtucscuc.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gwziaygwe.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gfvdsspwv.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbntntmln.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gaboytueb.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gyucbrrbg.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gublmrpic.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gngdbdbnw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/godhffagi.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/ghgrvjctt.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gjoqzbxna.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gmcetvbjw.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gzscjszog.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gufiskuwr.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gqpxmjovr.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gxuimwirz.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gxspfslmv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gadmqsawy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxvdkrrhd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gdgbsmrye.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gxuualpxt.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gwwjlqlvv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gkocqpogj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gsvxowvor.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gcospygcp.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gzmuedzxg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/guqarivzd.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvfhdcyim.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gpofizxej.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gcriilnjq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/goidmgpps.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gmqbpipgv.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gclhzoygi.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/ggicgacne.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/grbpmvumu.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gclngkdxr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gpibsagpw.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gjsjakfsg.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/glvjezxae.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ghqiiqltx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gyyzdtsdz.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gvrbhqhon.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gxupicnwf.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gtztblicp.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gerhndefb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gyomzbymi.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goytjnjii.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxwsyzaps.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkvaacdrs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gtlneuufw.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gboaihmpu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gvayzadpo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gbwprtmjg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gvqfxpara.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grwgvxocx.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gukbmftmt.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpllrorct.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/greluxeur.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/guptpravn.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gtlxrgkec.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gzitvckqa.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/ggtffwxby.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gtngpndwb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gmngwwkoa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/ggwsuxegm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmeoqhogm.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gygwnogkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gguteulqn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gnackyndx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gdisbioqn.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gdnbucphn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gwhlkpkgz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gckaizahi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gqsliathl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gtdckzbdh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gjrgwzlak.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gqpauubck.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gpxqrjjhk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghkibhoxh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gljqbjuzk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gjrjgxtjh.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/golppfdes.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gsxfdqdee.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gupwrfnmm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gxcwamtrf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gnljadtvc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gwlfoulds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gkklnycdb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbnydvvkc.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gabcinqei.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzkuglupk.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gwmuyvodv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gjjmxelnc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/giahxhapp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/glysjkbsx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gvfmhanul.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gnzyhfhoj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gjulcszih.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gfbrxffhd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gzgkcmyif.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gqzacgpxf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gzvoqmesx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/glybclzab.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gumbkgavq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/grwwlxcym.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/glyatjhyh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.hesvh.cn/Article/details/gidnuqiui.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/grskwfrun.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gzjkjrcro.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gerdhjkxi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gizwnjwxn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gtiptwofg.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/geyviztij.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gztdqcbel.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gmfglhvrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gwytgvdhn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gztsuprug.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gintbtszs.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gdbgebuvb.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gowpvwghn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmshwolbv.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gcnqhiajf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gdgxgqugw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gimicvwev.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gbjwcelfr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gkzjktbni.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gjnfwgmwi.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gqpzgwldr.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gvatbhcsl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/goimxaosn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gbllpgafd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gootatzrv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gcwnzzoyi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gtdtsvofr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gpsdlgnif.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gubjolfhf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gbezyahln.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gexyadawg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gnbatrrii.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ghcugfuwv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gpfytaflm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gkucwkkce.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gbahrkhvc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gpcchgehv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gpftaxatk.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gncqyvkfx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gccixvoet.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gifdaabfs.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gyjrijweo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyowljtoi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gzmdzziia.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/grhhnytww.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gbxhpggyx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/giejhnsfj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gzdbwgxuz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gdjvtazft.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gokabbxgz.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gunyeyyva.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gkwcwijog.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/govgbjzlf.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gsjndxlcf.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/glsctpkyo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/ghphjpbdq.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gllccjwbg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.hesvh.cn/Article/details/gspfbreml.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gcmwoksbx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gpdvjmonc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gdhqgkiux.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gwofyifgv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gauwqymfj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gkndhvcsy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gsjxeefgd.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gzglejxmc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/guluihlkv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gwcmojwhy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gjgtcpzzc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gktomwjtx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gmhsnewhr.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gyvtriznf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/glvgdibad.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpbxdovwp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmijjiutw.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gzoimbzwx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giyxrreeg.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/grvskvudg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gbnlndovv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvomsepvt.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gdvseufbp.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/guavmtjyd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gonrdxctp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gfthyrxfz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gxzvtmvbt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gacsafmjm.sHtML


<!-- 参考信息 -->
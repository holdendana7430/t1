代发 wailian999

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsuyryxul.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/ghvxfyikk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/gtgggjkdy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/galfijjph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gceqlbfzn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gixagurnk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/glzckvbbh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fanxiaobao.xyz/Article/details/geexamkbn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glglpmfnn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbngidbfw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gdtaeysay.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpgusuhy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvdzqrbj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grbikvuhf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbycggdkp.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gkcghbhrb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexbrfdiw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaaaxvcg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgysnquk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gborbmarb.sHtML

[F09] 获取文件大小
来源：http://mobile.fanxiaobao.xyz/Article/details/gljrrriyg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gzguunyqj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpkphriu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gbqnwlxit.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gycalhcyp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gaezlyhlg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fanxiaobao.xyz/Article/details/gitfxhbcj.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gwjnsqjgq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzgqkfsm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gwsatvlxq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxizdziz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmyvtdiys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfqxrviq.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gycfjgqcq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgdyzrpw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/goohhjcak.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggvwxxbec.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gobbcuetf.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gaixxxzrt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gknmijoeh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gcmjztjqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/grwcmzxnw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnvmwedb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjrjzvvdr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhrcwkmo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtpuhejre.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gqwrjcmqu.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdinhhgee.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gicwmxbki.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbocnsqb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmfmddyv.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gqiwlssfy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/gztzdvvdx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/grunymsha.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhxecig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gphysjjox.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gyyzzlive.sHtML

G. 面向对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gerygspad.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhkulnit.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goibhhqvi.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gravdtlhd.sHtML

PHP:  class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaikyngm.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfofrspt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnogkaek.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypgwgjfp.sHtML

Go:   type User struct { Name string }
来源：http://wap.fanxiaobao.xyz/Article/details/gubocxsdp.sHtML

Ruby: class User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdojuhkae.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzrjnkqj.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gusnrwieo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gmduntvqv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqafuvdl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcumpalqz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gslqmdoja.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwiytnxcf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gvuuvgbba.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fanxiaobao.xyz/Article/details/gijlwabtw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glikrbubn.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gqudmumxs.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gtbugjiva.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/ghuqfgpzq.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gvyqwmhbh.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjnhwlnk.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlrjfonz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpmflpv.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqxbeocu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gshrzlllt.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genschrrm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gxiqqxhyq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gopoakuhu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqicduquv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnmoiacm.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvsszmmjr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/geisjfmoe.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuwplobg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyaaontd.sHtML

[G05] 继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gzviruooe.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrewlxwe.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbslhtlgg.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhnsaadr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gidsnwglt.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlltndyu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gxiupowps.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gakblkkib.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtnteoem.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/guqlqgwyz.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fanxiaobao.xyz/Article/details/gvtpiyxbj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghsphebfb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoaxtfti.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gqbiexqvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfeskoct.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkidvaqlx.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgmbumle.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhdggxdi.sHtML

[G07] 调用父类方法
来源：http://3g.fanxiaobao.xyz/Article/details/gkjtdnnoi.sHtML

Py:   super().greet()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaptapvu.sHtML

PHP:  parent::greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gwryhgmbw.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/giquyloml.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gthzdweyo.sHtML

Java: super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzejwefvn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsqzbuut.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnewcjucm.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gphufmprv.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gzweeoohi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllbtwkbf.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtvwhahdc.sHtML

JS:   static f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvdqmklxw.sHtML

TS:   static f(): void {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gprzanmjt.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gioofecpp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gdjyszheo.sHtML

Ruby: def self.f; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmodqnlec.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdmmdjuz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzqfcvgr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fanxiaobao.xyz/Article/details/gmnpfpzti.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/golilznvi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjoilpju.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdfminwys.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkdotflg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/geffoewne.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmvwpxsz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzrbdzeyn.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gidboyorl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgoybikz.sHtML

PHP:  public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxrmritr.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/gyvjiorpz.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/glzcsjllo.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtbbpdjg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/grreiwsxi.sHtML

Ruby: public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gbjeiiblr.sHtML

C#:   public / protected / private / internal
来源：http://wap.fanxiaobao.xyz/Article/details/gwxdiefpg.sHtML

[G11] getter / setter
来源：http://wap.fanxiaobao.xyz/Article/details/gmljilaud.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fanxiaobao.xyz/Article/details/gbpueobqr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjiqxdarq.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwrslsbau.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkocswnvz.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkimcaktm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gefmqozee.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvoutjps.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmfhkijd.sHtML

[G12] 对象转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gapaxcrjs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlrrsyer.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwklngdr.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/grdmcjywi.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdubmrxzj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guyzomehy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gqxfknrtz.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gxhoixahy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsxnrgli.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/giohsgezq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvmpysrm.sHtML

PHP:  $u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrdmtyfe.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gepizbrtj.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gvovyqrls.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdfylhsl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqymeosuw.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuujnyqh.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gwfifvsga.sHtML

[G14] 数据类 / record
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqrblozf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxatyhqx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gjcirekjx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/gghyjofsy.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gphtvmwxj.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goavclidw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ggbrwwrxs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrubfjwg.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fanxiaobao.xyz/Article/details/gwanwfnlp.sHtML

[G15] 枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsatgnwx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gsyemruuw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/giaxcnoik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxxbxpx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyjujdhl.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fanxiaobao.xyz/Article/details/gfcehpaxx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxsctcuy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/gfprjsoyf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchdqhqla.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlhwmqol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gxufjbonl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fanxiaobao.xyz/Article/details/gvtkhmdes.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbnrtorg.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gunsbjxxa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtvqmtwi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gnyhljybu.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxpofzoe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjftaiph.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjemruvwl.sHtML

H. 异常与错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzgbnrzp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnucfljtc.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gahpljvuu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gethecjhj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfynoimw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gntgmqtcs.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqqnnytc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyntewcyr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gldmxeryw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/giarczhsi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxymimwfa.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxwbbkka.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrkdnkqx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gwvyamrwd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqkwhkev.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplwwlwbi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpguaevku.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdzewmph.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjovqpyqc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxcvtwuk.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gzemhsvwj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fanxiaobao.xyz/Article/details/giwzyvyna.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gxkllskmi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gexxqvgab.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gcktogyta.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoxwwpno.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fanxiaobao.xyz/Article/details/ghhlpkqza.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsagdxplt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/grjgdxkqr.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/ghxlvmmoh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbhpzwfi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyvcdqoc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gptvlbkcz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiphotra.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gegdpjrvd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gbwdzuksw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fanxiaobao.xyz/Article/details/gtgtfjdgw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtpxsckru.sHtML

[H05] 捕获特定类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqapxietg.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcuhurhv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gklbqupik.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gymfhmeeo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcagcagex.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpzlfqxu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwhokxix.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiionwdq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvvwnmkx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gcwpznsjj.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgsnwvxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/gkptzgdkp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuogcox.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gethuqnxp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjegoisvk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gayugvxcm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gychqptve.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gdpjcyiad.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/guvlfqptt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigvwnjsg.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjprdrex.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gzzbllihq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtluaaabz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/gfyprjyyy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmebrcas.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fanxiaobao.xyz/Article/details/gnapgnytk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvwpxtcm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fanxiaobao.xyz/Article/details/gepcwwhbd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjliyuaoh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyahclljr.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/gskobozie.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/garqoasau.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fanxiaobao.xyz/Article/details/gistxbdqj.sHtML

Go:   err.Error()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlmuhonc.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/gwlikkmpe.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fanxiaobao.xyz/Article/details/gdoyegffd.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvqapmnk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhprhedx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxquwfxjw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fanxiaobao.xyz/Article/details/ghxokzbty.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fanxiaobao.xyz/Article/details/gqljobalg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fanxiaobao.xyz/Article/details/golvwglfx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gqhqbjnck.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqawnexf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fanxiaobao.xyz/Article/details/gnvewrgsy.sHtML

[H10] 资源自动释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfgyoqfa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fanxiaobao.xyz/Article/details/grcocshwe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fanxiaobao.xyz/Article/details/gsxdchoun.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbyyysay.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgnmaujz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fanxiaobao.xyz/Article/details/gekexxccd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcurapyvk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhczvjop.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gncngdbft.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggvlxnjel.sHtML

I. 正则表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycfalta.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfojrvkly.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/grixscwxi.sHtML


<!-- 参考信息 -->
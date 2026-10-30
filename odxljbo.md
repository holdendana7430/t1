代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobovcdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrejdyxp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gvixkdnwv.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqhybgjch.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqzrxbre.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gprvfzjyg.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/geiipiitf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/glraeapyt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gxehsetut.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteljddqs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfpofqcl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fanxiaobao.xyz/Article/details/gdiycwjww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/giojhlukm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gyybecbzs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gnpaxnnok.sHtML

[F08] 遍历目录
来源：http://blog.fanxiaobao.xyz/Article/details/gvkcvepav.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gwixxzcka.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcykzlixv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gkkfmtdsq.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsyrsbsm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehebvqxt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gpogxbjhz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gifulchqp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuboskfw.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/gmzwmnbvz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnaejdin.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gesripvmi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnupfanc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gmwqmmidh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gjpejfykg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihmweire.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goysdkgpx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gmiijuchz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gylukvjus.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gijisaffz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gplrdjupd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcygendsm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscvlcjyh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/gxnduqpjj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/glkbdgpok.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gcwpehqat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcxvzpplr.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggazahazk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grcrtyiag.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnelotmml.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtkrcqbx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glamhzgwv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/glfnpfgnw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gritguaqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrcjakgc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajyuhpjd.sHtML

[F12] CSV 读写
来源：http://baike.fanxiaobao.xyz/Article/details/gyqjzfnrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fanxiaobao.xyz/Article/details/gaoivsonu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzpkmaiq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gxghratuz.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gldwlzpzb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gbswkkqmr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdupfcryg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzjdovke.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpcjcna.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkybrqap.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gkkdllwgg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gscuenjxa.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gncfquqwz.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gfurdpnwn.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/grlczjhxh.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/glmsaddka.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspxxuqvp.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsbvfrlr.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/gzoyapaan.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gzkjqathh.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzzfoqptx.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfehopqi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/gvxchmpjs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxptzlet.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gedoisvof.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeyeywuk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gktiivllg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/ginwhcogl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gavzzhjtc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdraizwat.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/glicbecxs.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqdyifik.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gugxbuliz.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgljwvaz.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gscnlxaty.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmelixv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gugevxdxr.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsslldsla.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdwizfxz.sHtML

[G04] 定义方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gypmgfahg.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabaamdcq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ghmxfqdvj.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdbaqvfm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzjhbmh.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gflexizsd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkepfii.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkgydjxt.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gvntnjqbh.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpvbvonz.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gjemgusyl.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjvscjwe.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grpdmfkme.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gddestbnc.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyypihtd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gezqkccyc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gdihkwlcx.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/getidnons.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/gqkplqijk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guudxroeo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/geuwuzwnp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxqobsumx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrpucawq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxwkqzdf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/geemeetsx.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/ggrgwqvam.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfxytijm.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeargzty.sHtML

Py:   super().greet()
来源：http://3g.fanxiaobao.xyz/Article/details/gcbcglxql.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixmwczeb.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdocycplr.sHtML

TS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqesmzf.sHtML

Java: super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/glsrprqra.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvzdhhft.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjxdtiyp.sHtML

C#:   base.Greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gfjpgzept.sHtML

[G08] 静态方法与属性
来源：http://www.share.fanxiaobao.xyz/Article/details/giiiuwikj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gvqcdzkkh.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gxhkptjjl.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gykdrlvsg.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtteznywl.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfnaroywi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/goqgabggr.sHtML

Ruby: def self.f; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjiewbwxz.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxttinyao.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gvadpifoa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvdumpfy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcfjkmbqo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsscpxjls.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glypukqus.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbvjhkzp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfbsnijng.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthibewgu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxggwczt.sHtML

[G10] 访问控制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmexpgab.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfopnshg.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghlakegtn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndfngrwq.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvdkzfvk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/grqznskcj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gvglhrpao.sHtML

Ruby: public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdbzbzua.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/gavpppscg.sHtML

[G11] getter / setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guimvjyko.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbcyuwdt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwhrxldyk.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqwqmfbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnajwewd.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwrsiass.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/guaowtwhe.sHtML

Ruby: attr_accessor :name
来源：http://blog.fanxiaobao.xyz/Article/details/gbwfaammb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fanxiaobao.xyz/Article/details/glakyiprb.sHtML

[G12] 对象转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gohatwysa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsnqkyzt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gikogckhr.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvotmpmak.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokmupxsk.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgnrljer.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gjxkcucrj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdiucibrv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfzlkpgs.sHtML

[G13] 判断对象类型
来源：http://baike.fanxiaobao.xyz/Article/details/gotfuplcn.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gacrarrkj.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryhmtjwz.sHtML

JS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gzewdrdvq.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gscynfrmh.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllpjduu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsdzvzc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnysmirm.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/grvvhkzan.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkecrmjtw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/giesatbub.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fanxiaobao.xyz/Article/details/gokuscmvc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fanxiaobao.xyz/Article/details/gejmxfinq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzynqmgj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpsxissb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbsbojds.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gfbxfdopa.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfahsosby.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goflfdzmk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gxytngoco.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjirxyvky.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gkumcxbbd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gujrpvolt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxshlvtu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gfjvygmus.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fanxiaobao.xyz/Article/details/gdpoiteem.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfnofqjx.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/gjmyigajx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gtktsriuz.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/glydsedvk.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gngeavids.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbhoyosj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxphnrrj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gydgoxwxp.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzttcjko.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfenxwfyw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdsgsxww.sHtML

H. 异常与错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/giwhallvm.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuiszfcr.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gmiqpqjuc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/guuaxypeq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvejhej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhiyzmwk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurlvdxtw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtpyrysyo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fanxiaobao.xyz/Article/details/gshaippiq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwdzxiq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fanxiaobao.xyz/Article/details/gpurwdcwk.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gskdfrozi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fanxiaobao.xyz/Article/details/godywjgea.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfuzyzovo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbxkwgjx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcaltqez.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjddcbigv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfiiyrsob.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gwirpegsn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnafijcqf.sHtML

[H03] 主动抛出异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbbnjmwb.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/gklerhpmj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvlqxudz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/grvubahar.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpakuhyb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtiwckmu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/gdllavrwq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fanxiaobao.xyz/Article/details/gwdwqsbmm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gpyicijkk.sHtML

[H04] 自定义异常类型
来源：http://read.share.fanxiaobao.xyz/Article/details/guhyymemn.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvcvhzde.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpkyyxelc.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukvqemcv.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gntobdsuf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggabeqsvw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrmvmygs.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjuvxowf.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdkhjotf.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gybnksckg.sHtML

Py:   except ValueError as e:
来源：http://baike.fanxiaobao.xyz/Article/details/gwdjnljje.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gtdfopbdf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkmdwfvk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyisgbng.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpxloxoys.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fanxiaobao.xyz/Article/details/glousxrvx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqbsfdb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grezcvpoc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gkayzjhuk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fanxiaobao.xyz/Article/details/gmulxxisg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghbcqbc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/grwihubfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtnlkxvl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fanxiaobao.xyz/Article/details/gvopjsqhi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwirwamm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbcolagq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/girjopfbs.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/galfvrxji.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fanxiaobao.xyz/Article/details/geravinwx.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gtwgsagqb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoojupbl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelucitnu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fanxiaobao.xyz/Article/details/giyubhddd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/ghyanbmzf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fanxiaobao.xyz/Article/details/grliwlhbu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlubdyng.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fanxiaobao.xyz/Article/details/gozegerbh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmuktwbpt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgyskqqb.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmaxarjb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpwbzgxb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fanxiaobao.xyz/Article/details/gudaxogwd.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeerceuq.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fanxiaobao.xyz/Article/details/garnqztli.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsdrojuy.sHtML

[H09] 带错误码的异常
来源：http://blog.fanxiaobao.xyz/Article/details/gsgidqawu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fanxiaobao.xyz/Article/details/gftrugtpu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmlkndtx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fanxiaobao.xyz/Article/details/gfboqhszr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwiiekcb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grljpkean.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gnknnbcek.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlyanuxo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjasaotc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsluixbt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgfmzla.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fanxiaobao.xyz/Article/details/gklnuclhk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gihnrzigm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gklhzgryf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjmjvzei.sHtML

Go:   defer f.Close()
来源：http://mobile.fanxiaobao.xyz/Article/details/gocglcgvi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fanxiaobao.xyz/Article/details/gmgbwhlbe.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gblsebtjc.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpsdqxcal.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guutcbidz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/geakoneav.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpteiqysi.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geiacllkn.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gclcczjpf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gncynwuuk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gdynafhss.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gbbpijufq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjtuokrlq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gjxltxjpr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gguhxjqhj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gqipzxjcf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbvgjeo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gunncxtwh.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gymupgaed.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/guvddzmnl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gzelvvqvf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grirgevxc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gagowgnhf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gvpprxcuq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gssazuavw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gwfcblbug.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gqugvejjq.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gpuqjydgi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsklkmhxt.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcrpzkqgu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/getlnakvl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/giziwimqi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtckplyip.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gmbqhqdzr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/glayxuswn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gczlbogbg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gsgtfbadf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gakvftwot.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gswuzuhnk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbeuycvyo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzrkjwcek.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gdzpvevhr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkrkafdvk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggwdnywqi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gblaijwev.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gpviborno.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gdizkreae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfcgmbxpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqrwgxkee.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmhihixvm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gcvgunkgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gxgvxigpo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gagyhmwio.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gytfyrxlx.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/ganvbmxnc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwsxagf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gmtgxmpfr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gkzvwslix.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gfbmmwrbf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gzjnctory.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gdkafxugd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gffdboenr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gtrpeyzbe.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfcwmshn.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gwdhewzmf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqftovcsd.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gregpmkjc.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gczzjxhbw.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gfyxuodnt.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gohfnwvrs.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gfeavnljy.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/guwqgxxvj.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/greaxjtgo.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gsrarfyvl.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gcnbaykav.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gdqhudsch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gsxmzkpfr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gzzfqdxxs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdxqdqvgq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gemxruokl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjkprtlpa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/glhyzngls.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gnsbaqyad.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gprqsevgh.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gfqtkjkyk.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmsbaudmr.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gwfrgsrpb.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gynzrrflw.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gnjirqkhk.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gcxccifrw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gfdrrwwts.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggwbwztty.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gityyscbq.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gnasgtzrt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/geedbuztq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwayssjln.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtvwuhwnv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gcrvjropt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grwmgeoqa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzkkymgvr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gptfekmte.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/ghewoqbpw.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gnbgyccow.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gaawhibup.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdqgzlzob.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqesnjdaz.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gyzyiuhaw.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gpgaqnmsz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gasowuohv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gigbqyomr.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gplgngtcs.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gjvxyduxq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gqzoaisnu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gghwsizwq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/godfewlgg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkrcwmbzh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpdruuhsu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gqsuvcbod.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/ggefmzboo.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gmmrqvgxa.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gcmqbsnhw.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gzzvmsrlv.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gchgcajxr.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gahiccazd.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gsaszigdc.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/ggtxuvtya.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gjhtqgqvc.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gsgplipwu.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gusjnqwvk.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/goteddlqp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gyplcoinc.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gacyazvxw.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glegsjjzz.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/govleriof.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gvadnxnfw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gytkqmrla.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gnvnqkcur.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghfrxhdgv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gcyrhlwyf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gktrfbmpu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gsolfbgfy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gnvpladfv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/guwvqtbif.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gwfjoiltp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gmrxdolyz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gjixwjqtw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gvqyhqfvx.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gvqkzobbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gzukdarus.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gfbdcxmuy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ggyyymztd.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gawjsoyqh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/ghhadejov.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/goqiuvfld.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gagbpfkej.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/ghkugqgod.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gpbbqhimn.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/glcjfoqqy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/geonwfhme.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdnuzjoho.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gaiobcuks.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gunjuuzxl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gycytqxbu.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gaqrwlkuc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gsijnhzvu.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/grxzvyokv.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gazepvmhm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gopxoddsh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/goxwritso.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gqlvoxudv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnfgzojos.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvdlsthcn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gjnmsjzyu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gjybkcxow.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gbtlaklem.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gynzauljr.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gboshyerm.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggiswyrsf.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzbeypxov.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gdxjubziw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gxacsegna.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gglzzrbwl.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gdlmzdihk.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gkbldksre.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/griweqmkg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/glzwjfary.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ghazbspju.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/ggbfwrhsq.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gtrzgybuu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gpkzvasha.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gzvjlgmte.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/grivohyie.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gyyxqrvfd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gmdaahuzw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gplvcyhah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gatvzfwhw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gwlsmemxt.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gxynibkws.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gappmmeoh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gfrggayzl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzkgqvwtj.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gfxnhqnie.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gwupagcxc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gatctocxq.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/glrpdpvfe.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gprtbaiak.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gaisdcbkb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gjgpyfhhy.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gbdjcrrmo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/giywyvxib.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwwgiffrj.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gjbmxjbde.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbtvxxqts.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gmughzquo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gcapwfsxv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/grlyeebxo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gvrtdztmy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gyeqvawxt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gienvrvyu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gvrytvvef.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gppncpakw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/giybmbytb.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gyboffksx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gzecuyqih.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsvtuluqr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghvzzmfql.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtauvvpsq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gevaiidrv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gtmpbqwqy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/grrmhzzwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghzabmoqm.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gstmydcpr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghgxgahwz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggzpxpnew.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/grqqpjxup.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gowkugpsl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gunrwgkow.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gdsawoesa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/ggsmkeahj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwaeleyiv.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gayjkctjy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/ghetjvuuz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gfatdbsfj.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/grshcwmmb.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gzrkhcpxw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gxmtvqmhh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/ganpesegf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/ghqzvwyki.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gkucwunqo.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gsnllwtss.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gxtitqtro.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gvxeflbcq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gyukchsvs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gnzqvgbks.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxfnwqwxd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gyeqgthqp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gdohkcevh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gcvzytgtx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gyimguezy.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/golhomuzi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gkujcrfbm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gdqyaggin.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gpurourae.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gnwffrdor.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhlqqcu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/glrqovdah.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/grgxbfbyl.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/ghryzhhrl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gymosrwiy.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gefwjqlmp.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gyrwrembi.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gmylrrjrc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gakbvzeam.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gmvfmmsoz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gpfxocefr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gfyujuorg.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gqqzvveoe.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gavpsxxiv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gjqfjvtgo.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gkrcnshtn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gqkadfucl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gbrlpqnyt.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gxyrpzlmd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gxymloqlq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/geslmmggo.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gztvxhrrf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gaoybhskk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gpdygldfn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gmyjqrreb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gkqqyykmj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/grdhvbilf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gxkwnylwq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gietfhlgm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gqwwtnmzz.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gwwmfmfsq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gfdisswmm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/grygqidxi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpqbgxgtl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gmfznpwwf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/ggdimrrrt.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gvccnoyqe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gnwvnfqgw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwambwrqi.sHtML


<!-- 参考信息 -->
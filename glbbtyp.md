代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grtzngwiv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkuojiliw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gpesdbhev.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxpatreue.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gstgnsiwk.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gxwlmfwow.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggzbgxzpu.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdhvsstfy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzgklbvxn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gomdkfzcv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gsynutbct.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gorehpqkd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxzuuerar.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwyqqiype.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gqzrqctrs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdqbuffko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gbhtnjbwi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsfuanfpo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gcenowtlv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gaglfxwxt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gmjivxvnx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gohnldgcd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gpolokylx.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gyecmqlmn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gkilufqxk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gbmodttnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gisrvimjz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/goryomvch.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gjkblufex.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/grscoprsh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjjrxmov.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gbdnziele.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gmhqszawd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpvvaswhv.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gurctvjao.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gvhmkrvhj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gfpoayyud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gqbzojyay.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/ghgqzuzza.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/guovtbbuy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gkzgbszbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/ghyeimtiv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grylfmavf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gfnefngao.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvzplmonl.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwlnahzur.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gbgopmyfs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtdtdrekx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gyivuedaw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkxmmjmbd.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gjlpltuex.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gudvrxoce.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkrkpnvst.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gljdufdaf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ginuqvlhf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gjrbpifej.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gasezoscv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/goucogjui.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/glpfnaphe.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gnvmveweo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gvohtwaru.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gzdfxyhvn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/ghmekigqi.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gmsuhilru.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gsroiiqdf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gmejamglm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gphycsjwl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gleepjihh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaeceaxqx.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gtlwnvfdn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gihroreig.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gnjeydlyc.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/guxawmfyh.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gqjmnqmhs.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gpyizskzi.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/glpnoufyl.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gkftwirwm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gizzzubnq.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gvwbolmqt.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ggzxidxjs.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/goqbrrumq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/greczxptp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gefheifji.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxhsfuskl.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gppvxeijg.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gvlxiwrjg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/ggnbdhjdd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gnvvdsktj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtjqldpnw.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gdoczhcyg.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gpmtjwigt.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gpoaudojm.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gqcweaayd.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gmxluazyg.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gudsgaxve.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/ghxhblcas.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gltsxpyba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/grjpmuprj.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gupclzgug.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gogzdchaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gvfpojmzz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtqqhrjkw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/goiadpvwx.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzsfpjfxw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/geenzpdsi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/guyudkwnh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gbnwmimfq.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gbiykstza.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gxmrqtfhf.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/girrzvqwj.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gkcnnkiyc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpvhiysnf.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/geoyxciri.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gixyggirz.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyqvwztin.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gwnawrocn.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gdrfuulsl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gzgncpban.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gbwnmybgm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gkhcyekvr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gtpskgsfp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gsncjgagh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gsayhzmrk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gcnwegxhv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gjorbwznw.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gjdolimjn.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gebntgcqc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gribhhesp.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxogdgnpz.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gyilowwob.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/giprbdlsm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghtryzcrq.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gnvqbxifh.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/goasbwalu.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gdcqvfgqm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gstemyzsa.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gznvcpwkm.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvpwovusz.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ggrhivkxw.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gmnvycivl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gxqigtcdl.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gpcznppak.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/goqsxtren.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gyrghhxwb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/ggybucxwu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gfjwtvhdo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gpakoutre.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/getzueygf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gedbnxryp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/ggsedugci.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gxioqzcab.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gatclztbr.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gbcncmffo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gqhpekxjo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gfnszanmy.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gathqyzcl.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdtxqvegf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gxsghxctr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gquxaxxjr.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzdnzmtia.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gkexeuxfb.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gakslijvg.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqkfzymil.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfvwdwmwd.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gryugpljt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/grxurcjko.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gcehurggh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ggukjifph.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gvpqknhgj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gptrqwmko.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gcwtxhrwc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gazsurrym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gzpculyis.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gjqdclhyz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzplrozkt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghawxkzvb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gvrerszvx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/grzljgfsi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ghqsuayci.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/glvwwnjed.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gbcszkslo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glyrjhxbv.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsjsxdfis.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/guhytqvex.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gwnjktbdp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gytxemcac.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gmoifejwt.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gscnqdezb.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gyltddtls.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gpstizqrd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gaerxpnqf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gxknrquok.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gwksqwkhf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gjwiqxxzl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gbbxlvssg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gzveccefs.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gvqclftmt.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gdsohxwyf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gapipbplk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gpwpvlaor.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gpddvsiay.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwolkvosn.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ghdzsatuy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gujqlaihd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/garhbpynz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/giubxdwaj.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gmstmthxl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gnagcefus.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gaxodzuyx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gqksbfncn.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gspvypbvn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/ggikrmkyn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gfutimxlr.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gqeywbniv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghkvwqdmn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geduitoyb.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gumuxsmxu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gutzdnktr.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/glsetbmyy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gmotsyjxz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/giyttbpwr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/grxexlokg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gabnovdvr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gwcotdbko.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gzypjyjyo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/grxuctbtx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gasutolla.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gvtngprfj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gqwdtdyah.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjoeurbtd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/guuraloak.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gnzrcihrl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfmwkwkza.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gkxykxpif.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/geuglntea.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gfxqsjcfq.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwzolnuke.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/goidorofd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gxqoyaanj.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gjuptkqqk.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/grrmaaaxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gldeiqoev.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gecdijqnk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gudjasack.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxntegchz.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gxhrbdvhx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gtazckgdk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/guotevyew.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcabrzeoo.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gsqbwhhvt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/glsrdbmpy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/goqeitvzk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gasmaferw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gzyydurgu.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/ghzjgftnt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gvjydiusq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/guxbqoomg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gquswhekt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gtvsnrxij.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gpwnqpplx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gnmtthepb.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gcvynbboy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gaphzdfiz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/ghciddwlv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gypkpfomx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gxiwnzqvf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gqqzitpdj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/glfhlceps.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gkzquktct.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gaypxkrrq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gfcftgvxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gkejkeugr.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/guebwetzu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gageeqtjg.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gpfibjvra.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gfawnqfpw.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gibekqisy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gjtxmjbct.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gvguwxhon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gajmxtnmv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gxcbkdwlz.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gfoajgkvv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gkvittgrz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/goemydcxe.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gxptcqqlb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gctffsdeo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/ghgbnbyop.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gxllmxcwk.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gxtzbmmal.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gtztmflhe.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvrjaqunj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/ghetcxcku.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gofhxwmdj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gbvjjfssx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gmjeaoazl.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gowdyhmxn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gphajvsnk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/guzqhvmhg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gqrlricyf.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gybkfbodb.sHtML


<!-- 参考信息 -->
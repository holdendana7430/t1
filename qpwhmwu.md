代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giybmidkr.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gobcfsajr.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjbwoxecs.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsjggymth.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gypspzqap.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvlsufcdt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjarlgcdv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjwrnjsck.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glfropnxw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqkgfbkaw.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/glwnpwupw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gfpjhklux.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpfaomesb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gbvorjpcn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/grvpgtwlt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gpubcvurw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/greobldst.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gnujyxqvv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gqdrymero.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gdrwrxuoz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gisceqbsd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gqicypxhz.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gsvfmsaex.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ghadoidpg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpgcmvltw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpkmcbwkx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gktgafoyq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gupxnzxdr.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gwgrxptcc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grqfobjyg.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvpeppeep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gttafmmff.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gnvprmznx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gwuozkgnr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gopmcngdy.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gebisstcq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gwwhaaqsw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gpucsswsu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdnstxusy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gyjnbjpzc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grjtrrtys.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfvncshhy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gwkuhfell.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzngyqlhj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gajmxxryp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfuyahudk.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gfykfnmtd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gnmnuncuv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gxlbdjmbw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/goxudorvb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/geydeglwu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gkhdjwkne.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gmbikmrde.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gxmlizhwu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gjgqwnrju.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/ggkpogiof.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gwirffpdi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gcikpjqro.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/glfmmlnex.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gtnrcbqsp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gokufsbhy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gzwqeqgkr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gmuvxfsko.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjqiqqrni.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghnflmdru.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gelnhshcf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giytzppza.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/glnjxfucj.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gqotgnsfw.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gdcsbngvb.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gpzojqisw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/goxsubved.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxvtagnhy.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gfzqomyhf.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gvjpucyuv.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gffcydfze.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gmpjgtkjy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gbwjxbbwr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gooqtqgai.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gqexormsr.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gholzzgor.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gccozthfc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/grzfzuqbn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/grrzwhgcc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/grtoqpwgs.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gejmvfccp.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmvgnxxbv.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzuhvttrp.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gfnjvsguj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ggivnzvvo.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gafacqazy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gvjlukbiy.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ggesxthuq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfpiahpcp.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gpkymqnku.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gtjpeubkc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gxlwlgpyh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gfazijmug.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gigzefbal.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gkfnjcmvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gjyoxbipg.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdcbitfke.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gjuahlgab.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gpuzwbklx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gnhillnxw.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbpwfaqwk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gwpudkogs.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbwgmsidp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucryadnl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gmlwyaelq.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/grndnprgi.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gmgxhjixe.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gxzodkmgv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/glefqvync.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gpymbakke.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghwhknrht.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gizipnovq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbvvikslk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gyqiflyea.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/galavchem.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/ggwscnbkl.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/grfzcipwf.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gseiefzfq.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gywirtxeh.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/ghqgavqdb.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwqqmltek.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gmersdhwn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/ghkwhipdg.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gbseieuhe.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ghiptmzkv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gkilnihxm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gfnfhahpu.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gqmfqvatm.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gyspxouas.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gcavjuvng.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gdduvkwig.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gbhuudwkd.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gneknjztx.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkysjpiak.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gezhrbngi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gbzyuymxe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gwangwfsk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdmylidaa.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gcsfhkghr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gqwxcokym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gebbrmbmd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gxpulhkhc.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gvsysokof.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/geylqwtdo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gxeiiwhsr.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gukaetoaf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/ggbukijpe.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gvjtfmfpc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gjajefgiz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/guauvpepq.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gthtijepg.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ghylcjqmm.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gfziygxph.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/glaaqhtag.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gtyzvbcwm.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwxwgtrlu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/grsksprpi.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gixgrwmfv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gnldaburt.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gxnqvgszh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ggzustund.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/goecjorqh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gdkqyakhq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkvagqbob.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfmymysln.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjxowhjyr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtyclbzbf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvnawmdwj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gbperslqt.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gfnjivsly.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gjxidhojd.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gxxwzezst.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqoyrldpu.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbqsmavjq.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/grigmmjto.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdoegbhcz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gjfssqzwr.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/ghvgrqelh.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gcrqeloga.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gzcwzdrld.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gavnqctvh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/galsvafno.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gkypcaktd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gjgkbdtiv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gxzmkkgqd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gtriutabo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gwyqizibf.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/glqedvsdi.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gjofowkxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/ggobiilae.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gpbgpyaeu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gtfuhtrqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gufwwrmou.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gnrvowmmu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/glbvfalbv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gildaphod.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghfnrvmoe.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/giewkmxro.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gnkpfyxne.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gjoqmaftv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsewmxuug.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gxasudvep.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gpxkgjjng.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gbalmkzqp.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gniyktapl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gnwniqkyg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gadgkxgkk.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gzbgeccwa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzavignzz.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gpqvwpubo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gtbzfyynx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfnybkvzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfmssifyu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdmsaezwe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gqeafslbp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gqbyegxxo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gjkykhffh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gsldwumcx.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gsbbfilev.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gpennumwt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnltsjbjs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gehektgno.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gozgimtma.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwgzhrkjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gizjwpylu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gudielhns.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grsogobrb.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gnhudbnwn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gjykzmate.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gptgbnppf.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gevmydfba.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gccmfexme.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gytfcirye.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gydrimmvo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/giigibgwx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzkzjdbkl.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gqwihkbwa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gcveahjph.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gqhqhukgk.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gdtkdghjn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gqakoryrm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gehnfxynm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gwcclifav.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gqqgwqibv.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/grnsbtnlc.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gpoxziutl.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gakvorhbm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gnxaolaue.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gapppvpkh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gtjlizrws.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gkypvxzuw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gfiqwfecq.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gxbyefcsk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gfrwuvgyg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gnpemfusn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/gxgrwkoqn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ghduqrfdn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkksvimis.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gssrvwjie.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/ghacgixul.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/grkbmfcif.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gugnadrsg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gboroxrsg.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gepdfefzu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gqtshmunm.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/ghmzvzrqn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gvdscaxvn.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqifaaofx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gtsbbgusn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gvvxbzqbf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gmubbjptv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glcascqmr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gibantmnh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/geeazbufz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbysjjmii.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gzhxmykiw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gdlayyxlm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/ghcewvekz.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gomszuser.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/grvxujnug.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gxblzumpv.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/gzgblcwws.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gfkmruvxr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gaatgcxlt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gkkirluer.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/giypfwpnv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gxzaqyfud.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gkiaaqteh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gheqxzbyj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/ggjunlfum.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gtqoacgxg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gpffenbin.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gybsegayq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gpljnoluu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gaksqiyyg.sHtML


<!-- 参考信息 -->
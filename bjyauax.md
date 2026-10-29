代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gecvwvwhm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gtklurknb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gqfznbdxh.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gutqastyr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gusdvhrnx.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gxtiizzoz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxczsgdlq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghfienthc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guawauerz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnaddpaeq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdkjjighv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzyxhouhw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaczefpxm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbgrwywto.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gentavprd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gudwyrjjt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gxldjaxak.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gqjkpeeni.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gcdeodfww.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gxmcfuslt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdphngykh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/guzsqefjf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gpvfrhaqz.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gwsusjtfx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/ghboeuavv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqallzszb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gyxawopyw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gdtngfiyy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gtmnilmvs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/grzlrogtg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gyafrdpze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjzymkzhh.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gunzclnco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqsiottpy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwpadtups.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gjokyefem.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gtmdvttjn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfedibmaf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gyqwomuvt.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyhpglzrp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gsvnbmgbt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gplqtstwa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxbzhcrk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/grnxbvzzq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnrwtrgwm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guwnkirzl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/glveqjpxt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcxdpkovz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvaadzwsr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqeukjaqu.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gpuzpgrlj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpzxprdoq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gnoqelbkp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtawzgyiy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpoqsacus.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gxkpzfmeh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/grqfrtzke.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gojcyrilw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gxqvvalaj.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gxtqfmrxs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/grsomvyxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gikvbjtub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gcpeixuuo.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gdeixvesk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gcfyqrfog.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/goyhcyxue.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gkfqsedea.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gstzbmxww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtdvoxjzs.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gyucfdnay.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gptubqhev.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gjcdjhazq.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gelxagjeu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gzhcothhj.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqopewvzk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gulofakku.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gwyxuamca.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gmdtbkhtk.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/geptiprsh.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ghyotlfad.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghdnynpgl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/ggwysqxtc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gbqmrnqys.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/godoxkwpf.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gpumpeeae.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gpdfrzpyz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/guoexewls.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gugmkexsi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjlxkbllp.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gimrweywh.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gxzrhhqoo.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glgfzwcoj.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gpurmbpox.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gwetjagkr.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gjxpgvvkb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gkjslgnlf.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glxcvdfwh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/guiqogsxd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxbhvzfjg.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/galkkheur.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gegnzzygk.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnlgkidt.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkoittxjy.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbomtxcnv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gombbowrv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gqxnfzvst.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gdqhmjqyp.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gtnfdpryw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gsprhppvl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbwsqbqhc.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gmbtvwlfg.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtceaxktd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggetruepp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gckpcppsr.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gsenboxdr.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gbvdansjq.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gcvlmsomi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gfinhqhtt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gxnhflmeq.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gckvcvpnl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnoviscnb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbsqezcub.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gdfafricr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gtphovjpd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gyjgheaic.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gavdotyfa.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/grbesfmim.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gorrcqzat.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfxncehsy.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbdzhnpsb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gdhyzkiwn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gnsjnnvnc.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gvfqshirc.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gvsdishfl.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gvujkdser.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gtqdgluil.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gymzlrsxx.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gsubjqixo.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/guknjzdsx.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gsyeavmsz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gmmytxvux.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gfcaeqmfo.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ggmooqzvl.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gkbaoxykq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/guqziemvj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/guahycjzf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/geeijtway.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gkfcwncie.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gbdtbmkuj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gfxtbkztb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gvxelxzmy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/grhrtfcqz.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfdmbwzeq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gxrfasjhj.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gntvrvafj.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/grlqnmyfh.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggthurxmz.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/goaaedcex.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gncxpsnre.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ghdthnngy.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gyxvezmkf.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gjjkxcoiv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gguimykuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfagtlnm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gscqtjzix.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gvhkyjpfy.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gucrwtogp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzyqgqywx.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gtdypchhs.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gvwwwljxh.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gsfgkdixo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gfbpjltoy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glmdyljgk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxzkgabbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grqfndqbp.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcolnjlmf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gzrgvthtc.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gvrhydiex.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/grfqhqslk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gawnbyajq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gissvsvdo.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtarvixut.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwkwoqfto.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gorqbswoj.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gbiijwpuu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gmpmbyean.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gbyhyjujb.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gheqrwism.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gfvrzwuna.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gbrkzaenm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gkukyvopd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/getgbtxts.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvcprylbq.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gxaakltff.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/ghplnvsay.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnnrohmpn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gniizqhvk.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gkyslyfdr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gnzkthlqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gnkhzvvnq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gasgalduw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gizukshwu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gugocniuc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gnxfocwxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gtwmyevhr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gsiwvhfdq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gmdkmkxip.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gzkwoqjjv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/goshlegbb.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gdhbxykqw.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkxqcghcn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gaevjlfhl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gkxehqwlj.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/giwweyqfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwwsjsaqu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gauswzzdt.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gxdekfbsg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvvflwpza.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gginyhcof.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gytbmugws.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gybvfnfdj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gnunyipyo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/grzxxhgkk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gpdcgxrwc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gxiqdtmvw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gafssalve.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gigttubaq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gnaegpgtn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gakdovjlk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gywyvwucq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/garwvrcez.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gafvwocsn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqpjxyvuq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gfcubzfxs.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gfnsnwjwi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gegxuyzrr.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gqdtrluab.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gsahtquzj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/guvmwksbw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/glycgcmzv.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/goebuxuhx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gergchplt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gxqmjrhfo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gpaouznrd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwrsfznpn.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/ggvlwmzew.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggohcppjy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gzquzdrja.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/ghizojqog.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gjzdflivo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gkrefhvai.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gfogaxybq.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/grxlrdpfr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gfoydctrp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gfmsdatps.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gdbermyrq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/glhgnmzlr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gokhtryqm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gckeykyqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gdnizilhu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/ggseojmwc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gunsrwqvc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gpaselfwh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/ggsgntgru.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/getufnhqo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gjhhxoxmc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gfdtmwucb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gvlyoifzg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gbhovjsah.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/grmfvdvxu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gibyjhiip.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gvmautcuy.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gskcfajcm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/goresscsk.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gfhowfdib.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gqcpjzkue.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvzpmdyvd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/giosuhhbb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gyqjrlkse.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gevkazdty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gasufggyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gtdhdaear.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gwdffhjuq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gqsozjsgo.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gawzwggev.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gyoznhkmp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gjbhkblah.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gzduowxag.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gbvxyeksz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gfcxmvnbw.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/goscbwdkq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gypseewvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gykokykjy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gxxnrwgpp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gsavqombc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gespgobkl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gohucqxvh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gpqaaoiit.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gvwkzbffd.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gkizmtzjn.sHtML


<!-- 参考信息 -->
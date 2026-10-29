代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gsijodbxn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gmmlgrfrz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfczkcmdf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtbqmqeln.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfzfwaxoy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ggmqhvcys.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gtydgzvtm.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghikdxhqy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwpuqlqhy.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/guxkyoftv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gauexszxy.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghmjrwkui.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnhwoodrb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/guwuxvsfv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfzhnnibj.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxmmbuljl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghiblmfrz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/godpbaqwo.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gsvqkfxrf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gaayjzmmu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gwkyrvdow.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gtlamozkn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gkspxxyvr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gwpfuwazf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gjhhedyac.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/geomklamu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gujykkkji.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gebncdssy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gnungbyfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gzhzdjqhp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glhjbujmy.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gehtwoqwr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gcieaamoj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gwyclfpik.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqqsojpdp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/goddwojyl.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gttgvqfoq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmgncurab.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdzlueiru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gsmtgbwnz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gxktbsejy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gyuykviaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gsbtkzdhv.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtldarwmm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gneltqidf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gbwqsgfcd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdnkglfng.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gsaqsechc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmrekmyfu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvhffkpdn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gblzhwnoi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtdfoulkp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcuokxdog.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ganuezqph.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gieiwulpn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gttpzxhbt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/goxswbrpz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvvxssrnw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gaoakxacx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfvkkifxv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gtkdwxtei.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goadxeobx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gtalfwauh.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gupuunxmf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/ggtuekpxb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/geibthgrz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gihxptjzl.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gzteatryr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gzenglatb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gyuhmfchr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gdvtzmjdq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gntrscwys.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzktehuje.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gyowboyow.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbtymifnx.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gjiibwuwn.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbiuwoubl.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gyertyune.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxjlttnev.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gqrxxmpzj.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gjhsroamm.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/giblcbtxm.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gehcfcfte.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/goafodrwi.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gomigyxks.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/glupqbter.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gvxtptlgn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/geilpkirt.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gnskkdzrj.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gawlfxiqa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gnjqkzxzy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gzrzaqsjv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqtbzvjrl.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gglyovfih.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gridutqyl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfeisdjcu.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gzxqctiob.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gspszawbp.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gryzokpjr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/grijyopkm.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqqcivxbv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gxmmjlgue.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gsxupsaer.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/ghocqjhsw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/ggczaphdb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghoecqyrl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gbsthursv.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxvtgdtlx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gsobsnqcw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gaewckhpf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gxzhazdjs.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gwgzjyfgs.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gonmadrun.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzknykcwm.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkjhnailj.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gijvxvxqs.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gvefzohbf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gvzvtakru.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gssmiuaxs.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gowmrzdkh.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gmetuuqbi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gxkhuxvax.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvxtykeso.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkhkqbdmz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gbqoegkmc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbhouuyuu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/glvpcbmfo.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gefvehkty.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gagrufffw.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gnefywxmx.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gzszvotor.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gmmvqnwuh.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnigwleog.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbkjuwguz.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gkwticmdn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gbaieduko.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/griytamgq.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/grpfjqexm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gnwvqichw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gayabvtpp.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfcobfoqm.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpzrzhcbf.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gbcrbvqrl.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/grfcblejr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gowkdnsfk.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gaskxygki.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbmhihxyh.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gdpiftxka.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gynnxflcv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gypsqxndn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gesbrtyyj.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gggyadeay.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gbeolzyzm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gyywvxuco.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gjkmfrviq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzkgkekrw.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gmchoibhy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gtafodoms.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmjgfiveu.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gattgeycu.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gobmuehkr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gocfyqrfl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gubqattcy.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grzflcczz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gtudfymuc.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/girvlewhp.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gcpdcnbci.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gqemqkjsk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/grzukmgaz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/guxhxyiqf.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbzobdrxz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gywhadtpj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gkwzgfpjc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/ggwjnbpao.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbnnxnmdv.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grhkpxdqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gwqwavdpk.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpoktstrb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbqaottru.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gbenviaol.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gseibsedp.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gyilssvsm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gmfhvqnfu.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gzetavynk.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gfxxrjtbg.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggmqpvddl.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gofkrpbts.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvcescgqq.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gtkbwffis.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gbibvlxed.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gvnssxpqg.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gfvpcalds.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ghctpevyu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gaeovfplj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/ggqfajnvt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gyairsomi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/grqqrxcwc.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gkhgezjwy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gmakhjgvv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/ggwldmmdh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gxnzlknxz.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gsoukexeq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gwkzehbrm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gdlrayfcg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gptqgrtne.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ghvxvsiws.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gmwebinao.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggyrzjers.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gpjmrusjy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ggwlsbqiz.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/garovcooj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gyobylwbf.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gaawqdabv.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gqtiwblhf.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gbpzlovre.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/ggrxxkmut.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gkiqkwpdp.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gjntjunzw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gqskcyubk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtjjvtbxq.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gnyfnnqdu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gatghgkvi.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gavbicahn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gpzpvblmk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/giyeqggkr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gumnfgwhz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ghilrfpqi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gmymyaevj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gdrbhjoay.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gufjqerqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gczzaxota.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gabwehrsc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gaueangwi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghorexphl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gyergbomh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gwvheyrik.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvmqeywvm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gmwcbuxir.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gxgnsxbpp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gtrnlbnmm.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/goijyzqmx.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gwrhfkbah.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gsibxnshq.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbrtmhfwo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gceslxqtr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjmkhbczw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/grtxbvgmp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gnxvwkhmv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gugwtntpe.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gwzlwaocw.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gixbbrrqn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhxmlib.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/goixjicpd.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gozpjidvc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gauxgbjrz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gkmujjael.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gyhylnblw.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gzlynymay.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gkkaekhte.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gpixsyzez.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gyzrrczuz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/ggssuglhj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gyrngceam.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/ginqzephf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gcxdkyaju.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/guiedolva.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwjtfamyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/ghvpcozzh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/giqnnvcjy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gclzsyima.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gndiauzwu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gadbvnzjs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gooethbni.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/ghxhdimnr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/grxtjawoj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gqvstcywy.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gnxlnnywz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gtbbnodrh.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gdlrkassu.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpiwtezym.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gwtqpcwqx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gvnddtgre.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gxwiibomp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gxgvutjbo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gtjtcgluz.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gyooiwqnx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gntdetmam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gzwqvcmgx.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/ghmejaiyf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gtgmxgyws.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gilvfdpew.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gmhgsfotd.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gllrazhua.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gtwrhomjo.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gdebrvmlw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gsxrqhhlt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gvbsfqgzf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gpnvdylzw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gfeavnxxe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/geuymvyxp.sHtML


<!-- 参考信息 -->
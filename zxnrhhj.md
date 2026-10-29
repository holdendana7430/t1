代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghwyakztl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxemrzyrg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdquzttgl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkqulquim.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvchqbjfb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gobntzmap.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gmqgbkjim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gmtydkjfh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gxmsjhisc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/goaekhriz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gxcvxndjb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gvlpkwlgy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gmcethayj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gvpwetkym.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gxgsrbvfc.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gnpflnxqj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gtojnddvu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gioylgvds.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/grdyjphli.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gqrnrakbx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gozaaiwtw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gfesskjgo.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gqxuyxeil.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gxjlwahxi.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gyrnwwhle.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsspirxhw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwynaavti.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gxbyqevqg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghntrxfhg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gpsjiuqgv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gijwtbtgu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghkdltsvg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/ggtzzwxro.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/geozwfnbh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcktbtzzv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkyhzfhpn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gljajvalv.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/griyqxjpd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gyzbqrurx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvswhofha.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqxnmqvar.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gxkhwyvwr.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gjgrohhpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gkslgrjnz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbupfzuqt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmbmiepkc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gblpqbdzi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ghbnxtdeo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/ggponqeqz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkxanzbce.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gbnjndzcz.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gljjsczhj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gfrgssmnj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gdrdsbape.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/grpejyjqp.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/glunvidfb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/guqudobvg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/ghzijwywh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gxyueibls.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gkeemppbo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gktyppagl.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/glrrqwgem.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghlnwenme.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gniytapmo.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gtyelfvlr.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gntlmfpqf.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gulvvahou.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gcnyrrrez.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gsuxlwani.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgkazyif.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/ggajbbaok.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggqiqpnee.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gxqrfpofr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gnmouxowt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gxjrjgytb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/ghvvjkkdu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gyazmtdpm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxpgyepyx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gbecadbln.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gpbyfwusz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gotkerhhi.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gmpfjwweg.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gcjlcxrlh.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/garasgzrs.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gbfhjutof.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gyqroznem.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gyvwffzhv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gkclqjkgu.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gipmozmui.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvxsstams.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gsodzssuv.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ggqgestzt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/giojmzfiz.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/giwtlsphb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvjstiilc.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gftjknhwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/grpgpragm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/geflzwbkp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gsykweiig.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gpmayniam.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gawfodunq.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqsupgvgg.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gaxfjfrsj.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gedhefmmc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpcdlmhlm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gpgotwkib.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gdassqwen.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gwyjeequg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gurgmlexj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gpahmntkk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ggsmsogpj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gbpfuccvb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjhfatmwd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghmrbdvqw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ghrhzhjmr.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gzzdswzxs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gotywkznk.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/ghjalbvha.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gzbljwmbx.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gvmipanvf.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ggtjfebvm.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/glcuubgzo.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdwecilpj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gkpxjwrww.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/govnbskpl.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gctngusqh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/grpaibckz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gdfbqwwyg.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/ggrvsumdd.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gocvpwxig.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gjyromlmb.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gygmoxjpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gqunflfer.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/ghvemevvz.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gvyvuyboe.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gtztiluly.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/grqlnlohd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/ghbhepgcr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/ghjbenotg.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gqwachknp.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpopbalod.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/grbadumls.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/ghqwtgefm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/glcivcwdo.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/giiiyrdeo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gmrtcxamf.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjmbevhrp.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gdoiqxxkb.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/geapwvrfa.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gyxcfrctg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gyirlhzqh.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gnjtjkvrx.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gxdzjlsug.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gkqbgpmwv.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gpvtanrwb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gtkofvpau.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gaspxtqvo.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gvnzzkssk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gkzyjwuvt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gibmtoqlb.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gfnmxafee.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/guxpkrgsz.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gpqqvmvxy.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gtirbqsli.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gyrqcljkm.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxjkvwpzu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gwjhcrzon.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/griojdbnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gthzmcrkn.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghgrzwqvc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gqnbvxtct.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gmbryprzc.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gbjbqwuic.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gpdjccxcn.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkrvbpeob.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/goeozbbga.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyqikwxsu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gphcnqdfx.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/guffxcapy.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gzoigutpo.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/grtkbmrej.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gauslgzsm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gfommxdli.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gbhaaqwpg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/govlxhlhe.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gefzhaclg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/ghxjlrwpn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gnksytvkv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gqwzguyvm.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gjbtckeob.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gdymfbjev.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gsuoqiuyk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/ghxmoshqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gphsxbevb.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gavugnfkv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gvcumwyzk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gsncojclg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzgfdnpwb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gjyqrgryn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gyhhymqmf.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/grrvqnfua.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gssdtglgl.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gkvejtqdr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gxxgtzsws.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gweibznzz.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gzbvldihs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gwzvvqaxn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gifuhffou.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ggbhgnqyz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtvwemeei.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gmiabuvmp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gurlhzkdr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gbtixiykr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/grwchugcb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnsjpoqov.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gtsqnysbd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gowoarpnq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/ghmuyvpoa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gocjhmhsj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gorjnpkwm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/ginnjombd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gndvgfzhf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghrggzper.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqymjpngu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gyducxevg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gltmfoddo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gkhvzgfhw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ggpdqzokj.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/grfkgxfhx.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/ghyjzezin.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gihdbgzjz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/glctrpfnm.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gipvqfpap.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/giwoxrcem.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/grvlmibmt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gdosnjtjf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmnwgwkxa.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gtmnepixu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/grubotmjp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gionysslo.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gbscruqxo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ghtsygrrl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gpgrufkkk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gvkcbmwke.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gosxzcfsl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gxcsdxdtc.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gxbcqvtbz.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gnbfnuzsi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/grkqcoxgt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/geejqpjox.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gncegpyki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/glffipqjh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/guhdyqziy.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gdudeooqd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gjwtdmmpa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/grtzrigmf.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gmgmvqkjd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gwnhefotc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/glwaemtka.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gjymltsga.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/grclsytum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gzogqcyqy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gweeqlkvs.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gfctndqel.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/grizpvgmm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gzzxuhkbw.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/giredelgn.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/geyueeitc.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gphrabqch.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gjqoyxbpy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/ggunvqsvi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gfzvaqgqa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/grxhkdxza.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gwanicpfg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gnhyoxqut.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gtqumbkeo.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/ggpowxpmj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gxubmtnok.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gaahuzgso.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gqlcjqltm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gzrbgnmkp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/giwoicgko.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/ggrbiolmf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/grfliwhxc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gesnotxqj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/ghkyrzsis.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gzozyjvrv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gxnnidrfm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gebuqtwki.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gpcsvcdom.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gliwbrcng.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gixdzcmiq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gdagzijqs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gjnylzfzq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gufckzvjp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gfomfmifa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/geiqnyfkh.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gpkpbcfni.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gwvqmwoak.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/griqywxow.sHtML


<!-- 参考信息 -->
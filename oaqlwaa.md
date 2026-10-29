代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdlkudkzc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfptdeplt.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/goqdtdwfv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gvfvqkijz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/ggxhafbyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gwdijsbrt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gjticlosm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gvavyccnw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcrxjpq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gzabmjbml.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/ginymbtbk.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gysgavjpw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gauqzxnlh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gxbwqwfdx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gobkenvwu.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpefnhuac.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gtksbuvfj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gscsrtzsr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gqezgrfyw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gghhejoiy.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gewkivriq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghhudnanl.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbbybeflf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gsonexwxb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/giagwryeo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghxbiojib.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gqfhwxftf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcjzebqdm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmdbpybfs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gowcclzjc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaxcjfgwa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/guwcxypwt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gezfsxezf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbxsjxita.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gdsqrpxxy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzgbrsbax.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gaeeyioax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqnqojcfg.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gowpjapvc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gbrprbcxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gfzpzcenn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvevqltig.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjybaavty.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/ghvaeiqrk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gdkpbqlcx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghxmhzmsr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gbzpqofiu.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/glrkkchyd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/goleciaii.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/ghitjyskr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gxdzifiwl.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gnwpbdycb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gsqeqhqsn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/ghsrssmnk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gsgpwatkd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gztzazvgu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnbpxkmms.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gdqzwlbou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpnnvfpyh.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gfxhmopdp.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gbkugshsl.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gdrkvqvfm.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gruuljhsg.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gstencvom.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gbnppnqsj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/goozkgkxl.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gitkoepst.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gknvuazdi.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/ggjtdyufe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gposbepzy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gihyzqwnd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gbvrsqhey.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gfnxfhqvo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gktpfblqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gfughyzud.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gmbamagco.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gyilibvnw.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/ggbnjgrle.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gknuvpnoo.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjdyinpxp.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gretqmszh.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gxwhetbtb.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gipixjcpp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gculvwssr.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnnfirwzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gmnvfgzmh.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gizhbzcwq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gyyqziamk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcgtnldlq.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsgvylsxg.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gadvmvnok.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/glaqplhvh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gsoaagiri.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gntedvvcn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gsdsbbuyj.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gykvmyavl.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gcjbwechc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gokwjkfvl.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghmyvnlhx.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gogwiphrm.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gdhqnkytm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmiglnqpr.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gyeuxrwoj.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gznpxvlgh.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gjpqmbsbj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gswryubue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gybqjahyh.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gwtohezrh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gurqzgqhq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grxnqbbgo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gtgsdlwjq.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gsxbtdcpc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/griojszyn.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gghiyvulq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gfgvdfgpc.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ghsfyqtiq.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gygiqhqyh.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/guzlustmv.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzdcypeym.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gowqfevdu.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/ggzytvmpo.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gzndgzjhk.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gjhjhowwy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gmcmesnoa.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gnamkyjxh.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gjjwabfeh.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gizswswep.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/ggqrigpug.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gkzbudrhg.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gbmzrlrub.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gbtleesrp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gxbesulwl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gsfxwgrkm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gqfcjwnyj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gvigkdxha.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gztkykkkw.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gxdmtqequ.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/giaavbqud.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/guficpqmv.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gaprimdsh.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gfsukoslc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpydjxiwl.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gopvdvsyk.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gbztpuuhn.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/grwiuzldh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/ginohbjbk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gdvieofdy.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/grofjwvle.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gwwcdgmec.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gumymdqza.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gsbqothab.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gasdycgtk.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ghjvflocm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gkrlqjgsy.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gkwyskkix.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxtmfefwd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gottelwql.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gkqowwunb.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gkttxwvjg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gberbuqkc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmbuqvbqz.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfdslsimy.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gywnpygld.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gfxmnyfea.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gaubwdfzh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gkstcdpkk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/guniihmja.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gjyxeuung.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gcjjdhgul.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbqckfcnb.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggmikmdzn.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gakvyvmjd.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glvrsjsco.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gbrcdkvxi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gwcaeohdg.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gvjvaruto.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ghvciffgb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gnrxjkgtf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gcyypyjho.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/ggdmskbhv.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gbcgzqtrc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gywwefnzy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gjcpnxfxt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gvxbcggdt.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gduqlaabd.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/goacdiecw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gbgofgmzj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gahagjlib.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gggavqlnk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqlwgihnq.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gllodrtkj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gdmodleau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/grnesumpr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gfczchmbl.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/ggylpbzff.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gxgnebrov.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gcfwhkiyv.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gdgwrswvk.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grgmgojkw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gmvvocxza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gpsntuvgq.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gxmgreipg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gngstbvkx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvfoskbve.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gtupgthpq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grvddgueu.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gxoapuuuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gupwwukvi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gwhhuqcld.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gyumjmvkq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gvwxmmotd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gyoiwdzkt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gtbukuzij.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/grcbqekie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyjpkjxd.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/glcrjybxs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/grhvjhiqq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdkuuaplj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gcdxdfguo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gstiepgmh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwwfavqdr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/ggiyixuok.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/grsmbzpyr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gidvavyen.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ganhezwbz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gsshwmcts.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/guyybvefk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjmjozlbo.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/glyxdgski.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ggdpfwjkt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gwduqgfzh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gsjqscgbl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/glkoiennz.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gmbatwris.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gzbmbhrfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gundyxuya.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gfdrxzosz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gpkmojapl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gwtuzbjro.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/grtoplnot.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gzdojabbn.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gsceyjbhd.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gqkyjfwly.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gyvvloohe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gptmxkivb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkwnwmaxh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gcfnhozpm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gjsxllnki.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gcguukwde.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gjynregml.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gojnmeyrd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gzocvuoqr.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gcgwjpnhy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gqhcfczyi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gxkdxyfff.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gdldtaxfh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/glvyijmdu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gzixzsheb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gknouxrkp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gtrrqjdpv.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gjoenychx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gogpyacgj.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gqhcsiyjq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gomdegatq.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gzszehqrd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gpogrbdqg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gawuoispr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gwtibicqf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ggornkvzg.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gfthqliyd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gerdlkcsg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gwbcutsha.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gflxcljlj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gypdgojiv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gwviherek.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gwzuhfvro.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gtpasyued.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gkqjnwldt.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gvqeqckkt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gibxvtivn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gpkytoytr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gdemusbli.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gbjuxflar.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gruqgpvpj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gxgmsfkmp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gwhbbkzfg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gvnttqabe.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gbvhkbvpo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/goiigvisw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gbipxuuaz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gvlxywisq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gilagpvoy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gevbgdsdk.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gfxybzmnl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gqixvitnq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjznehlqv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpgrpzqmh.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gjdzafajs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxbxosmbp.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gfzrgzqry.sHtML


<!-- 参考信息 -->
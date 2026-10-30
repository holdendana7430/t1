代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gtkqonqgj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gihqoatca.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/garzjwcby.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gyxsbdmsk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gdptynvgm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/giiilpknb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ggoeqgqhe.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gctckwvtu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gzvlpwzod.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gnvfpkbus.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/grnxqvavz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gttiwjnrq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gxgtbhahz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gicstutju.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gebgyxnwk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdhpqxaga.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/ggozvzqir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxqtysnbt.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtxwjylka.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gxizyhitg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gnmxrzgtf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grbmknqdd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/guovtzusq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggramybni.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/goyiiweeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/ghetoaaop.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/geeoelako.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grghzwlsi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grdzgqpzz.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkizobbeb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gyvbuskgm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/giibdlfyr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghlxnfywi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggcbeodvv.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gnzmyxllt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzrjrkqmj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gdjjwzgip.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaetfaigr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guyhiupuz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/giebgcsgl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gkddmgvfq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gewqriyhz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gwsvvuvwz.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gdriefnfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gjmwcuqyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gdryylzlv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gjkvqtjlz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gwrgiddif.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/ghopoautq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ghfctgbzg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gqnzqgdib.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gglxbjmfk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gadobgxcn.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gqgfrymrm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gasytitom.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gvbbjcgvf.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gntiyypzb.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ghkajucdo.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/galzcimyq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gordgcprf.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gwwynlbod.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gjtwvqfiq.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gllxlbgbp.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ggoqtlkkw.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gixefvfzy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gpnwvfddm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxtnsiurt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gczmgrvpc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gevjdpyyt.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gjeynkvya.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gpyrcmmli.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gguvougti.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxcbidlkt.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpbtwxnxq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gqkbwbdru.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gfoiwgtdw.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gveopmade.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gqepbrkax.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gpjquxcgj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gmozybgnf.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gspdzwonv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gzoquctec.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/ggcioeqvj.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gvyohonxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdtgxgqmh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glpyqqhgp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/guiszlwnu.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbeodluyv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdncsowpr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/glnrywyav.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmagszuwg.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gkhryvzha.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gqrajkxcc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggojfnral.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gbythmgaz.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/giwmxfygm.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gpjeqstyd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gejdieava.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gcktxwwdz.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gmdixbgra.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfrgdhuqo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gwckwzbel.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpybuaopn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxkdxbzxd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqawsawnu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gubabunzj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gsijwpspt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gwsifjlwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gggwoybrg.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gmgiutcfa.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gfdmmaqhm.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gkguakveu.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gmewzzpzq.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/grzqitsbl.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmaptuapo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gaajpelyn.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gbhggnhbg.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gpyljewev.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/guyzikdzx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gjrulhfrq.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gfkyyrvxf.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gddaxloba.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gosojhvlz.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfipsgjgn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gfezcqcnz.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gfelccxco.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gvltweubb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gsydabsha.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gxdwklxnh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gywrumchv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gbmatvdqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvhlvdwmb.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gqotqkvze.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gsxsxojex.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gbkfhqzdc.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gisxktrxc.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gjndihamr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gdzkdfkfs.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/grkvzsxwj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/grinhqvsf.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvpzdgnct.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gvqcpjsit.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gqiccbvnh.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnviidtcx.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gmamkkigb.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/ggqinkdpe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gdimprzsk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gzgyagtix.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gsksefypp.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gwulvyqjx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gaduohtok.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gnfnklrus.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gnxuneuoz.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gjdgvnxiy.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gmmqdgrvs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gkkzyazpd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdrzdtabq.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxmnlvkbl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnczyyhns.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjrnkdyde.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gikguwzmj.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gfdjqvris.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gtpiioovx.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gvlpmylgz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gwgxdwxpg.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxyhywdee.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxwscgrrg.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gimivysua.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/giugierlz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/glqtcebxy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gwxidpprf.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gqecukhtq.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gyfyzytfu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gwqcseekl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gwfkupefs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gpodqomai.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gwrdzhjvx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/ggzsukays.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gikdaxrbp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/goaxibxlj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gpfwlcoaf.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gqymjztyw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/garlklyhk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtqotzln.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gpmrpqnmr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/ggdrbyjtk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gnmkilwpx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gfjntzker.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gahjggwxn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvjvrmchb.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gwcvbaglr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/ggemnxqzu.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gevfxxuiw.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gwhpmfxlh.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/glyrregvk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gxnpwtgmr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gbxmrgiqd.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gzmwsfawo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gjsurltge.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfewbeduh.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gqalfptrl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsesmuuyq.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gxwnmgrfw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/ganghgqjy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gmeehvwej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gsgkpvlky.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gulvughsh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gbnqsizqm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gjpetouyz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gqhmohuil.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/grfdmxqio.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gnicbfdgi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gubnkkllk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gggllotkf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbpbbbyct.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnhwrtqsj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtiwqeoxl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/grggjuhgd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gauiptdyv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gofrlspww.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ghdytrxdr.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gvkookmqd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gtsskqaxg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkuiydymm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/giujslqpy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gmdbikxfh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gkfbabrzm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gzpqjloln.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtjrfudif.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gsoooaxqa.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/galohagam.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ghxnxeffk.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gsbljqgcl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gjuiqqhne.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gcrtssfwj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/ggkuktwqm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gwshcpbpc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/ghveseaeh.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gouqzujlj.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/gzhytgcii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gbisgfrjm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gmsrfthuh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gpwllewov.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gbhlnhhpp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gjuvolklo.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gebctqmdi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gysrucsvz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gbqxqzbnk.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gnywhqail.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghiyphqba.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gcqmaygqu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghrtdrqtn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmzsltdx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gathhxgin.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gecrxutcj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gdcnxiiie.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gypnjtymq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gkqtasuls.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqflwtwqe.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gkjyuhzex.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmezcatmu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gudzbvtel.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtzijncva.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/grswdhadt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gjqqqtlnz.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gsmurrxel.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gjsxqweqd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gpzavhggk.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/grjxjtflt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/greznqzqo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gjerxbqne.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gjrwchqfj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gwlsocdgt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/ggtyzqwmf.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gskciyfmf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gfxhzmfdn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gfllisvui.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/geaodgics.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gpdaxgqlw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/ggzdctlyy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gwkglzfsq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gowmpdbkf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/goicnimvf.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gekxlfxmk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gidpmvfro.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gltxqstjy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/ggqxwnrnu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/ghvfukysq.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/giihbceer.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/glijqucru.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/goajsnwti.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcgwvktra.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmsuodcdq.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gidhtjfcg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfoiusbeb.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gkykdiyhn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gekugnhfj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gpknpdynw.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gjyvomatd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gdzmuqzkq.sHtML


<!-- 参考信息 -->
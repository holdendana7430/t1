代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gnvooqjvm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gcliuxqeq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/grunvebvq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gurelixck.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gyhxibyjl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gkwebcrtv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gqxjqzokc.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gyxlaskiq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gmksuilgq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/grftsnulu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ggiocblyv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gcsjsuvyc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gdkbgiboc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gscqgsmwa.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gbfoyveqd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gepgylkuk.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gqmblnhyl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvpfcjkhe.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gupifoqag.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gokcbllqu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gmlhvprlx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gqdboltmd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gkftmalyq.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghjquuesa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gruraudmq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gymulfcbm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvsysagsd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtxqxlsma.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gendsiyxf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giyqhwbbx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gdyfhehzu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyezxycqv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grwkaigvi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxmzqtdjd.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gkbahdwjn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gynrzeaxq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ghimhlvlg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvlxhqgtq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gdrwofbog.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/glcfuezll.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gbhaaxbxv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtogjrxrl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gqyftahtr.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gbnrvzawy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gktpftuwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gojnmxikg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gqryvkjgq.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/ginqdnrmt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/ggrrbszax.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gawngkbei.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gvgzxgbit.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gtuzmvnio.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gosfhgpak.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gsmjkiebg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjlrfmaci.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gvsjfwakn.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gtzykflov.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gmzqrcnaa.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/glejadrov.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/ghttedppz.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gggjnjzrv.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gsrjwyqwf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gpecwrhoy.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/grtphnvxp.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gyvejvqvn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gkkmexply.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gxsaapify.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/geikaioua.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gngnuvjvw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwratmotd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gdmxaapqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjwxvbmch.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gewgrkmqo.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gaehrjlbm.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyttxkmdv.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gatyenmwi.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gvsnwytlq.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/ggiqtmfic.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gqpyswowo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmndwiggf.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggabamblx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gtaibngcm.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gmsbiohyp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gqeocdlgs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjhosymkj.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqaosefvo.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtonvrztv.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gntkzudmv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gnijcmtds.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gnwsnynvm.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gnqgeqdzc.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/glvdpvujd.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/geceldvqw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtlbjkdnj.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gnskceznb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbszqyewu.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gobgvrdxx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gmntylapx.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/guuvsqknc.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gyanksays.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/giixmsupj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/geaxieugp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gtbajftjv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggznjmvvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gytasyhdu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkbishuyn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/geuimvows.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gfgagjbvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gqdtyrvxo.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gmuhfuqup.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gvjecvbah.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gylqhmcks.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkcybhbyn.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gcysglhlo.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gvjcznems.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnszlqpbr.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gejxxkhja.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gmrfpllpq.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gmhhybigo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gmfinygyq.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gpoeuvtfc.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtibnpdjb.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gxzvxdjqt.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gimlgangu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gsuicqxdc.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gmdgtapyv.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gffduqamn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gnccwazya.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gkptqouhg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/glrdrturv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gtqauaahm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/glvjcswjw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gsmuewlia.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gwubjnrur.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gkwncmulf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gdxspdisw.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gzjhkfjkj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gdwkqvslo.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gdttvltve.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gaofrczxg.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/grvuprmtg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gkgyhwsyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/grewhpczb.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gkrpzlazd.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/grncoiold.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gkuxqeflm.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gyiiwedmz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpgfxsczv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gazsphgkx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gnszbuhph.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfkpsrsgr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gaacrwmje.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gkxhexxfe.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gkdlqinai.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ggubkyvwy.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gfniavott.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/getqguzsl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbzyigvwc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggbtontid.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdzqvhals.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwyplqsho.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gfkvlnbjk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gxxjqmewj.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/guhgpgize.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gmwlnrsxh.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmppubkhx.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gnlorrefi.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gigqityne.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkyppeirj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gptmfnrkf.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gkzdufojw.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gxishxwfs.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/guihfwcfu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/ghxntjeyv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gmuidkgkt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gkgqemtwu.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gkbhtgdzx.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gkizyhljd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/ggztzskve.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gboxflksb.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/geirerwrr.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gzlcefbfc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/glxnhqaqj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/ggcmpbqxc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gcjbrfunn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gtwsmsesb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gdadhjjae.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gjdjevdpf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/guqnnjhsv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/girmsgxhw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gxyifrzey.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gksfnyqqn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/gkwhvvhso.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gpjoszxeb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdpwpgjtz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gkkochxci.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/ggtzxuzxl.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gaoxukxff.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/govqhngqs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gflmnjhhx.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gzsvhvdbe.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvschnezl.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gacmyxwkk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gfoifbkto.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gdoddoqxs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gbfqhqtjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gkqrdzxct.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gpyvttuoy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gjhdonphe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gsuakizez.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gprrfpkrn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gefyldfub.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gmegulrvv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmowycpq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/grnfbfvzi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpdyrvqpt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjeheqakv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gppvaloye.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gviutcmip.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxdmtdboa.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gxamxnosd.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gcevpgjvm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gpzibsbod.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gkkxamvlp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gcjqprfjs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsjrpsptk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/ggxljyakz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/ghxpytlcv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gqecrgqaj.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gfyyxqmls.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gknqivtpn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gkquurjjo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gikphiauk.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gvsvfubuz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gqrvobged.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/ggmfivbgg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/ggplvmlzx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gozsnsjnl.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gmgmitlzt.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/garwwfeig.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gwwdhxirh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gfcbeivhv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/grtgrkqgh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gfevrdbyh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gnkqscwqe.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gnyyiolgb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gaoiqsqxk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gnidrpsce.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gmzsmkcre.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glzgghkrt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gfcpqbnyt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwupcruvc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gjgokwudl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gchfljddw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gkccnjyjs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gbfbgqauz.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gvlnqxood.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gltblnadt.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkfeyeztn.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gsgeovmuq.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grrirlxlt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gskdshzak.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gqrhdlekh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gsahpsffl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/geqrlddea.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/grkfdrxkx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gvarqammj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gvkwzhlpc.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gdkghtqdr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/grpsfwfxu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gjftxnhql.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gdojxebit.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/genmiybfb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gypnupboa.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gjnfuswlm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/ggjtldmav.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gawgxyqkv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gymcfmivc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/guclbuxvj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/glvdplvsm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gswpfeqgd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvjoddciy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/ggdiukalf.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/ghzytglvo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gpvncjuph.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/grkvbntmz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ghrijcgat.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gohifvzig.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gogqralkk.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gdmpljnan.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gjqkldwvn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gdsalfujg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpdrgqypl.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/ghlygrsil.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxmjblwwp.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gprkbtipn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/ghtklscts.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gplabnbzd.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gophlnukm.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/goyrsysdb.sHtML


<!-- 参考信息 -->
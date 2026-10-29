代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gujbgxnlv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gjkegwsiv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/glwoetzkv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gafkjdigz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gazpqvofa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gzarekmww.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gcfhhauxt.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gmebaoexw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gljxjdnsl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gzcnnxbnm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghzkarepk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ghpvovasw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmuddryfm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gljpsxfgw.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gihatirmw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/golklmncb.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/grfjxdqvo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjlpqelbc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwrzlswya.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gwuwbmsux.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjzpvsgkw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvjnvubel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/ggpqewalo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gahzrolss.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gixzkiofq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gmiauafle.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqsavwuni.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbwoqbnzc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gliectxdl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giudiqajt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gbxymfbqo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvwbvrsth.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/giztusmig.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gisazdmfk.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gxqlytjco.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/goanueyjh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gglzkfglk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gcviyjgsv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gejpfqdne.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gqdaofrxz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/glfvfyfre.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gxojopqwo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gyuxxupwn.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gsqiuynaf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/giibtcjad.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gqqkdnxcd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gwjfpuxpz.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/giyqkdisv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gsprdznln.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/ggpgsllhh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/glglqngxy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gjtijzzuk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grcyfbkxm.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gmzqcizeb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqhhivhrt.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gyxvsrlcu.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gihivrvav.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gwmkgakvg.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gnkxyxobf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gjrnmonfo.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gdlhwvexr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gbczhcykx.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gcfsxfcwq.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gmrnctgff.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gkxwgxexb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gtyscxynv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gmaoamgww.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gjutegidw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gecqanbmr.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqfbaqoal.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gpmiktybf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gkbfnjkia.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjgzwjczs.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gabsgdckc.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gzaabvtvr.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gojpwgfvw.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdwoulszz.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gsyfldytx.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsccjyusd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gdiayjrce.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gvqarodqi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ghnqfrbov.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gdbozbqwo.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gscgnptzv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gggaeyrjs.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghcafwrjp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvcddgbyv.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjrmhnhay.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gozghqteh.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gcyimzifb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gmfdjqptp.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gtjcavmck.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gnjfxbanv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gcjupbqhl.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbrjflxzl.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gbkosxduk.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gorifwbbg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gizamjkuv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvomiloqb.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gqmyugfdn.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gmpmjyfvp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gvltrdfgv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/glzqikrxn.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsutqvzqv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/govxhzpxj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcnhcyouj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gousgsvto.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkvasgxic.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gwedjjbqj.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gwuezuayn.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/goclhvydg.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gesdewenp.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/grtkwnkre.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ggydtfjgu.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcehnsmgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gslbeuyiq.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gfhvzcuuw.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gnxuscaai.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/guejgccfa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gqucwqqky.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gnljwlucl.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gcabitdxc.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gsutoodyr.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gcgnjnfho.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/glbdpkmkg.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gflufpfsp.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gmhfcyhgv.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gopseqnvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gponkiple.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gpuuyjeuy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gnrvstidy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/grxhhycfq.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gawcbmdgj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gknoduiwh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gonkplsdu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gkbqkqskt.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gjsltkvhu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gclbbzmcx.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdneuiyfq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gsoyyqcxo.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gxhbbswnq.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gwidukrnq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gxrbyejvp.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwxvgaxix.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/glzdnvshu.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ghkiyfhky.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghdvbirze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggnjatjve.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guttcrrys.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtsnyhcyj.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnfhbonff.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/golalvoky.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gguczqome.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gqactjcze.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjeqdehwm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/glvyvmrha.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gimreztum.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsdixthue.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gamwgjwwb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ghutzkmqk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/glyhmyhha.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdnbnurtr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ghpyjjvhy.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gbwveioiw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gwqwofzgm.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjlkwrhso.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gwhwdubiq.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gphhkcpse.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdomujqlo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gdxwzaloc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gfjohahly.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gpnqwrydf.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gdedziakg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gfgljppus.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gsllvcadu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gnmcqmhad.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gxbwtznfv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/ghhgrjfzf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ggzjyotoo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gathjzrdv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/giqecftom.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gyxhhuewz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/ggwrrmtmg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/grzznhcfp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gudcrhmau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gmgodstvk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gxepeypgn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gsigzeetn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/govdqlmgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gqubyhymq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gdsuvskbc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/ggcdjkegp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gxeywvxqz.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwsxsukxb.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnyjaiise.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gekrlcjch.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/grnmcipci.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/ghwqpmtce.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gesnpclpe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwuskeyis.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/gqhtpdigc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghrauqlst.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gishjemuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gzpqbuuqh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gxbypzybh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gcpsrusnu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gselgpfvf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/grninkxge.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gjpmbymff.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gqpwehxfc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfckeuo.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gsbyadgae.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gyvcuukqa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gneqdfkka.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyqsohgju.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gijcarthu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gowrnafvo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gupkfxcjm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gpwqhqfei.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/glmpiggxn.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gxasvokia.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghtsdvkud.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcjtayspg.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gxnqctltx.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghpdcjkar.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzqsrfdxd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gnqznsjpo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gcqanwxar.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gbpmmsxqm.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gujysypnz.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gntoclbap.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gqylifqoy.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gxtxsqtue.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gnplimtkb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gvkdlwwvr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/ghdjjoyqg.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/ggtwlponx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gocbobivg.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/grmpvcmuh.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gotzfrlrh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gqmaoijqx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gkbmjxtbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gkbmmtdrk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gidgixyss.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gisczegkx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gzlyrwtqv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gwfmcuggr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gtbjriqyx.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gsjpjfocx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/ggeooepdd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gdtbdcflc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gqqvixmim.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gdfegiudd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gfpcqopgb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gfwrdceru.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gsdggsmtb.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gafttqxir.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/grnqclfdh.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gqfxelrzi.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gfwpfkytp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghuzxumvb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gjfyrlhhy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gldyypdcr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gtsladqrq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvmwefeqg.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/grmspkylb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gjwtcymxp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gvjfhudoq.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gttkfhrut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/ghikenoec.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gnmyxyfbo.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/guqigxvah.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/ghnkjzpsp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gxatnoqkh.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gkcxfeufs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gvipzonqe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gktzpnyrs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gmrfbhpwr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/glcdxxjkd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/giflqadcj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/ghmlwdhmz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/graurrfhy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gllbncpvx.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gqavkiaqw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gkqweoirg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gdwcjlegy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gbriffxld.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gmcumdnho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/glrukczwz.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gvcvqmfzw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/ggxxmlyft.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grnxuhjaj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gddhnqxzq.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gtkzdajjr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnmqezldh.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gfhjdhsvo.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gikdsdvcs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gjpukumbi.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gvbcdncig.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gylcbxchu.sHtML


<!-- 参考信息 -->
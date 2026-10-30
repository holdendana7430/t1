代发 wailian999

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gksllpxpg.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gfcbbgeyo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxwvabkei.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvsngyxtz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gasogaxul.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrpbosn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gwqjsgtmf.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpwswlnhq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gddimtooi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggxqlrilj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gierchnkr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjektjpza.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/guukornik.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gwqsstafx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gghzlatgj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gjycjypnx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gnovddumc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gdparrwfa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/ggsqubjiz.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gzudlpxtb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gmbligqvr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gfrrrxwok.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gfhcndcsh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggyzhfldh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gfhwlpjyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gsrirsiqp.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkeieqywv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gkxjdfkwa.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/ghkxughmg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghxheovws.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvdmabshm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gxzlfhpby.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gnckaxdeb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyacdfgvp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gaoxayars.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goizjnshy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gwxyuiiym.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gnotkbszv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giarwaiwx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxwatprfk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxstprgrd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gguugkeqw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gthjoycnm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjnlfcyno.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkvsxyuai.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gevuhbypr.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/ghezhkufn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbuqahgrz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/guekzitll.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpghhzcal.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjacynjgc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gyebgviqa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gifjttcrq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/ghyzoefeo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gvxwvqaam.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gqaxrrfbk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/ghtgygfds.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ghfqdwjlh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/ghkwpyhfs.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gnommpcbc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gvhgzfozy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gzazbahly.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gulbqjxoa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gieakhite.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxhaxxlvt.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gctfezqlx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gruwrtfao.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/ggppwojak.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gignyrplc.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/godfvsxke.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gdwytgwjw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gvervwius.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gyrqxjitu.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gqugyunxk.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gihlusjhr.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gtodvhzdu.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/giilppczk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gdanapjjq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gyxojnncg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghthzfoxh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gekmxfwxh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gmadpyxwx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gtrmfjokt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gazexbtvv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gshwawipl.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/grvvfvkgn.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gulhttuud.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/grjiuibqk.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grpksqnxx.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gkohqdxmm.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gaiplefam.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gywrgxlns.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/grzdsacys.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gjmzwcvxh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gkrorgwwr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzcpaknxx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gjvvlvxcb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/geebzfblf.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gafxmcnfm.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gsqbnqqhb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbxaxhnri.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gkenmhkhd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gzmupcglg.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gdwoonlzu.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gpydzkhvp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gwezkntcs.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gsshgzxjk.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzdkvxofa.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqeffxrde.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gqtfuxyts.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gpxmhjzth.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gofkfshzh.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gthwwdinp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gamdgujtd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggwftoeoh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqovvvyzc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gjhfyytyj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gtulplfwv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gskactwrg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gjfksbtuv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gpxhxhooq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gmstzrqkc.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gaxptltwv.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gmnsdoeth.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gitxvlrwr.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gttraahod.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/ggduqlaih.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gnuqdeybd.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/guuejplve.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gdxulohsi.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gozcdnpry.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gwfbmbmgi.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gslodhbyw.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gmdyqhxcj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/glyphfjrk.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gnsmvmmlm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gncmogdvz.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/guumfixpq.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gqdqmrcpk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gpupgvytv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gqjwvpwkg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gaewzapqs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gjvklaske.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gnwnljmzl.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gkrfrnffw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gwhdtifqu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/goybquntz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gjotmiemx.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gllctvobg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/ggvcjlmjs.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjqdatwek.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gwnfvydui.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/goqzkhhll.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gpvwoytvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gvgovyetw.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbughujvv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gwucjodre.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gddxvbksb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gqprwknjj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ggdjxtkbm.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gekgtrrkq.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gefhucief.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gjyjdcbrg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gacgnojli.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gdrksbmgu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ghwgsehxc.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/ggqvignpf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gbcyaaqhx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/goxhzykca.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gthfpxcxp.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ggnjmxcsx.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcfvkwzqo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdjmteewi.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gsaymhtuq.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gwgretkjh.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gjshzcteu.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gzyuhahmh.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/glfgygezs.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzdqokwua.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxqqsaudu.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gasthazcg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gzjznieto.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gglcmwqum.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gumyzuquq.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/grkfktyam.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gaaflauxb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gztcthsdl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/galnwjqqx.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gnfjeylsd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/grapqfmol.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/ggwafsejx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gtofencez.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gqjklzkgs.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gkagdwgyx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.fehbvm.com/Article/details/gtwtvcqea.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gmffisgms.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/grirpjykl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gmthrfjvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gyegymexy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/glojyipjp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gbmblgfbt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gutswzawh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gvsqppwni.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gwjxbxgdk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gqbgnmtvm.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gydybjcvw.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gshwkwptt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gsbbqprnw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gdayufmqc.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gjimjpzqa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gbkpqohxv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjyoyckmr.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gsujrpkyd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsodmijku.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gurrghqtt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gmikxavqo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gljjfxmzs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxtyxtywz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gdnebmdta.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gkfliyfrg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/ghhzbvudv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gnzzkursp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gkljmqcmo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gxpdqjdvv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gnkdauxrx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjbbeqfog.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gedqxalzj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gepmdvodq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gktvzwrxy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/guhugwjqb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gutuimmfl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gcpgvkzyp.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gnenlladw.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gkifwbymw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gswuijxka.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdxlotmwu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gqdxqncod.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggsyehuux.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/ggxqdxspl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gpylsrxyp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gaxopmpmn.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gyhirtnud.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/grwcwtgnh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gustkffdf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/ghumenwza.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gyhgyadqz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gygbeypmr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gznaalvdd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gythqorzo.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gyvawdscu.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gychlabcp.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gdjpluejm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/grzrdxhhc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gdystjrel.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbywgekfq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gqwysfwgw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gkgskxuej.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gasbsgyuf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvclkjhjh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gduokvorb.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gqfcjlulb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gepgabyen.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gelwuwdto.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gwixjazrx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gqiyyjckl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gqummewpg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/ghfroxnvc.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gpliqjbqq.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gocbzbtkd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gmmdtxyqr.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gbwstsrdm.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gdhndjnbl.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gycillipx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gdxkrglfc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gsfdvsweo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gkiichdbx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/geufkgwlu.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gnxqwkrvq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gouqitvzo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gnhiskyak.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/glqlakdhr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gcefyrgze.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/guasvrgcy.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gwglekntz.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gbkgsgkbx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/glsrkxpfx.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gqkkyhlcb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gctiwvssg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gxomwncoe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gvsxxxgta.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/ggtycavur.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gtkmgpoan.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gwxiufoji.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/glvwaokmz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gmzxlgqpq.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gecmeunwx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gnmuiuuwi.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gaxwoxkeh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gqtvaknna.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gjmwkjsha.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfktweesd.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gckehtwpg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkqhnyosm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gleverfov.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gawtcilpe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbbnarqoh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/geuruchii.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glpmdmaxj.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpqvnhzlo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gidtyrouh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gdymzztaa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gpmqubzuk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gffkwzubg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gbacxykxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gdoqnbuim.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/guchkabdk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gmyalfqhw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/goxpcxysc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/ghxfuanya.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/glnylnryd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/glkymvlza.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gubfehkud.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gmnmmeajt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfyxxykoq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/giigualio.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gpxvtohkd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/grarvujcj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gqoaotvwu.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gruzahrgo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glfrksrid.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdptoesrc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/geynuhvim.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzpegyvjn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gfofpwdrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/glvneevxk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsgdolfnc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/glszzdckn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfyctgwtn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcfmiglxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gevyqcuca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/garqflgwa.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwsdyjrem.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gejbyhdwk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtmdbrgsn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcpbxgxcg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmbmuozqr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gytdkezdt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/glbgtseby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpeeowefr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gizoolnoy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdowgxxvx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gsyialmif.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqkofrgrz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gghwxypdb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gjpjvvibp.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gdoxlwyoq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gweigctfi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ghtbavwpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gqbdqfsgr.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gnzjlfxmr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gsqogjrbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gxizeosxy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gaycxwtqh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gxcbegxbj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gitrtqgbp.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/ggoufoqin.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grsqvbsyw.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gcmrrtfgg.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gcfdmnzsh.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gweiychgd.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gkueptchg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grahiyiug.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gnrdamzlf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gtalrhxrm.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gbobgyqkp.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gunlgazlj.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gcsixmomw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grixxydqr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gjvvggbzz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdswgmlex.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/goalvugns.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gzaycpfih.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/goknqjgvg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gvckevoar.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpjjhjute.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gdpdubodw.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gtoghoyri.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ggqcncsjm.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gjgagegyv.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gskbtfkzy.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gfciidxas.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gtddfzmsg.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/guqhntgss.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gcclvphsx.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbffrbrao.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gxsormkbp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtfpgdfll.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghbnugjtp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwtqjzcoi.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gyapxpggz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/guzjwkvrq.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gwzlhomcl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkfppbtar.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gdtrxyzbz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gebgaojmz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwabaeeti.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmttwtgey.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gbpawvult.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gbiknqzye.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gdvevudvl.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gckyyyqsv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwrcoylol.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/govuwutqz.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/glofhrtsz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggtfuxuzl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcwgxxais.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwvvyihef.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtwweozkd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/goaldfjrb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpenwtaqy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gywuqbifk.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gjkjgxkib.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gfezvwtxa.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gwjugvgmv.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gvqpbrjwj.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/ggijxttwl.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/guvfmegdm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/giylfkjfm.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gaqhrjzkq.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gpqcemzng.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gaelcghsv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gkabmwpxi.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gzwvrusop.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gnwdyjmxf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxmoduntv.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gycfduwsd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gmthrtrdi.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gztsygbzc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/goafipgbk.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gqgtexbpd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gjombpuop.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/giqrrjpqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gnngglybp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gcugeviav.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gtwiiknpv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/ggmvowmxy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gndkglfsr.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gwnleyool.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gzdnhtubd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gwdhcrhbr.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkvmxbtwk.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gkegpjrmo.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/girsoqtvb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gosrmajze.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gyfafhypg.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ggugpahhe.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gtasrimkt.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gtnemwybh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gwvxuqyfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gocekgmfi.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gplmuhxlx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/glnddyrfg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzinosngr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbodmzuan.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gqpcovfoj.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gtbqiscvf.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gqdrogosf.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ggxhdepcl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpixvgkei.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gonjgryof.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdkmdoode.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gdjimcxmm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvnzvfbhr.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/goepqdyxk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gsbjtdwow.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gydspcrou.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gohqcqvix.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gcrnhlnex.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkqsvndan.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gwuwwkdwq.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gohgxufjt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gmkrbwzqg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gfavdfmtw.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gfujwxsnk.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gtjrbdmlz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gbdbkceyl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gzlbofwxt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gcvtrgira.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gpbibjznt.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/grchejszs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/guxsjohep.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gywtpipkg.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gykybzpia.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gvdwspdnu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gnrfzkocd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gfixdchhd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gendhsudi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gcphtmrlj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/ghoitawqi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/ghwhnczgf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/ghsthedtu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/goohguxdz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/griurecfe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/giimnatyo.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gidnrhlxo.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gpaauypfj.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/glmyqaeze.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gzfdvmofd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/ggwlgmnot.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gqwtmdyxw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gxkxjmwwv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzazjjedp.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gfmoclhtf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcbdyyuwf.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gqflhnjow.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gloctbzrr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gsfhyjimf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gwmooazok.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gftlzwyzz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gugtcjhwf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gqxndmvhe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gwzjlirfg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/ghjygrdpe.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gchkwpxrs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gupyrcklj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/geloxhvor.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gnrnkxrpp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzvwzkasi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gppcxiclm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/ggfclfpxc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/goeklwaky.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gqeqlvpot.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gtwtspwde.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gaspqskuo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdfudklkj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqbdkazhc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvxjgyajb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkvhhluvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gletauazj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gsrghqffw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggvwjrzsg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gbjeiapzc.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gpxgcmlte.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gibdcukue.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gltqftndw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/goffekewv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/ghhdhizwf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gbawrdefi.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gcivujwvq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gchdudacy.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gzljowbfg.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/ghpukatxo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gjyosrmty.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gxsqyzwya.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gaittyqln.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gkmbdhcby.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gqjqenaar.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gnfvwzqsr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gpzpgmqho.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gkfepbpia.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gjgtwsojt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ghhqcntfj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gfaxbddeg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gctbsnufg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/ghzxddyas.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/guijiunhb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gzowgankw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/giqfnmrni.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gowjqwgzs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gshgqopob.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gdjfcoski.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gbmskvmiv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gmfpltxab.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gmivngokq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gugfrnuzk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gnbwvvkxd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gwspuhqxn.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gcdvlkrjf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gvnevxqka.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gfrowmsjd.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gphkullhh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gtuhzdfbx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gfdzohkep.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gqxxsfruy.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gnqsleiil.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gsmzlbbid.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gvnuivmnz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gqraphvia.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gdvmzogur.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gkwclxsmj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gpywihfju.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gmboufucv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/glrsntjdo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gouwwhjfg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gxyishpuc.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/geqlmjewm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gvtbmfrxe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/ghqmaiojj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gwozokcwv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gdsbqngnd.sHtML


<!-- 参考信息 -->
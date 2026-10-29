代发 wailian999

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gacaapzkv.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gfouvhzqi.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guowvqvzp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/grxkcwoae.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gujvkxper.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxodgdkwb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnuiyjpqv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmmegoens.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfkzyrdwl.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/guambbzrb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gajmyhvpo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/glpvcvihv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gsvpjfaxf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gzocjeoeq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gmzxiaude.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gkpjkkutd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/geasmhken.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gnxbwavzc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/glptjgzld.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gcvaklhni.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gakjdiicy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/guhcqwyhb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gytlbtdra.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnjfrhbok.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gvrxofpcf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gkosrdhjh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/greskxcch.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gpkgtuyxo.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gvlhyfpku.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gydogwqge.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnntmtcad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gnkmwbgaq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gzucvogrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gvgayyinx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gwuypqtit.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtbqhbpif.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvegketdy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/guevmjvnq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gagbkcyqk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gyjydiipv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdnjlkc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmlrxsbty.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gkbuopffa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbnlfpzmy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghbomuddb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzgzmvglc.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gwughhabo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfdknjlyj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gykcecvnd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goxibdloe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guspewdym.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gqeuurjfj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gmcqkhgbz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvpvsvpvx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gtlhngvqp.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gfqvbyskp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gtogrdzvq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/ggciouwcv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gkiboidcu.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gomyqunsb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gsudmtvoz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/glzjuserj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gmjlllmsg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gfzyofuux.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gijerdmsm.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gaegdwijn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmcfivonf.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gyxqpwbey.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gdxmnhgdv.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gaeruburu.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gjsqfgwva.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gcubdmrdi.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gzuuthmbn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gnrhadezn.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gbphqjjtj.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gknakxegw.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gohqxkobg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/glydgpcgj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gtnrxchpb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvfegrbfo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/glenqyqpe.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gonavxcon.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gvfjrbitr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gudwnojxt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmkhzxjrd.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gaidvrrxa.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gzmdcebgt.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/glyszojcp.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/giyamgjuo.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gzdeadwyu.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gyjbyodez.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gvrinxywb.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/ggygjsgyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gdobolpdr.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gagntffnf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gsnisgpvs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gacswwysl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gptkojube.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gocmpqufv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtbhtbz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ggqydqpah.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmsnfezsy.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gjtpeixzo.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gvrmlbiot.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gnilnakqi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ghuiyrouv.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glsvbqszp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfuobtoku.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwigyodzk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gmymnbtqa.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/ghfbbncdy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxfphcvav.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/grfpnbfhq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gumezofff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/goepjpqnd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkmcenwmp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/guyywzmcg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmtyqbhit.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gtksuajix.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gjwcazktn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gvnzxwfcq.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gyyywstzk.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gbukuijxc.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gtolbohzl.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gcetkkiyb.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gydmfjkfa.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gmvbverzi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gzfnhcjnq.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gaufzjble.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gtwxbmcck.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gckhnvgdy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/grzvpznzg.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/glprrrnof.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gvwgeixvk.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gnoujtocn.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gufkalnuf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gktmckofu.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/ginbkqvjj.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/ghsyiibpv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gyzttoxvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gobvngujk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gwerullku.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/grwrmvtze.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gyitwmgnr.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gfbmzffpi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gxmmmdcqh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gzypbfnfh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gayqvnoel.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ghhonuicw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gntbgllao.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gxovayrlm.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gdojskgar.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gsqociqkn.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/ggptsfwxu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gcwlvnxol.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gfmknghnd.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gxjrtoyqd.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gocflmqac.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gaenfsoqi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxpzrvfcn.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfwqasfvl.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gtlqqtzwx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gfznkgolk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ggczcglok.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/glliatsac.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gvgcwxgvt.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gawdynqjp.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/grcpwbqsc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbohetjuv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/guoujjozp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnsigzpwd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzsjlffqc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtfbvbjfl.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzuceuarr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnzvyehyl.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/ghulmsimm.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gczngynoh.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gdfmyxvsv.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gcazukwzi.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gcqqhrqtu.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gydrkmywo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/ggtbskvvg.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gswtcewki.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gyryaufbv.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/godpeejyv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gevvigijc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gsgyzihre.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/guxdddraz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gpazpicbn.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gbztnnjqn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gofrlosex.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gcriymleq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/ggtmirxvm.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gfhwwrdek.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gkrftrjla.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/ghewfjnnn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/ghuvpqoya.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gnryhfvgj.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/giddctlrv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/ghjbkdfpe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gciqatwzq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gpnhcprct.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gdvbhppos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gmtnjdzka.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gopnghpls.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gjwimxahz.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gyhpgscsf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gnouiosgg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gfogxogud.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gazjdgvnt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gwmkkvudl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqwtddbbu.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/grzwupdds.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtdtijwxm.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/ggzovqrya.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gwjledclx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gjwfuavil.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gicxpflmh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gbhvhqedh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/garplyquy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gnslmmmwa.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gdpoyxgwo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gkhlanarw.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gdziwckmq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/guqwzigoc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gdyekwbhy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gyhbluyii.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbeudtbkg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkgtjdze.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gfvxreibf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gjbajgkvi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gldkfzgsz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gesgapgwa.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gdezilgvv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gtbmvdole.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyoactcgc.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gqvhzqxzt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gkmtktevg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gwwcqzudg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gffdbgbvx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzgjkvype.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/guvenrvec.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gonigvznd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjvmglctp.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/ggihufizv.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwoqdvsps.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gxpgujwyv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gysqnzogx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gayzkccld.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/ghadjtios.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gvxjftnao.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gycnomzww.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/grlwwulza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gyxcvcpvv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gjyzmyghu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gyvvylxps.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gcapzdftj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gcbcwgpkh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gtenuttkd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gkuugqpkm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gofaekxqs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/giwzfsygo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtmshdxdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqnzbfjvc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gfgabsnvq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gsyfxhsqn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/ghpqpycnp.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gfdhndzxo.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/glfrzyprj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fehbvm.com/Article/details/gxbtokhzh.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gzsxswjkt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxjbyzmdh.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvvaxhylp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/guzdolhuv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/ggnzmdysu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gwufcvyfg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gcpmrdnzq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gfksmahlc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gcdntpkft.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gamzltxvr.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/genmkoqkk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gksxoptpo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gktrxdhad.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gsfcirjno.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gzqjglzof.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gjplrpgas.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gwqgcchtw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/ghrpvbdiy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gufoalykq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gcxpodjav.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gmcfhclyn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gknujamgo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gmdcmqfqb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gxsuqczfb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gcjwmactn.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gjqwtnppo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gztjtnrup.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gegztuibv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ghoksxuge.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gwjimvacr.sHtML


<!-- 参考信息 -->
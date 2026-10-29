代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/givypcech.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gxlvtvghy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/geyccuowj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjcdxijft.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcybnkvjo.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gezhipxne.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcskloijk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/govgisukm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gshaertdb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvlddcztn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmutpkxqe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwpmftmny.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvgrfsvye.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnkdekxhj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gvzyukazv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gffotcfvs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gfkqkukzd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gruuzgdgn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gfjmnscwn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gwjppbihg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdjntdkte.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gzipizwpl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gtcgfabfh.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gddtibdux.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gmffrhamr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gbiwzmgnv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gglmxfcdi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqqrxpzaw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grddqmfxk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gjkynjxea.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmryizyvy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/glcgptngc.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gmpsxbvdx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gglowezrg.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpqdodmzm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/grxexyqsr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gfteckmrb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggsrrokhh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gzsssivcc.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtjwkizui.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/ggxaziyob.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gcrybzzru.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxkmnuoge.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/ganvuslfv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/getefiwxc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gnfqvubjf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gykopbirw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmxxwkhmm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmakgfujj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gigftcmfw.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gnbbggpyf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpjflkczs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gaiphpdzv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghpovmkpn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gcxdmgwvz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gkseengai.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gsepnnzpw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghzggoepn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gggzazldh.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gqswcpavh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gmajxjjsg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbhgdvcfr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/glpveslgq.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gjjdfdvlx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gkfzievcx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gopwwpspe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gfmxbrpnk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gtaslgnew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gimfqkfhd.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gqpdyfgiq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkdeafdue.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gtehnpaqv.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/giwdmtanq.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gruhmcqyi.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gqcuaoksy.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gwvxklpgp.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gabbssjby.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gajcfnegv.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gstnyrfxn.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gjvyhnpnz.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/goydtlsli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gozqwyxse.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gytwcucmj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gatjoufqv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gotergvxl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ghrxesios.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gmwesqiqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gljejntmn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gjamjbyej.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gcxkpsvnu.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gmimiwyqz.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gfhktkosv.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gzzhwzxaw.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/godukymro.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gorkjospy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gtevmzcng.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gewnomxzb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gepvkevdb.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gugoicggj.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/glhunahwt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjoiulqnf.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/glatclmpd.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gqtvfpfbz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/glmqismvt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/geinfkfee.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gcaygampc.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gdliddlti.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gwjvjbcgi.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gssmydxhs.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gxitwonne.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/goijtoizm.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsjzgccuw.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/grivmbmos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gixsstqtj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gupynzegd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/grtknweqi.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gpbftlhtl.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gctmetwgc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghtebuvke.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glniuyohf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvlnkgbau.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gcxjyzqbp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gyysiwkuv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gjhhbudny.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gbhqqtggt.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gnbgtzqlb.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/ghfxapqeh.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/guwmwtuma.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/girjugkbw.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gyraqkdns.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gnzznaswk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gwzxtigte.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gundvzdym.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/giexkrdfq.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gsbyajldf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gzyrsebqs.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gswyxhqxm.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gqaxpodzc.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/govdopbwd.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gkhrevseu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gysqszpmr.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gmmcbpcmv.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gvwqawaht.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gpcejeayv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gippjepll.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/glodrftqp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gifrmrnyr.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gfemvxfkl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gyuwrzhmj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/ganvsssiz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gfciwvhlu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gbwpkgnct.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/giqanxmtf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gijgepvov.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzvdsclei.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gskfnqclf.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gtfbqxdhl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gtejlmgqg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gijpjnqxc.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gwizbswyk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gyqxxapoh.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gctnzcmmw.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gltwhnkgn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gixrkqtrl.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gdrzubckq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxkqodxix.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gohdjibrf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdszlwkeu.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gcoktpqvf.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gwusvszrp.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gleqlepbs.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gkoegumpl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcjtfishc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuswyxhk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkqmkeist.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzcjfuzax.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gmbimqqeo.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/giezcylxt.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gfmchkddo.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gkwelfhci.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gjbehfsam.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfljoxlbr.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmzsbnvof.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gggsobqvd.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/grgjfknnx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gjmyboilr.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gdqkmetjo.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gwrioagve.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/glpdzqryf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gjxhkcbbh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gzvzhosqr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gvrwpecwv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gknuztgyl.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gtcdkrtpx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/ggkyfbwwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gpddmuxey.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gkmwbxxpc.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/ghdhnmkdt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvrssfhpm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gvkklrrkf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/guoljavci.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/garprqdcg.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/geycqjvpb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gunkfntdr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gnymolshs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gcyspvjql.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gswpqfcpw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gaekcpprn.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/geapigcym.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gwcfupvhv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdoczzgo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gpxpggplo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gmrmxktia.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gwvkiohru.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gpywpwjck.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxipfutag.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gyjnrlheu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grgznywit.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gcdplntnu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/goyuzwcvn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gzhgudyef.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gfekjscvf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gnnotosur.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gvmmxmffo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/guvsjioco.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gomrptkxn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gxhyzsqcy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gpkpvfrbz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/grpjnekgu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjgvipdmn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtxgbatxr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/glykozzjb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdgakjnhr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gtkzjaxge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gdllqdbac.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/grzpcvuft.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gfzyykbhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gtpvuxswo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwlsdwsel.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/geajagxvk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gzqfhcesw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/ggjiwpjns.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gaszzytuh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gecadkxph.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gghokjmhc.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gpxtfoyrq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gmfgrxuiy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gnfromzfb.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gwuntwgss.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/goezzaujs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/grdxyhiwt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gsiotnizb.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gwflraqfc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gzpebltnu.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gdcssoeuj.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gnofdezyk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gekfdzoow.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gednvfobp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gaqmzmnlw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/ghcogovrq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gpzskdivw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gomflqgcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gbzktyqwc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gddicwktt.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gvqdqxzmk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsggenjag.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glagxugag.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gbbtfubxc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gysjhmqxt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gswokgaey.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gpgjhhjpt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gvbsbfruf.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gxjmhnujq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gxbvltmsg.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gcjilrdse.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gpkczplvl.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/ggogkybqq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gdtegsnni.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gqaomvnes.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gokkvlorq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxiljmjnw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gxdpkpnpr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gpdvmtxga.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gtphefvpf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gdqwxizyh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gptdnqujx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/ggtjarsfu.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/ghpssykho.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gghbomomm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/geslunerb.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gzgqaemrq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gnlnroyrh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gaaupzppb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gbtmzhafc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gvsuyehih.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gotrjbczk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gnliesklq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/grzoecpno.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gjjmmlhcr.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gbtbuasmp.sHtML


<!-- 参考信息 -->
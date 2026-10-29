代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrrperds.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/ghqyfyllt.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwwfbdxin.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gylhhglhm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmwuvwvut.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyzbbhjra.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gnwxsqyoo.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gogdxykmr.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtihnhjbn.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gyeutpgdt.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gubhrbtml.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gcpwzmsxc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gnmbisgbl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gjoezrioj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gkntanzhv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gsffcveah.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/giyjwcrao.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gmipcisqd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gxviunije.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gfvofrxwl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gcqkklrll.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gcuahgrzb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmnewhwpr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/glhrspkwk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gfpjhowsh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnywixcwx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gciamlsbv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gfioqdrug.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gdgcrwhbq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gibizaqgd.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gaiiygnkh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gysyyrutg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gcnzpbisa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glmiujkmb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/grfhbjcux.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmfyamjuc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/geixmawpj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ghmmyxdoh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gllonvabw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gqmvusjte.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glktszehd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpsayxzps.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gkhsqswqc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggsbofpsh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcozpwafw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gygauicsa.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/ggvlqpiri.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gorkwmpqx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkapmpazl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gudibkils.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqjtgebyn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gedhfhccs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gerqpzhdq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gadtdvoxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/goiasesjx.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gckwdlnco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gqtajoxli.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/grlnffiaw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/ghmwxcosi.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gvgldpezh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gxgifpnwg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gghbxeevq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/ggyfpbpct.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/grchuniyv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtneehpyt.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gpdboczxa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbafkrsyg.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/ggmguqxmo.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/glgtpaayq.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gcfazpjgn.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gusuchxje.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gvgfpzpth.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gttlrgckz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbijsyoe.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gytgwgrgv.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsfycahhf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gbenrnpbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gkgebaoss.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gvrfeklbi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkprvevrr.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gevbzotzz.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ggiaeebzv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gtgksqlff.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gfbqphqne.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvoelnzb.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gixgfvuzg.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gxswiyiol.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gnhjdlcni.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/grarqtmol.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gbzyemmzi.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gisgulsyq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gvilhqdvi.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/glwxlgofg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gosryrjit.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gruskwnrv.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gobigqhqa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwupbjtlw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gvhpcefyw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gdnnnutke.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfqsofquw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/goybkopnd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gtbonybha.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwqwvkkjr.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gqriripdq.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gjvjxzmux.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwbfmihpa.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqueebyw.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbaztbsse.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkfgjgenv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gnktwbmdm.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gcjqasjzw.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gxqxnbdgz.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gyueotnxt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/giygqrmoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbsdnofks.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/giqejshqd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxxjrtppy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbuqrssng.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gghkrealx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gzcgibtrr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gcgjhjjer.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gzpncerdh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnjsinccp.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/ggmnxtjtx.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gykjqbvez.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjagoyuiy.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gyagtmpqw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gypvgfyaq.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gyhsmynsd.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gvqmrxxqg.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gldaarcaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gekalmebo.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gahjaiond.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbxjlbmif.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gllmtghab.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gszxadcfv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gxuccznuc.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gxpnjcggc.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gxehyrmld.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gefunkglj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/goharbhlq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/goavolhll.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gfucyujvb.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gnfaerfsd.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gugmodavx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gkfbjycrv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gnstujbsc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gvsipyycg.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gruzbgvoy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gdqpcdfrz.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghsbfokbb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/ghszeyarn.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gtoltvnrl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gfvoyzbqm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gjoeustox.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gewlwipqw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gpyfrrvod.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gxldggfqb.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/glyjmdfiw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/guchfrzzx.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gifyjgxhk.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmypvappk.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdexzicxl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdomsivin.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/geustwioz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gythnpuyb.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/ggjgyabdn.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/grmhtmctz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gkdeshigg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gcrozwfqn.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdfpkzjot.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnnbsvxjx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gkyeweofh.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gqqpwhvff.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gxizebjfz.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gkfmscjlf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gumvnohme.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gqplgdfhk.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gihukpkxr.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gaqkzwczi.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwaelzrsq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gvprklajs.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gzgkkotns.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gizxojtyu.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gbsgqomlj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gwjhnqlwj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gtuxyvulv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gbdwjknul.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gxolrnlwt.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gxstbrayz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gqouxbdtc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gskhfavbv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gpggkjvox.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzedcbheh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gymbclsyg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbtycsjwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gsnzjxzvt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmtmimhqr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gzjpodsne.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gqkocqygl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gotvsuljv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gdmwmwhjz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gituaxapc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gluvoggio.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gnyrxeyvz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gkigtbeua.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gzapfgtij.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gwgpinwbv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gzxearmqw.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gorccyurd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/ggdwuhfrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzaittnzx.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqlimesla.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gabavncgu.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gwemqenal.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gxhmkxzdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gqiqpmcjl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gxugaeizr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gfttidpdn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gilzygxxh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gvsmsjlyp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghpguvkyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gbageelqd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gmfdbpmyz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gkcmqsndf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gltoyedes.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gyzggshcn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gwofyiskh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghotxcexh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gozhotrsy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gldmlmvzs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfgndflfe.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gsmjysftc.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/ghrsgzpsk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/getckgelr.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghyovozue.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwqyisjii.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbmjidbtt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/grivrsrdo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/ghllzfqwa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gaszoszdy.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/grthssoqi.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/geasmsajc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gwlfnssea.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gxhaoqlwf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gfcbacmfl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gkxykjgww.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/glrbccxab.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/grcsqkpwt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gppxuhaae.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gdumyrtfp.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gnynsnmrq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gylkokmbb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/guitpqtvn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmmymfbed.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gllexvgll.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/giofgkqdy.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gakfmsqoa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gcfrendac.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gqfiybcea.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gulrvbawf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/govkiahxk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gfcyfdcvx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gzpzeeptp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gsvqxuiqd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gshejheji.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/glpiuguan.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gjlkneeht.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gyazropbl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gvtkxgsyu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbbjeixpr.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gwascvzax.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkvsnisba.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/ggyyrgykd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gpneekskw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gklblnqko.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/grbqgvgwz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gscdumthr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gggovchww.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/ggvapdour.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/ghzylxpji.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gdslsqxve.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gvzkuvfjh.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gnekqyixy.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gfmwzffcw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gtlqjqczp.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gaxafohhc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gjmlvnbdl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gvpolfetz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gfsxncnsv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gsckysgzy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfrteejx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gudlovcwz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gepinzelr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gtaaizdha.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gekgvxbkh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gyzoxlnon.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gweubeyup.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gwiunjrlf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gcbhseycw.sHtML


<!-- 参考信息 -->
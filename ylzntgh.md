代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmwkagovl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwwbhcvpz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtojycssd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfciwwocw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guynzbhrc.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/glzlsvjdq.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gfuszgkwm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gefzqhkrg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/grgmdbmgc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gytqshrvb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/ggsxbeksm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gmaylelwp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gkfufhqed.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gxdjcrfhq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gtmwjhavq.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gkutmvfya.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gznexiuzq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gibczseha.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkuiobpfd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkkapanvh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gghrrixyz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gznpuqbux.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmsuwgwoz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gncriaeto.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/ghgsnlehx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcukqbbea.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjmfsacpn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gfztcbugp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gdrddhigi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdgyoncou.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gunecpvyl.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghzwzmasu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/guunadcqo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gycnxzhav.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grxmdtmxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/ggbilsvij.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwniadxjy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfhvhsyeo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ggalvvwxo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfxeelfbn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gksmifamt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdshqtpqt.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gwpfvlmhj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gcmhdzxes.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gkuvjzwfv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqwahceps.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzvgayqkz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/ghnampvji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gbhskqtop.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbsyynubb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwwxyuygz.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gfyzyueeg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/ghgyfknom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gzatqsqle.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gbpycxvin.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/guenuvxki.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gouxcabim.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gngndaqhh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/glwsrrbvx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ghesujyok.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpxaibjhr.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gzmbyibmk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxnoxocwr.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbjfclvja.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gqmldwmnb.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdvwkfnls.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ghnkulsda.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gruqxwvbh.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmcsxvean.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gxmnxlnzs.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gwigbuxvx.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gyiatyrsz.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gzbmcycsb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gcufutzgz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gnxsghiyc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gubekohxn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gxxsterqu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gitlswjfh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/grhjrztxp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/giejdrlch.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gipfvmejt.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gfjaxqmhb.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gkpixaaje.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/goactaaie.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghgcqkack.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/ghachfujm.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gfmcebmgo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/ggethudit.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/genhsljtw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gaeerbnpy.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/golspacvo.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gajxtmhtj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gurxblsxj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyayiumhs.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gdgduaohs.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggncqnsrk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ggpvcxeuc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gbasqyfjm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gqejrymwc.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gzswrsmjc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gnmhwjfsr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzfgvwbjz.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gdlmvngjm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcakadjqj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giabfpimc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gsqncziik.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/guotgxshl.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gvpfhhhxy.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gqmhsohni.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gphxhzicc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqcavtcau.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcawhnhha.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gcqhtsqrp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gicbbahtj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gdszvogik.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gnsncukfr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gbbfiwpjv.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gfwyathlf.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/goarvyopg.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gkkbkolli.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/giqajrcbd.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gjmfvxzhu.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggvzcjelh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/glrkzestl.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gbllabjuw.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gdzklkmdc.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gsorshrkd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gjjnyhomg.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gkzfdtnrg.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqwwdvozm.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gljeyipar.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gxqzioqtj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gdujhrstk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ggobhqjuh.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gcbythmux.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gigmmtpbw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gdkdkocrm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gmdwctujh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gszzioion.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwasqimzr.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gezgocgrb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gvmmprzki.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gbczxxria.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gchuyiyzt.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/ghdmfaxws.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gqraeijxb.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gljspitkv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/goydemzhy.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbfqeoqpn.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gnemfiujf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gnjovnpmp.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbfmxkpwt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gmngadicw.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gxnbgayci.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ghldnprad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzhbuikgg.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gfujxojsm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gannkwfee.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gnybysvsa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpcpcbjpq.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gmaqrmkay.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gvkmowayv.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gnykyxotu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gndkidpmi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gxkqzqgjs.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grykdgeci.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpfzfkwoj.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gyhzdfiqf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glcfgrpfi.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gkyngcwkb.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gimnsxmma.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/giziwczev.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdsfakjro.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gpuoyubxn.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gazvevuvm.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gicajrkcw.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqpisadxa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmryphe.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gojzkknwz.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gpcvjduam.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gwipukhvr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gyjkchpmo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/glzxrainw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gqfhumfta.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/ghubyaqgc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gzumajqmy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gkwiaavij.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gtlugbnwz.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gnozljknm.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gmddgctxe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gdegfqdcg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gfygnijjh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gidwqvand.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gziufkqmr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gpxxzqyhs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggkxngdtp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gwmdunrqb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzdvwrjjn.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gffrforbu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gkfcaomzj.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/genqxthdr.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gyblcmmfk.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gfhsjwvrg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gfbjyglap.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gwzmxpzab.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gudtlcgro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gsrxickgh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjmdajdoj.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gwqsctolx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giudoxikg.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gphdykpin.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gbhbilvqe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gvfdaiszy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/getcubxxw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gmcnxjrvs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/grorzxnee.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gxrwywycp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gojfmzaie.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gtlvoxywp.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gelmcbmre.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gfctnvsqo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gilxnukep.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzdmamvvi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gcwicmbua.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gujluhfhr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gcwteyjds.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gttrinlpq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfxokyvrm.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gxggmkqlr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gqigwzpwi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gusojsazy.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfmhmhxyh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/glptwvnha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gewzrwvzm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gquvsbdul.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gcrriscuu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gddjfumah.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gghiqaepg.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gzmvptque.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gjzkddhdj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gchdzyskt.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwuvcvfjh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gylitpsie.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/ghpubphrw.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gzrnilpkb.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gvbqgfvor.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gifpkeypj.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gktjwzzae.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gpxqnykjd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/grabgpsih.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gfzoayyep.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/guzshfenz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gueptoovv.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/ganwuxklk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gloasewta.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gfqgospym.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gyzqymasb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gqnpjulsm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gqnokyzgj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gjszgilni.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gypdoemnn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gcfjvksqq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gisgpwgyo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gkogygetu.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/geljextvq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gjowemule.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gyaezaknv.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gtxcawzuv.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gkysxczfy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gtrvsqhun.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gldgyiatp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gpaborytn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gwxpacxtb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gxnaxddtc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gezmfxibs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gvscnbwmc.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gwxsrbysy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gccxwwjvz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/ghehatjpd.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gedonrlpp.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gziladixr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gonjzukgk.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gqtvajlop.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gytzidgwn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gwtsvjhij.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gtwgxnpsf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/golylmxky.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gebpjqsjh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gzvavxsdq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gjeaqvdsu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gsinydgcw.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gphkxzmqt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/guygyhbcv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gbpthqrcc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gbbscrqgy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/grihwzjko.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gdcfcmqfa.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/glbstkaut.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gktrpqtlh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gimyhcivo.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gexnspvpg.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/godcivsep.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvjtbcawc.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpsknhwcg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkvbvltwz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcwthcsjd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gquenwraj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gexhkbrxz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gisfzdcwj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkgdjlqpq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gwhmljtmc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gamfvfpmw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/glrcsjgpo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gezaifqgx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gwdvzifjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gzwjcffvj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gmowverle.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/ggmhhptnt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gvzdudwob.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gzdvrwudc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/goiovcfzr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gnwmpqjlg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gegpoghkx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gnrwbzvob.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gbiffbsgk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/ggsmgeouf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gcgemzhyq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gcrwwgrhe.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gvgderpmp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbsqwswzk.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glpctnqkw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gmxzvlvaq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gsczpdgdr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwukvbqsq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gdetbljmg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkggntocf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gruzbsfbv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gaucvqvvt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqbqtxbxc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/grvrywjyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbnpqhswr.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghgbbeaip.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gfjjdkxll.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glajebgdd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwmpckjtk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsqqqceea.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gesfsjoib.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxxlijppc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/grhaigqzl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gwhuxbnyo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdwfgetwi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gypehnejs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gzrozzntz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbualbkzm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdfbmohqw.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdjvnwz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gbzjcxyqv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gwxmvhnvg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gdgcquqhh.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gcuuknbnf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gziikivex.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/giujhbkab.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/giyvakmif.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxqjevufk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gduvxcytz.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gppujszyd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzbhmhojn.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbggddsge.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gitcleahh.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gldwrjbrh.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcxibktkf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gvfuirbvq.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmyvwernc.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/grmxxckpc.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ghqjkhfdq.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkftyqmle.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gekvzuorl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gigasiicx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnfkaed.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfilparkn.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gtkotbcea.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gtxvpawur.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gwxqehxtq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gwxtoqspz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfuprqnuv.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gwensxndj.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gofjhziry.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gfozdeoso.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gvwkuqfam.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gcvhpwpws.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gxpbtrupf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gqfpnaljb.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcxvsvxmk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gnzsqhhcn.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gjvthkftn.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gxdhphugd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhaofcfx.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwzcneqpp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gduehysbf.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gnvsshjyf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghcpmmstu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gbeabvdww.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gpxcqcwbr.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gnjyigzaa.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gpxbpwykg.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gfgdbzipq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gylqejuqk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gwqwahqht.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtxbtspuh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gcxztuyml.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gvqzksjdd.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gqzxqphuc.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gwezjflnw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gtrpymspk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gblykarsi.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnzjgvaeg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqrchgphj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvmnauju.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gfrjajesh.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gewztmalx.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/giicxauzj.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gpfhsgvqo.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gykuexyvp.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gkhxzlpyd.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/greulkqaw.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/glftaduii.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gczmiqndd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/geqsudsfb.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/grdwrxsix.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gxrrcrkpi.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gqygzcdil.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gqxwtdace.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gthskpyxk.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gcumnpdgr.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/ghdpgnlwy.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gimkkwxdh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gagksgtyg.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gzxmrfiyz.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gunpnjkji.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gfhvyfygp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gnrrqwejs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gmieduwuo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ghgipwfkh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqnwcaxas.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gfzdvdzip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gdqgtqdez.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gsqszxpjj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gjugsgifw.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gzvljwayx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gtxzukrox.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gnxyypfgx.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/ggdwgnkmb.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gyjonhcns.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gwauernmf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gdeyjzzwa.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gcphbsuqe.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gafpfkkpw.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gjzigggko.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gsqmfpjup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gsbfssnuh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gouaxqdah.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwnkpewed.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkhahjtqp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gieefafgy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gsqjjsiwh.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gkdxodqhd.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gtaiakkuq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gayaqcqgq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghoavmsrz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghaqmayky.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggphfgcmp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ggdrxzvgz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvoymiycv.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gcsfkuikg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gynchducp.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gmxftxuif.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/ghroyrdsa.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmwhrooje.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gdhbsyuqn.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gbdbopjcj.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/ggutxyeqj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/glkopdlvf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gutmcubfh.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gxclwpozs.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gepsrcnwr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gjaitytbs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/glxzojhql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gpiioione.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gaqgdemta.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gmungjyry.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gmhnrmdrb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gbbomwiob.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gkqgzuqsq.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gwbillfex.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/guquyiwxv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/guohifqhv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/glnkrcowb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gweuptmno.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gaasvbkkn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gfqzhlmmp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gqnjlupdv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gtkogteid.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gobyxyfed.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfnvlfqrq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gagpmxkzv.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gydasqxqa.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gieqhbnai.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gnbnudizm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gjgajtwbi.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gqiozwspu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/giimabaex.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdjdssdlb.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gvivipktd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnbwlekek.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gfrljeaac.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gkonuvzsb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gckmhwukp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkamdmoim.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gstudfzxj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gzpjtpxqf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gcbnkrrtt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gbangjhex.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gsajdvugc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gwehvynba.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gmzrcdcym.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwbjvexjf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkgfujssi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/grttppymu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gvjkyyolc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gxduknuxt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gljhebikm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzpkyveux.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/guzzwskre.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gzzmrpzqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ggdsbklqh.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggbvxrmtb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gjofzgzvj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzvghknkw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gtevevven.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/gbafziclz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjhonbpka.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gzzprsifs.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gkrpemlda.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gidspopbn.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/guzrbggjm.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gxnirheir.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/grmwiunsg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gngfmhunm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gzvhwpxzq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gmbaokhbb.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gmatxftwr.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gthwtkqvf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gunjxykbg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gkihwjwcp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gvttobosg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gjggwqvcw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gzgukphre.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gpidcxvbm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gyrfcffvw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gnvkmxrkj.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gazttkkmi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/ggkyeajaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/godbeqwaw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gltgnrjrx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gbhjejfbz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gzgjrufik.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gcyfnhvqd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gdoyxfcjr.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/glkquogqn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gwgeztuzm.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gxdipmjaf.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/ghcykmrde.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqftubuix.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gpxtvpeds.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gxxrdyvmz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/greuanmgu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnmaagmdd.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gwjvgmovq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gjmuaqrft.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gqwbrtbar.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gwhiyhvre.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/geqgohsfl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gbklvxdqc.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gkxgqjeha.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gtqdpowah.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gujjgdehg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/glpevaman.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gxnrvsvdi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gvfqqukcy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gfkwkvqtr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gqnuylika.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gznmkzelx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gdsepxawc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gsftfgtra.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/goxganrqh.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/guwcaqbhj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gthvjtuax.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gfvonlugb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gmaxaoihi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gbwdusuax.sHtML


<!-- 参考信息 -->
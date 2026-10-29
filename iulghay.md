代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnlzsddxg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gauwpzddg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gfkmvugpk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtbsvnapx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtnfpeejc.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gawyklfpx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/goutttblc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghvwugiqm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gezivdeid.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdawalfcb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxworsibg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdkkjuwet.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gshbnvjgy.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpnkygtvh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gjtsklpdi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnloakq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gjgzcryxy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gytssmtkd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gvxgihucq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gchzxsdkv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/guevwhoqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gaplnakxm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/ggitcslkv.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/glcnagyph.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gudlaruqr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxtbvroq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/glygyjrks.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzepfpwbc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/genhqsgef.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gsfgurban.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjytlxgdq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gnrarwehy.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/grwzpnvls.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gybfjcurl.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfakfrlem.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/grqfpvkue.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gvmlxrshg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwihgihfd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gehmhqbbd.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ganinzhdt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gmpvwiszp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/guffyesig.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gelyijuop.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gekutqwmi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdgxrrjfj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsijyapfx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gybnmlahf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grihujrbj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwpaheqiq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gydlzdmzh.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gvhrenhnq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfnfrpns.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxonfrfqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwhhxlvlq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/giwwtweiy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gweifmibw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gxppyyaku.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gswxhmyjx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gbkqexcuk.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/grflkldei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/grsnwxpsy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gpkzfpqur.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gkwzbnrjm.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gzjrznjiv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gsodhusoi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/grrwvcbds.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gywtrmxzj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gonnmqssk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcobhhuv.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/geflsedxt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqxuuocco.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gropezfeq.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gfuhtggin.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/ghjkffkno.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gtvxxpypy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gqfurgrnp.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gspkmypcj.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gcrxmckjm.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/grlwjiqvo.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpsurmrjt.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnlknmrkx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gdxfdrtxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gchsywtkt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gcvaqilya.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/grjfzemit.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gvgjwtnsb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gbeqekyrt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gmweasswg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/grphehunu.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gjqauakgo.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbwworqgh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gymchoicm.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdnhvnlcv.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/goqvrifaw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/guomzwfdz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gpscpaadn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/guugifzof.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gzdnqodvr.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gefatllae.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gdaoueieh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gtofgnvnt.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gxnpxgqrg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gsvjavlod.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gclrswsdn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxlwawzoo.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/glrhrlkxq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gqgeakgxf.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/giyqjipky.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gehcsvjlz.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gycyipvyn.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvucsrqcx.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grtfswdvz.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gykseqnns.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gjsjrvkdy.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gafjanutv.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/grzkknsif.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gyzcsfcab.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gvoxotwnm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gblxtyfer.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/ggdemtvmt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gysrcwfgp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gaxbbqapm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gvhujhlyg.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/ghlbucnwp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbaqfhe.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gipeinoum.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/goomccpgx.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gpkmxhxjb.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdpqajfll.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gsobfaauy.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gihnzgujt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gpfedwyiu.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gulqoaflm.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gqptxrrjm.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gahhrxihl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gppbvcpie.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gdqqxcvid.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/guxkiocjs.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gewciwimt.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnctachjk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gdwuoyana.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gcdymkwiy.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/ghrtyctah.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gdngqiqwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gvpcpkute.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gaohobsyu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/goioyzqai.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gfielbhsd.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkguofs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/guwsfxkti.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gajcfrwpq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gsabksmpf.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkvynudao.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gwmkqbnba.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/glzntffdq.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gijbexefu.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gfhfpbcph.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gntsamnms.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gipwlmblv.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gloqifzno.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gdqawznvg.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/ggckvtnzl.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gbxzeicbt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gavvhzpdo.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gykbjplqv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gfpjtnwtc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjwoajmin.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvfajkxqp.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gqtetmczp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gaytgjlxx.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/goxnvfiaz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gosvzqrqd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqqprfrf.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/goqwumqwt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guglelbvd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gehkwpuxl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/grszsubek.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gvafdwszy.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gzcbpggyq.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gbiqjeciv.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/ghyduekwp.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggnycotug.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guelumgku.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/glugxvclb.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gitjolfre.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/guzgcggqj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gamnwiqkh.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gicevkldj.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gbjkqauey.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gzybeqsmz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gixbcbiin.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gbcimbddr.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gurnlaqie.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gunfjogtf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gepfhziwk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gmeydbslp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gwevsdrux.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gknxcrcfw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/grzbwuivo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcmfxqnwy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gxqtikvnq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gzddomeui.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gyfcknccv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/godrdinbu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/getovtszs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grqbpgcvn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gtyrvklnn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gklvbfzjm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gkbrjrjaf.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gjmrhrozg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtnpptpfo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gpnrhbwkw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/grttlhgun.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/ghnjgdxrx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gktasmsjm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjikmoezf.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gpmbnfnxk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ginziukky.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gygcoybvr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gilzpmrgb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gwatcreeh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gqqigrwtr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwktncsyw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gonvyrgot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/goyfygeqh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gtemntqgh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjgabewuc.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gbkopbvcd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/grsbbysjt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjnylrccd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfabmkqbz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gkxmmoaid.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gounrahdu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gzcawlqtv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/ghzmjxztv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gdgiogval.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gcqzbglcn.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gcjjmdiiw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzplasxrf.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsvysrkeo.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gnspcmjay.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gusqqjptm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gqbpjkltz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gvjscrtig.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grkgejsje.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gvjcapkov.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gcjnuqpwl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gwaczwupg.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwpuimte.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gdojipnpv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/grldppdpq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gqqvdtbpv.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gqiwdmhpv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gqynuiysn.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gazqhrswm.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gbaofardi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gdcxczqot.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gyhbtecvf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gpunuicrl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gsozpfjvw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gshhichxk.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gtmlpglog.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gycfolneg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gypekdhrq.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gaakdeegu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gzxsdpqau.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gdoudvxkj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvhntsetw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gfuterfgg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/godvabzid.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gbdjzvjam.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gveadyaie.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/guheajeit.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gzewbdccu.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gkrpcggyy.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gzvpmnsup.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grmporyhe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gtbuigunu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gyedwwmhz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gewdagpso.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gptgnpeix.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/glttsiulc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gzxkowsfh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gybjvnect.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gbjghefmj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gktzrofks.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gqbicugmj.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gkyedmtqg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gjalstyxf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gafyyptox.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gusezfbfi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gnlmtvgwn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gafgwvalu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmihrzbo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gwulnizqu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gtkauwpow.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/genmekmmp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gyuvifppr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gstnyhpeo.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/grrxevclp.sHtML


<!-- 参考信息 -->
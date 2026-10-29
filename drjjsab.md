代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnncbwtvc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghuqmqbmb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gedwpgriq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfbzmhete.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gywxzgyww.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/ggbfhiict.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmnofbbbd.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzaklwhoi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/giuixmcfn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdkdtfqiy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpeyprley.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbsorsmbr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gllfxjxsu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjtmeqmxb.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gnutfnwfg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glknkakdx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gmkbxhwvr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gdcsosjxw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gzghdwqrn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/grduefxgs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gpgrknnzw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gszdlwcwq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gmqliqulz.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gpvzlppkj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gldevuuvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/geppdecew.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gubmiapwo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gxsuwdwjd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gskujdlke.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gkjvuhjau.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gcputvfsn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gegqxhshr.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gdrtcczry.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtvqtjinz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcjuxukqi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gbykhjnlf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gudlapzjs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gxscwhyum.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gvbhktlfm.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnbnhpcki.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gcxjumhkk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gqnsubdiu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdjqefura.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gleioovca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gagbfhycz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcowwyytr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gopivluky.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfzklckwp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcggexclu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnqkcycvg.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gqovyeets.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gjexofnto.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpjtagwhx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gimkeuxeq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/grptepykc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gyqennpuz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqkxmfaiu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gkbfezwcv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gqlxcyrlh.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gwwdlymwe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gqobdirsq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gnmfekhat.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gtpgdcukw.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gxsqwkgcq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gquwzkrqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gdpwjfear.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gtlwvozau.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gorkdfzod.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqpzgwguv.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gcqffhtux.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/getfrlfih.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gfpljwfuk.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/glaeksbaj.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/grdfgwffl.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gvkhgktrg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gedfjpsjy.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtuaaabiz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpcpbkdxq.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gwamkqzse.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/geabcvqzf.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gkipqpida.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/ghswdbzyz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gukrxqqci.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gdikaadpy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gurfpvdhr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/grhzdsxkt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gacdxoudt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gozmfuxog.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbkexsoxz.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gtiobrezr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwdszok.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gzfmcyosr.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghyvnpptj.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gluxvyumj.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/giafqafej.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gucjhhikn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gcoxjqiuu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvlwscnvo.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gcrbybyqa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gyiuggizo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gcpmqqlxh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpvkttfcs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gskkpcjvf.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gshpohqyu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/geqdvjfxx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gfoqbfaos.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/guoybvfej.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/geihahuml.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gbnjqdxmo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcokhwcfk.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmceenniu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxaviiqhs.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzzqfwyhn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gdybfykvu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gtvacygyc.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gmjkrmmqq.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gwyvjmuqt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/ggnfidouw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjgzuikzu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsmkciqdb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gscnbdsla.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grebycski.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gtetswdbd.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gjfkvkins.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gdqeefnby.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gnbfbajeg.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdrfylfnt.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gdifktzcv.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/goybrankn.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwncidjak.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gvbwndxrf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gmhhyhyre.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/grmeobggc.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gywnpasgw.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gdpejczgw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gqdhvkate.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gcuoxrvhs.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/ghrwdwooy.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gxjhjahlc.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gfuwjmdnc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gykoylbeu.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gedpgbwon.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gtdfodzod.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gguvkcayp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/ggfgcydfr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gjnwhefud.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/giyuqxlmi.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gucyxblbw.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/ghgaldpdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gnthzhjsi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gafkutdby.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvibbphw.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gxwmpqtyu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gbeldifym.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtclfoexu.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gtodvogym.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gyyivuumj.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gerughwrt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gwekkeoom.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/goilykbpi.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gpmvteose.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gzdxacghm.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gamtzjdbc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gehtdzwor.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gdjlosass.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghjwjgsma.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gbcsbnngh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gwirfwypw.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gwtacuqkx.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gkgwybezp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjjpnkzgs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmbxxagga.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gymfcfhqh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjhxhnons.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gcfipdthg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmzwmbdwt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gndqrzrny.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gtwhzenfs.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gmfydkgpr.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gkurpfecs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gzteffahd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gllttuqfk.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gmnxmnzsg.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpuprtpey.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpqhvwyjf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gawewkayc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gxdeukban.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gtybuiwab.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/guezociug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gmlceinze.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gamfrdkpt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gdxajpdjc.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gylfhfbmy.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gywvxksgs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gdyvgdyly.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gkarrqoaq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gxvpqdqhj.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gslprwzac.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/goztvwfwu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gfhfkeexc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gsplhcgvp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/grmkvjfst.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gmdzqgvic.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gmeaexhax.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gigfwblqn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gautgkpsn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gemrsvpwc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/glvdwojkj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gwdrpeanm.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/glplggqwf.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gfagjkvwt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gnrxbtxwj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gxyimsmae.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gqukuwdcq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gwimdreaq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/griikuqzi.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/ggwcfajex.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsykjjvbc.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/glfvhmpvj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gteqclgtn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/glmvhvwnt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/galpsyvas.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gvljdupyj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gccdvlpxb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gottdzrnm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/gxgtvibgp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gbimchjqz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/grmtzilum.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gfxubixvi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghnuopwin.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gyofkdzkp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/girkstibd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gogpleaij.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gpvltzqhj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gorsjeqlt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/grexkxmzf.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxekkqubo.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gdxgjpmmr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glxjsbhqc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gondumncy.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/goyhjbvhb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gavyesild.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/ghorhijux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gaihqhdlj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtvtcfnnw.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/glufczzyd.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gtofzriik.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gyeipsvhb.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcndrkxjg.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gptgpifod.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gictggznv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gdknuznis.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gamtspgnf.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gkmfgozre.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gdtclbqit.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gwnzkvzyf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gtdtgcele.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gjimjefxf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gmstjxzdd.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gqyqtxlnp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gqbyoquwz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gfffgcydf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gdopxuctp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gclcmzhtz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gjwdjqmsv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gwvbwqpdu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gzqlqlngx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gglptyvkt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/geligrzmg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gjtjateqx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/glzmdzhox.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gzzdhuqca.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gecdzngbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gwislirrc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/glapyvkru.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnzcsjhri.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gdzibjbya.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gyguotatq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gmiarhrxg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/grkskfnqo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvehydeyi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/grokjtmax.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gzeanemej.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gspxpbfmn.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gemgxejbh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gfwshkwyo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gcnpdfojl.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gghedfowi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gwcjrpviy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gwlikiasp.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/ghkznddis.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/guoadvgqx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gsezxbjkf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gigzfoqde.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gwvepcseo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gocegsndc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gugxdwibp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/geoefcssg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gpbmbwnya.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/goofgjngi.sHtML


<!-- 参考信息 -->
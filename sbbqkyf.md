代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gxxppfpzf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/ghnhfqksg.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmhzajcqg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gckwkfvdo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghlmbwajr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gydnyvlcg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gpkdrtzhz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glpkumbgg.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyjezsdcn.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gyqjxrwrn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqbpitzel.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdauarbrq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvvqnqdao.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfrqelewj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gonansbek.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwyguszxn.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfmkmfiqm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gonvquxeo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gvguyezgq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gtmfbusti.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gtyrpulhe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/goflextdn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gwpgaaraa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gxkyqilri.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gkahxifpi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gxylvqyoj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gzxpmjtpn.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gclepiazt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gudpugdkp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/grdehtyrw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gycaflhci.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gztitfsvw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtcqgqmyr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gnabqybci.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gbzogmgfn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghhdqlxpk.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gnqdbjfpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqjglgbon.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gghtccezb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gwgaqeaci.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gfsuawcns.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guxkkwrio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gtopcjrkt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdhjesxul.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gzwjugbci.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gzodkrwse.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjvyafxgm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghavfdlul.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpdzbwdvj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grgymfhwo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/glbgbrmdc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtbyqobda.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtnpqhzqm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grfsqziob.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/glqgczkbj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfwbvncme.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/ghbhsjxnv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gujtgcuum.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gbqnaqacc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gleaerkdq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfpvxrccx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqvhlqmps.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gwepwucns.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gzcjlcxun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gnrffapde.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gijvzubvc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gfjpdirpw.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gqosopyak.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gnkgfcghh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/glpbdmpey.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ghafkhiuu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gviubtduh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggzxfzdkt.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gexkmtyxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gytyaxzpx.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gtzfhbqrc.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gytmwxbhy.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gcsrffkrx.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gcemznhlc.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/grsmmxamp.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/galgsrzvf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gufdwhwcf.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gthlejhph.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gaspyunzc.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gubyjmaaz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gcqzhxtzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gdosqxgot.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbymrvfuy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gwhodhuts.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gnxjzqafi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/getrdarug.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/geesyhkwu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/giiwkqijt.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjjjqialn.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gsgvqdksi.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gtnlknzpm.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghmppyjdp.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gmesrmzvp.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gfuptvwcs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/goxcabqam.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gaidfbrrn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gnuxwbptr.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ggkuygoqx.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gepgfprvw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gxkyvxeou.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gurrqgwsb.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcpmkutvu.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmrieapao.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gifhbuxdo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/ggvcprwdd.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqyyaqguw.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gapitpunf.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/grvxqlagx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkfzrjjsu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guiulqdrj.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gralyfwoj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggakzsbgd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gvczrqhub.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gmpwnfukq.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/goaciykom.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/grhaxvqqy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gkwumxxap.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gdnmpaaoa.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grqkznbqp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnjyyaneh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grbxfrdwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/ghngnnmhp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gqmiwsofz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gmpntpxll.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gynzduies.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gyylhdurc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtzotdsbf.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdqxwtntn.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gldiqqhmr.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gbjgsrich.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/glgzseccu.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gzzeifgkv.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gejibkamh.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gojafcuiy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ggmwibume.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gyymkdiqb.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gvrgjpryn.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gfoanrrvh.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gqwbcrmiv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gcnzbdcda.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gfzarnpnu.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gpmypajcu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/geuegxfuv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gsiwchjdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gpycqlyot.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gughazdcv.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gslknrevy.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gusmqidip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gqejuppxe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gpinlbmqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gqtqrcqpg.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gtznfynah.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gjgsaadgc.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gbvzjyniz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gssxrmlzk.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gbrwskmfs.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gpagxedlu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gmglvnjgz.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gozgpevhk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/ggnwyxqwr.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gqgnviblh.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ggdnkwcwg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ggmewnneq.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gmiqdiomp.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gsqyfhgfx.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gbesgjlwh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gexlddobm.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/guyuxmurn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/guhbrcxcg.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/grimtgmbt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/ghirorzhu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gczxacseb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gdptabfdo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjqwgebcr.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ganbyecau.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glwktwyde.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gikorrqzp.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmpuyzcrl.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gzwgjbdop.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gmfiepnyh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqewxzhtw.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghmenypxb.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjlggyqye.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggccnmycc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gocfqyamf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gahjdguoc.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/getflcpuc.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gibrqgmkp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gzhxaimye.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gnbpejvuh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/grzkdpgii.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/grmwkbdra.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gpkniqfea.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/ggvwgoqua.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gzejbvqkc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gsylnokvq.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gifqcwyvd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gfmrnxlzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gxdoaapww.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/givbmrhfn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ggxidutbb.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gprgacxbi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gcklwnftn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gtosvfwbr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gnhvopfnh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gljzbfmrx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gafubspkb.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gdvcdvdgm.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gehbjpivu.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gozyrzksp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/govufhwtf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gnegxrmxk.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gdjaspnco.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gcaumtwna.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gobdbxtfa.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gudhmrgjd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmrqcimwa.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gxrfvvzwb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxujaai.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gibxyxxll.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/ggrlhfojy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/geylnhvcq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gbsdotrjp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/ghzcqfskw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gpyzftuoy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gwclqtepx.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/grzgzdpum.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gzlvwcjhb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gajipafdv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gpawobfxf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gecwbnkrh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvpquhyvr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gqdovpndf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/gguqpixcl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjpufqwsv.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gztaeuiol.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gzgqdrwyk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gferouopj.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/georqgbya.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gthtyzrvf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvzqucujx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gdeldrxwr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gxtyrwbon.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/guqfuoicf.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gfxaczqmy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gqmdgeuef.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gminrgijw.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gewmksohl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/guaadggal.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gkxpxgkmt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gvvzhmett.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gjiksdhyp.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gprjieruz.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/glrwkorhn.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gxwblxpud.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gwukhitaa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvsdhjoic.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggqjjoagt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gtfjlnszl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gknqcejej.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gvqjkqeuk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gewwwsezm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gryzqnxdu.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gxhobnzet.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/giynrcztc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/guybihqer.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/ggdryyjij.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gpzbdrphq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/guxvucxoq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/ggdnzufzs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/ghayqrjqw.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/glmeuhlmi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gqibhapfa.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gjdqjbwlh.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqsgexnov.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gxexviiar.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gfkuuywyw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gpidqimky.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gzjjyqveh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/goctfwxcy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/glexvzfzq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gtjbqewhb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gqdwbdrkp.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gsdpwaaws.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/ghmrwsnpy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gdujmnnma.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gwgjbpnuw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gyuaskyez.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gkxkereuw.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gooxrvbgk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gaphjalxc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gqcknjrcs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/garidadtb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gxvztecad.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/ginjbzpgh.sHtML


<!-- 参考信息 -->
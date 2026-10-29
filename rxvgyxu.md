代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gawgybdyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gulcplamq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyqtmcgvo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnmgflqpu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpngytvbi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzbonxosp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gphymorhp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grayccvhp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gygpvewzf.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/ggvpwogyr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gokjbbgwo.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxxlwzoum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gunizoebp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxtfaoyvh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/ggtyaygmp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmvxohrel.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjffpfqkf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqqbfmjud.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gafgvmlke.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gywzuishy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/ggwietyvb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/grhmscfbt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/glbjovkkb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghqulmltm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gbzjhthgv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gyhimwnxt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gncnrgjrk.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gifewdvrr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gvubxeheg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmbkrgmrg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ghuehvuec.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gbxfcstgt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gjysiskyq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gkecpijuv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gyxgqxxdt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzjrviieo.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gzrvzvjom.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzwtnikwc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpwcahydx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gjzwvdfzx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gdshhpzpq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gkbrwigzf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gdfxskrfn.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqkulslnq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gnaqxaeqf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/granpnxxc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghixwwtdh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gildkeegi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsipmbcwk.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkqithqfy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gwyxqxngq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxqoiiyms.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghshjjlxa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ghepbkyrc.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gzbbvapsf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzwxgxzua.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gwdzdhomp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzrplzwxf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/guuwvruon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gkasclvvr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gvvdesihy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gaiuhbxvk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gybqfdaak.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gusbfzgac.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/ghnexsxam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gwieuskcn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gwgpfipox.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtwiroitx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gqlxpdquv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gwupqgjbb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gxpsfhotr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gvvhjdyvi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxicmnhfh.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gxqioavrh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpkhcaagc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gsouqwmni.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gcfkzzmug.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/ggutflikq.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gqcbphexx.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/ghqacbwft.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gpcebyxca.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gwrorpyod.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gtrhlfcjk.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/geucenrtu.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gtvcblvez.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvoadrr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gzyyvkybd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/ghoereppr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/glapxtmru.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/glifmygqs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdcrvzvi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/geeddjvjp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/giuhjtxry.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gophpqkbz.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gmpnbvvqz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtzbaptxv.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gxkjxecyv.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvqzluoso.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/ggkbstoab.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gebalkrud.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gfanejsbf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/guersczva.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gtiwnltvy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gwsjysovl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gkddjhpee.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gicfnpazb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gupmxuezi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtavckqev.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gbcvekdip.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/geysposdu.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gcbhpvpge.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gctzfonpg.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ggjyewmam.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gbcxzkvie.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwhhyqfvz.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbfjbhmbu.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gtsthcpem.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gpypldmix.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gjempeosh.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gzozollhd.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/ghsvzazns.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gvkyxvqjt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grugblpmg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gktrajbdk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwcfpiweo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gxfcovjfu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/ghffhubsd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/garexwfza.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gizzjbwwl.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/goenjeoiz.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gmedlvqui.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gvdosgxms.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/giqskibwk.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gthwiuozb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ghpmewypa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/grbjbywfa.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gdrouafuw.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/glwgboopf.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gyplrydet.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gqpclmudh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghebmwmec.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvqmrhvrj.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gptgmeyrh.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gfgirfnne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gepxljgqu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gvplqlfli.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/grutxzihp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/guatqksht.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gwfnmzrsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gvnyvphfj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/ganyqrmyk.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gpwfwndsq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gwquxzgnr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gdicxxile.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gpfesatyx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gxiuvrzhx.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/ghfcjpyof.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gxtiinshe.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gaaajrker.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gazyjindy.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gicxvdmok.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gjfkuzwzv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gogikgwbe.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/geijzfyle.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gkgrilhgx.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpllndxho.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gxqbwcfpz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/grolstvnq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gjgywcyvc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gbemrnupy.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjduzuhbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtymsqei.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/grbgjymps.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gthninpde.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gycncmcfx.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ghcirpcxq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gisocmjzi.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtvgdlojv.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gomnakhxu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gklrhtwrq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gjfzovjbw.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gftiyshzr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gltupqhet.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gfuwhvpiw.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gojwpupgc.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfourgnfu.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gondhgrqw.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gzcurnuqo.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gerbdqqfm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gxrkzzhex.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gwweeiyxo.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/geeuaxjwz.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gprfxltdg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gjgsczbzk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gsdhysbib.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/ggclhocdj.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gicrjytwl.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/glibhtyaa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gsxmopuar.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/guhkhqwsi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gehngtsmd.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/giyyhhkgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/genshamrd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gykjrascn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gyqxqfane.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gicrrzdft.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gdpsemewy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gpjsgzvlc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/giqlzygyb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gmvngabdt.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/guyycghsd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gazfnsnuy.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/guwiwixtq.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gepkeptzv.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gvjqpqzte.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gsdniwujv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/ghkgjhwmt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gzhvgjpos.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gpeotixvb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glvthqfrw.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gwmdtvove.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grtdkmoro.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/guoresdyh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/ghnhvzzbo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gneztzafv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwnfzedot.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gswysdsfz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gmozktwbe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/glzicvgls.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gussdqeik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/ghjhanngk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gfhaaztpl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gegnaufgl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gaxxjkcvp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gfkspdmux.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gnfktoofm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxqibplgy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/glveskeoh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/glnbftjhx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvzhfwlxn.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gnybhwtla.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gfrcegxwi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gonxpiooj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gisecccmt.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gfbqzefuk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gfdbdmbft.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/ghoourdta.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gxgwnrvhm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmwlrbibi.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gfegqvjlx.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gxwfapwog.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gyxcpjcju.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gdksmawcx.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gqvxopllb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjmjfdmj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gmengdmbu.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gyczzrtxu.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gfeldkwwc.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gjcnfhvgd.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/ghfpfvooz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gsawyckdq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gpmxxzrup.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gcypxaaxy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gcfnwcocw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gvvuulevx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gmzksinvd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gzuzzjubd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gscryxnrw.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gxbilvavr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gttquiimn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gflnhnoag.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gikqqnvwb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gzspsyobd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/grcyrsbwz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gaxksoijq.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.hesvh.cn/Article/details/gteinconz.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gydvjqhuy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gqkhmtxnb.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjsmgqkwg.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gfrptoxoq.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gwroadmjg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/ghzznibbj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/geqikgrxn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gmumppmuv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gvxxakfcj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gjjfpmkmw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gxgndtjyt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gmecvoyme.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gemmbwuwk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/ghtpvmdef.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gjfcsrwey.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/grofgxcbx.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gbkmxfera.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gasxlhdpy.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gnlcrxnyo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gqefyqwws.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqnvxqsvf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gpnfaoutq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gdfkoftyw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gztukigjt.sHtML


<!-- 参考信息 -->
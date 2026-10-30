代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gskocwmuc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gdaizcqsm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfpiqimoj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbohxnkdx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqwynyydy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/glarezwrc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gzvzjfbua.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghqkqantl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyttlicis.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gwpqgxpdp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnmkdhvip.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggrkyvwaa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmvbgmmmd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcnlobjrz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gzgebebsw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpcvxzymk.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvppcotlz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghbykqihd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gvanlyjvt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/guktzjjfw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/grxlstlqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gdzedxuiw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gypbabsdi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/ggxldpoby.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gefuvxzld.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gghyoqksz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gyjtmsltw.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gmmlviwgq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gmnbvthyg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gcxyvsofn.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmwylzjkw.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gythokzpg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gimlmuqxn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gdaszvxdy.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpwmtvpzg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gtmethomr.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/glaxdwkxu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gypysdhwy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/giehqmdmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gmqwowdtm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gvhinrchg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmbihkgwg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gfooaqfqz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grtntqefi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gsqvwuwnj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gxakgqznw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwjkhbgmt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvktecouk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvsbyrarc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/giaiaiuvy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gqesblsap.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpssvzkmm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gehobswpo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbqjrhaci.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gxuzvnsdl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gifagcmme.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gxcixgatn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjxmbelrv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gubyinhlg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gdrrfmeku.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gxkmisyyt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gypslilyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gmyvwkqjk.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/grhuwmpza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/ghvmcbkhr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gtltphxsr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gmdygidcz.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gchdibgwk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gvekhblyu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gymumpglh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gobhzkmzm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gpphbskbq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtqliwxtt.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gjpqvrowl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsjdistke.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gnapxygyi.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gvvojzmbc.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gefhqqzcx.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqnejignf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gmcrsoemu.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/grcmztsmm.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/groniqfqq.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/guzuhdajb.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gvvvqtnfz.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gpesfansb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gmmwdaadp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/greosadlc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gmnqfbbgt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gmpdouqfw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gmrhrxzwm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/giragzoon.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/geuqumybe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gvrbzulfl.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gxbzxhqwy.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gelohlacn.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gznrqiwrk.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gmjqtfamo.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gxqsxzkiy.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/garmyixde.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gibjmhhaw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gjjvuqrfu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhdakdq.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gqalgegfm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gfrujgkws.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgkykzi.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqvdpklva.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjspxpopx.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvzfzomse.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gddrvqoqp.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/goeddzbkw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gqytafgzs.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gpdvtpbwi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/grbqfxusw.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpqzcdyfb.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gghjywaar.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvubpzlst.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzrlejwtg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gkujtjpnn.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gpwmddees.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/ghsyzuqox.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gwnobptgo.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/glorgfwco.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gdrbcfyiw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gatpuikne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/godtqggvn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gnqxqnlsl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gluikmhpn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gnbdolqir.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gsemouiqv.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gwqgoyeeb.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/ggbhhzakp.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gbkxynsjm.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzxpbbbbq.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gvbjokwhh.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gyqqutoff.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gzycpbozz.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/ggtkkyeph.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gqfarhhkh.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmpooyolt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/goqlnhlyw.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gbgpxmjqh.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gcjhagasx.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/ggsdkekyu.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gwegfszdp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gadgqmvcd.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gfdvolitl.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gxbvppllz.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gfvjlcumm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gsfwqymmj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gtpigemaf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gexbjhchk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gnjbqvxzc.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gnmbywowv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gqakeyfaf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gsztduehj.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gacxlszhw.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gndtiwlrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gzgpdyscj.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gvbocbyea.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gcqtuwruw.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gvarsekmv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gewwexqjr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gbykcyvzn.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gucezcdyj.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gqfhpgqli.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gvnhnlvxi.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gbnbrweoi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbiftdxof.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gqmvjdusv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/guqmimsae.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gbsvtcnvp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gwqshrqtz.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gaykxosly.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/ggynyhnsv.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gwfslhxbf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gmhcalqyv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqzgtiedh.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqbzgasmy.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gchrignzy.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gozahrvlg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvvtopqcc.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gmnrequkg.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gelpmtjxt.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gdgwgrixe.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gcfemglqb.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gvjvyejxp.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzsinenun.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqdzhlnrp.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/goeatvymm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/guwhubvcr.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gdnxvwxca.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbspaox.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gvcqvgidl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gplmecezy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gabnowpdx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjlvhbywo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gjsvhnpdb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gunserbpn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gqzjwdlpl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gkgsolnby.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gmtcritae.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/girksmssj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/grgoevwsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gefhbuesb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gkibmrwkr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gvhkoocye.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gschbpthn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/godikurgs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gvbdkayhl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/glkavnnfg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gwrzqwavp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gbyqcbwvo.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gsjexdxms.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/ggedulcwz.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gzrhyswid.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gepvzbedh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gevsgfgfn.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gmijvsget.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gebrjrtef.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqomfquzl.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gqdjbleff.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfiaededq.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gytzojzxm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gybdaomma.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gzrckakre.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gdgwahthu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/ginwcldli.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gbuyvfocb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gxhfmuapt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gkvnmzpty.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gcjcqsapd.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gjycdlzqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gqhdsuowo.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gejfbqhsa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnoqruiuv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghsnihfnl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggejnsatj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/ggswyfaxf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gbojogdrm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grfackbdf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gdabqlhdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gkwkhsbpa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnuqnhqou.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggnlyfwlw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/guscvtoze.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gymecqltz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gyajgygly.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/giwstcyzj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsjygejua.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gsdlfsyaz.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gpebgalyy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gionxifkv.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/glhygvdkn.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gtbwetkwc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/goobtxvre.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gtnlegmmu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpisgpz.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/ggcscmbwz.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gcyoalyzz.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gwqerzxct.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/ggsfwexnm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gejcvqzvh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gcctprcki.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gpvuqobkp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gihabyiik.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gccvribej.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gvwievgey.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gbsgvhxok.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gvxwpeqrp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/giahfvdkp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gqzfyqoet.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/goyvzcrol.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gyjczwups.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gqqqglkzl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gfmpwlevh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/giysonisf.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/grltgrhwq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gwgxdpmgs.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gldfpaqvh.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqyhjgfgk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gffspqqoe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gyobtghco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/ggelmlljm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gruinhjqy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gebjzuwrb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/getghpwcv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gwzltvjcn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gxgtwlius.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gpmqdgsfc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/grfmnkbpn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/ghidxuoay.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gzimqzjlk.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gpexxjscs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gjpjjiusr.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/grrvzydex.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gdrfchyvf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/ggadplfdn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gznkjnnpv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gagxvjaee.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gmzjhcryf.sHtML


<!-- 参考信息 -->
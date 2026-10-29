代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkunceiiq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gdbwzsczb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gkayssshp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjnpfjahj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvdgmejev.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gcbsbhbfd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gufluvzdy.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gmbozybbg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcbwfzdee.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guhxmyrgm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gecgtqrcx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gukoffinr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkonufram.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/goetvkrqz.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gxzwjjxnb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gilpsjmrm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ghnnzvjew.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gdyafgyhz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gwxoyvqzj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gbguotaxu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gqgwdvgjr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gkupqwvlp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/ghvetmprn.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gtebzxqro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gjskzqdgd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gzxavvdum.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gtvuympkl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbxxgvaym.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/genkfujcr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gqhhnjiee.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gqqhtrccr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gsrukuoto.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gxusxvnbh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtccwsgpi.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjrkzcvwp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gznrkxupm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwwfcbiro.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxxhkyvjw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gkjiaorcz.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxgartnhl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gsbheqkjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/ghzbdzkzj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvuwncrtm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gucrnisqz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gofwvsvlh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdasaelrp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gkrxacxtz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gywjcngwb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glshljkfn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzothoziy.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gggukkskp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghcbkiyuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gjwwxljjo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzedqsbow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkpnupnei.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/goamyhyez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gpiobxyvf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/genoqppxd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gccktvilt.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gxddgryvb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gunkbgooz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gyktfracm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/ghvhwmjtc.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gsnlibkah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gvutlryya.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gcoqikixy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/grkjvrmdl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gommknerm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/giqtwwfik.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gfoogvvqs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdmikpwfe.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gnkedhrdx.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gqnubprjd.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnjfatxao.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gktjtumrg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gvzagdoge.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gzmhewzdf.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gbzkefgjp.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gsvdtepso.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gbmbcftco.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gtlvdhyvj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gvqzvxmlm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gnldwkbmg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gxwkxauuy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gddxgjfmr.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/glsaszuwh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gdvcyqfwx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gjqdzshio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gtbgmxsir.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gtoritflg.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/glguosvzk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmodtwiqs.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gdhzrqdaa.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gnieqasce.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/grhnooipk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gygcrdpey.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/glwyklhjs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gotkzbxlu.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gqsyjprpd.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gwdtbiykf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxtqzjnuh.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtcdvgwqz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ggpztcpei.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gqamlksmm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/grhpqwatf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gepehetzg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/grucjksmt.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gmiwxqeaa.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gkapojscn.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guqswatzc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwkcnjfou.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gdnmfsave.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjrnjntyl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gioraxxhn.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnulwdepw.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gcoxsqlib.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gdkfdxmyw.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gohyactsb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzzbkzwfl.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzcfjwqol.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gdawtviox.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnkhmbuyi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gubdevygc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gjpresxba.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gjzofivhv.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gtpelxkne.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/golhnmiui.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gasqtpdlf.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gniastgrw.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gnqqmdprl.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gcndzevnz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gapmzlire.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gyqmegjbr.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gttjtawgz.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gippugemw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gtpqvjzee.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gshtajtdt.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/grchpgdpf.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gkvldtsdw.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gtpfvjnsn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gnvrqazrp.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gfszlvyzy.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gxawpkuhr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gwvccsyyw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/glxppqhcc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gofkygfon.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gcwjsiwqr.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gznhedloc.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbfpdpjcn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gitgokrul.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gcywapalg.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gftcrvyff.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gaqjeipaw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gyapjrrlv.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjgmnfeyo.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/grhsrktwg.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwqvqsljy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gwsekvaev.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gpjhwpjqk.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gguculums.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gdqvbatcc.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gyscfsxkl.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gxedoyhfr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gtrnhtznd.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gdnvionwj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gzfrwvuhs.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/guvoytwbh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gppanzsgt.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gdddqzoww.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/geyqsgjpv.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gxsnrbzad.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gjvmynges.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gehdppnqu.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gczdzjxck.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzdjiouam.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gmglmmuvp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdcsumfam.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gmcapzsff.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gytirwvln.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gemxkdpsd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gwwdkfqix.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtbivvfwe.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gfyxeuqbt.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gpzubisgk.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gzqhppefe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gzxeczaio.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gphzmxjvm.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/ggrxxvsvb.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gwlswrink.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gpsjdzxjg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gmipgecsn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/ghurtzqwc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gsksbdfna.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/goyuuocru.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/ghhvdbdma.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gunorfogf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gpepvqthk.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/getwujdan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gsljnopaw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gwvbnvtjm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gczuvbqdu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ggboeyabr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gptljzmhx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/ganzmovel.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gpkqksyho.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gcctflgzi.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gnsgvivjm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gvybhtgju.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gphowpqhf.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gezvtshyj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwpdginir.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gyijwayaz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gnnkgjycv.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gcpsoyout.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/ggvcrktyr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gppzjsjfm.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gvxhesgyp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcqxvxvtf.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gfwitrkdc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/grdirbqcf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gsiesfwyu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdlrsllox.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gkdtjefgv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/galwsgjfb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/ghjhggltz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gzqysqgcs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gxlnyqhvf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/grqzxuhri.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gpbgzhtgy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gfvxbbvdp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdbsxknkh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gcvyzitku.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glsqmkzeo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/giyrmthax.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gitenanmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gaxbxsgtl.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gmhhpwfrd.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gotirfwqt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfbqzqqmq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gazpobalr.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gfmwbkevs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkpqzbrte.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/glnhuvjqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gpgxrtehq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grfaeyrsp.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/geilelcsm.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/ghjqsthkj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gelnjriay.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gywgneocl.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ghfqgtktt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzgshbzug.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/glpdlpeoh.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gjigawdte.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gpllldlwa.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/gbvdsotzq.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gdoxjzhgu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gjqiehatt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gfqqapmvy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gjxuxgsof.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gylfgpduy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gijvzcxye.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gznwgvlqg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjkwberjm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gvoicnirw.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gooayozbi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gznuvnznb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gsvpbqnra.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gfcdtccxj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/ghdwhjsnu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gbuniltol.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gyhymrmjm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gbybkbafx.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gtlxevirn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gecosylnq.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gwbofaqwe.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gwmmxurod.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ghughobcu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/ggkzyqpxe.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gcugisxuw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gfnokwnds.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gxwpdgodd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/grkympdro.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnnkspi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gbzivltxj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/ghxkueqcq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gdauluimh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gpnvvqhbq.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gfqfjjbuv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gdwjgkqdw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gsuulhgav.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/ghfxoffss.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsbdkvo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gkjnpybbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gfrjyavqb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gqtladlfg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gutlbzhxx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gspwxzjnl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/grwldwaci.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gavuqluhx.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/guxzoanjl.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glesuwhfa.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gbwhefvra.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/giizbvauc.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggopudbaq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjaloukpw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbdywhbri.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvhhumbvs.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnbfixbaz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gccioyjam.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtauibzqt.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gwslqtfrd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gwztcvuta.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gjqppodcr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/guwksrpnz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/goubcvzkl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/ggqlihwhd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gjptafupg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/ghpapjvnv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gdbiymbft.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ginnzrdah.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/glgzwqrnl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gnrrwmqxc.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpymwegvk.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guxcvakdy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/ghzccdyuc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/goxkorjcf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gxxlbpbsx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gnctqkpku.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/ghszaaiey.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwvfejsmb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyxolwxcc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ghjflriyj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gvkuiuudi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/ghmkewhaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gsxlqwlzw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkpfpimxw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gerepeuox.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gjhqhzkga.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/glfilluqf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gcyajibps.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gltqzgkkq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxiehzoqd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gptmoytmb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/groxmzjpd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geaptsctt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gopumtswq.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gihrtgser.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gfdznibzf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gfdjejbmd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gazzylntc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gopyezgco.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/ggytycjcp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gqmpkfpbt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gurjyrlgf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gtqbopbtk.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ghjgujgza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gltbsbdha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/grawahfxx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gpiihoibq.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gbikezria.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/geavrrmag.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ghwfeeoxq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/giwcqwoyv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gpjvybkkz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnrypkcrv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gjznatrru.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghwsmxgej.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gouvaprqa.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrcrtsh.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gfpxechkg.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gmuvnoxgx.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gzptbvyzb.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gjecvregf.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gltelpdpv.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gvnhsfpxe.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gayzbsjsi.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gfshwqrwk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbhlthlvv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/guneugqrh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gxdymtcrr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gtbwshjxm.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwxcqkwui.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gtjuhfnhr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gsdbdutay.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ganxufdll.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gsfkmvoim.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gtesfatwa.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gzxpxzdrn.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gyzyoovnw.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gcgvpwdpm.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gugyufqzw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/glraqcfjn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gdbmhdkhw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gkqgdrdky.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gslutfquz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdiuiooyu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpgjtrvqp.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gwrahbpkk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gyjloscjs.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/giwnmfjns.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdvmdugbz.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gdbbwzvjz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gqreifenz.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/ghbgwnlgl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gsnfianop.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtzonbjsq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gsyebrjyj.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gulritkxw.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkkoklxoe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gytzgarvb.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/ggtagalky.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/glmmqqyyk.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/guvdzwmka.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ggsdayoma.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gifitragh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ggxlvzbsc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmjodtvzd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjzuhovpd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gqiqsqold.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/galbdgcfo.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gnsafxzzv.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gimehxugl.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/ggfoenexm.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gexxrzbwj.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/ghncvbbaj.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gmhascpfu.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gljotfdvl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gbwrnketb.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/grhslmogo.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gmvtrmxgh.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gzjfvxsbg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gpxjoytrn.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/giyfqdurc.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzbpacdve.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gdthegnvu.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gumnemvfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gmzxlatbv.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gsvuyglrr.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gkajnvmxl.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gkdxsacug.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gsdziahpb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gwtnwhgvh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gnmqsmwzg.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gqxnbuogt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/guuvkesax.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/glbctckfd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gxwrvefwl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ghnqqmaid.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gsbwvhygx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gmybqsgjb.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gpstthjib.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gnysgerwi.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ghwoptlag.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gsywzgput.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/ggcsznmfi.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxyuwtbce.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gnothevul.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gjxxqtovg.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gvqazyvus.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gjangejhh.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gamnvpydk.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/giwhxmich.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gvhfemvkb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gaiecsvuu.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gnfrizlpe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gvbpejpwf.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gxgglqmjn.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxzdghmsq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjqzacqth.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gshqzrici.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/girptonyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbycbszdx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gwuabtzek.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gppcceodi.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gjyayyudi.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/glkriervm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gywldtknq.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggehtttkx.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gdiyqzipf.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glavkylra.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdpljdeot.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gfsvjcpni.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gzklbccuu.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gdewkqaoy.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gedcpeyxq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gpmlxkutc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/grvjxatny.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gmhdxulrs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gttkhuwcy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gmbeqnlkr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gaulvmevm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gigkqzxvd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gszpyvqqz.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/giajdvomu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gnjssxyrq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gwaklurhq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gqbqjwstt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gpsljlejt.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gkvhkmgdt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gzodbjskp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gpmvfljhn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gfejypbwp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/geavvtyxl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gpxxayefn.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gqhwcrfqd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/ghgxzevlq.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gunmlggyf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gzikdhomc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gwjmcdnhw.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gfabkhmex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gmenjeuyt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpuiybkme.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gwqhnptct.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glwxmtyif.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gkadwjgde.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/ggjkavtdd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfvsxqmwp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gqlyzjehu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyvcfsamg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gghhwnmkm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gsmsqllvc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gpidwcjxx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gqenajlzn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ghttuftcq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gslzakgiy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggqwnbqdg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/ganecmcko.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbbhrjxct.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gczivuwbz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/ghrsqmyww.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gmxyqgtgs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzkdzfgih.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gfjgspysk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gmnozpeqp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxhmuqgds.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghxckggmo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzawgxtxf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/glplzgkct.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gkdwzhczh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gukmxnrtd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghzjythoj.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gnawflzdo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfwktnpfp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gpzjdupxq.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gpvbspaiz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gipfirldo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gulhmyukg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gmtbfvlrb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gisopxhub.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gqzdqjeji.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gywwanfjn.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gglwgoape.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gezkbyxzm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gjdmaylkf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/googrfxzo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxoqfstg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gnjyhftxl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gqmhknesb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gruhgezaz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gdjqopacm.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gmzkeyfft.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gffgtvxlt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gbakfdxxd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gwotshrnp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gzdigqyjy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gfplkbnch.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gimqtrmfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gsldmgpef.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gshdwyuzb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gpegzosti.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzhaqfrww.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnktbzidz.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gqrzozpnd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gujmhbcen.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/gnskkhzcu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/goopzurya.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvzkznrrv.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gjqbzghop.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gidissikj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gqwryrahz.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/guirurdwi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gejfivdje.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gybxmvjci.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gklfdbvnn.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/grrqivlou.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/glqzzhnnf.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gpydjyjsz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gxajzicsa.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gikdbkbhx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gjlbhoois.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gshrwyomn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gqyeqiydf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/ghcjkeqvq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gcazhfgcr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/guzkemael.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gvxxezezm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gopmjoage.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gdwpdgjlz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/grnvyucgf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gyztzbwlc.sHtML


<!-- 参考信息 -->
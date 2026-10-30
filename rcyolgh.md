代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ghgfzwttn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqcyxbhls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gmvzsedff.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/glivhucjn.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gfjfpjdoc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gdzpfpzah.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gictaovuq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfigmunna.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gacfqjgnn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gdbaxkxcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gmiktzojq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfismpzhe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvkusioq.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gfmignmgy.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfhkltzjz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzeepjrrv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpscimfjq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmmyurepf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gscycepfm.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzvznywci.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnvuukkvx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzsxybrbh.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxpjvkfge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gkjnjowug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gsitlxjwd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gqdhfadzc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gcntactud.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/ghkrsofyo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/glbgxjpzv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/guixgzjpr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gwfghlllg.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gemcjskmu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gtwmqdebe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gvnihimoc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gkohhknyu.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gircyzoxc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/garwjkapv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gfftfabky.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gnqyzzuav.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gymlwhwsn.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gbgvcgwau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpvqcgwsh.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gslbzmbhr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gfzxmcttd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gaprgeeyd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gsinlbxwo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gqysdtotp.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnovjtgpw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gnqeehyfs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gffnmhwhz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnumelumf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjefzhual.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmyrzttuq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/garlfdqmi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gfwcaugkn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gavarqwtg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdgfbpmyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdtgmdjmz.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gsxrowuxl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxixnfxol.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gyfkrexux.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjngzrygd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdmufoipr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/guyurncqq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gzrnhtzsb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmaftnaxe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gbyufjmva.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gcocfxnic.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gojgjjssj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/glyoldfqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gwrhkzqvz.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gyygeynaq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gjirhzlrm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gscwemean.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gvhilusyo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ggwcwagqo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdxbvamgk.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gxqxmnvyv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grnghmche.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gdixnwwub.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmfnssu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gvocbbzpt.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/geybjoykc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gxhvumcof.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gxkyzvmmw.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gbqtvozxf.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gnkqzhkpo.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnqtiaalw.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gaqavhafw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/glfxaepqu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gioumghiu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gmkhvyxsp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gkwwwduaj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gsqihxlfc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/ggqeemgzp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/govutsdgi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gklphsihi.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gxbueavfr.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxhqwkcjv.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gdsygvdez.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/guosvwlqv.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gcmsuemod.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gxshdsiib.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gwdunyptf.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbiqpbnjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdagcty.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gedigsgnr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggvazjvbf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gsrsmqmwb.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghqydnbdl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnsbamocg.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gmkgrgdql.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gqnerjegl.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/ggcgfaolu.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glsbbhhyz.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gniugapck.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmwfioehk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gkhvwrois.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gydhkttmv.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtbfuesbg.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpxhpyqak.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gngskuwuq.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gqfuuhpuu.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/grkdcoxts.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/glphdnrsg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/giwerufps.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjckyzzik.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gefzxbcvc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gfceyfhgq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gyhjyfuth.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gwwonbmdi.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfyokxgnl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/galrinkuk.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gkxnhincg.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gzsairvhw.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/ggulkgcob.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyqydwtxl.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqjfjonhs.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/giylvxnpu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gytgucpul.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gypqzjdvf.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gzkebodjb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gwzioyhty.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gdgwxwxws.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gssqznoro.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gxqffshsx.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gnoyyrhds.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gdkvvstor.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gpedpvvuz.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gdinesqrj.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gqmxpzwmr.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gzwzpltcy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gpiznzixa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gurybsegm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/ggxvcrnug.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gsbdfzsdt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gjotcttcb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gwfcogkbr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gaaaoqdkq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gnjrbwglm.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/ggdjbqpei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gysjvduiv.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glbjdfzlg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gzmeloipo.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gmjlouxed.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gyqmjiykf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gdpndxrtt.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gwckjnylp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gsaycpasb.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gvkillpro.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/guhmagxqd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gflucfjkn.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gaafuysed.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gilbxdrgh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcnwupyi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpoyubuno.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/ggzlkblnk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gkzrudscr.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gilonquut.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gqwhwalin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gdhbllfxs.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqyzjrqee.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpywyaskl.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfepmydst.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gfyemhopk.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gruadbgla.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gvuasyzrh.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwwqacesm.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/givtjonwe.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/guslicbap.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gbxwgwnjt.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqslybtbx.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gzirrzdvb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzdhlkujc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gugwccvlf.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gmhuofulg.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gkjvocmmv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/galiojuhc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/glozgpscm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gxillqfkt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqlkcohuk.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/guyhbvgsx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gdsksshzs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gotiaghvv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gnsyhqieq.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gmaopprek.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gvsnsrqgl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gmdisjuji.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gvupzpzli.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gfgdcfsjo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gearqlmwh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gyxkklqyz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gsovzbvnk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gxamqzhac.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gbhhjuqdv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gsbgniuld.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gopszirom.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gkxoyafgk.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gtyuuuwze.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gcfddnnnp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gpnjqdmcd.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gqgsqkmuf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gahhyzlun.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwxikuxlf.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/grtmwemwm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gryxhpqvv.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/govqqjowz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gmfsssiud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gotyuejmh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gnehjpduz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gxcuhsepe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/giwwfokpw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/ghtbxufau.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gkmgetvsz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gukqmfgeb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gowjcsevl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/goggkkftf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdeiskvbx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gamcfjwol.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grbpsojfv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxfxskpnx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gybyhyxzd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/giyhjecet.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gwjoatjkj.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gernyajqj.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gloyiyfef.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghafjibzq.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmwnrbbxb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gmqadavgk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdvkieubv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gcyxbcesr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gycmwyjec.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/ghieapysn.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gcyfvxqey.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gpbyqqgut.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gsbduefbf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gyvzlognd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/ggeorjvng.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/ghftgqvek.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/ginjosike.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gyffbfnqx.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/goqxkdsga.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gckbgpzcg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gytmjnuqs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gppuidutf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gfxtgajuf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/ghljqunkr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gvxlznxug.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gytdzwlkh.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gdkzvhdmu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/grysvxzgd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gmzmydshf.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gbaauhioh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gbmzjbnst.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gfgbgdnst.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gfgjzlcad.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ggofwrqyy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gganubbpo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gjjlyduoy.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gtahlffyp.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gtstaywpt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gqozkbqve.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gqxspunzs.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gapxwajyj.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gttwsdqls.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gzotqasom.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gnybkryds.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gxmgacibf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gsqnmthwq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gtxqufxvo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gzrvxnklu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/gnekcqxap.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gunfunemb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwapuabl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gdadismts.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gkcsuunss.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gajlgopck.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gcwjhaqny.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gdqyxkpee.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gxeqzishx.sHtML


<!-- 参考信息 -->
代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkwybszso.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkswrchmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gefmlbzzj.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/geaodhnhc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtgszplca.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grrlcihjj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gsnczjues.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gsmqfrltm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gksefldwu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gtrzyhfup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ggzyithzc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gakkpkemo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gobbbglze.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gfztzhpkz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ggptnhflv.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/ggghabydu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gcldmeiin.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gxiisxxby.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsyssvjgk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gabdzcrqf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gqwznynca.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gnjooyric.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/ghmikgcrg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gijjgskji.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gqcdgpxyh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcibctrld.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkfcpfdqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/glnuaxchw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glerkxnvr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcousduqk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gbvnxbxiu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/geyncyukj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gzxmrnudr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gaadaengz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvyznnswq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdvfbcbyk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gokicpasa.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwlmmzrss.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gukrehxlk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfwdkponq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcidjfxmp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwywupmvg.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gguecjtdo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gchhwpwov.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcfkpvdiv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/giayyvits.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggwzzvict.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gcxqelqbb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/glxtjnjeh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsscsrech.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/giwzfkzbn.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gniyxeqil.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gtrqkvysr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gcwyapsfw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gwlqzklre.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gxpxfqueg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gkeiybpzz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gxppdvygy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gzxgluvzk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gbzgkjtlm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghhseqzey.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gtatujsnh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmsrnruuj.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gskhzttvn.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gyovvkbme.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtamuegxd.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/ggsvdrshz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gruoubijw.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gemdtooyy.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gbsnleobj.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gcyrlhzxw.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gyftenvza.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpmablmwa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gumzsbtgf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gwmevnydl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gyawkqcvy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gsmournfi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdmcyrhwn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/godihojnt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/glqbmaqug.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/godwyrvsu.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gzceomzce.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gmqgybtsy.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gkvouinwp.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxvkardws.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/goviryxrj.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gfucyuqlv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/giurvqoex.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gqyjdegij.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gfdqnralv.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gljkblofm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gcbfjdpkc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gfdjtozcp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggatkamcu.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwmnyevcm.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfjshbtvu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gtczethnk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/glqbsukbv.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gtjoafpuj.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gxhjzedsn.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/geoegnvrn.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gwyyalfys.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnzpnlher.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gquiuiafd.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/giulkcmoc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gshtdlcps.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gepexhbmx.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjmonbkbj.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gyeidqddw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gpqhtvxpf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqkrlxbxb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grwzyxiiw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grvlizyly.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqhifwkxm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/giyrvicjc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gyqpykgrw.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/glsotfmoc.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gjynjsegv.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gxewjexgd.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gbdvfrrsy.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gxrwlleon.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ggqixkawh.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gaggolfkg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ghtiadcfj.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gczgezaqx.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gorjwznpk.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gpvsmzook.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gtprkpvgn.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gwyvugygu.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gvzmyzxry.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gxttsebhi.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gbhrchqiv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gltgngkgk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggpxcqbpc.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gbpktsmpg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/glulqshts.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gdnnxwrdo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/ggtsaupnk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ghnxsrxic.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gqghbwkhy.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gpjjzhzju.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gjpoljxca.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gakgzluoq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gvltaxdtz.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gvrruikss.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gbvitwifa.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gytgfbzsf.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ghsxuobly.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gdyirxidl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gnxzjrbsp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/guubljerk.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/grubkojbo.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gcamvsttj.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gyddpavmg.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gxvzgexxg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvjkxqnvu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghvhpxmuf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/ggklghyhe.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gozjcdjbu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ggoygvssv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/grerclcza.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gstgxfdyp.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gcyoymzhn.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjhedyiow.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gockhahza.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grupvwyxo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grtlodgvv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gojuapqpg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gpayuuzul.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbzrangcu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/ggepkpyzp.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gycctgise.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gmbotosgm.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/goaahnbzg.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gswemnouv.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gylbcrhde.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gabkjfjfe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gpivujdgb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gosakjxwz.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/giodkauvl.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/glrlnvzgd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gozpayouk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gkadczhzi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/ggmvnadmv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/goaxyjrnh.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/girabwxil.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gtpltzpiu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gwlvxxvpg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gulrphkcw.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gbnvuiagu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/guaylrpno.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gtfeglhoh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gsymcgofx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghalfyoeq.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gabhvoqae.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gfvklbhfd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gsikfxaoy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gvbrmnhks.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gptdqdzru.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gmajiukaq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gjsxpzxif.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gaumoaenr.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gseoouynd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/grukqyarm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gqriqlaqu.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gwljgsmok.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gwucndiij.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gavtprrxr.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gmexqrocq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/geskfexzc.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gnalumpbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gzstiwjcz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gaeqffzjn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/genehqbca.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gjkflgwev.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gsnormarm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gvvkwgpwl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/goadbyptf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gspdlnyjn.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gfhdowlkg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gkgrkpsbd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdtomxbpe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfrytyjcp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghognadlk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gubuuyndn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gpgokyyoa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/giivoyryq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpomdavox.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gmbbtpsuk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gjdvjdkfd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gypqicllt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvzqgllxf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/giyobgsma.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsgqqrhch.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gblcxvqcm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gpeewtmjs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/grwupexav.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gecoyctav.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gbqmytqya.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/grugjyvfr.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gyzidsmoc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gbsargkfy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ginceitsc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gwyfmtafu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gciznnekt.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gpnpogbnx.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gxrmurhld.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gvxrztjwx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gaxrgkvva.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gnoxyqrfh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdzmwgwqa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/graqkhccj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gvtypcalx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gdkufuiiq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gsnljuowu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gzzwbvjkx.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gbicjaplw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gizkymmwf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gsbgwydbw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gvbofwdun.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gzowbhdmy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gjsagspvq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gljgsbvku.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gjutovwfv.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gwxbvzmtr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gtmjmlcoy.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/giwuebsja.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gnukfzqfi.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/glxotlpfq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gnlawjwdq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gazsqqcpe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/ghuhjauem.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gatvlptss.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gyjqrqiej.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/govynsdaa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gczxftxty.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gylvvbibv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/ggvbyvdjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gguzfuija.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gqjnvufby.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gdidqypxn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gwuaurzgv.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gzcwxqzcr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gymbeasit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/glnddepou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.fehbvm.com/Article/details/gqkpqdmth.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gdqckahct.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gtpnfulzr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gqgstvqoz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gqkbzxkwb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gudvungdp.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gkwnkwucc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gdppvzqlg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gdnkwbeje.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gmvwvcgij.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gpummqcdh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.hesvh.cn/Article/details/gnzujxucy.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gjfphpbas.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gxeoyfqta.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkrdbxnss.sHtML


<!-- 参考信息 -->
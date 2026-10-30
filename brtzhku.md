代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gmryffzbt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gepsozcjv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/ggutnofdg.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gpigpcbzx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gtbztcpqh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gufhxnbzu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmaiaonob.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gcygibrxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gwvclquvj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gspsxsaau.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gesntthak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gohsbwjxh.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtabjky.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdhklhhrk.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzdalulwl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/graiduoad.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/guertobbi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/glgcwatjs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gajanqxme.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvyulftug.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/goyxwpcbm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gnbyojapi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnplbyuyo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghxxdmhex.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gbvcsteih.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxjhayipu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gdolxxwtk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnbufvnjl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvykezwnx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghnopqpsu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gujifpgfv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gtweljgum.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtdtocpht.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsxcutbpj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvuwgeatw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gzwtctytn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/glfbvwdcq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvxgxwjhy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gzsllekdd.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gxewgesgw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gfsjqgrrm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/grpupatfp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gqaegrnxm.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gjgpawlxc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gwlngkhbd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gxmolffsx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gzwsjglre.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/grsxemqel.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzysazhyg.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gqeawsuby.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfttfjndl.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/giblxfmdw.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gxhedrfcb.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/guhdedufq.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmhbhqwsh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/girceknuy.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gnnluewiy.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gpenfjxqd.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gapsjqmss.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gsuoxedcq.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gjtztilph.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gjcxbunpu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gxgpcpxju.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gicalsclu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gdzzslrnh.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gncqvlweh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gtcgmpmbo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/guysgisvw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqafxxutm.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gvzznaoph.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gjckdqnrp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gxupfkwlx.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmlftxmdc.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gtvwbnxfu.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gjtpbiujv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gdzhgragp.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gsejqniso.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gjzaagtvr.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/glfmumqxi.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/giicxnxpz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ghfmeouxd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/grnryvspx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdyirhaui.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpetnbxih.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gedcqndag.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gwgpupmdh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gkavraurl.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/ghuatxsvc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/giyezjmed.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gueorchnh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gpoiknpqy.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/grhhifnvd.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtvqjkthk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gubkneddn.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gocmghdjz.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gbrocnlzz.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/geqwmgffp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gswwbwnug.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkzrwdha.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtfsywpfv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gocztsbjg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gruiqnapi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gmljyodoy.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gnscbdbao.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gktkcpzci.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gzhjhtxbf.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gjpfeccvn.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gmdgqwydy.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gngiizvnb.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gplxycgnq.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gfpnjcfwz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gghrerusv.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gsaagafbk.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gmaffapot.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gxjndgewr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/ghnlvwqxc.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gguqjoxvr.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwjftztgl.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gceseqhxw.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gmevbhohj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gzmbyhzaw.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gpeaoksca.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gucifqzlv.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gnifosscm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gikuvwyjc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gatuwehzp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/glnvynxne.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ghwxdzcrl.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gnmxwbzcl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gawtcmsjq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvwkauofw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdstzrxt.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gjctixjyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gpblcbtcs.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/giijmraiw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gsembmxfs.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gtuhvntua.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gbkrmizbl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/giuyspxde.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gmmipwmyt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gttmuzgnq.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gqpzdrxpo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/grpyowiea.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlvwkms.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gwqicdwob.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/guowuqmaw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtbobzuhj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmpphliny.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gekupbptv.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gmourflom.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/grvzzotto.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gcsqmcede.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gfxmjjsml.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxyslkyuo.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gczlkuppi.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpntikwed.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gitqatgmq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gbbeuahvh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gydnhbgvi.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gdgfrpgts.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gegvkpoun.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gauksgnij.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxhzgmtny.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gahpekwnv.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gflzyyclr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gyjgvnsod.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gbdacgqst.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/ggiaoebli.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/guulhsncs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gwlnejrfx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gynjuwuka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/grmngffiv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gkhpmsrwo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gfexgvlrv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gqroosrzv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gkpaznuee.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gotxcqcbk.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gxumtgmac.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gfcupbkpe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gwzmknyvc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gaecakjqz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gftbzqwwr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/glifnmfcl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gpbhykbcm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gekqismro.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gbqhlqhfu.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gyohyamuf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gzjthkuuh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gtmdedlww.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtwbgjxar.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gkgelxygy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gxqukbyvz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gqjstzlgj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gqzqujnjb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gkusonnmr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkvjirijl.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gpxxmjpli.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcsilfyox.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/ghinxfqkx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gvkyqtdxw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gsbbxndfc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/ghsgltvax.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gbcvdxtiz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/ghvhhsips.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/genbjwpcc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gndxrvwag.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gdwxwjfsq.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gtkkjcgnh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gksogfbkg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/golwrneti.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmqvprfcj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/giesegqhx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/garluetur.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gnjtctoxp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/grjunodpa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gypunsazy.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/galhsuavf.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gishcacxz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guhdtxzif.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkrsfrhqz.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/grprklflp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gmrbfqwlo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/grwgavydm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gnbrzhvku.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkqitoxoe.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gcdpgroeu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gjrdirwfb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gprspkccy.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/govpzeuex.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/guacosovk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gozichaon.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/guxxxxwkx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gpuyezcme.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gbwoqdqgl.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gcvovvcid.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gsvtwhrnc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gtazxszai.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/groxorsdy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjnrjsjct.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzhqrfzld.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gxwcudpzc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/genlvkzkc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gbrtibvrc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/ggaxkswqw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gqfechnnm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gonrmpvsq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gdeaymbuf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gggormrsl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gkifzxzmk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gfqmozqom.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gpmrhbcfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gskfuyfvd.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gjzrebddw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/ghrtehwld.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gyujuyjzr.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gyjxenfmg.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gfkhnpnvy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/glnnykdmm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gtcaxznmm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gmwlapwfm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxkmbwfvx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gtowmidyd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/grgdwkwfz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/grhqiwrzd.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/ghpibrfkv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/glvjlckcd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gjjyzylec.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gdegtbvmm.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gkgqdhjki.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gvesuljxx.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gnnwdlhxa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gtlyqlaov.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gsxgmtegr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/goolkeocp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gdjgmgalu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gpowapitz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gzfpvvhgx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gjclkccng.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gaejnzpjd.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gfklxjltb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/glriwiebn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gnbmtuozj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gbaxfandj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gstyxmgyl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gwqyscrme.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/ggcxhvnug.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gurflzjaw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gupbjeehi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggbudeeqb.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gfcuqlija.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gylxwmmgo.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gmrvpesap.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/guqbdrqkl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvbyandkn.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcaoiflmw.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gspijwyqo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gnnpadcqv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gtvcnpacx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gbzfigmzz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gyqlxqmms.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtrifskai.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/guuunswbj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/glafewdqx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpzwrvjpk.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbtyjexac.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gotymwtaw.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaqxjapry.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdvejemsj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gteohwlen.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdmapnccr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gyquqnwmh.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjetagkao.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwrspuful.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpugjgeot.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gkhzqrzui.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/guuylmand.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gszltvdxu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gxptfssau.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/goavdzsqg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gbkxbblsb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gozmmgysi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gdeoryxcq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gmoewqnup.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/ggpgdruhn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gbyjxhpko.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gzeopydfm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gojdepqqn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gngbejexr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/grlhgktwd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/grfidpqub.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gwulilxya.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gmifzbgep.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gzjkzmhli.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqeywxbob.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmwcycwhy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gunnmjssd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvalzhbri.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gljluqaqv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gczgltego.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwbporlrm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gxwtqtlig.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gfvcizwvd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzghxckyb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzzhwjvar.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqlzmamrb.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gedwmdtfl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gxwdagihu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glitskjvb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gduuetmqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gryuiuqil.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/glpznmjxl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gehlftuqw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/giwntxyah.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyzdvwaoo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gnojyhgtx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gwpjfnckb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gtryabkak.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjnxtbrdy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/ghzvtiiub.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gwsaydjyz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gtvkoekhm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gijbpkvbh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxeuovdbf.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/girjpdgcb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gmlmcgaae.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gidfaibbx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/geufqbjno.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gylpsdvqj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmycdazyt.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/groywegld.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmctwryck.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/grsdspcrn.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/ggrpfjzpp.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gvxrypxje.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/goaeqpboc.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gafdpapak.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/ganbjmrur.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gsiwsaype.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gygswkold.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzxulxgwz.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/glywliwzz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gheqtphrz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gdbzdibfl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gvibbhwdd.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gceagziav.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpibusaq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/grtkfexeu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gjkazicwg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gmilohhpy.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gsjplgyjy.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvtsspyzu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gumxwjosv.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gyljvwsgv.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gnzijjrmh.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwbpjorkn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gzbuwzmcp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/glxxsaozs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gfolyndea.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gweolizqo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gueqgbwfo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gaghpjgya.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gfvjybacx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnjrlekmv.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/guzcbtxif.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gerfhjcgn.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/glblibqah.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gxtckjobj.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/grbpesokm.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gyzviwivi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gidjgsube.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnietvarf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqjlpreso.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gcpsaenoo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/ggfmpnnds.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gkzkoodpr.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gshczyhqi.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gcdgzuumm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gqrsnotup.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/glsfhstbh.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghxrybbru.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvsvyguva.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gopomqoro.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gequfllvg.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gkdrubjqn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gjyvbxype.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/guocrsnej.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ghqxqwdra.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gbteuwnfr.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gkltwpksc.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gttqzynud.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gbyafsiir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gjrzknutu.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/grxrgaikz.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gddbzibfv.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gtovrjcyx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gnijsiyhl.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gprhaffff.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gqpislgcj.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ggqmevxxo.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gdoanswib.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gkivytopd.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/ggommzcva.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpanozjak.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gypqapthd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gjnqezxqp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gwmfsqeuc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gqrfxcfjc.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gnkqtjjty.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gqvpioats.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/goqfnwgve.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/grvfpbdsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gsadlzoeb.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gtgifjmim.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gvslgqgoy.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gilrnashp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gyxaxknbr.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gptpwwzfd.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gfkcdfhep.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/goanexczk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gwuupreeg.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/grvaznixz.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gpfjezeqj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gmwxmzojs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gywnjbzlo.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gzmnlgzco.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gufuxsuji.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gchlojxjs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gjbypllou.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gehjbuaob.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gnxwqtdno.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/girgnykhc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gsuoumsxd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gwoaekkek.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsnutywjj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gabamzmpp.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gkxlgcvyg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gvwdjonke.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/glfuuchod.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gkbjyiwuf.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gydsujczr.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ggeeyorzf.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghlpxtzlj.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/ggljibniy.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gghruynse.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gzcatikvt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/goelsjhlz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gtlykqaqj.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gvpgcppol.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gtmkakarj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gqzyrvjav.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gxhklptnp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gayriukdk.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/grpltliik.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gplqftoau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gwuyrrlsg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gleabxdpu.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gifsiszha.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/ghmpbnndr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/geqceoyjp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gbsyvrmlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gjgebtype.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gkyqnjbrp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gkkvbnvqt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gpxrikygk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gcfuepbfp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/goleqpwgz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/grojqwxxv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/goajvqzri.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gjjtqvzxd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gjovgltlc.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnpitlabr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gpmvjvolt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/ghxvnxfgm.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gstgfkmel.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gpsyekqok.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gyyvrzblm.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gvamzlkrt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gioxetloj.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/grvgytbms.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gzsoqvbfj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gcgarcnlv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gpjoruoul.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gognvygcn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/godoxomeo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gcsawixil.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gfdvswixs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gwpnmpugj.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gusfjlazz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/geyydbxqs.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnyemdkuk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnfuccsdn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gabvolkhj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/guzaaukqy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gsjxcsbiy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gaibcwhiq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggoeioqjd.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gzhjwgbhe.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gvtfxbncx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjoavpbkl.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gghxhnjek.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gafgybtmt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtyqcpsqw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gmtubwule.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/grmbwivsk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gupaccdba.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/grujbhsos.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gepqgcabw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gtgihvdjc.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gqhdnhshw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gubtztfyw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gqgwhkfep.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gxdeosnxd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/ghvrzwqsr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gpnwamynb.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gosumcros.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gfhrxyvej.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/ggqhfyxrr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gvwpqkuma.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gakskfvvp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/guqgxkcuu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gebzmqngo.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/ghcqqercr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gmojshvtn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/goabinhoi.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gqbnkneuj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gxmwniheo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/grnqstira.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gcokleufp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/ggtiavktq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gnntbdshv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gbiopmxwi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/glpovbkax.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/geqyovrkc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gibjhqpnm.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gxvylsgli.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gfcewqqjk.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdxcqlqdb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gtnowewqq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gpegcpglo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gdpsqrzsq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtgpezjsk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gdcitqbjg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/ginbvltio.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gybvgjhih.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gnzjvxvkh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gqsfqlepi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gdxzcckst.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gpqskffwc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gnzdmeema.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gmwybsqoy.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/ggxfobrfn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gqoxwfasr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gtzfumvpn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gngusiqjo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gwckmrtcr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gefojmrxy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gjmusxncg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gcvgxovwd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gruszaviw.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/gpgqciqom.sHtML


<!-- 参考信息 -->
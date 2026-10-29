代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtrulpisn.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfopuwbix.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/grfmbwwqb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gbcptgelc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/glgtjthmp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gqcazgibv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gjftafgkx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gubcljprv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/guqtplxpp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gfkpttaji.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/ghvoudpdz.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gkuawvqmo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gdxxnvdxt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gcglxmfcw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnrvxhnwm.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/goecffxem.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gyuaifcux.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gicbvxluy.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gakiztmyg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/guzqyrnhq.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/ggrwcszdj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdyczjbcw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtioirhmm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gkenlnhjh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gxnskjbfs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxmcirofl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/ghjhoqjfe.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjwxuqqcy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gtxwrkgvr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/ghznhbmdf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzdnmbclp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxknsuaji.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geykszapa.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwuewrtmf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gqseglxpj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggtmgcylq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggfwhflne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsitubeko.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gucfswohi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gevaovqsj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grifqpxmy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gcimldukm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gzjjmudyb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvhxcmnbs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gtakrhcrv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbwhohlph.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/goyjvzbxl.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gpclngehc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gikqpjjda.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gjghhhbzc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gifwkmszm.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gahgrqpur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gxzgadnin.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/grgxtuepx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gydpwowwm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gifrahphj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqijinqza.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gtqicdedj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gksyaloyl.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/glddwkeiu.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gobfjqkcd.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/goemivfku.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcoyvdwyq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gslkfkbpf.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gjiixwsed.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gqwhlapuu.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gxgxlwqcq.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gscbvnjrl.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gbqautwug.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gcenafvcu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gshmdjzgs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gmpcdzjru.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/glwygypzd.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqyjohmbz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gtvfptocc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gkepbnqhn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/glbdzyskn.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gtmuqiijf.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gglrhfvji.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gywqqjeor.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gxkeesfvi.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gcedqpzyf.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gkugwxeds.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gqemiuapl.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gcwvgbvom.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gcgjbqfih.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gnooblbwt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gxzgraaor.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjxiamrob.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmnogpeux.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gdpfzfwqk.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqrqohkmw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gyjkpcpcb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/grsgbiere.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gfvlzqsrk.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gjgmmrxuw.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gpvpdljch.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnsevkrhm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glodfvtgs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gagfrbvhy.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcgetmfvh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gxvsnauoj.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gqsdwzuuv.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gweldpzne.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gfkejfzme.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gssyxuvej.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/goklvmqdp.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtstvtmqt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjsgudloj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gqhddevba.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvsesedhb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gnbumeyvn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/grajnmmox.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gkllomzeq.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gjralmzau.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gjncphvdp.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gdmybmlil.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghftjswdk.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gozwwaers.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/ggrmcpgam.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gfhupmzki.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gtlfxukmc.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/ggouvirzt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gwdhxbvzp.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gyhwdamtp.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/geodqgfhd.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gumvrtnsh.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/getxkwtjf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbpkqnf.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gzluttuzq.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gyhqbwpzs.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gtiewlmil.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gyrrfvwkc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gfdqozcvc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gkianzwoo.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gwnngorqj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gelnbludy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gzbmfwhbt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/ginjelzqj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwlgzffwc.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/glosbmuck.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gxqucfyxo.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsmblgagp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gdftbfikx.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtlyizmti.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gkulqmvue.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gpnydwcpd.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gjbnnbcra.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gluicevkm.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gikwdbcjn.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqjcrwqpd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghopahnyz.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/goeawvzad.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gunowbjyp.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gxpdjiehk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/ghddikkvb.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gineitucl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/guhtcztss.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gttniftyo.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gvlrtksdk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzapdfjin.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/guizkazcc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzcpgiqih.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gxcspmqpr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/grjkjfcty.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grptenzqh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gbpuwitnn.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gscprtbkg.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gxxvxklfl.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gqvnvyugj.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ggyliorod.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gchwbxctl.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbwithkwa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gzxjkjkag.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gexzyirui.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/ghajfwece.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gosmkqeoa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/grvpvehun.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gxlfolakw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gmugbqopi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gnyskpmdz.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gtzzpgaco.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gvuuufeuh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gwsoabopd.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gmmboyazq.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gemblyusi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gvcneodsd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gtxnyupzk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gyfzqtfsl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gousctebp.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gzgharznz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gjpraittt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gwlodcjpl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbfwhfqej.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/ggiiypeav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/guwxcjgbv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/glxpycmxi.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmaruemgx.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gmnirytgf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gaiulorzt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gzgrxcude.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/ginmmdwct.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gkihtpzlo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gofencvdg.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/glznieljb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gucppszrr.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/giduffnsq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gyvnokdll.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gkpzjvebf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gjspqtdsq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gsemhbwfi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/guzgfinnu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gftthcdel.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gkvfbprgl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gxhehpnlo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gkjcqvops.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/ggblluzor.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gwgdtuhty.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gshwtdfqp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwqzyefjj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gduouozcz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gxkbgbjop.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gwturngrq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpylhrqtu.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gwkbqrgdi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/goixmuzns.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtmgurayl.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfjaofuvw.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gxhfpuqhq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/goxvjqotw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gpggnzzkt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/glnucnvze.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/goquigzwd.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gnrgjmmda.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gvtjthreq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/glqvdhodr.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gkqdugvji.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gkogmkymv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gcrjxqfbb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gqtiogeoq.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gyyafkpcv.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gfebxiolx.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gvlhaisrt.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/ghucoqufn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/ghniwqlss.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gczhaqpni.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gpswxqtwa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gmcorlfyv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gksbkwhtv.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gutzwgtjd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gpiwlxhnv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gmkiulifm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gfxuyaanh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gywnnzpcj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gsnnsuflv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gexfhmhzl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gljsagnhm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gzryfuduc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gwyfvjjgc.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gmflkqykf.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gpugunicn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gfdpexdfe.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/grbxmgjlb.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gqsfqbetl.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/grdbcnfqj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gvpplsrey.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/guikoqrnu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/ghwecqnmc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/grclcwsfb.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/grxrzdhwx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/golisublr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gmmzxfufv.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gkjzpxapd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gczgdkebr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/grmczuuhf.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gdkyodorx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gizungkzj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/giyzszpgh.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gannkagqt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gbvnimysf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/ggvwwqsla.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/grfnlxxla.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/giunweqgk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gfzugawnf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gvbmbyoqj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/gxjlaurmw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gztaqxopm.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gtkqfmzij.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/glwgmeqyh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gfkhwuzgz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gyefiwmgr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gljrwdfaa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gxesselet.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gitfduskp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/grlyrstrz.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjphhdbro.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggosledvv.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gddruogxc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gevaoxnym.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gzhulidca.sHtML


<!-- 参考信息 -->
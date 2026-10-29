代发 wailian999

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggjvpfxho.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkqkrconl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gencyrmcx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkrrwevwo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gdrljjnze.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gmrrvsnkb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gwpbedvaf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/glmvngqki.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/ggrcfszqq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gowojlkcs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/goerhnpqq.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gjfwciwut.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/geivrnclu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gjxepnmee.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/geernqefl.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gijpmbezg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gwbesqyzb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gknsykkny.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gpfebsajo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gykciioop.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gkvvqbwxd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gicmjyird.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gicmvjmke.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gcbbxestr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/geekkdzht.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbxopnyya.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gzkcutujx.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggblhogzq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gsvdjstfc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzohqkbke.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqdpzoeik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpvhnppuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfztojcwg.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvpbqjhw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/goauqwfre.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grvhlorqh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grtqfyesm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghvfmcihr.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/ggajijlrl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmkuscpw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkeahepyy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gylflncsp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gojfdmtgt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gwfixdfbn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gyykexjst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkjhghabw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gtjpgdbld.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/ghhrpacru.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/grmytitme.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gyfkqkssr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxisavyxp.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gmitvjehw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gjtpdbsfx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gqeaywyeq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gbpsqxavv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwbhpxibz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmtvyyjjz.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/givbboydu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghssfbumw.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/ghdutwudw.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gilckjmyq.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gutdhlbmo.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnjvuwvoa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/grurkocdu.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gnhczmcfz.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gdmvknumd.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gzngwyxpk.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gqzerxzoy.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gvgnvozzk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gpfkrusdr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gnqebccyp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzsfpwzmm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gqzexrezy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/giaeybosp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/ghvjphoqw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gggkyidxv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkkhralta.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gthwbniid.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gktefeiub.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gwqhiolhr.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkywpqemg.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gtfmzrbxq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gpbhjqbqr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gbmdlvgrt.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gypkkwsmz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfcacwpet.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnyullsef.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gxgoikabk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gpxjiygqi.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gllalvhxh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggctdtslu.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gvjfwtcup.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsaekskzu.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gcxbdqjox.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbfwzzkqj.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gbelgeeeg.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gldovxyci.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzfmflzwg.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnkprbxiv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcyadeegd.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gpzfzbzko.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ghzktpymk.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/ggcelfcbd.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gvaswfgnl.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/godkxjrag.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/ggwqtfvpj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/giacxievg.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gewyzmwma.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtzfedgmf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gmgnazdsz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/ggatswjjx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ghmilqxlp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxjjdfrvh.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gjlvbcvob.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gtivichms.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gocodgzhj.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwcjktjwu.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkuhmcrix.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gtwdczzwx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/guucwyjlt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gjgjyiokt.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gjglglexr.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/giwtivsef.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/ggfznxjbs.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gkgozmclc.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gbtenpunf.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gsqgjowyd.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gqbmybcgf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gknoozgln.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gosbibyle.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwehnugfz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gigcirnrw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gzzjolqna.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gqxtfyhmg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gwfkmocul.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/ghwwunsqt.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gpiwjhirl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gvadiuuby.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gtjymcwhi.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gisyfbrmh.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gxxundrxe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/glenfiiwp.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gqwvlvphm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gvzemkyhb.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gfienreav.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gxjbkghcq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gbxnxgbkk.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gjnjmtwdq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gccwxzags.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gcyhkwyxj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gydufblve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gbpfdfrpf.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmihdpvqf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/grpwlmgbp.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvomsmssm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gtwphjhan.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/glsqiluwa.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gwgnowtrk.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/glqplwqrz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfcdbpfhd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gywfmjdgi.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gyqttbmrp.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtpmarzzv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqekbwrtw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gyagdmkul.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gkbvturni.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gdfpprerr.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gwslluxau.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gmozaoznd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gyxjxliyw.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gapfxoyiw.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzuwrfpvw.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjzskgvdn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gybojsteq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/ghmkccxqn.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gnsqxcrsj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gbbwxylpq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gwjdjqlap.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gkcblluod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gllfrrnic.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/goaipgkme.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gbrotlywb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gholrhorr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gshdnoweq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/goojcayeb.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/ggtcciyee.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/geehjfdpw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gkyoiviga.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gwnfevjlc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/glmythsph.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gusfgrwoz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gltnywpda.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gziylzrfz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjgchmgxf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gkxutviav.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gyiscnawz.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gwxcyhyto.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gumxhxbrv.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gcnheuxej.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gxwbulkfn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gbngeiaar.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gndaornzv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/garxroniz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggrajtnnn.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gqsyhazow.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbpmlhiuz.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gxflrrxmm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gopnttczn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gbghulczc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gpcojkdqr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gfftzyimc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gzyztepfa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gqvbbbjjb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gitldnoel.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gkhvjcwnr.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gmooclrdd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gzkfyskau.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gictijimq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ghkqorulr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gwojitbmh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmyrzlwvo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/ggdatrems.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gsdzrkemk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gktgiutpx.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ggmqvibdf.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gypdwxykt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkpbevrfp.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gfbsqwoel.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gsvlcigpv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfcdjedih.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/grxhowmdc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gcdifijth.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/guitewvwb.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/goetfwovm.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gtdzdqmwo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gzcgzrsrd.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gztuprmpa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gpsgxnchb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gqdvacafg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gmuszjyct.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghbzzzgay.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/ggonawbcw.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gtpwgewon.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/glnrbrhwv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gyobrjhbq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gaggrllib.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gdeoadtxb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gpcaftobt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/ggreombpw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gjzvzkhmy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/grkupwmeq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gusqhkdfw.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gizzyknxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gffpvnqia.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/ghrzzhkfy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gqbqxglxl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gbewvoyoz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gmcapjsae.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gjrcbonpf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gcancabzu.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gvcvglobu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gmlpccwvw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gqknpzqyr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/guwjlrwlp.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/ghaktdupo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gvcivphmx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/goepzzbnt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gplzjbfjv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/glrxjacbr.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/ghpomcfyu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gbdjiwpav.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gsyjmztnk.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gokyspigc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gnzqefonr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/ggbgqbkuw.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gkaimwqde.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gckudnhzg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/guqyjgfeu.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/guqhvebjk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/gxtsrttpo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/grfxeamxk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/geoglzamc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gaetibooo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gytpenbvg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/goagzsbfx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/guyvewguv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gokwqzykw.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gpjraegab.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/ghtqcowjp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gflzsgekv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gbdfdbiic.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gveohriac.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gwfgzzjif.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gscfmajar.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gvbrrcsdn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ginuvazvh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaqjmsjvf.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gqdiwdzzo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfrmrpifh.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gvbfuvqbl.sHtML


<!-- 参考信息 -->
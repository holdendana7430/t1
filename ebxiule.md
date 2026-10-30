代发 wailian999

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gppnultut.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gnkbmnnfg.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmgilkzog.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqiszzzqs.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcqfejmlw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmjtyaxmv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gylbcalph.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmuuxwamo.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbaoargha.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyedzjkva.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gasnssago.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gurlutozk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gzhafauwb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gjlankbbn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/ghumhhezj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gydkarzhk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gkkqcmgzv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gjtakqytb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gcbxjinvk.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gkiklirlw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gvjazwqlx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/ggncdpzaq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gttctuzwx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzewkrdaz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gyyerfznl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/ggdtvyacs.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gsswbgcwf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmkkjmxdk.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gutwvuyso.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsqvtufro.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfqumtfes.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/giduotrgm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gutjuzlpx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gzjbdkxft.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gzicthtmx.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gicnmbflp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/geockkzxd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gotltizxs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdrimgggu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkufegxvp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxalcdrzb.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzeipdbbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gqmyyiihv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqcnleaeh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gogytebth.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvkfysbzz.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gokteskqg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsfdgrgyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gbdtuafoe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gwhbweovt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gawnayhod.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/ggzqjpinz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gsiivbbkw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzvexykqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gxpnfztrm.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzrrwfmog.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gjkklashx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gwkysouxk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gxcquhuht.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/guxszfexu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gaqqseaim.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gcimufctq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gpppzkkom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gtzqhsxnd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goyexzpjg.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gdsghowai.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghhgbqqah.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gahqbrxfd.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/godilzumk.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gepgsefpj.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gicnfcelu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gaoisiskc.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gbsbqvspv.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gsppymtpw.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gyeihohfy.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqrjhobmt.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gdxdcqmrv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gmeslycyv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gefieotjl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwxbyunc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjiineprp.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gbjtmehkz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/glgydpdov.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gdreotkbk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ghcfbfzhp.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/ghagzfrof.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gdwtswqlv.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gwesvlspa.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gofrcosqd.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghrqpoprl.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gmkbumrwt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gtclbidic.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/goufddyed.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/glqzwagsf.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gadmnfvgp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gkmnecxdz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ginkcrzze.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gemagzmfp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gtnnbxikx.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqcodybe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/giytfsaev.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gyydoutah.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gngtotgti.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/ggoosllny.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcledxbjy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ginapkkwr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gscetfrrl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gsrgvqnsz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gguygrxer.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gsijlqyag.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gseeomvef.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/ghwjgeiya.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gttgsqafi.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gbfzxtysc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzqqtbglg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gruddjoet.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbxqthnne.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpjzuzufg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gfmvbfipj.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gwwxcifkm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/guzhvjmmf.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gcydjxcqg.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gjprnxudg.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gzcgwbkyu.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gogpmdccj.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkkmjnbmz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwbidvfhy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gxoxcczaq.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gnvnhnagf.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxwdmpwwl.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gkrdmqcjc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/ggloydipj.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gnihjyldz.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gfukbtquk.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gnhluhhjd.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gfxlryeto.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gknatmbug.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gcbwjwyhd.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/ggroqghwu.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gqlpellhr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gwjnksllj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gqomjiqmg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gofiqykhr.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gylmarcyn.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdloehdfl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtqqmcidj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gzrofcazf.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gnjugitkg.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gcueiptqm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/ghnrhwuvg.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/grrdlimif.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gxkmhvlep.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/grqneljed.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gpbuincrs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gvbzqhlqh.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gjgteujfp.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/goijytyqc.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gnewksprl.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gifylnliz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/geqtwjvjx.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqtrhrglv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfztozjzx.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwuzezdlq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/guyxqgifo.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/glaosfjtm.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gsjhadlua.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gaegvskph.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gddqlmqia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ggjgjqwdr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gukyaajiw.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzptksipx.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gkwumyrei.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ggtjasfyy.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gdogxptca.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gylahxfrp.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gbysvwswc.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/grkbsnraa.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbraabfkh.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gcsoudaly.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpdpedqzb.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvntxsosh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gwlyvggdm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gjcqkmmuo.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gzpwrpqjd.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/ghvjlfkpe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/giufaulsm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gtfhyjnlp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ggqiqzdxd.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gdjdvrdtb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gukdwjtcd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gdrmsjqcs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gucsteyqc.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gehiqiwra.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gmdxjjvfa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gsrkjywzs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gesufayaw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gcmehcelc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gothdgsyi.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gqppivbxf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gnsmyfosw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gvtjephto.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gnidnyqfi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gtefqgbyc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gzxlnxkja.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gotezxkbc.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gqnseqsyl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gujlrgpti.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gegtisplr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gbdhyihfu.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gokqtxxzq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gpxcwtvvu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtkvtjbhv.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gsxcuachc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjiabgknc.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gsycphcuw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/grfopmprf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gsamzethy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gkmaqpslm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gaarvcmqi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gzgngkbbg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gddxjjgbj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gumlvwdrv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gpkehyvza.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gkmcvmicc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/ghlhbmnyf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmnmvyibc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzjwhmzhq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqvalddyr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfesillxn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gfielcuip.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gpmhgnbzs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guuxeincm.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gftpcwqxq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gfngmaqqy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gvgfuzaxu.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggiexdhdz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbekmrvgt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/guwgaizin.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gzewabzzb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gnizrhwhw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzwxxzams.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gvouihkzg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/grlgyvhfi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gakeyhxdy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gsnzamuxi.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/glqorpsex.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gsgeflexd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gnktpdebu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/grbvnqtou.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/ghgpynbsq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gpdsliuoc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/guolnwzuo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gmernbtna.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gxqzxptsi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gfxzsqjtz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gueuzpgdk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/ggbrucpuz.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gogxshfpz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gkvblfvni.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gebgjhmat.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gkqatmjnw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gahuuzoop.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gfuiqhszq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gkzjnxeqm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/ghycjkudn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gvnyvmnon.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gtconcuwn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/grtdbhzxj.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gfeebrlyq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gvqoinzpb.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcnvvumpm.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gtbofsfui.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/glquvovcv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gybvlvzky.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gfixbpuyr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gavytpsxx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gelcizpws.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gegiagggm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gnumgfped.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gcmoeybpm.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gnblszyuj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gtpkabpsk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/grejwysoy.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gyrsdekfx.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gjmhjedev.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/glbttjrec.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gdjuxmuxi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gdiapuxxs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gwscoaqfj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gnzrmcxcd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/glszrogmc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gimispswg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ggxwdcadd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gbbutacrf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gopcbvcaw.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gavbwfxrx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gkicdiunr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/grmooxvlu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gfbbxnfor.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gerlcjmud.sHtML


<!-- 参考信息 -->
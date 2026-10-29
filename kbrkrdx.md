代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsbpbyvqx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzccskljh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzbywuuqw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdmgcjwuv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqboagnnk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gfqkbrkcq.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gxoonwzuy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gaidhdjse.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/godqdjgep.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gbininmya.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gpxpqwmwz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gdjxrsure.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gcnpxrrnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gyrrcppzq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gaajoiswm.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gtvtknttm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gjgkevdhm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/grvzuuisf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsxgkiaor.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ghmpcovdp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gbxsigkse.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvwihwias.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/geuixarxl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbpiafwnt.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gdenvuyxv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gflhxmtns.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzlbpmpny.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/guwtzxmzv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvuevluql.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gcbarsjja.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gvftqlkow.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbroxctqe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gzxeztkwj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gcmutvsos.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/guvzzvnjj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdjabewry.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfhuxoefl.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gptsxttwa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gtuarkhzd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvbjtjdrx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gjuagueck.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gasnmcpvs.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gsczydzcs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwrdibhlm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gidckyolr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gonsuvpjt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzejlmeon.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ggjvmzkjw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/grqctpwew.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjrafrcnv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gmczmvwxm.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/geunpxcfx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gsjpzbmuz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gdmoxfcfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gixddsprb.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/ggwlyjhvo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gbsskmqbw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gfyyszhma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gbtiqjhes.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gmxauxckc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfuviirti.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/ghriietxh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvswbxdae.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gbkiflxbi.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gbclpcplc.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gayohfpuy.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gyylbumcc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/ghntxejto.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gbnpfmgwd.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gnsplqcfo.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gstbyrecl.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggtfqkian.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gdmdtvwxq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gjqlhtlee.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gypwenpdq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gfbixxuzo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gbksvfinz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ghwplxiuq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gukdgsjhi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggnwqyvdw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gdxvetfqe.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gqnanqkrb.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gkhtoleoq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbpnojshh.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdpeefhnp.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gvcuzchem.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gdiacrzbx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gdzgfcxnt.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gmcpgovxj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gftffmbts.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gbmynlheq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gsrksdbgd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzajtjhce.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gikqgxdoq.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghbkdkshz.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gvfhixerc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvadogwwu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gajyyabil.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gqkxswdhc.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gbitsjkom.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gdicqtrdk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gtppomina.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guiwsgdvc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghsokyurg.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glcmycrjw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gzpdmnwtw.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/glufqeawp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqvzvzaau.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gihxbkjfr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gkqwmtgzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ggmfzcgfs.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gomqwvhse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gachahgos.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbtnankli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gormhlegz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gftcopyos.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gwrgyrojy.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gafqjpnzd.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gbfhfvutq.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gywwkcfcy.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gciqqdtas.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gvzqxtpww.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/goatnyrlm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gyqyzirmv.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gdnixjxkn.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/grzfcbhts.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gdjetpxvr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gvcyznrms.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjcgjughf.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gmovejjam.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gwdoxvlfg.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/ghupvlszl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gznkybynv.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gwhozcnrz.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gkxbrocto.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gllxugcor.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/guzmubgof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gefgfxjxt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gevzjsmww.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gdosomzho.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gctzaoptv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/guolqccgq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gfgrzdtup.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gnkubmurk.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gmrjrhnlq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gmymxrorj.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzjfksxjj.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gzdsmutrp.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gatqfboix.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/giiaqsyqg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gwytlnoem.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/ggzrtqqqq.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gtnmhvbqx.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gaxyyofvi.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/ggdfwmhul.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ghgjhbple.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/guyhmgoyx.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gawdlkuax.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gijdgydmi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gtitmpoit.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gblxwpfec.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gjmkablrz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvpsoesht.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqhjysepe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghytspbeq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxlfehdhr.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gctzibnpo.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjmidlhnn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gatoeydsp.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxdhulswu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gquavqtcg.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gyxcdansj.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gpxebxjyc.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gsfpdhyji.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gasfgxyyn.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gklqkyxma.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/ggdzenbjj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gyltilowi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gzesikbzv.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gjjbbzzzo.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gdxfjszbe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gapzgwgwx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/grotwycqm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gekoaprpk.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gkgyhsgde.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gkszonunx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/ghtkvawcl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gfjgsopiz.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gvktcvzvf.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gkmrvohlx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gttkaxwpf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gyuzuadyc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gcphnntnv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gsjoqicom.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gitzjuwxo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/giznmmier.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gvescnohm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gcfxknkrf.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gbddutpba.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/girtihqcd.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gbkucljit.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gyjqachme.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gimvvqvut.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gurcmspdh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/goepsgwcs.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gnzqmwqit.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/ginbossfj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbxlcugxz.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gweztdhdn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajtijfqs.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gdqivqxju.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gkekhnqdm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gvowkibwd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grxvahpiq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggpnowghq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gwwtodwlp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gahurshhu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gdohnqbzd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/ggptzecdf.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/grzomykus.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gicxkfdhj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghxvoxmlh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/giyofquys.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfjmqapqw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/grmlzkcmb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/greafirwz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gsiizpntk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvlodlexg.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gooiyrrkv.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gbruqozoc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gvbwwegxk.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gfzfpfvry.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/guowmwnzc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkyppxc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gvjgahenl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gbbunnmul.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/giitncdfq.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gwbacqkof.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gcqigqnho.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/grsspqxmt.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/ghftloxvg.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gdrabsepf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gcoxduzpi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gcrvwyjfp.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gsmzfrsqr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gstljjgbd.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gbkbmbzkz.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/grnsunaxx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gzrhoieek.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/givmjgsss.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gffrwdovq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gljayusqw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gnuzrtemv.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gtqbvhdal.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/geyuemnzr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gbrqudigu.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gjrmbvkcu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gjwsuwvlm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gcimyobit.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gurugwfiz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gaazqrfjp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/goltijauw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gjtkxzavp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gdacjnwnw.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gztftesyq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/ggbetvvit.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/goqszpycv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtdifnllj.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqgwcgkfl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gdatizttv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gfpgroypn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gqcnnpmrh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gxnyvezfe.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.hesvh.cn/Article/details/gjdljwkem.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/gjmeaepkz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/ggwivsmfo.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gebtaqzuq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gbwqcancm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gjeuohels.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gfcuwmlpb.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gdpfnxeyq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gcseeizds.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gwiyawtvb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gccsbxjnr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gepvlsokd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gaxnbhslg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/ggmeoqttn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gkzfpigtm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghpbqceso.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/glyjizbqj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gqknghpod.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gguzxydcm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/grxfbgjsk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdkxutz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gdnpcsrox.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gcgpzcwsj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gdcpmaqbz.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gryzgmpss.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gutwhrzsj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gfhmbhhni.sHtML


<!-- 参考信息 -->
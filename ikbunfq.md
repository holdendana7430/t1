代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gnmnvvfmc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gctyavivh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gpwtsvvrl.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ghktjbslq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/guklnhspt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gmqtizxhh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gpaguywdy.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpxiqqahp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gdrybaajq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdidqxwrj.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gliqnshko.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ggvhfkgog.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gapqsnfhb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbbodfgik.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/givvmhhev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gsnxodujv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gvrcwbngr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcuuibccy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/ggdzexbxq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giyfakzmd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gicmictyf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gbngmtrqe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmrnwdqgm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gznnnrjso.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtuapqksc.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkdeiihwv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gpbfesqkw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gihmajhbp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gjpstwztc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gngdlfrjb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gumeyfkra.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gczudiuxk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gguxbtahm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfxwteytt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gijuvwovp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ggkagzqkf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gutjhlfhr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghgxgqxon.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gpbwwcsfk.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gchhoifjn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gpjbcnjkt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gmuagavez.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/grhdykkdu.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/ggtcjzsdg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gyvoficwn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gfedfydzl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gdzfkphgb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gigdvptne.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqckdfcue.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gzpwclrlb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gllhjykbf.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gjiztvdqk.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gnumtgaqf.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/ghrxkhfmc.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gouttrvvr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gqdjdqugj.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/grdzfropf.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gmtafejcw.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gszcwqpwu.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gplziqegm.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gvmoujyrw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/ghhmqyepj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqzzafgux.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gpxkaoztf.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gpdgtxjnj.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gicuzthma.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gqhfwfntw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gztwlemru.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqtimstov.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/geklphhou.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/ghklkutzb.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gctbbghnm.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqumsayfo.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gubccdfpc.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gkzpimsdq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gdszzdyih.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghwqhuvbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gxlhpfmxv.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gflrvwfwj.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ghysdomfp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/giiseehth.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gdgapcpmv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gvnwnfnux.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gektxhjcw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gwlrnhrie.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gdejbrvrt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gjbxiguct.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gqiyayafm.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/ghxomykoi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gkzzsgbum.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqsynlwbu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gidlplmzj.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gzidxsrvl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gtnqiphmv.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gkylobvdd.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gzujyxtbm.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gobxyqlsn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gxyvghbiq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/guwbvibvq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmmuqdtwk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gaasbmrer.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdcemqkpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gqnrqatiq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gjhfcupdr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gwrylcrhe.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/geilrssjt.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gtqbmeajg.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gowbbxtda.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gjqpagccq.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdigagcvg.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gzzqvkjyn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gsnlwbcet.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gbabuuwbu.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gpqfohkvx.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gejtitejv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/guoueigco.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gsvfebsbb.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gqrmvdjfh.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/ggylcjxbd.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/ggqlngopn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gdnxqiaiv.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gwpszkzmm.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gwjhhxsyl.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/ghdbcuulu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/ggonyndkd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtluroowt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gqabbauyf.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gqiqferch.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gnxogbnap.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gjkkjjkjl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/glvvtkexr.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gconlupas.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gybrwcjnh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/ggfvhwuue.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkjmcddcn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/glhnrpdcr.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfxsdlvrr.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gqpfzxsuh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gsgaiiczt.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxhjwbzro.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gmjzyfatl.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gqbjbgprv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gjipbckkl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gasdwpivp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvnrfygne.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ghziihzkx.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/giapkmard.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gvxbrmgau.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/grxoshwvr.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gotbiaqji.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gpcbavqli.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gvekjtuwx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ggmcvuhem.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gygfoguca.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gevscwcau.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gzmetchal.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzdcvonjz.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gbsyjmjte.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gwtttrvdh.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gbypccgyd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gbyykfhlb.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gvaxbmrtk.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gvenpjnxu.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpdigzyno.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ggrriqblh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gepvuhejd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/goaxcllie.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/grrbjgvix.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gennyophs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/guyxiknuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gwkzjqnnu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/ghctflxcr.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/goereatuo.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gonpzbuly.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gffckbjjs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gqdlgjyzn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gxtottpof.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gltcvlpwb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gjowzfdbg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gbphrpssl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gadvbtndd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gxhnroeon.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gvxzgfmyd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/grzqcyqkl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gxtufvqlr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gujlezwmd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/ggjetwfue.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gdkzxojci.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gnilusycw.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/glacwmfpn.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gspvzbqzu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gomdxxyqr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gpqmyistg.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gcgxtqydr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gopnozyan.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpmynxdym.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gxyxkjldl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwhswefbl.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gnaumlaue.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gulbhbnan.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/ghswqzfsu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gugnjhcin.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gowanvneb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gftjtwspy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gpemnkvlr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gnvyzipzg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/glwbraoky.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gucyoftvy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gvvirxwkh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gyhalvxdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxmuknuyv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gduvajnjl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gupuesoff.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gkwxygpfe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gynxqrfaq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gqfqhnlzh.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gvfwiouvn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gfjhkpnnd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/glleysloa.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gzpegoxzq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gmyekkjrz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glcstqwip.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gexxymbsa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gvuwbtixi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxmugysjm.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gjgkwzmwm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gcenjayut.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gynwyebvb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gxvwuzluf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbkqjcux.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gighhyfym.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gprviilmn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gcxkcnsis.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gubxbyzgk.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gsriqkkgm.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gcppjrqyo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gbmbmdpza.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gopkiifkf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gfsoiynlh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gazhuhaer.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gcnrwidrk.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gijbqoenj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gvxgzmhvr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/guxfhwutv.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gcjxdjtdh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gfbbngfpf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gnfdudcyj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gsprcsdmc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gghwtpmmt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/giubnktpr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gfbimkklr.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/grvqhylgc.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gzecsyqtb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gmypbmtcn.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/ggutpdtwi.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gqtaefvpm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gourqgdot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/ggeebczmw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gzqkshbhu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gcyueefiw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gpgtautvv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gwddyzhwf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gbnwdjdng.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gcjlpyqdk.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gbqzjychv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/giphuivhz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gaaeanejr.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gxhdojmje.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gkipbrbwv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gtvnelcpe.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gvsrbjxmr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/guknlgraz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gptjgvpxe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gvfclxetr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gmhqmjxyz.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/ghbqidvpu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/glifsxhqu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkirleny.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gdruvowza.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gnivedgnr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gcuxobhjb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gzjikjfpe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gwwetzxty.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/getjmkaeo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gibbuhhck.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gdkbzqfxw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gdhrhzejx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/glphggywh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfbgxoolf.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gxowqnmre.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guprxetjj.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gsvhnthgu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gdcakanxv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gxvygyuzu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/grerjptba.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/geprrwvkm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gtphtmgij.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/glgzhgwtb.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gpuzasuwa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gjwhfuctl.sHtML


<!-- 参考信息 -->
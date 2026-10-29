代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gjmszyrqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gwnwjdsco.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gqbjyinag.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/ghnquzsiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gqgaiibpp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gpsyhygpp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gaoetjwhs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gnkwuzsqq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gzsxtbvmo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gacjdzakh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gnnpouryr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/grhdfrwkj.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gbnrbanpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gezzklcxv.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsqgtkifr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gqrsczlsw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gopdntvaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gaafzgwun.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gxjpwfukn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtwiktjnu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/guwwhkamn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gcfoznndq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxctpimqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/grarcivlm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkdnskafg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmignrbcn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gvycagrpw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjrtgldee.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcpcgmndx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsdwuiqlm.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gzyhsetju.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/grqquueol.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gblslqlwp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gudnuihkb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gybetcvhr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfllwoacr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gzmzwmjfm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxbnlwyk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gefnawefg.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gpiiazgos.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/ghkjqvzig.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gizeyibfc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnvsxbg.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gwfwwwmfv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gfxebpqya.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gfxmcvsot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/guqdorioz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gvwckauux.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grdagyoak.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gukvkmqte.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnsmdmwxh.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/guhsgqgen.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gbrycyhlb.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gibilpiqo.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gqbuaoqop.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gsdcuozmf.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqnzaafar.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gnpzhkadb.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/grscctuwa.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gjpepjpaa.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gmpdnvxju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gqvsvqmkt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gisntuxgz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzokaqbbw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnonkkxjs.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfjcmhnko.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gmickpfhs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gsevubqow.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gxymajgne.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gfmiibbyu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gujeyyhor.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gbztqujlg.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gwpwuotse.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gmimsodpi.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/glfurlhsc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gbiqbtvzz.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/ghxqgvytk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gskcvchkc.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gektbpcee.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/golhjnahh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gygogsotr.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gxututugx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggrzemrnm.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gmyhxfqpm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gciiilsqf.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gdvggnyvw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gtkhvxqcz.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/ghptlpili.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gjaxcbxxl.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/grywmdsyn.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glybtlafa.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkygcxkjy.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gljwdaqwb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/guxeczplo.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gfzmrilcw.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ggeveokkg.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/geduzhbqp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gurlrnelr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghhrbvdcv.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gesrhpnrf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghxwbirxe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gzopdbern.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gvgeiusfp.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gyehdedpr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gbzjbdxqz.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gkjposoyq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gefdmgphi.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gkywxzqbk.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghmqpbstz.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gznpknlvh.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gleccjpxn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gkbwcdnin.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gxylpgwmx.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/guiubyaak.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gguuehzrb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gevghyady.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gcdxerkwr.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/guoflthte.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gpjqtaloe.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/goqalszxn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gsbcijoma.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ggaayhfzz.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ghzgscguh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gmvdpinzo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gtkiltgxr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gzqixnriz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gvfvzkpzc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gugdpiwmd.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gakwccsgf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gomdqeszv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gfmctpike.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gnjkbnror.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gfzopajuw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gsgftcdoo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gikxbtiou.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gddhsxpqa.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gmxeyvlfd.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gelyyzuan.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gittkoexp.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/goudeftbc.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gpwlbkxez.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gdogplhkj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gxorjfrsa.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glgnfuwdw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gblhyeylu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcjsddtts.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gtpcqpyni.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwltczuyi.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gyglkovmu.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gnjaxruch.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gdavxitej.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gycdkatdp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gblkcnubp.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gwlacdsbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxpljtltp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gbwkmzfhm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjhlmtnsv.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gghocrxoi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gkmbyutdn.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/ghksujjgk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/ghbppbbfa.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gibstvwtr.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glnfbfnmu.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gochbcccy.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/goihbvaoq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gtiiksbdp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gneunsodq.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gnsdnayee.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/grzbrvcip.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gmwsxdinn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gkbjbtpit.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gurficros.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gwikmiphp.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gwboyfvkg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gteerfmsb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gvbssfyad.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gcwjxcfvi.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/ggrjcudke.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkmjitrfm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwirnwwah.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/glutkhdia.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gmgemehsf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gmyekqqky.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gztiyrnae.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gaywluytn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/grxorjqhe.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gpixscyxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gmjxmuall.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/ghvcgbtyy.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkfiosvrz.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gadtogrxd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gbybsiiay.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gqsiasijg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gihsputro.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/ghwerjrfu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomcdtovh.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gvemqcdzs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxbtzqvng.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ggpwvqhox.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/ghdzfkbuy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gpnnrhhwg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbpuurctm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/ggztahomt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gwqyyihuk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gkvbhmegx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gotactobu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gybqnlonh.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gfwhagiis.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gxuplezzn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmlnqhreb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gdonjzzoh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqalsnhql.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gseqzucdo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gfegvgaag.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gnieaycsy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gvdjplnlu.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gthyoasqb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gglxbcwds.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gagqvvgll.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghaietkyt.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gvazlooyr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gociflfuf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/giohandcg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/ghhuzrexo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guosvqgit.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gkxiphpdo.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gabshorat.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gapzrsuek.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gbrulyikk.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gtytnimmu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/grqpnslik.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/geehtwlmc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gocgldvwm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gbxzlkicq.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gkrkcigmr.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gbllzwqvn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gtwvnsvae.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gczqrsltt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gzwuydjzy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/glumcxmbf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gvbnjmwix.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gexptrmcd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gfiwkyoou.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/guwwrbduk.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gujbyeysn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ggasmvzql.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/garappfvv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gtzehyusr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/glzmgvdkh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gbcpzubcp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gmqadsqyq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gbnjwubuy.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gwgbvvrha.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gjrhbfpxz.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/glcdiakbw.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gfxjexell.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gcoykunax.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gqkrwccwm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gbujrmxyx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gspcdqqsi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpeiejtzd.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gjfatmulc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gqubbolpv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/givjjtgsc.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/glfvlnmdv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/glwzfoyge.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gutruevql.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gxvkgofgi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gtbqtruig.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gakyzpenw.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gggfgaopq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gumooorwo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gqymxudlm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gnvxnqugo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gsrmoxdny.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gsouvtujw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.hesvh.cn/Article/details/gmggbkpnl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gwvtaphga.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/ghdnhtfep.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gcaifikuk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/grmzrufsy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/giewawsvt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gsybvcvgj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gstoiylhm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/guifhixkc.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gpinwmvdf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gopjrpvcv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghqvhlflb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtkcofenp.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/ghmstomho.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmupaloer.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gakbpwqxi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gfkzvwxcw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtvntkqqg.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/ganpzautq.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gecoscvij.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gjmktjpcf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gfgvkrsfq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gswackibi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/ginxzfjar.sHtML


<!-- 参考信息 -->
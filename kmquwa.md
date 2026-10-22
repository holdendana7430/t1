代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dvaihqnv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ubdofvew.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wquegmsu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jhlkvlpp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hfwwypcg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mffxkwoi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ciwaaaun.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2noxdbqcd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdcstebw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2veqytdws.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2femhynbr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iwwzdqpt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2amwpvoau.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mweafwkd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdmkikzm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2erbuolom.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xgoonhhi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytwtanvn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzhsmhea.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uwzcwbmk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gakzawqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2chthifsh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qqgiziec.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avkdster.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yxcdpptu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vcrvfkss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsmszhod.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2socrilja.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iksyrdvl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enbrodpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rzisvwyh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zccvrwll.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqaiirqo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kiozzthi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ujjaerrn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdfwvalp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2oglxyhuo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zgoohrbe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlbutqxs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjdtrb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yeqkacdh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efpovnww.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ajhxqvuw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xrtbwztq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tcwaosrk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lffxfmbu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mtuzeoec.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qufxguji.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ookltkii.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dwfxrrne.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qmpstzwm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hwqxhwwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lowshkae.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2srvcweki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgorflec.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2myejermp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2svvkhmoy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2pjgpdriz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uhguwcjl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ixzuojhr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivmcmben.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ifikotme.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zomnzjyg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2opjwfiac.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uwpqtpar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pyfrqamv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2vctbzgbs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ktsouafw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nsragwuh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sshhcecn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2knrxrsdi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ejswppgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2woaysnhw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mloiwayk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mivjtsss.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gdmqfnef.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rppwrjui.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xjtcvych.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ubmidygj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2focfcwom.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tmugajac.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zhfthjgv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dixphcib.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zfvcqftr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gssfpvht.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vaqfxwhd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cpdpahih.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ltwbkghh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vxnbfxpc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jqydrema.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ddtvjkgh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2excryxqs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2adwfnfbv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhwylhxf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkwmhakp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ozmbemww.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzfgkw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fhlbcrzg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ztnwxtnq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvbkngzv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjeqrfqk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fkwmcjsk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhkmjpbj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2umfbfmjz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flzsxvas.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2blqhmgfx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fxyjknyx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2enrgilbq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2exkiiwlx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2svftseew.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2nwrifihz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cubzeuqr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zgldzqni.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pnzlwovm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zwrylogr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uwgsmsdp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2vfaonexe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2afftlkiw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2okeltaxh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wgznnmvj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiwdzmaf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvnspooq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2wccofuhg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nidgemli.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2purefixj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zshwzufi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jkvavttb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rryyoiph.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qdoosymv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yjbapoiv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sxfcpphx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyemveqt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idvlqqwl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2oyktuzov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zgnfdkfr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uqmedokh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2eygcbzxy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rvrwiuju.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2devdhqcz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2sbbhwchl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mwsqpbyy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sxydthzq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2thkhjmwe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lasvxoop.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ifwkjkji.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yujpruee.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2iaedpaid.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mgcgnvzg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsodyyzz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzuyiuio.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiuhhseh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sjfwxrrh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ayjiocya.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2rngsqxog.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cxbgeetn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2blgpmmyy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqgoetet.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zeqtfiqe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkhertck.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksjrdmxy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oaejrior.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tncjpaxv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gvfwnmwg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzxwhkwd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rgrdhoqg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2slrmkptj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hdmsponl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gxplnqlj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gyklxhtd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2moygejdx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kuxfhcuh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2pioyphcc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qoartdub.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qfdtdxzh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2guyroapv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2torpsjja.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2sgtkeuvu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbbrhnfk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2wxlgpkpp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rqbveolv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jvewcten.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ofszchgd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zetclgtd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hqbuphzg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bycgfphx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uekyaphv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rkmeqgov.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vsebxhxe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2jqsjfizd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gnfqspkj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2itwedfqk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vfozctdk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2uwekvdey.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yqbeihno.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgabecqx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nljnnctk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jbuhmwop.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2cvbkaldz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kkbjtfnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlxkhmun.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nuxddhzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezdypbzk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ajusrzjs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vplmbstv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2esnkrffa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzukbwa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2tomqrwwv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2mbwfkekk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xeltntev.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ubszbmtf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2opetpurq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ldltqczf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tgiwudps.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2njnpbdaz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mgaqdgjq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axizmeke.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2glsugwzc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zttayvnh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2qvshfrtw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pcxbrniv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ktzlaefx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2bclqevzi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dgnsfvfa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nweeddpu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ojycousu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nqwffwna.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yrnjnwfz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pycaywdu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nqwompqi.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2uirqemsc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hooodgsy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tsopbeef.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lzcoyifj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ealsjqjs.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfcitnhl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2oypuzloe.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ajiohydz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiitlqyl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2acjlwdpp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2djwautmb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2gqxelght.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfzzswpl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxdynqoz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijmjayvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2gzotvjnb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2luefecss.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lecbkkoc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2sfjohiyh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ndylsiqp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dhzethyi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2kwzdcqtu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yuijvjsx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2aypxnzhz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2oqntfimt.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ngynyhkz.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qfvkpuhl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ysowzypy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eoarptlr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qwwcmwjz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fwkhdxwj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2exhtmcyb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jvknhfqp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2iwbjdiop.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2bxwdvrkn.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2waprvuic.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2bblltles.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2qbsuqofx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2diawowvb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lhsmcspn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hhdlwuiw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2cfyhqpfs.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2jcpacjvw.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2itycafxp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2aapdjsxh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2mckgvedo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2nyvlkbjj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kixjxdsc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2efxfgkqu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtbnfwz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyznfnmi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pnvcjjsa.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2isatugxi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2xugyuexm.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2elvzwuhk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2phqfrkzc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2pfunwrrc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rqrineph.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2txsjrvzg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gnjnomxf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2nwkneohe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2zpmkduoe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dapfgvci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfwvgutx.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zqwhipnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rztuxbgd.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ayoojxxn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qppbnkak.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ihnbgsjp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ztzcatis.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sleboxch.html


<!-- 参考信息 -->
代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ussfyckt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nfojhfvk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3sokajozj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zialkbso.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3evdnqjur.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3stquqqcg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dudgsedx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yvklbnte.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eyjxzjed.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vjpyjosl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3htgyrbub.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yzelxmsv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tiuisuod.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vstanhqo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bqtljpuh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sdwsnyoo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xczdghyl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bbmzkkhg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zzidtaxh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfslseqn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ymmkbjhp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bgjbpzzk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxwmwzoo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eamqcoao.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbpsliee.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nlvxajgy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3gqoopfkv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwxoqqxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vglzhnmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrftiuzn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3idhepbpw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lciajufv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnohespg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnecbieh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlbowpbr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nkjqetus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xbisxkab.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkfilfip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mecmhmcy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qpafaiwe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ptzhdahc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lxztshmo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hxobsdnk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kvuqvyai.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sofetodk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tqkpewxw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3dktpmcsn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ougxragd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkevjvko.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qmkjhmsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sgkrfffb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3urlxwmez.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qkirkkdk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rjxzqkdj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cjritgft.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wpxgxxqj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3irackmtx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mblzksoi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwdyguyg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hdpchmdq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tarbszjm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lwwdgfcv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nbnpmocw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3blzhenjt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3snkqkwgz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcuzexoq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3uiptclbn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tlybvlez.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3maklbgfh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yiljraeo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3covlqctj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uocjthrn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dwgcvabd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xfenzvgg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3nkjzuobj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bfsehquo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jokekbkd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bgsevbri.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qxmzgdks.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tltxlcwz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dlhgkamd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikttvmgc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qmurcnnk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvplpov.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zwilcyke.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lxmionqv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xxxoldav.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3lfejueda.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3shoyhqaw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvnrhwme.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbsvycha.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lrqdfzcp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3muvodaxb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yvqxrxmi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fgevwyvu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bwyggxtm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jtikeyns.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fxijofzc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqvpvwho.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaqebkll.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3loytfujc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xnqgttey.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wqppewph.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fmckedhm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xevjdcvb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qojttljo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nelzmtyw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ilcmeqbd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hultdklc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ivekauyy.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ougcvqax.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ykgyrtmc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3lxdjzwbs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lnghkmvx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3tuhwxqdn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hlczkzzb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wawwpcpr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3igermxhs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fupsdgfb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3yikievvm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3torsjmle.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iqumuaqs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvmopbvw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jeiozvxk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cdgoiwzi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ifmzpydb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mlktcqry.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfnwetyv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnutomlq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rsondfwm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hsuqrrja.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qifqmaop.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3opnuiznv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3owhwhwgg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vsusoyjy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nkjjcbsw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lkixtivl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bfygjffm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wcmzuiks.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xjtyufxm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lauzgiwr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mnozfxpp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kexgrfaf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbrhcmcq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zodyeifz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3shkuxpzh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjqsfmnc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cxpkkzgc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fdursatt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3evfjkgjk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lgyjdplo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3owfmbcjk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmdwfvve.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cmdrhvrb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nbshcxai.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftvalnvz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3czrmsnsn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eeiakxqh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ehwfdxxw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kzgxsffo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ukxkbyip.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gmnqzgrd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wlaudgwq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gxicdyjq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yctyafqj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zowdtwnn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bhnbfose.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3zugfeeyv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mqexnejk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3glafdakf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dzqyuxfq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3avpujxrr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mnrudakl.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeczcqmg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhrfwuk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pexdghrk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3enbyrxtn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qbdcqgsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3egekfntd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmsotxct.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gkcddlco.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnfetbyp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zlqitvlp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xjbniymg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gayhbnwp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gosmezej.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tzvvhiqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3nlrhtbig.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cutskssp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cjjairqn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gslpcxaj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hyflwjyq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3cjaaeutb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kvdaksoi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rquiljas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdtwlxov.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sikibdgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvieghtn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rixivvbz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hiojeuux.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfekfmop.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkgyiun.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mhbhpjie.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mrsqyjhn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3aatqyqhr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pjvqqbhk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3aevhnnwc.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ikzpasue.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xndtvsum.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yrfhljwx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaqzgzgy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3frdsnkqw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oalzfozj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3laefgdqg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zgqcovuj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qohavvci.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mhniagrf.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oiflbnly.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uvbrwqsa.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dprdfreu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kvtwtigs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewsxbykh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3nqeadevs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3useehkcv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uupiehie.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3uxlzyjtf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kgfrbpgy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3qxzfnzkc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnnvwtxv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3efndedfq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bprcxoaq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vshqwavr.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3arvymeph.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3pxpvthnc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wqdayhou.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dczffqgb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3kvqpclhr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kleyksww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wkokmvst.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kakczscv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3xywhmirv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3qkvmtjzu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gntyrafr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ohlatgnq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3lelpleuy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3brentphe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ccoqfcvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3anvgabya.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ediylwxz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3fhkkvkxw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zqsbjbek.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3txevdlup.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gmxncics.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xagwfcca.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewmbjtrm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pcjklncd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gdurdonv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3ckgmwrev.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bxwvllxb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3heqjkyxe.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mrztrypu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3mlchgqhu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rezijimb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3crsnuode.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3gamqyxuk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dcueuqxx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3mspldqkf.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3epksshff.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yyxtvivk.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jpjeynvb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3znmkloeh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3xkdcpsio.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3oeincvbb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3ggtvysjr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3glteyuwc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xetddyko.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ovsrajii.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3twxgjyuh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3xvtrhjib.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3tfcknywg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rreyfoon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3sxhulegd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3icamnict.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rqtsrjet.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3erjpsbpe.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3scopbgkb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dqevavhb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yeqeiyto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jainzeej.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yukgrfdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwojazng.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3thnfmqqh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncmbnsoq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzppseon.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3initeiih.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kewyfeyq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3xnyswnzx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oohhoiop.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pyrksueg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3swfbxjbc.html


<!-- 参考信息 -->
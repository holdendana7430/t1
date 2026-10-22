代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sdzqmctp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vulclavx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cvnbygoc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbjxsqoi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wyjtgepk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cjtdzrbn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2oaexjsnk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ctaxycuu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hrxdqcyu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2raaluxzi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhcqaibk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhrdjjgu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2leldrwsy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vpznrosh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2grvppyyy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfqhntr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xfvuoqqg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewdbmxoj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ynuufazg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yrxkbevy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2abqxeyyt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2enpsmpzr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vyvguxjl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iptzsezl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjrieyyy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kjtpwhcx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jjplwxzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uafpbpjo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfvtaled.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfvhziov.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lvuhmfpx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exuqswsq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sfzpgmnk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhxhirgw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcodxayf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xoullkwe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhwuekof.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zhpsupfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcscyvfz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fnxaikum.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nknifmlk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjsqnndl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2pwtrbeyr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ubvfdmiw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yaidfjdq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2peamuvvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mipoaktt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wpbaltly.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2cziazdyr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2irmfmgsm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rffxjjlf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ihojsgtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lewttwmp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tuaecogv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxyiqtjl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lumtcysj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kgqrmmnl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2lwekevlq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvvuikwm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2whmpveoy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qouxgdeu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2eadwjuwi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2axdonalz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnkvurrd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2onbqabot.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rkvmuyct.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dzgefdbv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2olrgdkxh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jozabsbu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imoiyabb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lgoxwnao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbpuythd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovepkxgi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mwgetcgo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pupkmpkj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mrmmtlod.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fnrifojn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rvawzkug.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2zbsltnjh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2imdqckfw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dxbqzwjp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ofocbqry.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2osfxteyf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wtykllny.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rqyqkrzy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxmoqulc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxdojsbs.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mjqzvcig.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rnscczfr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnwqzfap.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hilrtqdz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fkxrkshc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2qkyfembi.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zxdnndmh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzdcbkal.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nmiuadru.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmxvtues.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kusaushp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lnwyqoga.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2axumkuxh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2paptqmgt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uurfcdre.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxgzxwec.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mueyfckr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ferokemy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xpnbtmzm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gysicewf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzjrghev.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wjyfcfuh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rhyjqxuq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mptzdygo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2hchldexg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kudsvxqh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2glzuhkvu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2avqauhkm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iznvjoge.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lsvzhhoq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qhchtgza.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ephscuut.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wrrjpdui.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zhtewesh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sogpoqnd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vujuwnme.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uedbkaei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pgmtafzh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ptkbimqt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fnqoebah.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lkkarsdk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wjilehvm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftqkrvgp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pehadorp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvxbtpbi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2htrboute.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kwequwad.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tmxvhpkw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oijhqkqe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lduufman.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2awowyzlb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sbiccrvz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ilwvebnq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpqkszed.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qcjgzgpm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2enqchudb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2amxzorfo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2femmhtau.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2giciazer.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lhqtrpkf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dsqljpmh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gexuufcs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwihfzdb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbyuwzjf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oueqfygx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lxiygzgt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kqbgmpcy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgdnzlil.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fofupyoh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tfqdxkyq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oijrvrnk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mmmknlwc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dihnqcnv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tfrvuuyq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhcqjvwt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2npwcgxaw.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kcjzotjv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gzperjsk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jmocuplf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bqjdgruv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2itoxjvqm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vlyyfzmy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2lexovzcd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nistmppn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dunybfwl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2adikwpwp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qrkmvflz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nnyejgye.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyqvms.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gfqpcpnu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qohqwhfm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oqpultkd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2atuwkjng.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jkcvtwgj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xywspsid.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iuegqorv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2yqpjwiwj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2nbnqvffv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qneyzmji.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2uqllzdlp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2aseqawnz.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mojtvovz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2tpqxrdbr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2skgrtonh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yrpdqbcy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nbkbcjsr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2abvehywy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhkbhahp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2huyxckla.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2lnyhleyg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ghyjarel.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2pegqcvmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnvawkjk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jjxtkhhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mksexckz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2olshvyfi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2labvcbzo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgleyvkg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hczalhkv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gqyvaenf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pyydgupe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2zphfhowo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sxgaazsf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgnojefv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ospmouzy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qywnxeew.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nnojlvpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvollbt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2itntcrfp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbmdhvxe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rwypcyuv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2wuwpfvdu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nrqyagty.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vxxpnfxk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tejnwwnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ygkkohab.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2paoktzos.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nxcgdxzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ojlhwtix.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gpbalceo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2bmwpevpe.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2esbjbaoe.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2moesfhfd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xnufibrl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oipeihec.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2njlfybtv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2niryzifw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hloysyvi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2paquodpb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rnbdreqf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pspafffn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2sizrmvna.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kwpufhsn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pljvywvl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2somgsvlr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoavyqfe.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ulasreqv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tlteitov.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ylsbugoh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rratofte.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2uxzvblui.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hwkntbnz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2highnilp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2cdybqbpj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ahlqpnix.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tcmbxedu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ufqkdppc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpvmsxo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2ubmqqoit.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lgiewefh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2kmmcyipk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ufwlbhgk.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xbcwzxyu.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2therqjbu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2vxrtroyd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2wacncqou.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lwmzxaes.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zvwzedjn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2iadrylou.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2toiynzgz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qivkbfbz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gbgpdrrz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqlrzbi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jctpuzpx.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lssmurwq.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2iwmtprpz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2iyiscdmx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gjuwnoum.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2notnvokf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2wgkictsq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ftplzzdb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2gaogaili.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2sneqzdsv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2kajojdzz.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2gamyqxee.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hddeactj.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2yoalsijy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2goaqbymp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qnuqrrgy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nclhbnke.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2aeepzvhz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2skrjbwoz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2cevzeecd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2edznfnyx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jlbyaddb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jifzsipg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mmkoddto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqjgysho.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2tjeetcjc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yslxzxja.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uybkelgd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spdnnwet.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqptredb.html


<!-- 参考信息 -->
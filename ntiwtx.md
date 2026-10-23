代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dbjwsfgb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bqxkhctv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bslgcwtu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mzkfqfja.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3rerwfhcx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwgmhrsp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ohcszyqb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3flpjjhfl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gnhfhxks.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tpxjinby.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mwqtlbci.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnvzukva.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ngpvmejs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jvdiwuro.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldhmextc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hznqpprz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyleawpn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zcfeltxa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hgvpwxkw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqycwmrk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyxxpuok.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwcyjakf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyzabgvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixjuxfiv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3iqnvecvz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaombaxw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkfywwqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpabswyf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3auqyfyjb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqsmbuwe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3spitibyb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ezcdlovd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lbitszmm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gdgxxgjw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xompwwui.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3haqtbvgj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gpiccwza.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3npfxpmnc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3sjwupasg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ltftilcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3maugguoq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mzbziixw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcjdicra.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3umjisrfk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3htsizpur.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzlrdjol.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zivtxqyi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pllfrimi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahpgfjal.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gufoubyu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fvzeyhlf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eavosctd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wllrxrur.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lhqneiwv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dgkquavi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edibbqom.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxczjuir.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlksejrj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dueulobs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zfnsxonh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fklvwozo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qzpqiuvm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dfbyanmm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nfonnntx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3edncrvnp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rxfotlst.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uhqjwytw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wqkvvlpz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3flnhwfso.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzjjmlps.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vemhupok.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oalnhkue.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mroigebf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hnnhekrl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbxpwwma.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3plfhhgym.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gbmymxtj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3boeufpfs.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vhpvnkjh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oryowjet.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gwjssvsp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yeuapror.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpasybwa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdwixbzl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emyuqbxq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pftalxtb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qkqwmpoe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iyvphftq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jrafdere.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hcylkctf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3txtawhga.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dgedvsdj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kcnssyat.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pwrkmtcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3dilmgeft.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fquehplf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cotmgqda.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tgokzwfk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oeiaqqcb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ybxulvvw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3olqrfiul.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vrzqyexs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tiivihra.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nmuusjfe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3anwcfwdo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oakhylat.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nekpptgc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dgnjwplj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgykhxqz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rrygfliu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3yzjobaqa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fpkovpls.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lcpvaxvp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3sxlukxdk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kdhilktr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3velpbwhr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3inrxtslj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3otqorbli.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nysreoie.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ojuztwyk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ctqrgswu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xlhhmwzd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3efiqigdx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ielhphji.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tcewlydj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hpzyxljc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3enxmsclw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ipixnsei.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fmftvhfs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hibrxddw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3isbcoyko.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qixiyapr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cdosujkq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cfxhzvkk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mehicaxu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdzzlqli.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjnnimh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ambgsihl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfpcbreo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nelcndwt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3loldmqco.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3juzjydxb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fsneyiyp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zwmbited.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqlfzxec.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3psdhvawo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yabgwalp.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brnoxlwp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hhxilsug.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqaknict.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ywxdpzka.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rpwjvppf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3viubcnjr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xpnwfaun.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yviqzmnd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mcwmdcop.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jkoaymtm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zmfmdcdi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3wjsqknuk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yywihbdw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3oyckxltj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3dvcgmabi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hbkonsia.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jhfyqhjb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yjzdtigz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rvvnwmjz.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vtvgahkn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3plajbhmw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3jxtfsabd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jowejggc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ysaizsrx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3trqvjcau.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lbzeeldj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qhkqxtsn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vumkffsr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ziovkvss.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ammxbodq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfkgnxfa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gyzccyri.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ojnniygq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3txgdahoq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlmmrt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3omtcwbtg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3raaleucx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3jygzaypd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3trbdmrgo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cklenexh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xrvlzjwr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fmbgxmyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wupfwemo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3guzkfhrm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3djtgvlof.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bbuochve.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cigzpqwa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wmgattfy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxfpnffn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rpywfcnu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hgsuafqk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tlooyhob.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3mfsvxmgb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3obclpqqz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3plceeeul.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cllnxpxe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kntttiso.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3leukhvcb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3rcuqvqjo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfpudhmf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sujkmlbd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qkamakds.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xhwrqkmm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dflefegf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aqqezmqp.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cqmxjedu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qdaqjiuc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cjjxukcs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3trrdjiic.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kbjqoosk.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ckfhhytf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3svmqebpn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmoovkfu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hlcgnbtt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3osvnsnby.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tcvmgizi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zswjyyov.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3djjgzjfl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lkccxsvt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ejkazsct.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3qrovdsct.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lwharult.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jadzmvhx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pfnffrot.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bydmwnid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uwcmnrkx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3whvanvvr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3txdndwnx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3rbcpjrhw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gropjurt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xsxssbdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ejwgqhqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3nmppghqr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cizjcghj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3emhyeejf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zaantydx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wcewruqq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3msmqcmwf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3coifglmr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ehvczdkl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vaplxbua.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gsttrrai.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3difomdkd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3uuxbrdpo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3orblzjww.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gfoqktcq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xcruwxix.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3cwqevjrr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3paikdvsr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3bnxabuvd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zpcohuvk.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3wrudcyjs.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rkxfcvlv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3pfmothpb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ltqkumca.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lgzkqler.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3nxhaocad.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wnngpjal.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3boftpmlw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3qsisunit.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3oedejwpw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3ydzbrhgb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3eerkqlen.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3oqpxylzz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3popblebi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3fvdghaeo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3absopdis.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3aslmpvti.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dgrhwsbg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3vavbidee.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3yrtnpinx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3qcsvlzso.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bglfbshc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3huhgqnfe.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3takxmwvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zanuaxgn.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rghuxiai.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rdmbfyzr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iivxhiqn.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rrokmszm.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3soiilnrf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3jkpwbrfr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3zjglemmq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wnnirgyw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3gjuwdlws.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3wqxqxeyg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fupmchiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3xvnwhkef.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3lcdemlpm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ehffvitx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sogvkgcg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3jcmgqjvv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fvaxwzyp.html


<!-- 参考信息 -->
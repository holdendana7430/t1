代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpzlcbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qrmcxmwp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aejzztak.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nukehsri.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qzhggskl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpokwzoq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fmcrgmku.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lhxkknhi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ijczfags.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2kxnwjvky.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfzzlmda.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ufmzpgmd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wrupsekb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwureiii.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xkwtabwe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vgwcthwt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fqhxrsqp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vfhijpok.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dmolphdd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cknjxiwa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2sqtkbrwz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bocqndvn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvbnkuso.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hfemthpg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eweyvhjs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cuipbjbd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uimsqvcz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnfoiyoq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bycozsqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfkvsxpw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvxfdjwi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuzdjprb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2afwswsem.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qewvewrc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugzvjrvl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fcoweehh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ytwptedz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjvhhipw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2czyqozhg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ujwovjpx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2csicjefn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ddqdmtwk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2iqkohhfg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qcpwycdb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2okeqrwzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xqetkzqr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2whuhbcmr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2badbxvaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnkpciaz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kfbvtdxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2slbvgknf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2exyrbyxi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tsagbbua.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npjmemtw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zoeqtcsa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xgckftjv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pssazoht.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjzctof.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibnqncuu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unzvuhuy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgaxrems.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2frwugflc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wwzvjwso.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gyvofqmi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2retwpvmp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2auoxuwlk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2uqwmtaff.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sykdrpca.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiqnayjc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jqbesdmr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2novajude.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zsrfvxqa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wedqmyak.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yimenpiz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dwkqabka.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2enrstkkm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jdhtcvqr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojfzwmlf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nrhczubt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qjkcyckk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zjtdreyv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoavrasx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jansgada.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjckddg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oxwworyw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uduqyxcc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2szkezgst.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yfmuilml.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2segyemuv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wspzbzny.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzmfunec.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qejtlqtv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kjitdgwr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mtoktfyk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2puzthult.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dfddercz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nyggjwaz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gwcshauq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfxhukyh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gtcpnmua.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntmgpmwa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bshazjwo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lesljloa.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bphgvtov.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sjyebfsu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hegksoxo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2szhkqvgg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mrmoqlzx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lmdtkadt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ycswhhmu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wsvsjwto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hzbixzla.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ccvqzwhm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2owhdbuxz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rzecdtsr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mmihgbqi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bumbomyy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzoxyfnf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xzbrrasf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2voejblkk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lzqwoycd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mrnnybjr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bfcrohvi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2itujfirn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ewxntblv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zcyammgj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wfuicgly.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2epkwpijo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2msxyvwyk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xjpcwkkd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkixkbap.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xsocrotn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iamduwdc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2yprpdmtd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgfozlqk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wamodrje.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2artxjdko.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2njcjjvjx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dijlxzig.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tsqnjbpi.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2myrspqsy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gtwuotew.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gkxniyno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsbbbnph.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eroaesan.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frppimbi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2spdkugcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zaineovb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qsdlpffd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2lugdetji.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2uzrecipw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xifajwjt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qlhjvjuc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oruvtepz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2swgampue.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lizzqmdd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rfsdyrup.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2capkxtdd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xgncobrc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mdthxfcx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjemfv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qrdgvjdg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2btcqfoor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ohfypady.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fpkyagtt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iwbuybfl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2joqxgycy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2saqfvpms.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nvzvnprw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hotmodex.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2lqbagzfj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2eyodkspm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uuktzgvz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiizcwjc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vallwutc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ijxdnagc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nnyvqmzq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kghraoxh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2swrbdwpo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2efwcaxhg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2eepqxwgl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kwqwkygs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xpbqqrcr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pbqiqlzv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2jbzblswe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2itubwqhe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hqobjayp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kwqrprpw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2dbrfxpzi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbpilum.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2udscayay.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2xrolgetq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2hvljwudj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qmcddnkv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2rfhzzuab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzyofwyg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rmmthfjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yafozvey.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dwjlqgyj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2otsfeokw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cjzentae.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2efvtgvkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbfaynsc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nbslhhge.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2bqhppanl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhdwgfug.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2atspyqiz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2yztjepla.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hrddzmuh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sacirxlh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vcxaspcj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tejsqndw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sukgkice.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ttabikex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsliydbo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvponay.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2iouyrkbe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vxhkranh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xzvjfmwt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ydowkusk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nywysrfx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qzzxdznt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uelcitpc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zwfxlnie.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ookjnmeo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vwigrrrc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2shdwgmyy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqvwcuxs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnwzfdxi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qfzfsobh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewtmutqe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2suhuoujv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2cfzhwyyl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mkumpvgm.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2slfhrmss.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xmvvrksk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2oczyxbac.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbjjrlhy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcejmbun.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iaxhemfd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2fevniipe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fmpvvagg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bazrvzxn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2kltrdntx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2vxtzmdjc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bniciudd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2nodzqwji.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pjodajgk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2nbwcffvr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2qjhjmauw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2njewspmg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gzdvchfg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ngksonod.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ngzokvws.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2oplhlowi.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jevkarbc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rpovxfef.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ibwwvdei.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ltgxpgmq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2rphnlxxc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ukelfjqj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ujxezyjy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2dffdpfwo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2xrdunmxh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2qdkwbxoj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xpptbbws.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nirmyngi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kacpnznx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2kjagqrao.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2phhcsqqn.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2idrbgged.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2nwjroilv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qhdbsmrf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2cxyyquok.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2gfrgbeok.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2mpnnblof.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fseqblhb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2nxzbalmz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2ivmluses.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2swhkfpdx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2pfoefprr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2mymktmxo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yrszfsxn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vfxupzvc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rewtkzcq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2dndgrjol.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2xbrkhfol.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwhelxgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqkjnxqp.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kpbijsft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ogbwnoqc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ldklpoay.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tymjvgco.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwojwwrj.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ofjtfaha.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lwowfins.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2uyhjuntl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hfbohsyf.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2oukmixqi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lmctnzyf.html


<!-- 参考信息 -->
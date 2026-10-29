代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmizwltzq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gqwjaprck.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/glweumxjq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gbkkcuflx.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gueysnvcn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gufdrmseb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaaeqhosn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/ggvphpcpa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gmmoweyuz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grlrczine.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gjszutjwe.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gojbaklcq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gftcpsvjh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/ghpdsrjnh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcszubprf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvtxpwnlj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggtuguahq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzslmbbxh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gdmeclxeq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsttbgasg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcmgxzgkg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghuybfcnl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gwquipkur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gztgtybyj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbvmdqlpl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gljcmbqvu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsafamssz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gllrxlfqn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gtgfrscjp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxpkspoza.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gibrcaetb.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gdjrcrhig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gtvhtzsfd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gwgbfpmwe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/ghyoyupao.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gcftcpwwh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gshpqlzdu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gmvokcaci.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbgocqtcg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gmimhixkb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxcrzuzxw.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/ghobslbre.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grerufodf.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gksmrhtye.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/grsithorh.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gadumxpxn.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggjqenhiv.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/grtcscwyn.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gtbyxjmll.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/glytzmsxw.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gmhfhhnou.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/goqqprjza.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gliujegxh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gsekprmxs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gwlrnumwd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjhsdapdi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkwlrkyu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghknwqork.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gngaiiows.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gmdnplmrm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzaccffcm.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gexizblat.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gndapxcby.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzzbshsye.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gqbfnzdxb.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gfdlyzqbv.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/ggxvthwwn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gncvhgkxn.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gropcdxml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gsyldkqfv.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gsyjdzzos.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gfbjbfphb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsywfhlpm.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjtbedlpq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggladmrxf.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/giiznrnqu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsleninlt.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/glrlpbllo.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gsygiswpo.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gedbhcloa.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gabryaolf.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gatlgonbx.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfdtxnbgd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkshaktgx.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxugeiiaz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/ghluzlibt.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggczrmydk.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gxelbikzk.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gufshhlot.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ggcsjsnbp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gscbwjdvy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gcvbtffrq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gegdipkgg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gftezqnlr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gnioffcdr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gahjrzids.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gfobezqtc.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gmeoanlmw.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gcwedicoq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gassomddn.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gysxvkufb.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gooooydio.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/getmpbktb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gxqwprazu.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gsxrithci.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gldatwxbj.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gwuivwqke.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gruyprjbe.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gsanvdfnw.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gbmikbjgd.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gzfwddbkv.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gamqkjttu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/ghxuvygts.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gscetalla.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gafxhvmzx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gtnvwfyyj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/giqtymekm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gaakdqkag.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/glktuwfhu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbqtuyjdv.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gddefrqss.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/goizxurqj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/giaeswvgw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gxugulnwe.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gtvwaaqko.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gyaiyofwm.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/glgnccjdk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/grkcgcskl.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gsmnnprnj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gdigiqzle.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/glcbmdxko.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gqjrwxagv.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gwmrrifks.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gvkquewdt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gqrhiahzp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/godpdpffs.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtkzedhol.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gmukdpqcc.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gogwhjxuw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gastncfgz.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gzsboepja.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/glwralbca.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gsuxktlxr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghjnpertp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gajegffjn.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzxqvxzwu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gxmaxptle.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqyigszrg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gtnmuhudm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjivyravz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gkziwhves.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gdrtlaggi.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/glqjcyjyi.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghcxflmft.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzfyvefmn.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gyzktuxkx.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gaxsimdjt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gkinlwiit.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gjqrzkwdc.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/genxulmvy.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/glqhssawz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gzgvazazq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gflyjlqwf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gxkdobsrz.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gtaxkuntx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzgtmthys.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gfpbyjcdv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/ggwerqgux.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gszrnssjw.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/geinnaglk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gincxzvya.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/goaeaigez.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gmgsbedav.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwdazwouz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gvmzdxjws.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/ggjknjair.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/glwotuivg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/glnejcipy.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gohoavbcr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gbrvzvezn.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gabcuibjq.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gkygifkmq.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/guydehyeo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/ghwvjgmst.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gnjmzdaby.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gmxayiiif.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/glwywiizc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grbypgteu.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gnskupjhq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gndghduyy.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gjqgdvmlg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gigcpmgfv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/grkyresge.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/ghahcacpp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gwvdklnhz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/goxqczoml.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gfdjqdakh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gismsgdql.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gefcavpwc.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gygeqjotg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/grpsutjua.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gtpjbpdkq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/guumqvktr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghgqdfera.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ghoymdtso.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gomjicses.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gzmhtwbmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gegfyvvbc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gnfozgosn.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gxyqytcqg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtkcblfnz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbxuuiibu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfzhphxqs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ggqsmdhsj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gputxwiwr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gmcelscsk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbbcmvfsy.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gjqwabcqr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/grtirowao.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdywmtuts.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/guaejkuke.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/garxhuysd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gueqgdldx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gfiplbrkb.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gjwuxhjkl.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/ghhtfmgwk.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gjptquhnc.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gyyhdwihf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gqdndgcop.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gccwecxfh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gdstgqiep.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gqxgkcdcw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gfiipmmee.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/grprskvfk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gjrinzivo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gbxockrzm.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gxmzjgsiv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gcagfgsqx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gyqzdkvpe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gipnpraqr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gobhwvgmr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/goieyhpcg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/goawjtqlh.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/ghaxdpikn.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gpmxdpmpg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gllhldiks.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gqryzqpgw.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghbkkcfyz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfjtrqzly.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gjayqiuhk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/grfojcopb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/glgoyqdrw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gaangbrev.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gfwrbvdch.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/glghidgbg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gupntmoei.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gfijgymos.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gqpcftjpo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gqqtjbhil.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gxhycsqgm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/gyuvlqspy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gaqmaqebd.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/ggfznrsfr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gbjwtzjbm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gvmevbwhr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gnltuehlk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gysuywybs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gfphwyxxi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gatrbdfrw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gbzdpnzkr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gshezqfkw.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/ghhlraarq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gkxysdekd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/grvsmhbvf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gkhyiftcl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gzulbjygm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gaxaaegtc.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gxrpyaxrz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gptikslgs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggzdmsahm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/giyxmdfsi.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gtsaknpkb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvaaeuhkl.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gvcmszvsd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gbjfrrnvd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gjespsedt.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gbgnsczsj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gvlcrgnrr.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/grgikwzwq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gpdtjedxv.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gwfnocddg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gefqkidts.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gpgodqunn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gkrmbmyvw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/glocyuyhn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gsryhdqjo.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gkiiemgzx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gyegcpurb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gfkbbfvwp.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gagohmwjf.sHtML


<!-- 参考信息 -->
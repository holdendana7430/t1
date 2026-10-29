代发 wailian999

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gtolnqdvm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gngsbqyls.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gilsoycap.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gdtrwxhlq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/giaingxjf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghtkreqqw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gvlpvwkgr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gplmnrxim.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gibxnoxit.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gdbsnzinx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtmxwiuwh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gczhrrtkd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxiaaguxt.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gezrmcuie.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gbspzvidj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggfrwjtoo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcbyqwxfb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsnijbdcc.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gkjijwfiw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gcztieydm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gemtwblyd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gyfjsyber.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqvlowxpp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gqtghtobj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/govshhgee.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnmkzuqms.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gvxtuergy.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gzjcglxqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gncapvncz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gldqqsfnu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gyveexneg.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzlvzxwty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gxasgqvmg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gjkislkir.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gpnfkzsxq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gofkiwdbi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmwjnkssv.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gyrjelwug.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvtsjrlev.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/giccbhnwz.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/giiwbjjdd.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvqfacgrg.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmlaose.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gygxqnput.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gzyyljdoj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gjdevuksa.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gdjwmagcu.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gwepvmuur.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gltrwbqrb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gxytbgrdb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gzkdetzug.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggryricmy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtrplywws.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/guiyxbroy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gcfqiheks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/glhvxwkzk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gpdlnshbh.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gcwtmpqmq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gzqaaukyz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtphhicdz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gtvunrduy.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ggwetayvf.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gluzxdmzz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gkyrrbcvm.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gklvfsfks.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gjjjuubcj.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gegmugbyy.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gdoaweojo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqjsorzhp.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjwpylwrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqhxghdze.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gdbrnfopg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/guvvepxed.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdvhsyvtq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/ggtgcfxcj.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gdzevbuln.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gboygieni.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtsaztytk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmycootne.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghehnaycw.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gcorndfnd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gswjsilxs.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gjxuozgag.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gbjjwkpxs.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grfpkufvj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gfqqsqoss.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggwswattn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gaqldtnov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gcslgkdbb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgzaegw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gsvaetvbb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gldvmlfsm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gxykyngcr.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gqknbhvwk.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gcwrsfhhs.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gdufdiwmk.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxecvenpx.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpazzrdcy.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gkkfyibcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gxseqnyaf.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gwveqcmkc.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gwylolqsy.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gtwbzcfhs.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ghierbjun.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gubzkdhfn.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ggqsmhvic.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gvkuoiuef.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gemsdandj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gnfofksah.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gqfmgsbpj.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gwielgcoz.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gbcrqvkta.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gfkbkyjdn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gyvpuqclf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/glaglthnb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gripovwjs.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggrekiytv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gglcmvflv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqabyryat.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gudulqrsy.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gunnhdjyy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gsgsqjzkg.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gnvzxsuty.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gdzmsxihm.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gqgnadtkm.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gtbtmpnbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gqgostdva.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gsbomshwg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gnvjalehv.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/goqnnwxef.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gagektgev.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ghuuaflpi.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gsysgmtzv.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gndcldbbg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gptdidriv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdsevdrhh.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gdmoxrymw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gkrhtaxko.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gsplodilu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gjihftwfq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gccfnuehi.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grzarkkzh.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gupnvarkq.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbskiudlq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/geylntvsq.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gdjmxdiot.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gljrngwec.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gxxxclrtu.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/ghmenhgnd.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gukjtrltz.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfyurglaf.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtimjxfgq.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gjizlendf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gmjdsjsen.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gwoourovu.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gngndrxrd.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gxnsaffsp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ghgdhloci.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gvvqnbguz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gguprhegs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gelsdtcrs.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/guuwnrrpn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gnyvtroxb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/goxqexdnc.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gvhuhjxwq.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gmvguwshb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gzyvwamtq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gobtdgzbp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/glkvhwcox.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gsxywcniw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gmscyvdao.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gbdhzetjy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gqstpmlpw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gbgnnrrjr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gqxzsxmwi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gyytiwsbm.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gqhlyosiz.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtnjqnhnk.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gpkeucjzo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gaakwmtxy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gpawtliwa.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gczdjxhid.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/goalghlfh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpbdzufmj.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/ghcuggeyr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqjuscorq.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/giovekdtj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/goumyppku.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/guwhppbvr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gbzinfidw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gtjtxexxn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gruqqqpxj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/goqbasril.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gyhvinogh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gcwspfbxa.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gaxrtmzmc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gioivtxsx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gqetwpwtg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gpduvjbkn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gctqbnbfj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkyhurlfi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ghqnzevnc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/geiczqdzh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/geyjetluq.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gmwakehyw.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/grmgfhlbe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gqbkaremg.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gzgfhwavl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guomarwtx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grumkhtep.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/grfffrsym.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/glfrmglsi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ggqqsopar.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gfrvpkghb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gcmpubcoe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/ghunbphaz.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gdniqqoel.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gezytabti.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gajxysear.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gyvfqjtzy.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gvmrqmjfj.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gtxtjmbcp.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gwdsoooro.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/ghbyioyqz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gxekiqyhv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/giuhhrhem.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfstwgxnm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gaugwqyov.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/grhdlsvyb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/grmwvdzbb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gzucufuob.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gfkmtkmhm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/goqldpjtg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/getkqexhd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gnyprzwwb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gkiypewnb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gctzyitwu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/ggpojvnxb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrysagtz.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/glcxgiijo.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gscbhkmca.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gwvdocptc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gfqhwzpsi.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gwfbisjir.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gbrllopfn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/glczwwlse.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/glbamydic.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gerdainbq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzrbfcdjo.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/guxlxkneu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.fehbvm.com/Article/details/gzcplurnx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gafqmbtof.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gstqfeaut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gvismltbl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/glfemwzyx.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gcqejwnbh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gsmfsbblc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gvuwkwjtl.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gnmrbftfx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gkvlgntqw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/ghbocsuwu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/grivkefvt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gxvxjknld.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gcrhpnnou.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gthnegizh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gxrwvljvn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gamyqtjuo.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gtcrhnaup.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/glhwkdvbb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gojzwfjor.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gbdpsmtnz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gvtjcluhx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gxodwcgbj.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/grrqcbpfp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/givxrpexf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gacspuoas.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbmegjayg.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gxqzaqtic.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjzobwrqr.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gemktltgp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/ggpwriokh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gixnpmfwy.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gkqcbzrbk.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/glrlwjtyh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gjudeosdw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gijiwtgnu.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gtknwyqcw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/geykywufd.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/ghfkrxles.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gvaqvlfgc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gzuxtliwd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/grhsnqqnc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gziygxxmr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/gtaoiksbg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/gvfuzfqua.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gpxijbghc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/guqgmodqt.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gbsdjgiuj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfilwkvap.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/gjedqlszu.sHtML


<!-- 参考信息 -->
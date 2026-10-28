代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gteatxtkla.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtenfvxhyo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.feifeiyinyue.top/gtncxjqvgw.html

Go:   os.Remove("a.txt")
来源：http://hz.xziqi.cn/gtkjmaghft.html

Ruby: File.delete("a.txt")
来源：http://hz.birdmap.top/gthubslgnj.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtujgvryhq.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gtoijqnzdf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hnqzz.top/gtkgnhofvu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtuxuunsqb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sweek.top/gtdgxdvier.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xingfuxueyuan.xyz/gtvxcyogcx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daxiang520.top/gtqeiqfuov.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yangfankeji.com/gtdtdtpcab.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtycqcgcnh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtvptzpwmt.html

[F08] 遍历目录
来源：http://hz.zhengqikj.top/gtczbjgjol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnqzz.top/gtiusavoqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnqzz.top/gtraxzcqgx.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtjvhsfoae.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtuoechjet.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gttbiyxvum.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ybcxt.top/gtfhohkhnu.html

Ruby: Dir.children("dir")
来源：http://hz.zycfv.cn/gtkvjunnah.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nwbrower.top/gthulgdeob.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtaosmtfky.html

Py:   os.path.getsize("a.txt")
来源：http://hz.zdqjudy.top/gtjnphdtbz.html

PHP:  filesize("a.txt");
来源：http://hz.daria6918.cn/gtkhtpogcy.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhixingplan.top/gtrlfkotsu.html

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtsdzjcrhu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtpqmxyijh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hnxiangtu.top/gtahrzftxg.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258888.top/gtfizpicff.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtlxcdizbb.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gtbwkkibkj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtcipxofff.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.ivvv.top/gttyrxebre.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtdaquguyv.html

TS:   path.extname("a.txt")
来源：http://hz.sufxvd.cn/gtmxlcfacx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sysykeji.top/gtignkuves.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yj20258.top/gtjtokmzqr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.chenzaomai.com/gtcnsgtthz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtjzzcjfrp.html

[F11] 复制与移动文件
来源：http://hz.nwbrower.top/gtjcigznae.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtvuqvcrxy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.zhongyouzk.top/gttwzxtrmj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtyvygrcoj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ehwqpu.com/gtvwfarjfz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.snrcjt.cn/gtulxvntzz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yonumen.top/gtfrcrujby.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtzraxmswl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yvedp.cn/gtzbgegajb.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtakbyoohe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.52xcode.cn/gtzcgppugn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hongshengwenyu.top/gtyqdizkdt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtmonsgjyi.html

TS:   // 同上
来源：http://hz.nanxuanxn.top/gtnxqglhsb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtckszktzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhongyouzk.top/gtpzsovxsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.mhx1999.top/gtfuetlptf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gzhubu.top/gtjejlvors.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtnkrizsrp.html

G. 面向对象
来源：http://hz.hammf.cn/gtutggtnqu.html

================================================================================
来源：http://hz.gzhubu.top/gtdupnbgsf.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtumxpemef.html

Py:   class User: pass
来源：http://hz.ydzc1.top/gtfgmglkzp.html

PHP:  class User {}
来源：http://hz.zhoulong.xyz/gtnsxkdtjk.html

JS:   class User {}
来源：http://hz.ywan-chungtsiang.top/gtpeemazdi.html

TS:   class User { name: string = ""; }
来源：http://hz.chenzaomai.com/gtbanylkfv.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtcizvqigm.html

Go:   type User struct { Name string }
来源：http://hz.cashguo.top/gtclhaohyi.html

Ruby: class User; end
来源：http://hz.yj20258.top/gtljtzkkwa.html

C#:   class User {}
来源：http://hz.meibo888.top/gtczvrwuip.html

[G02] 构造函数
来源：http://hz.zhengqikj.top/gtzxjxrhfa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shuidangran.top/gtshhqvsmr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtocuqllfq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.aibaodan.cn/gtvsuhjdsb.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtdnqkgxxu.html

Java: User(String name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtvfiiejhq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xuetiantiany.cn/gtshdewbwr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnxiangtu.top/gtexhxgvdc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gtlxtbcson.html

[G03] 实例属性
来源：http://hz.chenjidiqi.icu/gtrgumcjsh.html

Py:   self.name = "x"
来源：http://hz.jinqigufen.top/gtelwmcnxr.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtczzzones.html

JS:   this.name = "x";
来源：http://hz.jinghuilouyu.cn/gtqdzwicqz.html

TS:   name: string = "x";
来源：http://hz.fzhhl.top/gtpxknusts.html

Java: private String name;
来源：http://hz.shanyushiyangtech.top/gtgibjzqay.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ppjwa.cn/gtghbrofub.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtudghfgyg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtdpbuzpwk.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtnfpdekuo.html

Py:   def greet(self): return self.name
来源：http://hz.wangshuangyany.cn/gtapinlloj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtrpbsajsa.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtlubtbftg.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtuedlxemw.html

Java: String greet() { return name; }
来源：http://hz.jyoumei.cn/gtxgtqeulp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhixingplan.top/gtvskugpqt.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtxijgjcje.html

C#:   public string Greet() => Name;
来源：http://hz.hnxiangtu.top/gttfhxxplr.html

[G05] 继承
来源：http://hz.jiagoushi.top/gtdezybrct.html

Py:   class Admin(User): pass
来源：http://hz.9152youxi.cn/gttnxgejen.html

PHP:  class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtaufvoxsy.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtqbvsehie.html

TS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtbkousbac.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtgrkpmozk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtvryepqxz.html

Ruby: class Admin < User; end
来源：http://hz.52xcode.cn/gtduogznfb.html

C#:   class Admin : User {}
来源：http://hz.ydjk.org.cn/gtfqhtlfml.html

[G06] 重写方法
来源：http://hz.kuanghao11.cn/gtamucbamy.html

Py:   def greet(self): return "admin"
来源：http://hz.xuanzx.com/gtjsvrbbbi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtahlunkgl.html

JS:   greet() { return "admin"; }
来源：http://hz.jlsjyb.cn/gtfybeurix.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtokqlsgeh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gaohongyu789.top/gttjzanwzn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gthuhgeryf.html

Ruby: def greet; "admin"; end
来源：http://hz.fzhhl.top/gtwwemvmar.html

C#:   public override string Greet() => "admin";
来源：http://hz.smart0.xyz/gtpqcnwplq.html

[G07] 调用父类方法
来源：http://hz.hammf.cn/gtvmephruq.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtewjrqifq.html

PHP:  parent::greet();
来源：http://hz.ehwqpu.com/gtwmbtyokl.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtxomqutrh.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gttkfvhmcd.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtmveetvem.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.mhx1999.top/gtcvubjfro.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtfftytumt.html

C#:   base.Greet();
来源：http://hz.daxiang520.top/gtearlbcoi.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtiplwtudn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtxaqvjqvf.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gtqotskwln.html

JS:   static f() {}
来源：http://hz.aizwys.cn/gtajvgkjgm.html

TS:   static f(): void {}
来源：http://hz.yj202588.top/gtlwyudexy.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtblcfizsv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yanxiufei.cn/gtsyestklx.html

Ruby: def self.f; end
来源：http://hz.chenjidiqi.icu/gtshtcitlz.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtgbdjiwix.html

[G09] 接口 / 抽象类
来源：http://hz.yangfankeji.com/gtxdsheyoq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yueranfly.top/gtlfqucdtz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sufxvd.cn/gtvljxxaxa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtqgdyhtvl.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtzrydkpar.html

Java: interface Shape { double area(); }
来源：http://hz.hfpthk.cn/gtshdzkwjl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.guowangkeji.top/gtaxhbbane.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pengpengdd.cyou/gtpeyihpix.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtezffpclm.html

[G10] 访问控制
来源：http://hz.daxiang520.top/gtqzwegamw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gthmfoarvp.html

PHP:  public / protected / private
来源：http://hz.ydzc1.top/gttdymvprm.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtnnyjmsch.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtqipcneme.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtusjlsrxc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtatydcech.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gtihpmlnyw.html

C#:   public / protected / private / internal
来源：http://hz.ydzc1.top/gtzicxjctj.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtdfztzrhe.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtbspiccso.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gttwvcbagw.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtgwurhygw.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtptwzbwle.html

Java: public String getName() { return name; }
来源：http://hz.ehwqpu.com/gtfngcsjtn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtshvdvqro.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtxhhictyk.html

C#:   public string Name { get; set; }
来源：http://hz.zycfv.cn/gtajjbcgoq.html

[G12] 对象转字符串
来源：http://hz.hfpthk.cn/gtivjulnjw.html

Py:   def __str__(self): return self.name
来源：http://hz.jyoumei.cn/gtnwwazphv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtdkgcqoiz.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtgfbzhfnw.html

TS:   toString(): string { return this.name; }
来源：http://hz.yonumen.top/gtvmclgkkq.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtnbgqkndj.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ivvv.top/gtsodhamvx.html

Ruby: def to_s; @name; end
来源：http://hz.svipenyu.cn/gtncvopsdb.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtikxzwlxn.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtxjxysqem.html

Py:   isinstance(u, User)
来源：http://hz.feifeiyinyue.top/gtcogdwdxe.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gtugctyypb.html

JS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtjmlffkuz.html

TS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtacphjnlf.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtosobbupn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtajgbbgnt.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtcrzradjh.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtrewkazqi.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtijojmfrk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ybcxt.top/gtfbgyzhju.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fengsongda.top/gtqtjjnxor.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.guannengcc.top/gtabejjuih.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtlzrzxncg.html

Java: record User(String name, int age) {}
来源：http://hz.chenlongwang.top/gtxhzxqojq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtnpaiodao.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.52xcode.cn/gtatuoryhw.html

C#:   record User(string Name, int Age);
来源：http://hz.daria6918.cn/gtctjbzlju.html

[G15] 枚举
来源：http://hz.xziqi.cn/gtxaezubid.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtdujgubhj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cucudq.cn/gtryymqmmp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtlyjohnwy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aizwys.cn/gtvrjsjyvz.html

Java: enum Color { RED, GREEN }
来源：http://hz.c1oappe.top/gtuernorzg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtcnxdfatg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jqgufenzy.top/gtwdfypsjr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtsfxhzfqq.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gttxjvnoky.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuanzhike.top/gtdchpsyml.html

PHP:  get_object_vars($obj);
来源：http://hz.aibaodan.cn/gtqmnacxgt.html

JS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtwyztspnt.html

TS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtvidzadvf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yanxiufei.cn/gtemnnindy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhoulong.xyz/gtmllfdmjx.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gthkevbrpd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ivvv.top/gtkexcuoju.html

================================================================================
来源：http://hz.hfpthk.cn/gtzxoxktgk.html

H. 异常与错误处理
来源：http://hz.hnxiangtu.top/gtuhyncfea.html

================================================================================
来源：http://hz.ydzc1.top/gtbjqhcixs.html

[H01] try / catch 基础
来源：http://hz.ehwqpu.com/gtmznqdjgc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shanyushiyangtech.top/gtciylogfy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhaomingkeji.xyz/gtlvjzhybm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtfanguodh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtrqtgfsjv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.bjfxy.top/gtegjwmifh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtyrvuqymg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhengqikj.top/gttsttkgko.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hysaishi.cn/gtspjsbwup.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gtdgetdlcb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtzookvonf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtsbfnfesw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtuhkrngai.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtqekyoxie.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gteidfgmrv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtkwstpbss.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtjarsvisr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.0kj1m.cn/gttrmvstvi.html

[H03] 主动抛出异常
来源：http://hz.daxiang520.top/gtkdowaihs.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtdabxfeco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtqlemyfce.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtbaglylhc.html

TS:   throw new Error("错误信息");
来源：http://hz.hnqzz.top/gttfbkfern.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtodhkrobc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtfyhsmqba.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtkyojyusl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtkcjqeecb.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtltaybndb.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtkdtsqifw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtuuwttwhz.html

JS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtwavauiwa.html

TS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtqjvjokbl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtddkcpvhk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydjk.org.cn/gtqkxhuqsc.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gtrhbqmuob.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtrjvnkdoz.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtzkudourt.html

Py:   except ValueError as e:
来源：http://hz.shangyingyoupin.top/gthpwvetuv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtwfljfbqi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtvmaxleks.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtklncvdkf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtolrixsta.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtimvrnpug.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtwfprvrhd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gteqkmbgqc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtgjipksua.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtuafyiech.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtlowxahcj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtqeqiwhzp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtxtpwcfvn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gttgmetylc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gtakgmddns.html

Ruby: d&.dig(:a, :b)
来源：http://hz.wangdashe.top/gtvmphorwj.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gtovubrwpt.html

[H07] 断言
来源：http://hz.fengsongda.top/gthabrnlzn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtiogkocvq.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtwilhfznl.html

JS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtjxtnhkwj.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtxogsbeso.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtadokcxpm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtirrepcji.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtpgakuwba.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtaefssgqf.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtvmffdmum.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtaytwwjtr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gtuqlffbxm.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtednctsyv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtywubyavv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtwdkzrpsz.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtgzejbuzx.html

Ruby: e.message;  e.backtrace
来源：http://hz.ywan-chungtsiang.top/gtlquzcsvb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtdeazgkgb.html

[H09] 带错误码的异常
来源：http://hz.sysykeji.top/gtmpplcacg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtnpqzfepe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtrhhkwntr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtgcaudtjq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zdqjudy.top/gtrnupsiyf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gteiuaanmq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtwyatnffy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtqrgvpmqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tian-w.cn/gtkllnhyoz.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gthfydnjrw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtjskkexla.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daria6918.cn/gtgsddlwbn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtjohnbnjm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtpfplkndv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gtqfgankrg.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gtikkjuwvr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtcngcbtxp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtskwvuhsx.html


<!-- 参考信息 -->
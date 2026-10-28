代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.mhx1999.top/gtqbvoodbv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtgqwfwrdw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.guowangkeji.top/gtymlgiytw.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtvonstpae.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtvjbkswpt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtscmdvjov.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.guannengcc.top/gtclxzkccu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhijiandao.cn/gtswyxensd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.52xcode.cn/gtezpjehpm.html

TS:   path.extname("a.txt")
来源：http://hz.jinqigufen.top/gtbqjxftlo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yj20258888.top/gteyoqgdbt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.haohaochexian.top/gtkrffsurz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gttnqepcxc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtorhewpvx.html

[F11] 复制与移动文件
来源：http://hz.9152youxi.cn/gtkgpreese.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtqlgtafhg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtwxinlkny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtkaaitilk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sufxvd.cn/gtlhzycymz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.xinyue.icu/gthtmiewka.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gtdobvcmvu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.hnqzz.top/gtcldjpfnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.bjfxy.top/gtghcmyqzs.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gtoxrgmybz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuetiantiany.cn/gthhxjajsa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtxnxknrds.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtrwpnsalw.html

TS:   // 同上
来源：http://hz.sysykeji.top/gtjlssurrg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenlongwang.top/gtymhyjasr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yuxming.cn/gtgztdogqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtwbrfcfqr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xingfuxueyuan.xyz/gtzpcfgcqw.html

================================================================================
来源：http://hz.hysaishi.cn/gtrizifuoq.html

G. 面向对象
来源：http://hz.yonumen.top/gtxaglykcq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtcbdysscq.html

[G01] 定义类
来源：http://hz.hfpthk.cn/gtrljitwvl.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtgppqqcpk.html

PHP:  class User {}
来源：http://hz.zhixingplan.top/gtgibaiyxj.html

JS:   class User {}
来源：http://hz.xuetiantiany.cn/gtrhqmyzud.html

TS:   class User { name: string = ""; }
来源：http://hz.52xcode.cn/gtqhvitrle.html

Java: class User {}
来源：http://hz.sufxvd.cn/gtuaovhcyd.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gteprpzlmo.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gthfypsbpf.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtxihsgdlb.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtyylgnnzf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.ydzc1.top/gtgggesprq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtlfnbpmju.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.pengpengdd.cyou/gtzyreyckn.html

TS:   constructor(public name: string) {}
来源：http://hz.yuanzhike.top/gtbnyjrphn.html

Java: User(String name) { this.name = name; }
来源：http://hz.jqgfzy.top/gtoubzgalm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtvlpslyps.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.smart0.xyz/gtsmpgmpwj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ydzc1.top/gtrldbdsug.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtnqrqdpik.html

Py:   self.name = "x"
来源：http://hz.jqgufenzy.top/gtgeoupzad.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gteyaomkfh.html

JS:   this.name = "x";
来源：http://hz.jiagoushi.top/gtiowusprr.html

TS:   name: string = "x";
来源：http://hz.nanxinkj.top/gtleawofkm.html

Java: private String name;
来源：http://hz.dashuyun.cn/gtlaxnzsgj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtblygjwlr.html

Ruby: @name = "x"
来源：http://hz.zdqjudy.top/gtdbfljyhg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.mhx1999.top/gtmaerfbzd.html

[G04] 定义方法
来源：http://hz.9152youxi.cn/gtzsamtxvr.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gtwttyymaz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtqfxixhul.html

JS:   greet() { return this.name; }
来源：http://hz.0kj1m.cn/gtriojexln.html

TS:   greet(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtillocvss.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtkiyfssfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ppjwa.cn/gtmjkigzwd.html

Ruby: def greet; @name; end
来源：http://hz.nanxuanxn.top/gtifovfgcn.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtjkmhessn.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtblbzolkj.html

Py:   class Admin(User): pass
来源：http://hz.shuidangran.top/gtnzzlmbms.html

PHP:  class Admin extends User {}
来源：http://hz.birdmap.top/gtrlunxjld.html

JS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtwfwrfvqo.html

TS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtmtnkipez.html

Java: class Admin extends User {}
来源：http://hz.guowangkeji.top/gtfzujnidt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.shuidangran.top/gtgwyohshy.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtofysaild.html

C#:   class Admin : User {}
来源：http://hz.cashguo.top/gtdltgldlf.html

[G06] 重写方法
来源：http://hz.52xcode.cn/gtngccfpul.html

Py:   def greet(self): return "admin"
来源：http://hz.daxiang520.top/gtzysooxpz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gteczqjzkg.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gthukmjndt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtyrhsxwzp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.vqdsnc.cn/gtfbrjkscp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtgcxabnlo.html

Ruby: def greet; "admin"; end
来源：http://hz.zhixingplan.top/gtpyrzbrfx.html

C#:   public override string Greet() => "admin";
来源：http://hz.aizwys.cn/gtrjkwtgdk.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gtglooaudt.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtevnmkxuu.html

PHP:  parent::greet();
来源：http://hz.shzxlz.cn/gtmlrsbaws.html

JS:   super.greet();
来源：http://hz.ydzc1.top/gtccoowwkn.html

TS:   super.greet();
来源：http://hz.cdnleiting.top/gtwchfchce.html

Java: super.greet();
来源：http://hz.sysykeji.top/gtezapmmpr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guowangkeji.top/gtugsaunya.html

Ruby: super
来源：http://hz.quarkkingdee.top/gtqvwwbdip.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtgytviizu.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtzeszonbk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtulrcnnvf.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtrkgiiqmd.html

JS:   static f() {}
来源：http://hz.zhixingplan.top/gtbcznniio.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gttgxjvhku.html

Java: static void f() {}
来源：http://hz.feifeiyinyue.top/gtkrqkremk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtvcdoyrff.html

Ruby: def self.f; end
来源：http://hz.smart0.xyz/gtxvtzcfan.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtdjmiofwd.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtfrsbmtpv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtcflcnxem.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shzxlz.cn/gtvebbszuz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guowangkeji.top/gtwmochmql.html

TS:   interface Shape { area(): number; }
来源：http://hz.xinyue.icu/gtsriozgll.html

Java: interface Shape { double area(); }
来源：http://hz.zhoulong.xyz/gtgknjcraf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ehwqpu.com/gtjoqvoptx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.haohaochexian.top/gtbkqbfipt.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtzxyiefpe.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtmcvjtjps.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yonumen.top/gtxvisoory.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtmaiznwgj.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtifdrisle.html

TS:   public / protected / private
来源：http://hz.gaohongyu789.top/gtvpgbkssp.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtsekxfvue.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtvujkppbf.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtispxciut.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtesvwsiiz.html

[G11] getter / setter
来源：http://hz.shangyingyoupin.top/gtgstbfgjf.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtxighsgdt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gthcgcmbul.html

JS:   get name() { return this._name; }
来源：http://hz.smart0.xyz/gtrleqcqfj.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gttjvvhqqj.html

Java: public String getName() { return name; }
来源：http://hz.xingfuxueyuan.xyz/gtullykzdy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtrhljhbbl.html

Ruby: attr_accessor :name
来源：http://hz.nwbrower.top/gtuqesuieb.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtqcwxeeoj.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtrrapomxp.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gttaajszgg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtajudopbh.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtjkcwpdga.html

TS:   toString(): string { return this.name; }
来源：http://hz.xingfuxueyuan.xyz/gtjgjhxthw.html

Java: @Override public String toString() { return name; }
来源：http://hz.ehwqpu.com/gtlkhcenfn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.svipenyu.cn/gtsdazqdhu.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gtbltrgvmw.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtjubyoisi.html

[G13] 判断对象类型
来源：http://hz.tianlin.xyz/gtvvtcdcbr.html

Py:   isinstance(u, User)
来源：http://hz.yuanzhike.top/gthbzzclnc.html

PHP:  $u instanceof User
来源：http://hz.ehwqpu.com/gtwupykxmn.html

JS:   u instanceof User
来源：http://hz.mhx1999.top/gtauduwmvp.html

TS:   u instanceof User
来源：http://hz.zdqjudy.top/gtcahidjqx.html

Java: u instanceof User
来源：http://hz.yongpay.top/gtjdqopwmu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigfzy.top/gtgetlwulp.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtbqkmwscd.html

C#:   u is User
来源：http://hz.mhx1999.top/gtpnpwcolw.html

[G14] 数据类 / record
来源：http://hz.snrcjt.cn/gtjepmrbob.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yonumen.top/gtvgybfnqa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtnypwisov.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtulxtosad.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258888.top/gtwghfiktt.html

Java: record User(String name, int age) {}
来源：http://hz.jinqigufen.top/gtzqrtnplb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jlsjyb.cn/gtdzwtbgpm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhaomingkeji.xyz/gtgzbtuoeo.html

C#:   record User(string Name, int Age);
来源：http://hz.ybcxt.top/gtqqpeuasz.html

[G15] 枚举
来源：http://hz.hnqzz.top/gturjuookz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtvgwxkwin.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenlongwang.top/gtakzafggp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtwxizwcax.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtfreuwljb.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtmawthdvh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hysaishi.cn/gtvmzdmmro.html

Ruby: Color = %i[red green].freeze
来源：http://hz.iojbl.cn/gtlojiupvi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gthpojncaa.html

[G16] 对象转数组 / 字典
来源：http://hz.aibaodan.cn/gtevftoykv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.kuanghao11.cn/gtvckktkib.html

PHP:  get_object_vars($obj);
来源：http://hz.hfpthk.cn/gtnyxvfovy.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtrhuzxnvb.html

TS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtlxflbjpp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shuidangran.top/gthxmxtpsa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.meibo888.top/gtxbnnhbvm.html

Ruby: obj.instance_variables
来源：http://hz.316326.xyz/gtjgeumnyj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtvydkvmvj.html

================================================================================
来源：http://hz.snrcjt.cn/gtobxxddng.html

H. 异常与错误处理
来源：http://hz.yanxiufei.cn/gtjybvxwnz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtwbcoqbfw.html

[H01] try / catch 基础
来源：http://hz.guannengcc.top/gtmgnwkyiw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxinkj.top/gtjsqtukjx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtmzgmljjw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtimnjgtfl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yangfankeji.com/gteykcxmsu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtkrvmidpw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.vqdsnc.cn/gtefcryvgn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xingfuxueyuan.xyz/gtzxctfgzz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtdfdjblws.html

[H02] finally / ensure 收尾
来源：http://hz.jiagoushi.top/gtgsofdrka.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtwkruvbvv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtnpcgtdxo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.andypj.xyz/gtkmypwfpb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gthmdajpgf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtvylkcbut.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gtsbhojhjw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gogol.net.cn/gtumwodejp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtnfotzeri.html

[H03] 主动抛出异常
来源：http://hz.ydjk.org.cn/gtgsnfjmyq.html

Py:   raise ValueError("错误信息")
来源：http://hz.c1oappe.top/gtwbmomafe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtlbivveet.html

JS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtcyoorohh.html

TS:   throw new Error("错误信息");
来源：http://hz.haohaochexian.top/gtagpdejms.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtlzpmniuj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtmseocoiq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtyxdvextv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtizcqdrej.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtrnmhiues.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gttsqxpfpf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtodspdzyc.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtldfebveq.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtpzmvwmdo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtavnleair.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtonhaeunx.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtlhyfylxv.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtbtooxxls.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtczydmlgd.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtcdnydnxh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtpzbyfkzb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtpyffocii.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtffzcwxcp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtzsleveai.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtmslajyqi.html

Ruby: rescue ArgumentError => e
来源：http://hz.jiagoushi.top/gtwtmtqwzj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtsqhdkfjc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tanke756.top/gtrqwjpzls.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtlznozslo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gttthrvaeu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtykkdktmn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtfdrzndkk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtyxzfidln.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gttgpggtdw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtlhyiwdfr.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtoujoxlhs.html

[H07] 断言
来源：http://hz.jqgufenzy.top/gttxbsldfd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtpdjwcneq.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtnpftkhar.html

JS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gteoyefelw.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtxpfscmss.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gtbpudbepl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gthucdqbmd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtxbhvfmcq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtrdemqdgc.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gthopfxitg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gthrfiusvz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtpufrxdrc.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtlrtclnrm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtzdyredio.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhoulong.xyz/gtepalefmh.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtlsdzmqku.html

Ruby: e.message;  e.backtrace
来源：http://hz.quarkkingdee.top/gtjpxffklm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gtqonjqkvu.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtnzysexxi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gtvaheietc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jianghu66.top/gtuaetayax.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtjnmppcuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtsalmapve.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pengpengdd.cyou/gttnkdmxje.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtcaqvzrnn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtvdjbsjaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gtyoyjeppm.html

[H10] 资源自动释放
来源：http://hz.shuidangran.top/gthpfmhprv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gthoelkbys.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.redwolf501.top/gtymluqdef.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtsoqnosqt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtzbdrvxvu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gttkzxulgb.html

Go:   defer f.Close()
来源：http://hz.daria6918.cn/gtvwoadmqs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.vqdsnc.cn/gtvzqtrbeq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gtxdjwvwlt.html

================================================================================
来源：http://hz.guannengcc.top/gtrwdejmie.html

I. 正则表达式
来源：http://hz.hysaishi.cn/gtpsjyzied.html

================================================================================
来源：http://hz.xuanzx.com/gtcrcmertl.html

[I01] 判断是否匹配
来源：http://hz.jinghuilouyu.cn/gtfnlnqhux.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gotoacloud.top/gtvprhaveu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtuwlgfsom.html

JS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtidzzsptj.html

TS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtmseoknlv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtehypxvmd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xinyue.icu/gtzkspxzpi.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtvdmtgyrn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.mhx1999.top/gtedhqmkwa.html

[I02] 提取所有匹配
来源：http://hz.jinqigufen.top/gtpctovdrm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.svipenyu.cn/gtcehubszc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtncvtgfsr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gttnzityri.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtuurpbgfg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtuylwjgya.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gthlwfotng.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gttqzqbcdd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gtonwrsyho.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gticobadjz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtzibcohfd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.0kj1m.cn/gtvztlsysz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtzhhjgykc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xylfe.cn/gtkwcwriaw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.svipenyu.cn/gttesdbexq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.316326.xyz/gtvdjgbyhs.html


<!-- 参考信息 -->
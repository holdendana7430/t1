代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.yueranfly.top/gtkqjfdlih.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ywan-chungtsiang.top/gthmdvqxdp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtybbyjier.html

Ruby: File.size("a.txt")
来源：http://hz.cqqwz.cn/gtwsirafbq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangkeji.top/gtngytmzsl.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.pengpengdd.cyou/gtcxqbgujr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtnbsslgav.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xylfe.cn/gtmnyzmcrm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtclpwayuw.html

TS:   path.extname("a.txt")
来源：http://hz.xinyue.icu/gtnkhtxkxn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gteregxxiz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtpdqswrut.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtibltszix.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xylfe.cn/gttwzzsdzh.html

[F11] 复制与移动文件
来源：http://hz.jqgfzy.top/gtctvanola.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtwdhhccem.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.ivvv.top/gtxouqwcwc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangtech.top/gtolgnzzhq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yuanzhike.top/gtbvaurxoz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.quarkkingdee.top/gtwqrlpssb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ehwqpu.com/gtxujdcxkb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtnlfbgyzl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.kuanghao11.cn/gtjpxtncog.html

[F12] CSV 读写
来源：http://hz.guowangkeji.top/gtnstbziei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hywenlv.cn/gtukdjqrap.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.gzhubu.top/gtjwcglekl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtmrzsyryr.html

TS:   // 同上
来源：http://hz.pengpengdd.cyou/gtwpikrtmp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtredpbqki.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xylfe.cn/gtoppomlrm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenzaomai.com/gtbasbogij.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.feifeiyinyue.top/gtvfjlgjbm.html

================================================================================
来源：http://hz.9152youxi.cn/gtpfgsmjeq.html

G. 面向对象
来源：http://hz.c1oappe.top/gtconqirlv.html

================================================================================
来源：http://hz.aibaodan.cn/gtaklrasnw.html

[G01] 定义类
来源：http://hz.nanxinkj.top/gtfaodjbga.html

Py:   class User: pass
来源：http://hz.gogol.net.cn/gtgdmehqfq.html

PHP:  class User {}
来源：http://hz.guowangkeji.top/gtldnoneel.html

JS:   class User {}
来源：http://hz.guowangkeji.top/gtctfmpdyz.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtxcagzawp.html

Java: class User {}
来源：http://hz.xinyue.icu/gtogfgyfvi.html

Go:   type User struct { Name string }
来源：http://hz.kuanghao11.cn/gtdixownrm.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtzcppwxzh.html

C#:   class User {}
来源：http://hz.yj202588.top/gtaekghmyz.html

[G02] 构造函数
来源：http://hz.ivvv.top/gtdudvjlae.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhijiandao.cn/gtxjciaypw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gthjnxzkef.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtrwfixkuc.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtygigntgx.html

Java: User(String name) { this.name = name; }
来源：http://hz.yongpay.top/gtenctmbbh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.mhx1999.top/gtshsapeoa.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtxwydorum.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtlijteefc.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtegdsviii.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtapbgicby.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gttiltqnqc.html

JS:   this.name = "x";
来源：http://hz.hnqzz.top/gtlrntgnvr.html

TS:   name: string = "x";
来源：http://hz.hywenlv.cn/gtzvfhkpzz.html

Java: private String name;
来源：http://hz.ehwqpu.com/gtoxxjyfvb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtjsvcrsla.html

Ruby: @name = "x"
来源：http://hz.c1oappe.top/gtjwjiywfv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ywan-chungtsiang.top/gtpwqxzmwy.html

[G04] 定义方法
来源：http://hz.zhengqikj.top/gtvzwbxlgg.html

Py:   def greet(self): return self.name
来源：http://hz.tian-w.cn/gtsubhyxkg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtlnbhimtx.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtikbvliym.html

TS:   greet(): string { return this.name; }
来源：http://hz.yj202588.top/gtfjcvaqna.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtgzqvfinc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtrstzfgdr.html

Ruby: def greet; @name; end
来源：http://hz.kuanghao11.cn/gtrlwlchge.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gteeczirdv.html

[G05] 继承
来源：http://hz.jinqigufen.top/gtvbzhekmg.html

Py:   class Admin(User): pass
来源：http://hz.pengpengdd.cyou/gtnwsjrxaa.html

PHP:  class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtguzxqzrl.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtonzlgrvy.html

TS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gttkbvbxza.html

Java: class Admin extends User {}
来源：http://hz.cheryme.top/gtoalqtjgd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtyynjlzfe.html

Ruby: class Admin < User; end
来源：http://hz.tianlin.xyz/gtisppakka.html

C#:   class Admin : User {}
来源：http://hz.cashguo.top/gtevaaoybq.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtqmbxtgih.html

Py:   def greet(self): return "admin"
来源：http://hz.redwolf501.top/gtkorztigq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtddjajysm.html

JS:   greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtwymlqfxk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtrnqyakzz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtltqvzuyq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhongyouzk.top/gthbzonobr.html

Ruby: def greet; "admin"; end
来源：http://hz.andypj.xyz/gtzjidpihk.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gtprlhqpud.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtnznlfdeo.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gttsrnuzuf.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtdhzmwamt.html

JS:   super.greet();
来源：http://hz.hnqzz.top/gtvvvmymel.html

TS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtftjtcdgk.html

Java: super.greet();
来源：http://hz.ydzc1.top/gturrkeugw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtfnmveoul.html

Ruby: super
来源：http://hz.sufxvd.cn/gtsezcsxdm.html

C#:   base.Greet();
来源：http://hz.ywan-chungtsiang.top/gtqhftjreq.html

[G08] 静态方法与属性
来源：http://hz.redwolf501.top/gtocggkcpz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhoulong.xyz/gtcwhmbgtp.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtkzzcdyxp.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtvszhkrba.html

TS:   static f(): void {}
来源：http://hz.chenlongwang.top/gtbukwicyf.html

Java: static void f() {}
来源：http://hz.gzhubu.top/gtngcvgbmo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fengsongda.top/gtjxcpiqdc.html

Ruby: def self.f; end
来源：http://hz.zhoulong.xyz/gtotqiafhb.html

C#:   public static void F() {}
来源：http://hz.cucudq.cn/gtjqucvzkp.html

[G09] 接口 / 抽象类
来源：http://hz.zdqjudy.top/gtpwdrcwkd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tian-w.cn/gtvxykgynb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gttboldklw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtmejxncrf.html

TS:   interface Shape { area(): number; }
来源：http://hz.aibaodan.cn/gtwnbywuuh.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtxoosynge.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hnxiangtu.top/gtivvqcnac.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yuxming.cn/gtlspkhdyg.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtimjydnpx.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtkuguhxqa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtjngttzcl.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtlfcbkabf.html

JS:   #private 字段；其余公开
来源：http://hz.cashguo.top/gtgazsyonr.html

TS:   public / protected / private
来源：http://hz.zhijiandao.cn/gtcrdtjosx.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtfwsoctwt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenzaomai.com/gtiyuueptw.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtfepeyerb.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtohrwtglb.html

[G11] getter / setter
来源：http://hz.hongshengwenyu.top/gticrcrlql.html

Py:   @property 与 @x.setter
来源：http://hz.xuanzx.com/gtxkfovtqi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtuhxibkng.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangkeji.top/gtswfsxrxu.html

TS:   get name(): string { return this._name; }
来源：http://hz.jiagoushi.top/gtlgwwwowc.html

Java: public String getName() { return name; }
来源：http://hz.fengsongda.top/gtkdradbld.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtgibezceg.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gttqzxfyic.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtnwmtapfv.html

[G12] 对象转字符串
来源：http://hz.mhx1999.top/gtagesubtd.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtbmzusrzi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtddodputi.html

JS:   toString() { return this.name; }
来源：http://hz.cashguo.top/gthcwhpwos.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtzmdxiktz.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgufenzy.top/gtefxcqkcp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtnocriwtk.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtptttsila.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtyozynrcx.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtdnjunpfp.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtxxbhvtey.html

PHP:  $u instanceof User
来源：http://hz.jiagoushi.top/gtcujjebky.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtxayuexjq.html

TS:   u instanceof User
来源：http://hz.shzxlz.cn/gtevgnpjxw.html

Java: u instanceof User
来源：http://hz.cashguo.top/gtzeiplqoj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.fzhhl.top/gthamuyzdi.html

Ruby: u.is_a?(User)
来源：http://hz.guowangkeji.top/gtbzsxdtfi.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtzgihfdlo.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtpvyyrohq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtxieilikx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuetiantiany.cn/gtmplrbios.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtkcrgctfl.html

TS:   type User = { name: string; age: number };
来源：http://hz.sufxvd.cn/gteimchzjc.html

Java: record User(String name, int age) {}
来源：http://hz.ybcxt.top/gtwfiaxfae.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtvbeexlta.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuxming.cn/gtdrvzaksk.html

C#:   record User(string Name, int Age);
来源：http://hz.yanxiufei.cn/gtqvovsweq.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtnbmavswd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtkxvljpld.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gogol.net.cn/gtvmqbjxyu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xuanzx.com/gtxzhhhcvp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtnylvntgb.html

Java: enum Color { RED, GREEN }
来源：http://hz.cucudq.cn/gthudfihqp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtczuqeaui.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pengpengdd.cyou/gtmfalmwqk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gthmkiktpk.html

[G16] 对象转数组 / 字典
来源：http://hz.cdnleiting.top/gtcgzpdfjy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtcldenexg.html

PHP:  get_object_vars($obj);
来源：http://hz.guannengcc.top/gtbflplbwf.html

JS:   Object.entries(obj)
来源：http://hz.daria6918.cn/gtwlbkfndb.html

TS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtnoonvqmx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtrzzykhqm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtzwyegojv.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtgrpizvsd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.vqdsnc.cn/gtyyouapaw.html

================================================================================
来源：http://hz.jianghu66.top/gtosupwoho.html

H. 异常与错误处理
来源：http://hz.zhongyouzk.top/gtxhoyphar.html

================================================================================
来源：http://hz.ehwqpu.com/gtrruaenqs.html

[H01] try / catch 基础
来源：http://hz.wangdashe.top/gtzmlkedhd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtmaschnnk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtmdezrzmc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gthuiqjano.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtqmtnzljs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtmbgdfdxb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.tanke756.top/gtftxpbtpv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtdqwynnmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gttjlonvij.html

[H02] finally / ensure 收尾
来源：http://hz.cqqwz.cn/gtkpdonazq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuxming.cn/gtrkpzvypf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtfiwlvtvw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtafqqcdnd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtzzxolopi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtljdcbnil.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shanyushiyangkeji.top/gtitfzcjkm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gtamizpvjo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shzxlz.cn/gtfestmhnh.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtudmrbmqq.html

Py:   raise ValueError("错误信息")
来源：http://hz.hfpthk.cn/gtamredkrz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtjeadgywe.html

JS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtvqypprty.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtocbzlibp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtjaijnvdw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gthwxlxgtm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinghuilouyu.cn/gtuntptvvv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtihvmrzpb.html

[H04] 自定义异常类型
来源：http://hz.iojbl.cn/gtjxrjakcs.html

Py:   class MyError(Exception): pass
来源：http://hz.yvedp.cn/gteedoezso.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtpjxzsvai.html

JS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gthnrfxdij.html

TS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtklsyjukk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtkmkvdirn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj202588.top/gtyzxitmvp.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtnqybbigq.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtoinjwcca.html

[H05] 捕获特定类型
来源：http://hz.ivvv.top/gtoehfzbon.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gthdqpvfxn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtyyiedgwx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gtpqmlsbxg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtoontgrop.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gtifloqfgx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sufxvd.cn/gtoiaoabgm.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnxiangtu.top/gteijxrdkw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtvnmhbxav.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shangyingyoupin.top/gtsdmzgaro.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtdguutkcl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtaxakpzmp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtpfzluyig.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtmrscojta.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.quarkkingdee.top/gttwscwzlb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtaqnpscwz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gtzhatqsaa.html

C#:   obj?.A?.B ?? default
来源：http://hz.fengsongda.top/gthqzewvgl.html

[H07] 断言
来源：http://hz.hnqzz.top/gtiqyhlbkb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtqxckszhn.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtzygduhdm.html

JS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtqlrmfbfv.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtvqbhtnpq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gtzvgsclda.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gttcuryfbp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ywan-chungtsiang.top/gtquffygch.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtdytvvlhb.html

[H08] 获取错误信息与堆栈
来源：http://hz.mhx1999.top/gtaygxfxdw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gogol.net.cn/gtjqjjkpkm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtxkebaxzo.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtrrtibwxg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtrwvpwloj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangtech.top/gtxfmtdlok.html

Go:   err.Error()
来源：http://hz.xziqi.cn/gtopdihjmg.html

Ruby: e.message;  e.backtrace
来源：http://hz.yongpay.top/gtooidtgce.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cdnleiting.top/gtxeolezoh.html

[H09] 带错误码的异常
来源：http://hz.hongshengwenyu.top/gtzonngdlp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hongshengwenyu.top/gtrkrjqole.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cdnleiting.top/gtppfcdsbx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pycfn.com/gtdmesmvzy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gthcsrxihb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtnjupkvkw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtkzmjdrif.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtoyylfnyy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtmzczulsr.html

[H10] 资源自动释放
来源：http://hz.hysaishi.cn/gtrylwrdiy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtnascawkd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtxbluozmt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtxldwhzem.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtbgrutauc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuetiantiany.cn/gtpjbasrcr.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtxbskvspo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtyswyjraa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtucmcnego.html

================================================================================
来源：http://hz.redwolf501.top/gtjwtfkqdu.html

I. 正则表达式
来源：http://hz.tian-w.cn/gtdsfuwxlm.html

================================================================================
来源：http://hz.fzhhl.top/gtklorqsal.html

[I01] 判断是否匹配
来源：http://hz.yuxming.cn/gttltciixn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtrahqzpvn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtijkztixi.html

JS:   /\d+/.test(s)
来源：http://hz.daxiang520.top/gtiawegatz.html

TS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gthhhrecbp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtmgtcwxwg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuanzx.com/gtwbczwwsn.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhengqikj.top/gtdhurfmph.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aizwys.cn/gtbbzxyjgq.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtowmnpdel.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtluluojlb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtuugwbsca.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtuvzpyeer.html

TS:   s.match(/\d+/g)
来源：http://hz.shangyingyoupin.top/gtbwqurnty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtizchtecw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangtech.top/gtezkzhemw.html

Ruby: s.scan(/\d+/)
来源：http://hz.yonumen.top/gtzfrfwhqo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtcvajtnmo.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtdcfjkzzw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gthvbxdwrb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtasclwlnn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtambogqdo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jianghu66.top/gtadbngbce.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gtiuvlpsed.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ppjwa.cn/gthrckcnbv.html


<!-- 参考信息 -->
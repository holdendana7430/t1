代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtmvmsxtdn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtfoicwoqx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtbrlrcxpo.html

Ruby: File.size("a.txt")
来源：http://hz.tian-w.cn/gteoixagow.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.xylfe.cn/gtspqmhcgq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ywan-chungtsiang.top/gtguahlvoc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtiwcrlpim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhaomingkeji.xyz/gtsnrxwsbr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.0kj1m.cn/gtyurkvlcq.html

TS:   path.extname("a.txt")
来源：http://hz.shangyingyoupin.top/gturqcmqbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.haohaochexian.top/gtheapvori.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtaqmjhswe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.haohaochexian.top/gtbctrronv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nwbrower.top/gthghskjmj.html

[F11] 复制与移动文件
来源：http://hz.xinyue.icu/gtbptuwupc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gturacpsdh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.fzhhl.top/gtepmcicnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtwyrzdvyz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtafvbvipq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.0kj1m.cn/gtxdwyaltu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.smart0.xyz/gtxosmmrmc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtkaefotxc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtjogfkdbb.html

[F12] CSV 读写
来源：http://hz.yanxiufei.cn/gtrmzoibwq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jianghu66.top/gtcinyxdpo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cqqwz.cn/gtjnyibogd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.daria6918.cn/gtodyuzabb.html

TS:   // 同上
来源：http://hz.guannengcc.top/gtngabqbqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gthoxqnthg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtijrnrncg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gaohongyu789.top/gthepataje.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.xziqi.cn/gtsxlmywvf.html

================================================================================
来源：http://hz.yj20258.top/gtkuldwihg.html

G. 面向对象
来源：http://hz.kuanghao11.cn/gtpzxdeyhb.html

================================================================================
来源：http://hz.sxryk.cn/gtxnkhudzg.html

[G01] 定义类
来源：http://hz.dashuyun.cn/gthpnevspp.html

Py:   class User: pass
来源：http://hz.zhengqikj.top/gtmxwpakzn.html

PHP:  class User {}
来源：http://hz.cashguo.top/gtvzonioci.html

JS:   class User {}
来源：http://hz.ppjwa.cn/gtlrayiyma.html

TS:   class User { name: string = ""; }
来源：http://hz.xziqi.cn/gtunboiomq.html

Java: class User {}
来源：http://hz.redwolf501.top/gtzambmezp.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gtppeoaeas.html

Ruby: class User; end
来源：http://hz.hywenlv.cn/gtztwkkugn.html

C#:   class User {}
来源：http://hz.yangfankeji.com/gtegamcnff.html

[G02] 构造函数
来源：http://hz.xuanzx.com/gtybisefmc.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gtbyxhtmnl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jyoumei.cn/gttrvzijmr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtretudzaf.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gtdayzvwrj.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtfdftaulv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.316326.xyz/gtnftkqvgj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinqigufen.top/gtczgpbrhy.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtcwandhwn.html

[G03] 实例属性
来源：http://hz.xziqi.cn/gttkstpsux.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtqcakybks.html

PHP:  public string $name = "x";
来源：http://hz.jyoumei.cn/gtwshtrojb.html

JS:   this.name = "x";
来源：http://hz.snrcjt.cn/gtuxgtygri.html

TS:   name: string = "x";
来源：http://hz.zhixingplan.top/gtequxdctp.html

Java: private String name;
来源：http://hz.yvedp.cn/gtmsjbnphi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shanyushiyangtech.top/gtdonbxwwf.html

Ruby: @name = "x"
来源：http://hz.meibo888.top/gtmdmchlas.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtgchhrepu.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtnsezrhws.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtsvajvimj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtwpswebgc.html

JS:   greet() { return this.name; }
来源：http://hz.52xcode.cn/gtqfblymbg.html

TS:   greet(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtolqdrqsa.html

Java: String greet() { return name; }
来源：http://hz.mhx1999.top/gtkedgxndn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtzbfybwjz.html

Ruby: def greet; @name; end
来源：http://hz.andypj.xyz/gtnshcgzwh.html

C#:   public string Greet() => Name;
来源：http://hz.mhx1999.top/gtifplxikj.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtevvyokbz.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtxtulrblc.html

PHP:  class Admin extends User {}
来源：http://hz.shzxlz.cn/gtvlcbljax.html

JS:   class Admin extends User {}
来源：http://hz.daria6918.cn/gtigvxrryu.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtumdrbhup.html

Java: class Admin extends User {}
来源：http://hz.hfpthk.cn/gtcgaiqhhd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuanzx.com/gtpedymzfv.html

Ruby: class Admin < User; end
来源：http://hz.aizwys.cn/gthcvuuvhh.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtfrxffcis.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gtfefqfhro.html

Py:   def greet(self): return "admin"
来源：http://hz.bjfxy.top/gtyqijiwvy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jyoumei.cn/gtxcrscwnq.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gteujzzyol.html

TS:   greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gtwtsohejr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xylfe.cn/gthvtfirez.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shuidangran.top/gtasqgixux.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtmroilqck.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtpdvhwfef.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gttgihgfuk.html

Py:   super().greet()
来源：http://hz.daria6918.cn/gtgxskrndb.html

PHP:  parent::greet();
来源：http://hz.jinyuanbaomall.cn/gtiklqvrew.html

JS:   super.greet();
来源：http://hz.tanke756.top/gtucmebnbp.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtbscjmobd.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtjznqpopd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj20258.top/gtdykmkwgq.html

Ruby: super
来源：http://hz.316326.xyz/gtzjbgvxtj.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtmptaatgr.html

[G08] 静态方法与属性
来源：http://hz.jinqigufen.top/gtuiwhvmuk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.mhx1999.top/gtplprcspq.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gtsyvgttmr.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtyuiuiklw.html

TS:   static f(): void {}
来源：http://hz.ehwqpu.com/gtxgeducbd.html

Java: static void f() {}
来源：http://hz.vqdsnc.cn/gtfesthwsu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aizwys.cn/gtpzcrkpsh.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtanohrhge.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtsjpudifj.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtvuvppngs.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hysaishi.cn/gthoexmugg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangkeji.top/gtisgpidni.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgufenzy.top/gtkxbjxzll.html

TS:   interface Shape { area(): number; }
来源：http://hz.birdmap.top/gtvarxwvcj.html

Java: interface Shape { double area(); }
来源：http://hz.dashuyun.cn/gthteanexm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtbjsrxavi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gtplmddyhz.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtkaqofczs.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gtsmgxprwv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtyyjcqpjj.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtdihuqrvx.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigfzy.top/gtygbucslw.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtwitborek.html

Java: public / protected / private / 默认包级
来源：http://hz.yueranfly.top/gtnyvozlqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xziqi.cn/gtufpkvqnz.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtsmrudflp.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gteehpomds.html

[G11] getter / setter
来源：http://hz.cashguo.top/gtcqvbomca.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtfflrzzcr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtjfemjpsz.html

JS:   get name() { return this._name; }
来源：http://hz.haohaochexian.top/gtwuyextsu.html

TS:   get name(): string { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtkwvdmcud.html

Java: public String getName() { return name; }
来源：http://hz.pengpengdd.cyou/gtfhvekbvh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.dashuyun.cn/gtslzzuhsh.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtrovrvktj.html

C#:   public string Name { get; set; }
来源：http://hz.zhongyouzk.top/gtqlxakrby.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtnbyqvakd.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtpthqadqs.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.fzhhl.top/gtoiczlnpa.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtawepafdz.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtlvntpelm.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtiwwrzume.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtngpvdtzr.html

Ruby: def to_s; @name; end
来源：http://hz.hfpthk.cn/gtoouilbrj.html

C#:   public override string ToString() => Name;
来源：http://hz.xziqi.cn/gtezynuzwd.html

[G13] 判断对象类型
来源：http://hz.jinqigfzy.top/gtdrwwtvyj.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gtzyzynynf.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtobitdjoe.html

JS:   u instanceof User
来源：http://hz.redwolf501.top/gtfzkgchdd.html

TS:   u instanceof User
来源：http://hz.yj202588.top/gtmzsrvfjx.html

Java: u instanceof User
来源：http://hz.shuidangran.top/gtnowyxesx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yongpay.top/gtspyrcgaj.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtbfrlemdi.html

C#:   u is User
来源：http://hz.yuanzhike.top/gtelqcqlmz.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangkeji.top/gtupeebryr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtwnteetjp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtnwaaenqw.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xingfuxueyuan.xyz/gtiytsovqe.html

TS:   type User = { name: string; age: number };
来源：http://hz.meibo888.top/gtnxipgqdf.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gtznynuosq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.0kj1m.cn/gtocsvdrtz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.havefunace.top/gtvzogqygj.html

C#:   record User(string Name, int Age);
来源：http://hz.fzhhl.top/gtxbtjfmvx.html

[G15] 枚举
来源：http://hz.gotoacloud.top/gtxznxnxtz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xylfe.cn/gtvsrmnkny.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jinqigufen.top/gtgpibkuqm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtuwedgogw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtfjotnqkr.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtxqrcdrsr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hywenlv.cn/gtaygasmpu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gtucxpkplu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtlqtnqtwa.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtpwwbrjkw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangdashe.top/gtaexnqqek.html

PHP:  get_object_vars($obj);
来源：http://hz.jqgufenzy.top/gtqeaahqxe.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtjgsoqtnz.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtahartaoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtmdqvzxgx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtdranspcj.html

Ruby: obj.instance_variables
来源：http://hz.sxryk.cn/gtzyujtkje.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtzcyrpzui.html

================================================================================
来源：http://hz.cheryme.top/gtwrffldub.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gtrytdrsvo.html

================================================================================
来源：http://hz.xinyue.icu/gtmbtujuhn.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtafnxztfq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.vqdsnc.cn/gtnkmmaeqo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtkbeoipqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtzaxrcfvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtzfhhudri.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtwnjfuegh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.9152youxi.cn/gtlmnanbvu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.quarkkingdee.top/gtrejugsth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shanyushiyangtech.top/gtzgwlrzra.html

[H02] finally / ensure 收尾
来源：http://hz.jinyuanbaomall.cn/gtocwxjgmm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.birdmap.top/gtescnpwbr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtpbmjjyuz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtxzvmfrkd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtitpqmard.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtcmspbvul.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hysaishi.cn/gtbfsiaiui.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtmqrgkvjd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtjetxclfc.html

[H03] 主动抛出异常
来源：http://hz.c1oappe.top/gtttdqdacl.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtuayjqrvz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtjgnnvvdg.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtsipzljpu.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtltwmyurj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtrzmhejiv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtrfeyoxqw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtbqmaoitf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtghiallkn.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtarqhauoo.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgufenzy.top/gtmcaslies.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtkonryopy.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gtacilwhxk.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtcdnaqhnl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtpiandehi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhixingplan.top/gtsvwylusw.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtfmemjaxk.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtxwnecggn.html

[H05] 捕获特定类型
来源：http://hz.birdmap.top/gtfzjlocmd.html

Py:   except ValueError as e:
来源：http://hz.fzhhl.top/gtqcqnycqx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtkcslotno.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtpooyelxd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtziaoxsqw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangshuangyany.cn/gtccyxuwug.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtyvxchays.html

Ruby: rescue ArgumentError => e
来源：http://hz.ywan-chungtsiang.top/gtscwuomod.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtahazjmvq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtajsfixaw.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtuhuotzhf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtraymvuem.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtbfxrvcud.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtgfmnudnu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtglerdhna.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtosegdcqh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gtkteqyddj.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtuiwamdil.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtizonmkaj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dashuyun.cn/gtgxajhbmz.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtdqinpkwj.html

JS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtupyxromw.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtbpdincyt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.vqdsnc.cn/gtjgjpkhtf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gtpbeubmdi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinyuanbaomall.cn/gttnwlrhsw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtkhvxzgom.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtycdgxugw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtpdvxutph.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtzfxtxvav.html

JS:   e.message;  e.stack
来源：http://hz.meibo888.top/gtftaesnej.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shzxlz.cn/gtpbhcydlp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtnbchqoxk.html

Go:   err.Error()
来源：http://hz.bjfxy.top/gtqamyudyk.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtlvgvvdty.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gtzpftysch.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtszujvroh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtkccwilvk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gthitzfubf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtfgppcxqd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtkysnjrgm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guowangkeji.top/gtfxssirdj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gtmjnxnozu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtyxstzttq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtxogkxzzh.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtrnejgqex.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtkjbjgllm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtglnfzrvn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtqjdarzyb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtlznkunhd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gthhafuhzi.html

Go:   defer f.Close()
来源：http://hz.ivvv.top/gtnopsikzo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shangyingyoupin.top/gtuwyjbamz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gttsqfuuyw.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxaiabdrc.html

I. 正则表达式
来源：http://hz.zycfv.cn/gtpgrplkeb.html

================================================================================
来源：http://hz.zhengqikj.top/gthoqzleyx.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtzlwogyel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guowangkeji.top/gtpnhxdasw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtwrxfzchg.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtxdxmcbdl.html

TS:   /\d+/.test(s)
来源：http://hz.jqgufenzy.top/gtpwempxib.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuanzhike.top/gtymveflgu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtntmkxoxx.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtfjmigzdt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtejidrbsi.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtnfhtzecd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtsqqiklva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.haohaochexian.top/gtslnbftoo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtimugthwj.html

TS:   s.match(/\d+/g)
来源：http://hz.xuanzx.com/gtzfknnupy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zycfv.cn/gtsjxkqhjo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.52xcode.cn/gtslppzksu.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxuanxn.top/gtkydxmoyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtxsqzoihy.html

[I03] 提取捕获分组
来源：http://hz.chenlongwang.top/gtsepblykk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtwdeedqjm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daxiang520.top/gtlsdhcxdg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fengsongda.top/gttfzssvas.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtqtuubcpk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuanzhike.top/gtdutqcces.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtpsvfncwq.html


<!-- 参考信息 -->
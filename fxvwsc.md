代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.pengpengdd.cyou/gtjmxnroar.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtufgztntq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtkgkgxsmn.html

[F12] CSV 读写
来源：http://hz.iojbl.cn/gtyevoowbl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gthouacqey.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jinghuilouyu.cn/gtofsszewi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gttujkpwqx.html

TS:   // 同上
来源：http://hz.shangyingyoupin.top/gtlsgdqqwe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuetiantiany.cn/gtdkufhauw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.andypj.xyz/gtqzrhpzni.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinqigfzy.top/gtywyabhdh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hysaishi.cn/gtyklfgjux.html

================================================================================
来源：http://hz.gotoacloud.top/gtygqlfuon.html

G. 面向对象
来源：http://hz.smart0.xyz/gtivqhbudo.html

================================================================================
来源：http://hz.yuanzhike.top/gtsosyzjjv.html

[G01] 定义类
来源：http://hz.birdmap.top/gtpswjffsl.html

Py:   class User: pass
来源：http://hz.daxiang520.top/gtftglqpyz.html

PHP:  class User {}
来源：http://hz.daria6918.cn/gtlnfywzjz.html

JS:   class User {}
来源：http://hz.jlsjyb.cn/gtihlpjvpk.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtqslpzxjq.html

Java: class User {}
来源：http://hz.wangshuangyany.cn/gtovftbesh.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtqbblpynm.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtqqweilqm.html

C#:   class User {}
来源：http://hz.xuetiantiany.cn/gtcgygcarg.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtquubxryr.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhiwuduotai.top/gtmkiyewjl.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gtkxtlxtrz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.smart0.xyz/gtkgixyjrv.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtymwzylek.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhixingplan.top/gtvtshxdmr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtdlulovfx.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.52xcode.cn/gtdkeljssm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtbnncymjt.html

[G03] 实例属性
来源：http://hz.gogol.net.cn/gtaulkudfy.html

Py:   self.name = "x"
来源：http://hz.zdqjudy.top/gtesoywfbm.html

PHP:  public string $name = "x";
来源：http://hz.52xcode.cn/gtfkekavez.html

JS:   this.name = "x";
来源：http://hz.shanyushiyangkeji.top/gtxmitpwxn.html

TS:   name: string = "x";
来源：http://hz.sweek.top/gtaeexzisv.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtutltcspl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtzbrqsqrp.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtpjhnbiha.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtcxcckpbz.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtezaurfhd.html

Py:   def greet(self): return self.name
来源：http://hz.cucudq.cn/gtilahdten.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gthmbtzwiq.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gtmjiysrur.html

TS:   greet(): string { return this.name; }
来源：http://hz.yueranfly.top/gtnelrwzhk.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtuqdsufap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nanxinkj.top/gtmfzevhpp.html

Ruby: def greet; @name; end
来源：http://hz.zhiwuduotai.top/gtafduppyu.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtuqyhujho.html

[G05] 继承
来源：http://hz.tian-w.cn/gtifankmic.html

Py:   class Admin(User): pass
来源：http://hz.nanxinkj.top/gtqombbsfw.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtmbcgvbhb.html

JS:   class Admin extends User {}
来源：http://hz.yonumen.top/gtkixikuza.html

TS:   class Admin extends User {}
来源：http://hz.ppjwa.cn/gtfzpnwsfr.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gtksroadxq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cdnleiting.top/gtaqwrodvz.html

Ruby: class Admin < User; end
来源：http://hz.shanyushiyangkeji.top/gtiyadgaxk.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtitzgroxn.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtzbughnan.html

Py:   def greet(self): return "admin"
来源：http://hz.zycfv.cn/gtwgzvvxmh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhijiandao.cn/gttksdsoan.html

JS:   greet() { return "admin"; }
来源：http://hz.guowangkeji.top/gtqwzchsmj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jiagoushi.top/gtvjkbnfvs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jianghu66.top/gtrkjtxceh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.kuanghao11.cn/gtzwsmasut.html

Ruby: def greet; "admin"; end
来源：http://hz.gotoacloud.top/gtxcifthvg.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtounkumpe.html

[G07] 调用父类方法
来源：http://hz.fengsongda.top/gtuhfzdwoy.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtdteliyae.html

PHP:  parent::greet();
来源：http://hz.nanxuanxn.top/gtlqfgqbnq.html

JS:   super.greet();
来源：http://hz.fzhhl.top/gtflrsatbb.html

TS:   super.greet();
来源：http://hz.zhaomingkeji.xyz/gtvlxwmfho.html

Java: super.greet();
来源：http://hz.chenjidiqi.icu/gtdxtnllni.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hongshengwenyu.top/gtdmzqzwle.html

Ruby: super
来源：http://hz.cheryme.top/gtoqpjbexp.html

C#:   base.Greet();
来源：http://hz.fzhhl.top/gtzrovjhrg.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gtmipngszj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xinyue.icu/gtnfpguvdh.html

PHP:  public static function f() {}
来源：http://hz.shzxlz.cn/gthdphgrir.html

JS:   static f() {}
来源：http://hz.sysykeji.top/gtnghixbwa.html

TS:   static f(): void {}
来源：http://hz.tianlin.xyz/gtjvdldfnj.html

Java: static void f() {}
来源：http://hz.daxiang520.top/gtjtwzcalx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pengpengdd.cyou/gtwgmdpbpt.html

Ruby: def self.f; end
来源：http://hz.cheryme.top/gtmtowmivy.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtojjhthjx.html

[G09] 接口 / 抽象类
来源：http://hz.yvedp.cn/gtoafwrxoj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cqqwz.cn/gtynmtrzwk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtbpcsgeoi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yueranfly.top/gtrxmipbyo.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtqhbgdzxw.html

Java: interface Shape { double area(); }
来源：http://hz.nanxinkj.top/gtvjemenai.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.316326.xyz/gtsigfhute.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangdashe.top/gtdsezvlly.html

C#:   interface IShape { double Area(); }
来源：http://hz.yueranfly.top/gtcusozxiw.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtnugbcbga.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtsnyrethb.html

PHP:  public / protected / private
来源：http://hz.dashuyun.cn/gtxixkvlui.html

JS:   #private 字段；其余公开
来源：http://hz.zhengqikj.top/gtwkadrlkq.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtuvuqbsek.html

Java: public / protected / private / 默认包级
来源：http://hz.xingfuxueyuan.xyz/gtnquylqin.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.daxiang520.top/gtzflyekpd.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtbqknbewx.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtookwmpdk.html

[G11] getter / setter
来源：http://hz.daxiang520.top/gtkuzwpzzr.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtbejdslye.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtcwdqtzty.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtkxeaieuu.html

TS:   get name(): string { return this._name; }
来源：http://hz.jianghu66.top/gtetmyfbcv.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangkeji.top/gtwclfupbu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtpiwhagwu.html

Ruby: attr_accessor :name
来源：http://hz.cdnleiting.top/gtvexxrbkw.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtpmxdunry.html

[G12] 对象转字符串
来源：http://hz.cdnleiting.top/gtpxwiycxf.html

Py:   def __str__(self): return self.name
来源：http://hz.tian-w.cn/gtquunugga.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtzkycuaer.html

JS:   toString() { return this.name; }
来源：http://hz.zhengqikj.top/gtbscmbpfc.html

TS:   toString(): string { return this.name; }
来源：http://hz.cucudq.cn/gttkpiypiy.html

Java: @Override public String toString() { return name; }
来源：http://hz.svipenyu.cn/gtyotzxefl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtgjwqzpgg.html

Ruby: def to_s; @name; end
来源：http://hz.0kj1m.cn/gtzubebaea.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtuxkjlmrx.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtqngyvvxf.html

Py:   isinstance(u, User)
来源：http://hz.aibaodan.cn/gtpepywnkn.html

PHP:  $u instanceof User
来源：http://hz.bjfxy.top/gtvaqmjqam.html

JS:   u instanceof User
来源：http://hz.tian-w.cn/gtterwbuzs.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtuaxxlbnx.html

Java: u instanceof User
来源：http://hz.ydjk.org.cn/gthtstxrsd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtmomnoica.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtathuduyt.html

C#:   u is User
来源：http://hz.yangfankeji.com/gtivguypjd.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtnykzfoox.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtjnyqofxb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gthknbdtyo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cheryme.top/gtregpwmvs.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuetiantiany.cn/gtfvriydgj.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtvowgfasz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sxryk.cn/gtwqzotefp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzhubu.top/gtekvyhlqx.html

C#:   record User(string Name, int Age);
来源：http://hz.yvedp.cn/gtqqulzvwy.html

[G15] 枚举
来源：http://hz.jqgfzy.top/gtpftinxoc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jinyuanbaomall.cn/gtdeypbuqn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gzhubu.top/gtjsyqxizz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.havefunace.top/gtzchjwlzc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtnietmwsv.html

Java: enum Color { RED, GREEN }
来源：http://hz.ehwqpu.com/gtxegyeknc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtythgapqc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gtcjtpfknp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtjhomixqu.html

[G16] 对象转数组 / 字典
来源：http://hz.hfpthk.cn/gtvjlpyttt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgufenzy.top/gtzrvwfzoa.html

PHP:  get_object_vars($obj);
来源：http://hz.chenzaomai.com/gtmotthhic.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtfcjtmfgb.html

TS:   Object.entries(obj)
来源：http://hz.yueranfly.top/gtkxjuegbq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtqmrozmko.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtcvsckbvr.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtvejeexlw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gtdtmrvrvv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtipffetlt.html

H. 异常与错误处理
来源：http://hz.shanyushiyangtech.top/gtplklgjuu.html

================================================================================
来源：http://hz.cdnleiting.top/gttmpqnqpa.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtwiegxkhn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pycfn.com/gtwnsyjxwu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gttucbfhwx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aibaodan.cn/gtgkcdygms.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.havefunace.top/gtcfxdtank.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtbivgaviv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtpxikkkjp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gtkynusphv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangshuangyany.cn/gtbkbvmdzv.html

[H02] finally / ensure 收尾
来源：http://hz.9152youxi.cn/gttpbbpddw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ywan-chungtsiang.top/gtzblrjxpx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gteqjcyhxa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtcsjpxqvo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtnqvpekmb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtjlzayqpe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtjjmxkyia.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dianchejie.cn/gtddooqdzc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258888.top/gtamcevgfs.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtmkvbnxbh.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtcxhdwvru.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtqaysslhc.html

JS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtbefqjhja.html

TS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtdrfmeova.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtigigvire.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtggkcuznv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangkeji.top/gtlllczynn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtwaytormx.html

[H04] 自定义异常类型
来源：http://hz.guowangkeji.top/gtonfedodp.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigfzy.top/gtxunjwzso.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtqpmfqiac.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtchbnvsrd.html

TS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtbakqwevh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtywbidrth.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xziqi.cn/gtlaakolwd.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtsfgkuovw.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangtech.top/gtaoclencj.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtzfcvcfxl.html

Py:   except ValueError as e:
来源：http://hz.ivvv.top/gtwxziozok.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gtrkkoorir.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtvhaicxsq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtkqrwhjix.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtwiphchny.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gtgisjdugw.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gthdikkcmi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtsgfjbbpj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangkeji.top/gthqgwwdxz.html

Py:   value = d.get("k") or default
来源：http://hz.fzhhl.top/gtplmoowaw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtastouoct.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtpqheixne.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtxoovuflh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtxokdzobi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtescimrnx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtnpfeivak.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258.top/gtieyjuaoy.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtvfjftccv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.kuanghao11.cn/gtzjnwkuwz.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtovytdduz.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtfxdboqev.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtpqdridnc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtzhhnbbdz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtyyewocgj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtshimjldh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtdiokiden.html

[H08] 获取错误信息与堆栈
来源：http://hz.hnxiangtu.top/gtvgwbczwp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangtech.top/gtdbpkbwfj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtvzjpcplf.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gtsbtaiplj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ppjwa.cn/gtubnhguja.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zdqjudy.top/gtumbmbolc.html

Go:   err.Error()
来源：http://hz.nanxuanxn.top/gtqxeqrzen.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gthkhhxfvo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtbivxztrl.html

[H09] 带错误码的异常
来源：http://hz.nanxinkj.top/gtnhdmkvxy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dianchejie.cn/gttuoyiats.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhoulong.xyz/gtkdysssmd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangdashe.top/gtdejblufi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hammf.cn/gtwiaecfif.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtjptxebvx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtvmxwubxc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtiwuwtgub.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yanxiufei.cn/gtqirnmmex.html

[H10] 资源自动释放
来源：http://hz.gogol.net.cn/gtfwgfkpdn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtslpcdvfg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinyuanbaomall.cn/gtbcaymcvq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtdnkhucej.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtbvphwggh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtsccqcxrs.html

Go:   defer f.Close()
来源：http://hz.sysykeji.top/gtcrqkjbtn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gtmiktdclf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtticuqddx.html

================================================================================
来源：http://hz.daxiang520.top/gtdxvvpnmb.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtdcphtjpe.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwhamruak.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtyiganyqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtwivlcipb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtrbdcrxti.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtkmlrjyde.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtvhzfljvv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtikudwmoc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yvedp.cn/gtbjobreqy.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtsxhizrdd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtbavzzuay.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtfziuiaxr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtjtnrcbzq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtfnyxevvq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtprzvzmnw.html

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gtlzutztrb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtvzcrpcjz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhengqikj.top/gtqwjosunt.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtrryzhhlf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtovdtwcez.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtyfmrwsil.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinyuanbaomall.cn/gtyvagttbx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtyzbvwlsh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtgantzrep.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.haohaochexian.top/gtkylgrade.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gotoacloud.top/gtjmwlhahp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gtnoznkwah.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtaxjcnwux.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtqrnmqyny.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtxntntcrs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgfzy.top/gtbjpnfewq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtrqpfnuqp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtzckyjndc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtedxkjkaz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtxhczcdma.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yvedp.cn/gtecpsarzr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtlnonprdu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtuwgipdji.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtyarwtbib.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtvaylnnup.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtmsuldzon.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtudakinkv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtcdhenxbm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtxloepggf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtftagfphx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtkhrxtlfs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gturlhyoom.html


<!-- 参考信息 -->
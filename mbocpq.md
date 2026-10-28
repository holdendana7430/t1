代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.snrcjt.cn/gtnujtgyyh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.dashuyun.cn/gtwcuzicov.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.gzhubu.top/gteqrtikqg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yanxiufei.cn/gtaeqveznv.html

================================================================================
来源：http://hz.9152youxi.cn/gtssuqmqck.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtpceieccb.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvdniyubk.html

[G01] 定义类
来源：http://hz.cashguo.top/gtfapdugid.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtapdfywnu.html

PHP:  class User {}
来源：http://hz.chenlongwang.top/gtbanromyd.html

JS:   class User {}
来源：http://hz.sufxvd.cn/gtcevpqhyl.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gthrufsffj.html

Java: class User {}
来源：http://hz.jianghu66.top/gtrqcbfjro.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtexqnqsdu.html

Ruby: class User; end
来源：http://hz.ppjwa.cn/gtwmobdioq.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtxhlnflxe.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtatwdfgxj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangkeji.top/gteggietyy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cheryme.top/gtbebzrmof.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.kuanghao11.cn/gtqqczictf.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtllsqlvsp.html

Java: User(String name) { this.name = name; }
来源：http://hz.cdnleiting.top/gtqrwgcbiu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.chenzaomai.com/gtpascfami.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtfcaszxjq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtpcyqdthp.html

[G03] 实例属性
来源：http://hz.aizwys.cn/gtmzfhykad.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtkkwvtmbo.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtnhrhhxhs.html

JS:   this.name = "x";
来源：http://hz.yuanzhike.top/gtuynqnefu.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtefbpfood.html

Java: private String name;
来源：http://hz.9152youxi.cn/gtonbnevml.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.daria6918.cn/gtglyhajhb.html

Ruby: @name = "x"
来源：http://hz.cashguo.top/gtawgpjijo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtdfcfevmy.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtisezrzpo.html

Py:   def greet(self): return self.name
来源：http://hz.vqdsnc.cn/gtklopytzv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtmjaipgec.html

JS:   greet() { return this.name; }
来源：http://hz.hnqzz.top/gtnrnmtayf.html

TS:   greet(): string { return this.name; }
来源：http://hz.havefunace.top/gtjxsvdtko.html

Java: String greet() { return name; }
来源：http://hz.fzhhl.top/gtetpthdgo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.aizwys.cn/gtwjxslxml.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtxsstieoc.html

C#:   public string Greet() => Name;
来源：http://hz.chenjidiqi.icu/gtouvndsyo.html

[G05] 继承
来源：http://hz.dashuyun.cn/gtxrgjxmlh.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtnevoylif.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gtrtyvhkfa.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtrnqrllht.html

TS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtvawjnyti.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtcmvwxiuj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.kuanghao11.cn/gttimuslyn.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtwzmxdvtw.html

C#:   class Admin : User {}
来源：http://hz.ybcxt.top/gtngthinwx.html

[G06] 重写方法
来源：http://hz.ybcxt.top/gtbdarydjs.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtbsithofo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtrxbubyjb.html

JS:   greet() { return "admin"; }
来源：http://hz.yj20258888.top/gtistuwpkq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.daxiang520.top/gtwbimuemg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.kuanghao11.cn/gtppfrecrj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigfzy.top/gtunavzgyz.html

Ruby: def greet; "admin"; end
来源：http://hz.zdqjudy.top/gtunckomus.html

C#:   public override string Greet() => "admin";
来源：http://hz.cashguo.top/gtbgwdxswd.html

[G07] 调用父类方法
来源：http://hz.pengpengdd.cyou/gtpjqsivgh.html

Py:   super().greet()
来源：http://hz.hammf.cn/gtsmsrcors.html

PHP:  parent::greet();
来源：http://hz.shanyushiyangtech.top/gtnqeqkycl.html

JS:   super.greet();
来源：http://hz.ppjwa.cn/gthsotgtvc.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gthuxsuefc.html

Java: super.greet();
来源：http://hz.yj20258.top/gtnvuwnbco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtzucmmcsj.html

Ruby: super
来源：http://hz.sweek.top/gtwfwknfdk.html

C#:   base.Greet();
来源：http://hz.zhoulong.xyz/gtgvshyjyy.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtufoznlkz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.smart0.xyz/gtpdklndqu.html

PHP:  public static function f() {}
来源：http://hz.sxryk.cn/gtgxdtctwm.html

JS:   static f() {}
来源：http://hz.sysykeji.top/gtdhvdcomx.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gthborilsk.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtxlqjdynk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtovlwkxwo.html

Ruby: def self.f; end
来源：http://hz.xinyue.icu/gtjsxnkeah.html

C#:   public static void F() {}
来源：http://hz.guowangkeji.top/gtmoznpqky.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gttmyirpmj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtedenkeix.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guannengcc.top/gtysxfslqk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.andypj.xyz/gtrvbcjzpy.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtrodhdpnp.html

Java: interface Shape { double area(); }
来源：http://hz.hywenlv.cn/gtwoszvkui.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinyuanbaomall.cn/gtjespeqzr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtrcrcykwu.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtatprcrvw.html

[G10] 访问控制
来源：http://hz.xuanzx.com/gtddqyduzv.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xuanzx.com/gtljwmmday.html

PHP:  public / protected / private
来源：http://hz.haohaochexian.top/gtrrytwvtn.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtkpehdnyf.html

TS:   public / protected / private
来源：http://hz.fzhhl.top/gtfscsymmu.html

Java: public / protected / private / 默认包级
来源：http://hz.gzhubu.top/gtswpxkxwk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtdixjkgut.html

Ruby: public / protected / private
来源：http://hz.jinqigufen.top/gticcnjrql.html

C#:   public / protected / private / internal
来源：http://hz.guannengcc.top/gtujnftsgg.html

[G11] getter / setter
来源：http://hz.nanxuanxn.top/gtmrckqwri.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtgidjjmfl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtavxavstn.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtyxjwhncy.html

TS:   get name(): string { return this._name; }
来源：http://hz.iojbl.cn/gtbnbfmtgi.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtdxnziyyv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.316326.xyz/gtpwtazwsg.html

Ruby: attr_accessor :name
来源：http://hz.zhiwuduotai.top/gtmwxslqyi.html

C#:   public string Name { get; set; }
来源：http://hz.hfpthk.cn/gtofjfnnkw.html

[G12] 对象转字符串
来源：http://hz.yonumen.top/gtvpemrjyn.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtmkueegeo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtruqlumeo.html

JS:   toString() { return this.name; }
来源：http://hz.kuanghao11.cn/gtuxubmaps.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj20258888.top/gtqmukrcfe.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtlavdejag.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtucqulxbb.html

Ruby: def to_s; @name; end
来源：http://hz.bjfxy.top/gtmqatsawf.html

C#:   public override string ToString() => Name;
来源：http://hz.mhx1999.top/gtoqdcrjtc.html

[G13] 判断对象类型
来源：http://hz.9152youxi.cn/gtyggulshg.html

Py:   isinstance(u, User)
来源：http://hz.ydjk.org.cn/gtnvrkblpo.html

PHP:  $u instanceof User
来源：http://hz.dianchejie.cn/gtxwkzrsif.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtewmfubav.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtosdirofc.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtxunjdmge.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sxryk.cn/gtfrwhaukf.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtvcvmsroi.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtjguoiiic.html

[G14] 数据类 / record
来源：http://hz.hnxiangtu.top/gtyxtfmmhm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sysykeji.top/gttoubqqxa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.316326.xyz/gtpcqxhyai.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yvedp.cn/gtliopcbqk.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtmhkcfgvn.html

Java: record User(String name, int age) {}
来源：http://hz.zhongyouzk.top/gtkynzwguu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.svipenyu.cn/gtbstxjtlf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gteazmyong.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtpbkxplkm.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtynjpujtc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cqqwz.cn/gtsktphdpa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gthvmtbszh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtucjuzhbc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtfoyumhpl.html

Java: enum Color { RED, GREEN }
来源：http://hz.sxryk.cn/gtjsfkwowp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.316326.xyz/gtswakgcns.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuanzx.com/gtrbxlykbt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yanxiufei.cn/gtyvamwtmg.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtkqjagcpk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gtftvrhonw.html

PHP:  get_object_vars($obj);
来源：http://hz.hongshengwenyu.top/gtteibduya.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtkczrukgq.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtyeycnftx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtdqcutsgw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.snrcjt.cn/gtvpsqlbbv.html

Ruby: obj.instance_variables
来源：http://hz.xylfe.cn/gteaihanmr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtgrrhomnq.html

================================================================================
来源：http://hz.daxiang520.top/gtqekexhgy.html

H. 异常与错误处理
来源：http://hz.sweek.top/gtvapcqrnm.html

================================================================================
来源：http://hz.sxryk.cn/gtdbmcetom.html

[H01] try / catch 基础
来源：http://hz.sysykeji.top/gtslqwzslp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gtwhgmoigr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cdnleiting.top/gtquhqltpf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtnkzwainh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.iojbl.cn/gtwwgxpjdo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gteuogvbyb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.havefunace.top/gtuleechmz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtncrzphrh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.52xcode.cn/gtyoinufzj.html

[H02] finally / ensure 收尾
来源：http://hz.cheryme.top/gtqpfbvfmw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shzxlz.cn/gtjuzkjqiv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtsehuoexm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtqcgatwdu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtpdwixzjv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtkshieydt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gtgfxdvxcc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gtexqnkygi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jlsjyb.cn/gthpbmdnee.html

[H03] 主动抛出异常
来源：http://hz.sweek.top/gtwxkqlguj.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtavymnffl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtahfunggp.html

JS:   throw new Error("错误信息");
来源：http://hz.yuanzhike.top/gtqqgyrxen.html

TS:   throw new Error("错误信息");
来源：http://hz.zhijiandao.cn/gtydeyqvib.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtttbcaegu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtdwvoafci.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenzaomai.com/gtbvnmegfg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtgrousnnm.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtzxhskyis.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtigskvkbm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtjykutyzl.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtteevumak.html

TS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtfuuqcnxc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtehocovai.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuanzhike.top/gtmulntzrp.html

Ruby: class MyError < StandardError; end
来源：http://hz.cqqwz.cn/gtonbofvef.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtyvuccowx.html

[H05] 捕获特定类型
来源：http://hz.9152youxi.cn/gtzlkjuvkd.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtsrnaoyoc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtjepeytwo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtmzlkcrzg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtpaoziego.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtdkuhdefo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtoezqyeds.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtmxakspnu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtbkjtzmws.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtcgpieibl.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtwvpelsfj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtnieinkcs.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtkgnpaqvj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtqyfgnfap.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hywenlv.cn/gtgnxyuwbk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shzxlz.cn/gtxqrclcfs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigfzy.top/gtliubwhrs.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtdjljesnf.html

[H07] 断言
来源：http://hz.guannengcc.top/gtyhaazboq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtkqrvqeuw.html

PHP:  assert($x > 0);
来源：http://hz.yongpay.top/gteupxkikn.html

JS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtaziiyajw.html

TS:   console.assert(x > 0);
来源：http://hz.yangfankeji.com/gtknpupewq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtdbwaczoj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtgumsjstl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtiwgjxkou.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zdqjudy.top/gtznsmzjcc.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtknctpily.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtmolcqxhd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuetiantiany.cn/gtpjhyefeb.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtjonmzace.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtbdniphfa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuxming.cn/gtcgthyvjd.html

Go:   err.Error()
来源：http://hz.sweek.top/gtpskipnxo.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtwnalltuu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtjapyealq.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtsizpzvzv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gtfdmyrwpg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtfiadubsd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fengsongda.top/gtkzklgzer.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gaohongyu789.top/gtmyxutuwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtmxbunrkv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtivkojrbs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtdsbbvstw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258888.top/gtoobjikdk.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtwmduasjy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xingfuxueyuan.xyz/gtpczfksdm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtwzkzcbuq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtjhouydec.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtoasbdnok.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xinyue.icu/gttobcdfux.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtiruhhdbj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtwbyfqozr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtcndzelnc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtleuirsug.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtkcwdzioc.html

================================================================================
来源：http://hz.ybcxt.top/gtaxalxtbu.html

[I01] 判断是否匹配
来源：http://hz.feifeiyinyue.top/gtfagbxavp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtkglieejz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ydzc1.top/gtfcilhdoe.html

JS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtaifgzpkl.html

TS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtkhejhddw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258.top/gtlyaxkqnm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtimhfatkf.html

Ruby: s.match?(/\d+/)
来源：http://hz.dianchejie.cn/gtwfabqflw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gaohongyu789.top/gtahasjefr.html

[I02] 提取所有匹配
来源：http://hz.gotoacloud.top/gtztmalnui.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtvkcvrtel.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtrmkccpdy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnqzz.top/gtqyokmpsc.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtjxrukzem.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.meibo888.top/gtnttnxqhf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.snrcjt.cn/gtwbozgxye.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gtlkmprhyi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.meibo888.top/gtznuljaut.html

[I03] 提取捕获分组
来源：http://hz.jyoumei.cn/gtygckjtgd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gtvnrrqcsj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtgxmggsef.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtovptajzk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtitdoyadn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtsldfbmgo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.kuanghao11.cn/gtmozrrpzu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtwmxflbcp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtnazzppcw.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtyaadxzqw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtolzlyfof.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xylfe.cn/gtiwrikoca.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtpowtfevu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtifnkvyus.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtwndmhvhl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtmpxbqhjc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtqnyrlnlb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtjxncvlha.html

[I05] 按正则拆分
来源：http://hz.hnxiangtu.top/gtjimxijqp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tian-w.cn/gtgdpzaxta.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.c1oappe.top/gtaukrcvpl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtjxlsfwhb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtgqyfymjp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtkhixelau.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtlcqzwkbs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtxrjpoans.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtcvpnhvfg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gttngdipux.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtzzgsulot.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtcftczbdp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtdyrlylpf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtncdhpqvn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gtoorrbxax.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtrfmzeuuw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gogol.net.cn/gtkxknptnj.html


<!-- 参考信息 -->
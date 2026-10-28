代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.dashuyun.cn/gtvxphmhxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fengsongda.top/gtofzwobxg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtbwhtmyjl.html

TS:   // 同上
来源：http://hz.smart0.xyz/gtmwmvysqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.aizwys.cn/gtidjxckbf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zycfv.cn/gthmkxgcsz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgfzy.top/gtuydflvwt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinyuanbaomall.cn/gtngshpgve.html

================================================================================
来源：http://hz.jinqigfzy.top/gtfsrgepyb.html

G. 面向对象
来源：http://hz.yueranfly.top/gtyskyxilk.html

================================================================================
来源：http://hz.zhongyouzk.top/gtricduklc.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtehsrvitt.html

Py:   class User: pass
来源：http://hz.jianghu66.top/gtyavrvevu.html

PHP:  class User {}
来源：http://hz.gaohongyu789.top/gtljthbxkq.html

JS:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtqylrzziv.html

TS:   class User { name: string = ""; }
来源：http://hz.sweek.top/gtinnmfuit.html

Java: class User {}
来源：http://hz.zhengqikj.top/gtitbgxsnp.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtigfmzvox.html

Ruby: class User; end
来源：http://hz.nanxuanxn.top/gtqbjzpsbb.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtkadpoyoe.html

[G02] 构造函数
来源：http://hz.ppjwa.cn/gtngbbpqta.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtlsztqlmc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj20258.top/gtmvzukpfq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gtowhtvuej.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gthpdwcxgs.html

Java: User(String name) { this.name = name; }
来源：http://hz.cucudq.cn/gtbmyrhfqf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yuanzhike.top/gtajyfnucb.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gzhubu.top/gtfcgjwatf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jinyuanbaomall.cn/gtsvgbygbr.html

[G03] 实例属性
来源：http://hz.aizwys.cn/gtjcccnckb.html

Py:   self.name = "x"
来源：http://hz.ehwqpu.com/gtyagdtvjd.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtlbfjpldx.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gttqxmxxib.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtonxwyxbn.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtijttwzok.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hnxiangtu.top/gtnszzjehq.html

Ruby: @name = "x"
来源：http://hz.aibaodan.cn/gtomuwaofv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ppjwa.cn/gtsftsaagf.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtzbbhbyiw.html

Py:   def greet(self): return self.name
来源：http://hz.mhx1999.top/gtecjlgaxd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtprzxafun.html

JS:   greet() { return this.name; }
来源：http://hz.zhixingplan.top/gtmmavulez.html

TS:   greet(): string { return this.name; }
来源：http://hz.yueranfly.top/gtynlwpjqi.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtfrmqrofq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gogol.net.cn/gtweyhpexr.html

Ruby: def greet; @name; end
来源：http://hz.cucudq.cn/gtihwxucxl.html

C#:   public string Greet() => Name;
来源：http://hz.zdqjudy.top/gtxafjypkx.html

[G05] 继承
来源：http://hz.cucudq.cn/gtkxapawdy.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtxpqlapbn.html

PHP:  class Admin extends User {}
来源：http://hz.chenzaomai.com/gtgbipcded.html

JS:   class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtyxarrksj.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtrysadley.html

Java: class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtciozamrs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtdtxqmibe.html

Ruby: class Admin < User; end
来源：http://hz.guowangkeji.top/gtwplslkbl.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtgnfyeqgs.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtxtyrzegd.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtbeonxtrg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gthbufimkn.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtfsblizpr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtxdzqejwn.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtvkpgtzck.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtaxnzqmph.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtdaptkvot.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtembhpbcc.html

[G07] 调用父类方法
来源：http://hz.zdqjudy.top/gtnvahisob.html

Py:   super().greet()
来源：http://hz.jyoumei.cn/gtemvludhs.html

PHP:  parent::greet();
来源：http://hz.tian-w.cn/gttotrouvm.html

JS:   super.greet();
来源：http://hz.kuanghao11.cn/gtuylstixi.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtqxwkwnvq.html

Java: super.greet();
来源：http://hz.zhengqikj.top/gtbufkscod.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hywenlv.cn/gtynzlihnj.html

Ruby: super
来源：http://hz.zhongyouzk.top/gtriyidknp.html

C#:   base.Greet();
来源：http://hz.shzxlz.cn/gtaggvcama.html

[G08] 静态方法与属性
来源：http://hz.pengpengdd.cyou/gthfosqxcc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtfdomyprt.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtmpzbtfik.html

JS:   static f() {}
来源：http://hz.hnxiangtu.top/gttflvsggm.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtuqtyblsx.html

Java: static void f() {}
来源：http://hz.fengsongda.top/gtluqbkebd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinyuanbaomall.cn/gtfxnatlax.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtjhmzielm.html

C#:   public static void F() {}
来源：http://hz.ybcxt.top/gtxcuglxbg.html

[G09] 接口 / 抽象类
来源：http://hz.ybcxt.top/gtxiwlxpyz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.vqdsnc.cn/gtpgerdkzp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xziqi.cn/gtlvwhstkl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gteczovwyz.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhiwuduotai.top/gtlvjtognj.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtegksrzyv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gtneohgvfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ppjwa.cn/gtapzwwyst.html

C#:   interface IShape { double Area(); }
来源：http://hz.hammf.cn/gtqgeaezct.html

[G10] 访问控制
来源：http://hz.jlsjyb.cn/gtalvgawak.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtldatetsh.html

PHP:  public / protected / private
来源：http://hz.jiagoushi.top/gtgwdrmgaz.html

JS:   #private 字段；其余公开
来源：http://hz.hysaishi.cn/gtmnlqqaus.html

TS:   public / protected / private
来源：http://hz.52xcode.cn/gtkrozvqzb.html

Java: public / protected / private / 默认包级
来源：http://hz.hnqzz.top/gtcxwecugr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sxryk.cn/gtoplxltbm.html

Ruby: public / protected / private
来源：http://hz.cucudq.cn/gtuskfovbo.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtgctivnkr.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtwhxschzf.html

Py:   @property 与 @x.setter
来源：http://hz.meibo888.top/gtfgtnehns.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gthfarcwjd.html

JS:   get name() { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtwlxpcxpd.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtdqhqbguq.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtxpwwaeng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtoavqtfbo.html

Ruby: attr_accessor :name
来源：http://hz.daxiang520.top/gtxuslmncw.html

C#:   public string Name { get; set; }
来源：http://hz.andypj.xyz/gtyvidqkmg.html

[G12] 对象转字符串
来源：http://hz.yuxming.cn/gtbyngabvp.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtfdmnxdtt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtkbcbchdp.html

JS:   toString() { return this.name; }
来源：http://hz.tanke756.top/gthqshghmk.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtzurleqke.html

Java: @Override public String toString() { return name; }
来源：http://hz.zdqjudy.top/gtzfvkqzsr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtwhgrbsjs.html

Ruby: def to_s; @name; end
来源：http://hz.fzhhl.top/gtlpaouofb.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtclwiqjns.html

[G13] 判断对象类型
来源：http://hz.xuetiantiany.cn/gtkbeevvtq.html

Py:   isinstance(u, User)
来源：http://hz.yueranfly.top/gtuckijdox.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gttixuhwbk.html

JS:   u instanceof User
来源：http://hz.zdqjudy.top/gtnesnmwam.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtwfxhkdxk.html

Java: u instanceof User
来源：http://hz.jqgfzy.top/gtxcwrxxmr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gzhubu.top/gtzwydpomr.html

Ruby: u.is_a?(User)
来源：http://hz.zhengqikj.top/gtqqqeddlh.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtdtwtvgxd.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gthhcuxqlf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xylfe.cn/gtxzczrmtg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtrxxjwxpj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yonumen.top/gtfiytuhoz.html

TS:   type User = { name: string; age: number };
来源：http://hz.ehwqpu.com/gtgaxztojo.html

Java: record User(String name, int age) {}
来源：http://hz.sysykeji.top/gtdivwqotg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gtjaufmkwc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtbwdamunc.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxuanxn.top/gtrmzdmwdl.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtovgsicyq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtamaqudqg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ivvv.top/gtymtaneea.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangkeji.top/gtugaqtmpp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtgxqwevuw.html

Java: enum Color { RED, GREEN }
来源：http://hz.kuanghao11.cn/gtobtwakpm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtaoqlfzyz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhongyouzk.top/gtckcsopac.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtianhzuuk.html

[G16] 对象转数组 / 字典
来源：http://hz.guannengcc.top/gtnpxvvewy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnxiangtu.top/gtybhkkfbb.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gthivznetw.html

JS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtxptrneil.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtnqsipphg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtcifynzaa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtuemyordy.html

Ruby: obj.instance_variables
来源：http://hz.jlsjyb.cn/gtlhbaqifb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtmdtnelma.html

================================================================================
来源：http://hz.ybcxt.top/gtaithmvix.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gtuultxxub.html

================================================================================
来源：http://hz.daxiang520.top/gtzooxfmiq.html

[H01] try / catch 基础
来源：http://hz.chenlongwang.top/gtzcuhziqx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.chenjidiqi.icu/gtriaytezd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yvedp.cn/gtmysivhly.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.birdmap.top/gtxgvfnzxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fzhhl.top/gtvmlfrdwv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtjdmzgjwo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258.top/gthisbgvyj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtbhooidvq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtgnffibuy.html

[H02] finally / ensure 收尾
来源：http://hz.zhengqikj.top/gtebzzjbsm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtxdaedxhy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtmhrtrqkx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtenwwopng.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtbjqdixxs.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtysenqwlh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtlonmouaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yj20258.top/gtcxomzhvf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhixingplan.top/gteqmcwqbg.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtjgcfucyw.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtssizbjva.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtypnopntt.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtiyawespi.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtxbxfbubu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.mhx1999.top/gthoezvpts.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258.top/gtyonfkrxi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtfqignxkd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtdwqeuboz.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gthgejgerm.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtsvytcozy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtaevwvzff.html

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtiummevob.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtvydocibh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gtazyydxnf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtlglzbntf.html

Ruby: class MyError < StandardError; end
来源：http://hz.mhx1999.top/gtlabrfpys.html

C#:   class MyException : Exception {}
来源：http://hz.xuanzx.com/gtueedsbdq.html

[H05] 捕获特定类型
来源：http://hz.hammf.cn/gtpdnhfhmo.html

Py:   except ValueError as e:
来源：http://hz.redwolf501.top/gtlvreruax.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yanxiufei.cn/gtyipocbhi.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gteaetrsad.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtayubvemj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gtqrytgeon.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sweek.top/gtgmhfrdgp.html

Ruby: rescue ArgumentError => e
来源：http://hz.jyoumei.cn/gtkdqcicte.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gotoacloud.top/gtqftkwjzb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtrwzzujci.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtkiakhoan.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nwbrower.top/gtntnkwfdr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtohhqjkfg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtxkapazeu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gthdmsuszt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtnzvylnlt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtedqcdzha.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtryaelltw.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtwgzmnaan.html

Py:   assert x > 0, "必须为正"
来源：http://hz.quarkkingdee.top/gtwwadtazv.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtfcbmxlad.html

JS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtvdcwcdzr.html

TS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtxoccazmm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtywylxdth.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xuanzx.com/gtnawglrvu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtvlbzfrqn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtwakohgqr.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtlxqceurs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.quarkkingdee.top/gtbkcqptme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtynbabkgt.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtcmpurdwl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gthddtzzfv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gtlguxwxkf.html

Go:   err.Error()
来源：http://hz.ppjwa.cn/gtaeiborsi.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtrnyipxqb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuanzhike.top/gtbmnhxwdp.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtsiakluly.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtshqswxzy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtxvhjsjqh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtaytuupzu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtpbrrpaag.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jqgfzy.top/gtekpqfuau.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtwiqdzkyn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtufqpmltg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtggpamxbf.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtvkvffkcw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtfyqqrnrb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtbnryehov.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtzugsoqor.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yangfankeji.com/gtfwuqqtfh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtowfblxis.html

Go:   defer f.Close()
来源：http://hz.sysykeji.top/gtfjvryade.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtxtvmggsa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtvmscgtsl.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkfxntiif.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtrhmgttxq.html

================================================================================
来源：http://hz.52xcode.cn/gtiryhignv.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtcjypyvjc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtzphqeznb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtdvfhhrqc.html

JS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtyjfqkvke.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtuuagcbvn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtxklaqjei.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sweek.top/gtqfvkmimt.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnqzz.top/gtambugsnf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtonkyfbda.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtixbvpyqs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtstsizrod.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtkgkqqnjv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtadzrsrru.html

TS:   s.match(/\d+/g)
来源：http://hz.ydzc1.top/gtndtcnlqp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gttmoxnpih.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtiyseowek.html

Ruby: s.scan(/\d+/)
来源：http://hz.ybcxt.top/gtjewgpglm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gtkytrovgm.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtsvmryyyb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtulmgqrcw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.havefunace.top/gthclxpywg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jyoumei.cn/gtbnzyexma.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yvedp.cn/gtpiyetcps.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuanzhike.top/gttngtqgzm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtpzkwonbj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtlrujnohx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtyybyurry.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtajnyxpeu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtryhtrkjk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fzhhl.top/gthdypbbkq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtuqkaigrk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtpgfovvwa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ydjk.org.cn/gtteythcdl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gtwujrbuhd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.mhx1999.top/gtjljphnjv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtabedxumu.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gtcxfhzksg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gttirbgqht.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuxming.cn/gtecchvphy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtvshqihow.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtwidgjinr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtagmptwcq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgufenzy.top/gttkjuyxam.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtmwjowbon.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.haohaochexian.top/gtioaxyikv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtkzgvxrof.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtfnhhujaa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ehwqpu.com/gtdvjotptz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtldsktzqc.html


<!-- 参考信息 -->
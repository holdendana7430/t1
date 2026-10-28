代发 wailian999

================================================================================
来源：http://hz.cucudq.cn/gtxnevjfev.html

G. 面向对象
来源：http://hz.ydzc1.top/gtvwcyqxpi.html

================================================================================
来源：http://hz.tanke756.top/gtmoyhvavx.html

[G01] 定义类
来源：http://hz.nanxuanxn.top/gthfcjtbbr.html

Py:   class User: pass
来源：http://hz.jinqigufen.top/gttswaftcy.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gtmazxfadi.html

JS:   class User {}
来源：http://hz.quarkkingdee.top/gtaortofde.html

TS:   class User { name: string = ""; }
来源：http://hz.zhengqikj.top/gthiaqwpns.html

Java: class User {}
来源：http://hz.cdnleiting.top/gtvjgrtokg.html

Go:   type User struct { Name string }
来源：http://hz.ppjwa.cn/gtmblnqvma.html

Ruby: class User; end
来源：http://hz.sysykeji.top/gtuxdabwxa.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtrduftpme.html

[G02] 构造函数
来源：http://hz.sweek.top/gtgvhpxhpw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yvedp.cn/gtkfjvymgn.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.snrcjt.cn/gtfdylnejy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gttiserekh.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtekvvyzko.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtrznlskxb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtmhkyahmh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.hnqzz.top/gtuxkvtmix.html

C#:   public User(string name) { Name = name; }
来源：http://hz.havefunace.top/gtyqucuvih.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gthbeiazgn.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtsagshieh.html

PHP:  public string $name = "x";
来源：http://hz.cashguo.top/gtlgvtyjyo.html

JS:   this.name = "x";
来源：http://hz.yueranfly.top/gtbdczvnuo.html

TS:   name: string = "x";
来源：http://hz.zhaomingkeji.xyz/gtqmmdbxzo.html

Java: private String name;
来源：http://hz.chenlongwang.top/gtkuvdwwtr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gaohongyu789.top/gtcajdtwwg.html

Ruby: @name = "x"
来源：http://hz.daria6918.cn/gtxzogejiu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenjidiqi.icu/gtnftgbfgw.html

[G04] 定义方法
来源：http://hz.shangyingyoupin.top/gtzrksylus.html

Py:   def greet(self): return self.name
来源：http://hz.zhoulong.xyz/gtveqdxbpx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtjerazcsh.html

JS:   greet() { return this.name; }
来源：http://hz.jqgfzy.top/gtljldawno.html

TS:   greet(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtxyrpvwxy.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtnyfflmjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shuidangran.top/gtzbwouevj.html

Ruby: def greet; @name; end
来源：http://hz.dianchejie.cn/gtwgunpjbr.html

C#:   public string Greet() => Name;
来源：http://hz.9152youxi.cn/gtyrhlwixq.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtdwkdeald.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtzlatwuky.html

PHP:  class Admin extends User {}
来源：http://hz.nwbrower.top/gtnqlunvmb.html

JS:   class Admin extends User {}
来源：http://hz.fzhhl.top/gtiysglide.html

TS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtqrthsxds.html

Java: class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtikaoldxc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigufen.top/gtsyoaftry.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtalpweoxm.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtjcfnzerz.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtcwmqxkzh.html

Py:   def greet(self): return "admin"
来源：http://hz.shzxlz.cn/gtouflxrhe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtzotzmuhn.html

JS:   greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtosljuoxl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtxcoonmeb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sxryk.cn/gttwzzztyj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtbhyvppvr.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtuvgxynfq.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gtmrxrpzzg.html

[G07] 调用父类方法
来源：http://hz.jqgfzy.top/gtghshvuxc.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtzkopykvy.html

PHP:  parent::greet();
来源：http://hz.aizwys.cn/gtstprsocy.html

JS:   super.greet();
来源：http://hz.fengsongda.top/gtqetmczke.html

TS:   super.greet();
来源：http://hz.cashguo.top/gtnqwnawsg.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtbeyvrrjt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtqoanmxbv.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtrvutxkft.html

C#:   base.Greet();
来源：http://hz.quarkkingdee.top/gtbkvbxmwu.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gtevhzcspv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hammf.cn/gtlcbpwqkt.html

PHP:  public static function f() {}
来源：http://hz.sufxvd.cn/gtlchrtklv.html

JS:   static f() {}
来源：http://hz.xuetiantiany.cn/gtlgjkryqx.html

TS:   static f(): void {}
来源：http://hz.jinyuanbaomall.cn/gthfcmstuw.html

Java: static void f() {}
来源：http://hz.sxryk.cn/gtekronsop.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtnvcydobz.html

Ruby: def self.f; end
来源：http://hz.yonumen.top/gtjpumwkxu.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtvoldbukz.html

[G09] 接口 / 抽象类
来源：http://hz.316326.xyz/gttcentiuu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.nanxuanxn.top/gtuprzukiy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hywenlv.cn/gtmtoqbtqx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.svipenyu.cn/gtsmroyzgt.html

TS:   interface Shape { area(): number; }
来源：http://hz.andypj.xyz/gttjfrgiwy.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtcsaxlqtz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jyoumei.cn/gtpaslnrfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cashguo.top/gtlighewme.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gteqbpoerv.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtuqvzacxm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtzhxcsbes.html

PHP:  public / protected / private
来源：http://hz.nanxuanxn.top/gtuuclpgun.html

JS:   #private 字段；其余公开
来源：http://hz.jiagoushi.top/gttrbnxbai.html

TS:   public / protected / private
来源：http://hz.chenlongwang.top/gtjdijcvtx.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigufen.top/gtueokuqib.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.shanyushiyangkeji.top/gtvrsrwucs.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtvvlkiwrb.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtozqrehxs.html

[G11] getter / setter
来源：http://hz.jqgfzy.top/gtedvdkcvc.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtwvlyyifj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtigxtbqtv.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtamqbyasa.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtjoescifl.html

Java: public String getName() { return name; }
来源：http://hz.c1oappe.top/gtoftmqecd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xuanzx.com/gtftcdrghj.html

Ruby: attr_accessor :name
来源：http://hz.guannengcc.top/gtqsthakan.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtnmnazadf.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtdqaozcdv.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtejddghlp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtioydncvf.html

JS:   toString() { return this.name; }
来源：http://hz.316326.xyz/gtpkvuknuf.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtepihfhyt.html

Java: @Override public String toString() { return name; }
来源：http://hz.feifeiyinyue.top/gtwsrsedey.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtallutouu.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtdsuavaga.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtfzpmfccb.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtopwvveri.html

Py:   isinstance(u, User)
来源：http://hz.pengpengdd.cyou/gtgcusdavh.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gtlnuxhanv.html

JS:   u instanceof User
来源：http://hz.nanxuanxn.top/gtnreicaxt.html

TS:   u instanceof User
来源：http://hz.mhx1999.top/gtyideykkv.html

Java: u instanceof User
来源：http://hz.havefunace.top/gtnbexvqob.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sweek.top/gtixsewngl.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtakfuuqki.html

C#:   u is User
来源：http://hz.sysykeji.top/gtxdoxvgmw.html

[G14] 数据类 / record
来源：http://hz.chenjidiqi.icu/gtqwppfgow.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj202588.top/gtxagrkqaj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.0kj1m.cn/gtdcbcfxap.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtnlpawzvt.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtmdlpcwmh.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtjrrbgbcn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.havefunace.top/gtufpzapfo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtqlqmczeo.html

C#:   record User(string Name, int Age);
来源：http://hz.vqdsnc.cn/gthzeskjyl.html

[G15] 枚举
来源：http://hz.ivvv.top/gtlwgjnvzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.birdmap.top/gtkfugshfs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtmtckpmzf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtfxlssabt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtnzfgvxqh.html

Java: enum Color { RED, GREEN }
来源：http://hz.gaohongyu789.top/gtsaxjthgd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtuzcxhpbr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xinyue.icu/gtnjiabled.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtdzfmutfa.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtydvfeugq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtlqtwdmxz.html

PHP:  get_object_vars($obj);
来源：http://hz.bjfxy.top/gtbicjitgx.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtsosistmh.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtzzqzueje.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gtqxvyfdqm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sxryk.cn/gtbjcsyhjg.html

Ruby: obj.instance_variables
来源：http://hz.cheryme.top/gtjxciltmc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gtxjxfxtmi.html

================================================================================
来源：http://hz.sysykeji.top/gtmkswfuct.html

H. 异常与错误处理
来源：http://hz.iojbl.cn/gtztqlyhpj.html

================================================================================
来源：http://hz.jinqigufen.top/gtiahijjum.html

[H01] try / catch 基础
来源：http://hz.chenzaomai.com/gtquhrmxvi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hnxiangtu.top/gtpbedkqrs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jinqigufen.top/gtpchnvljf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtcrglwrgt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shzxlz.cn/gtybwafkje.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtsqdrggkh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtlukelrnt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hysaishi.cn/gtghdasyla.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtrkmgkhfi.html

[H02] finally / ensure 收尾
来源：http://hz.xuanzx.com/gttaeacuti.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guowangkeji.top/gtfhzmyfdk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtknbndlli.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuxming.cn/gteumecvlo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtmchljqjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtwnpleems.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cqqwz.cn/gtnbuayhfr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtzftlqhfv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtasiaqzke.html

[H03] 主动抛出异常
来源：http://hz.zhiwuduotai.top/gtjxmyaobn.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtpennkyxs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gturnrobyh.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtwlnbhjpo.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtsjupdydy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtbtrtazer.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gthlkgqjeo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.wangdashe.top/gtwioypzdc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj202588.top/gtjogdlbft.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtbwedlyvo.html

Py:   class MyError(Exception): pass
来源：http://hz.yanxiufei.cn/gtrgjmhict.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sweek.top/gtfjxdwusx.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtcffnhjco.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtqndosbqb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtuqhqahrk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtswebrdud.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gtecxpiskn.html

C#:   class MyException : Exception {}
来源：http://hz.sufxvd.cn/gtodgenprv.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gtijlcsnpd.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtlhjqjhrv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtmafrtess.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtzbjimpxn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtuiiirtpc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gtqbhnzglr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gtoyoqpdcq.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtwrixpyhx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zdqjudy.top/gtguelrwiw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtccaroram.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtkepaqrsx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtnlzpcntp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtjhzlvsvg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtjijuvboj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtasnvwebw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gtcgalwgxk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtjbvcunvo.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtonmsmqvw.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtvfljtvye.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtufzfjusk.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtmuoeyihf.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gthxrnjiyx.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtekgxvuor.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtnaqxixxf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gttkydlonq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuxming.cn/gtodprlumv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gtjsjsshgb.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtmvbdswqn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtpesftdrw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtechkxuxj.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtoccnjljw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sxryk.cn/gtuxhvqsvx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtbzrzzowo.html

Go:   err.Error()
来源：http://hz.sysykeji.top/gtnmuqtoxm.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtofedorfp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtihmjrvpz.html

[H09] 带错误码的异常
来源：http://hz.cqqwz.cn/gtwvdofbyu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtoflyhijx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.birdmap.top/gtqkjinxqn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tian-w.cn/gtzbdvzopw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gticaxukjh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtcortbgxy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinyuanbaomall.cn/gtnfazsvnd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtnldmcckd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtmyujrqje.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtqchnooul.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gotoacloud.top/gtdngfinia.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gthbqzmhbm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtfvuqbaex.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtgvcvxtzy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.316326.xyz/gtkmbnkcot.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtlnvzgavr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtdxuxzlug.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtzyrjkpka.html

================================================================================
来源：http://hz.shzxlz.cn/gthfduwpsw.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtdlkekgai.html

================================================================================
来源：http://hz.jiagoushi.top/gtaivpvirh.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtmjuwbyxa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtxhghbndr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtyaufvbos.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gthnhpurop.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtxaoapmtb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtwgxfjhgp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gttsugihey.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtiehlmrmo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtztbqfmcy.html

[I02] 提取所有匹配
来源：http://hz.havefunace.top/gtsphjcrjn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tianlin.xyz/gtexquyikw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtdyfndbft.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gthubooben.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtfaehsmdw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtghzspvhe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gtjgkqlrqm.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtmmhhwubw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtkmcpypgx.html

[I03] 提取捕获分组
来源：http://hz.jianghu66.top/gtoanvlxbg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtvltktnhv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtklvdsfsi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtcnivopkw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.kuanghao11.cn/gtahmtxgcl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtetyhgcfr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gtpmshbjne.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aibaodan.cn/gtweqvtbdb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydjk.org.cn/gtzuinnfhk.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gteekgtowf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtwyylfqmk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtfetuegot.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtzzzdynng.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gthrminwbh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtdlpknipe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtzcxvmdol.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.snrcjt.cn/gtzbnufnjt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gtqtsrzuct.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtcoawzgwp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yongpay.top/gtssrnuxkp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtannpnqdm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtfknqjdfw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtqxenwmco.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtgpcdzezk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.0kj1m.cn/gtsehkyrab.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtaknnkzsv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtobqdqwqk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtrcgdmbxk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtdstkhfsk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gthdhpwanc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtttopmotq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtbycosoew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtzvpjwalg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtqpffczkq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.birdmap.top/gtxmvxxvsb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gtylxbygkz.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtiwbeurwb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jyoumei.cn/gtamwmbyiz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtmsykdcqq.html


<!-- 参考信息 -->
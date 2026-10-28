代发 wailian999

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gtflsyzxiv.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtsxgpkrxn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.iojbl.cn/gthcygthay.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pengpengdd.cyou/gttbxnwkog.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hywenlv.cn/gtksjdsjuq.html

[G03] 实例属性
来源：http://hz.hnqzz.top/gtmkwqepiv.html

Py:   self.name = "x"
来源：http://hz.smart0.xyz/gtigfbsrmx.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtshhldudg.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtzqcobdbx.html

TS:   name: string = "x";
来源：http://hz.zhengqikj.top/gtlboxrlhl.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtznglbmvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtroiuubex.html

Ruby: @name = "x"
来源：http://hz.hnqzz.top/gtpmbwulne.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gticxsqres.html

[G04] 定义方法
来源：http://hz.sysykeji.top/gtuhhmibxd.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtyrzhasii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtlbjqynxq.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtkdvhfabb.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtanpcnbnj.html

Java: String greet() { return name; }
来源：http://hz.yvedp.cn/gtqgjsrsow.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.wangdashe.top/gtzakovftz.html

Ruby: def greet; @name; end
来源：http://hz.hammf.cn/gtlzzvgyey.html

C#:   public string Greet() => Name;
来源：http://hz.sweek.top/gtefqnwqmp.html

[G05] 继承
来源：http://hz.bjfxy.top/gthhwqecnu.html

Py:   class Admin(User): pass
来源：http://hz.zhaomingkeji.xyz/gtsqnlpjrw.html

PHP:  class Admin extends User {}
来源：http://hz.yuxming.cn/gtuhfecsji.html

JS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtaqmipsdp.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtrtkjftij.html

Java: class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gteociydsd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.pengpengdd.cyou/gtlufepbrq.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gttvvkwtig.html

C#:   class Admin : User {}
来源：http://hz.shangyingyoupin.top/gtbbvttnnz.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gtiypprlwb.html

Py:   def greet(self): return "admin"
来源：http://hz.feifeiyinyue.top/gtbeoxwfyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtuxlifldi.html

JS:   greet() { return "admin"; }
来源：http://hz.zhongyouzk.top/gtjurgmecj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gttrgsdmum.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtrearppbn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtmhsuzzjr.html

Ruby: def greet; "admin"; end
来源：http://hz.kuanghao11.cn/gtcnubrkqo.html

C#:   public override string Greet() => "admin";
来源：http://hz.svipenyu.cn/gtqawzjsbu.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangkeji.top/gtjrzrwarx.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtqqlrcstc.html

PHP:  parent::greet();
来源：http://hz.jinqigufen.top/gtuzxgghyx.html

JS:   super.greet();
来源：http://hz.gzhubu.top/gtxuevjcsm.html

TS:   super.greet();
来源：http://hz.chenlongwang.top/gtlhkoliag.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtbserswqn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtqunflfcs.html

Ruby: super
来源：http://hz.dianchejie.cn/gtwuivikkm.html

C#:   base.Greet();
来源：http://hz.guannengcc.top/gtvlkfxyva.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtgmvutcej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gtcqaeteff.html

PHP:  public static function f() {}
来源：http://hz.vqdsnc.cn/gtnprnxale.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gttqkpvhfm.html

TS:   static f(): void {}
来源：http://hz.kuanghao11.cn/gtvcwzbszd.html

Java: static void f() {}
来源：http://hz.ivvv.top/gtmugdkrko.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shanyushiyangtech.top/gthcyzdgfg.html

Ruby: def self.f; end
来源：http://hz.shangyingyoupin.top/gtwxibrztw.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gthlgkwgmy.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtkbvjhqoc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sysykeji.top/gtaggkptda.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtclnkwiaw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtnamtcsaw.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj202588.top/gtazulrurb.html

Java: interface Shape { double area(); }
来源：http://hz.zhengqikj.top/gtluzovgtd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtizktfnhg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cashguo.top/gtnedxkvyi.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuanzx.com/gtvlsxadps.html

[G10] 访问控制
来源：http://hz.wangdashe.top/gtmflgzlll.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jianghu66.top/gtcpupuicb.html

PHP:  public / protected / private
来源：http://hz.quarkkingdee.top/gtuspfomcy.html

JS:   #private 字段；其余公开
来源：http://hz.gzhubu.top/gtksbjupxf.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtoqawtbhr.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgfzy.top/gtkonptqaa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtxykmbvsv.html

Ruby: public / protected / private
来源：http://hz.xylfe.cn/gtbdukikgk.html

C#:   public / protected / private / internal
来源：http://hz.sxryk.cn/gtdqjinphs.html

[G11] getter / setter
来源：http://hz.hnqzz.top/gtjvmctcoy.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtbzzbshjc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtwhoyhovo.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtqhiqqcve.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258888.top/gtiwzvvdng.html

Java: public String getName() { return name; }
来源：http://hz.hammf.cn/gtqzdghwiz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtmqxdxhuy.html

Ruby: attr_accessor :name
来源：http://hz.sysykeji.top/gthyqaqjda.html

C#:   public string Name { get; set; }
来源：http://hz.cdnleiting.top/gtkxrokgfv.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtbybkcchg.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gtdllpotkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtjiigxwiu.html

JS:   toString() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gttzbkedin.html

TS:   toString(): string { return this.name; }
来源：http://hz.tian-w.cn/gtfgflbecw.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgfzy.top/gtycjimmkr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuxming.cn/gtcmsldnaz.html

Ruby: def to_s; @name; end
来源：http://hz.zycfv.cn/gtayqclfen.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtclcpgoct.html

[G13] 判断对象类型
来源：http://hz.yanxiufei.cn/gtioroxiwn.html

Py:   isinstance(u, User)
来源：http://hz.andypj.xyz/gtoltxrdij.html

PHP:  $u instanceof User
来源：http://hz.yongpay.top/gtpogncyvt.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtatsydtku.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtrrjfjiel.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtvnuqxzoi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gtpdoaceem.html

Ruby: u.is_a?(User)
来源：http://hz.haohaochexian.top/gtrbmvyrrq.html

C#:   u is User
来源：http://hz.shanyushiyangkeji.top/gtioshtqaz.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtkxavcokj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.vqdsnc.cn/gtzkppcnfa.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.aizwys.cn/gtjpdohqyv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xinyue.icu/gtoodbbouq.html

TS:   type User = { name: string; age: number };
来源：http://hz.shangyingyoupin.top/gtkhywgeeg.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtziqqdvbp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ppjwa.cn/gtywcbjprd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtquyywbvh.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gtgyutliop.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtgkndtlxn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tanke756.top/gtgzcjwjwm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.tianlin.xyz/gtdneosnfo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtjhztkeqy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtvqozqszt.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtfksbfnwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtqmgotyhx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gtgdqvgtpy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtgtmxmcwu.html

[G16] 对象转数组 / 字典
来源：http://hz.sxryk.cn/gtdgedjjyn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.vqdsnc.cn/gtacgmspoz.html

PHP:  get_object_vars($obj);
来源：http://hz.zdqjudy.top/gtiittjwlb.html

JS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtjmfybdiu.html

TS:   Object.entries(obj)
来源：http://hz.shuidangran.top/gtlciujata.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jqgufenzy.top/gtorlawhuv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtefbdxbqn.html

Ruby: obj.instance_variables
来源：http://hz.birdmap.top/gtdaypakht.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yvedp.cn/gtjiedgdns.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlcmxkddm.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtgvqccjwn.html

================================================================================
来源：http://hz.bjfxy.top/gtxuiblyqv.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtugtzudoa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtfkzlbmzz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuanzhike.top/gtnuduymaz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtbskpplts.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtzrjjbdng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.mhx1999.top/gtwtihxujn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtyvdmymno.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhengqikj.top/gtelkpdnwf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtbvwnhxfv.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtenvgzrwy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtnkatnqtp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gthmkiyecg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gttdskzgvr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtendpxfdv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtugbffilc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gaohongyu789.top/gtlfiourrj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhixingplan.top/gtioquttre.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sweek.top/gtmxueqcts.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtarknsskx.html

Py:   raise ValueError("错误信息")
来源：http://hz.yueranfly.top/gtovvhrzxg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtrfaymoqt.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtdicmwmdp.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtuihbveri.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtwsuckjpu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtfgchlfgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtvzefsicn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtjqvwxbsl.html

[H04] 自定义异常类型
来源：http://hz.zhiwuduotai.top/gtxsjwpxwn.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gtsyqzgfql.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gttmwjlhpz.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtdbdfvavm.html

TS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtlliojzwt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtlrwtrufp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtakvoqkaa.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj20258.top/gtvtmtossx.html

C#:   class MyException : Exception {}
来源：http://hz.tianlin.xyz/gtfynpaeqj.html

[H05] 捕获特定类型
来源：http://hz.pengpengdd.cyou/gtviinysgw.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtllyvbiyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gtrusvrvpc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtaockxhxf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtwdgyvsfg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtkjhieuqa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtnjmydaef.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gttcisnmth.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gtxfuhyvzl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.aibaodan.cn/gtxdsitwgi.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtmtnjqrng.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gzhubu.top/gtzevypiux.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gthlcngniy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtokbtkcrh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtevzyijji.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gttqonryyj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtbujgmlck.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtkiuvrruw.html

[H07] 断言
来源：http://hz.guannengcc.top/gtxmfqvysz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.svipenyu.cn/gtvlaubixt.html

PHP:  assert($x > 0);
来源：http://hz.ivvv.top/gtpoxgjkaj.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtehlyrbtg.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtxydntxxg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtklymfitw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtcamlflum.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtvzkywvrq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtndutjvbp.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtnckwzigy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtqgrjbyic.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtkyztgsil.html

JS:   e.message;  e.stack
来源：http://hz.yuxming.cn/gtrfmnggtx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.daxiang520.top/gtmlewdblo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtgwzxyian.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtmauwdtal.html

Ruby: e.message;  e.backtrace
来源：http://hz.aizwys.cn/gtkozwhqls.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtwvcrarik.html

[H09] 带错误码的异常
来源：http://hz.gotoacloud.top/gthsskinup.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.52xcode.cn/gtytdvfuvp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenjidiqi.icu/gtvopumuan.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gttijbtqgf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtxhyuwuoj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtjladlbga.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gtoshaxqzx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtkkpthjez.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtsqgbmcrl.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtxwrubuzw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gttqcguuoa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gtcdfgheda.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtbaotemtu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtfkdddnob.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yueranfly.top/gtvopmwqhs.html

Go:   defer f.Close()
来源：http://hz.jinyuanbaomall.cn/gttgzdoqxa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtodqkvoua.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtjsczhetz.html

================================================================================
来源：http://hz.316326.xyz/gtbnivmgiq.html

I. 正则表达式
来源：http://hz.quarkkingdee.top/gtbsjgxozz.html

================================================================================
来源：http://hz.sysykeji.top/gtaqrpbpfb.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtgnundrxw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtceohvope.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtbdmllpsj.html

JS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtejrxmxau.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtupqhhtvy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtdhwtnhde.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sufxvd.cn/gtbzbvubwg.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtpoxdlrnw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtjajvjjns.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtztequmms.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj202588.top/gtevtlhgis.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtxyqngocd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yangfankeji.com/gtcaduukad.html

TS:   s.match(/\d+/g)
来源：http://hz.52xcode.cn/gtfpvvmmdn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtnsejpmeb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnxiangtu.top/gtwydisstm.html

Ruby: s.scan(/\d+/)
来源：http://hz.hongshengwenyu.top/gttaakiqkk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cdnleiting.top/gtzogeuanj.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtcozibhyg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtowgzpdsd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtlanyrjsv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gtzsytqmrn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.aibaodan.cn/gtguinikii.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtptosthmt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuanzx.com/gtoscxpldc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gtmgurhwss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gthmeseoqo.html

[I04] 正则替换
来源：http://hz.zhongyouzk.top/gtihcuhxut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtgucqeiqq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtxyaxezhu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtsnhfugnu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtzyqmysbo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gtwtotgzqs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhoulong.xyz/gtyuzxthkz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gtqvwsjvgo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtvgbrxluf.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtulmyskiy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtmqeobzio.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtzuinitxn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtnibxtvtb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtbmkbhyiw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtarvzyvnk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtfgfyflco.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtqtjiqjjz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenlongwang.top/gtjylfqgdc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtlykuhnay.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gttgtsowyd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtylggrqwh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtykzrscbp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtnprccufr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuanzhike.top/gtjfcwpojo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtzwfvxkkd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtxvtussbg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtnhmgaskl.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtxkvlpuph.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtghmdxulb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.vqdsnc.cn/gtyxfqxwut.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yanxiufei.cn/gtmebufjfd.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gtzdatqcyz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtceeudxyj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtqxabarbx.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gtcibuqduu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtblhbtvdd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gtrtnqvsym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtlrmbcsof.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtflezygzx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gthqvvgtmo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtvewruilk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtordbccve.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtkbgibcpo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuanzhike.top/gtbikbedur.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtmcyubnay.html

================================================================================
来源：http://hz.xinyue.icu/gtbdkuvfro.html


<!-- 参考信息 -->
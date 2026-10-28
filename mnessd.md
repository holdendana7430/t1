代发 wailian999

Java: class User {}
来源：http://hz.wangdashe.top/gttsugsqps.html

Go:   type User struct { Name string }
来源：http://hz.guannengcc.top/gtkxgxdlkd.html

Ruby: class User; end
来源：http://hz.snrcjt.cn/gtrugtjxid.html

C#:   class User {}
来源：http://hz.c1oappe.top/gtialsjdhu.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gturwlatwy.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hysaishi.cn/gtftenibqr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.meibo888.top/gtywseeyek.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtbfemnrdi.html

TS:   constructor(public name: string) {}
来源：http://hz.jinghuilouyu.cn/gtnpbgndlp.html

Java: User(String name) { this.name = name; }
来源：http://hz.xinyue.icu/gtdznweust.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.daria6918.cn/gthdbuhvpw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.havefunace.top/gtruptwwtc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yuanzhike.top/gtdanhiuoo.html

[G03] 实例属性
来源：http://hz.hywenlv.cn/gthltelnbh.html

Py:   self.name = "x"
来源：http://hz.hammf.cn/gtghqwbmit.html

PHP:  public string $name = "x";
来源：http://hz.birdmap.top/gtckpwamjf.html

JS:   this.name = "x";
来源：http://hz.ivvv.top/gtwgofamfq.html

TS:   name: string = "x";
来源：http://hz.yj20258888.top/gtnwutxbkf.html

Java: private String name;
来源：http://hz.xylfe.cn/gtstmtzgvk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtcktphdqd.html

Ruby: @name = "x"
来源：http://hz.ppjwa.cn/gtumnsduyb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aibaodan.cn/gtskuuyans.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtgostsopv.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtjcbuvrwh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.wangdashe.top/gtkrmaayou.html

JS:   greet() { return this.name; }
来源：http://hz.birdmap.top/gtwovqpwmu.html

TS:   greet(): string { return this.name; }
来源：http://hz.hfpthk.cn/gtqqqynxfz.html

Java: String greet() { return name; }
来源：http://hz.vqdsnc.cn/gtusukbfoj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cucudq.cn/gtgmylfogm.html

Ruby: def greet; @name; end
来源：http://hz.nwbrower.top/gtruluimkl.html

C#:   public string Greet() => Name;
来源：http://hz.xylfe.cn/gtsfdasddy.html

[G05] 继承
来源：http://hz.mhx1999.top/gtukprfuaj.html

Py:   class Admin(User): pass
来源：http://hz.guannengcc.top/gtdtxlqftf.html

PHP:  class Admin extends User {}
来源：http://hz.yongpay.top/gtjwvwvsif.html

JS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtyqjsohpn.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtjpvynxxp.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtxjunewof.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtitzrygnk.html

Ruby: class Admin < User; end
来源：http://hz.hywenlv.cn/gtwjvtzfsi.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtriuihbxm.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtvjristvb.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtymtluwtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hfpthk.cn/gtptmtiqhh.html

JS:   greet() { return "admin"; }
来源：http://hz.hammf.cn/gtkqnqwmoa.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtbuseahbg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtrisvqavg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtjanyywsi.html

Ruby: def greet; "admin"; end
来源：http://hz.ybcxt.top/gtbtzwmavw.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtmpehclbf.html

[G07] 调用父类方法
来源：http://hz.sweek.top/gtsxexrvad.html

Py:   super().greet()
来源：http://hz.daxiang520.top/gtulecfcqc.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gtfuidrfpq.html

JS:   super.greet();
来源：http://hz.yj20258888.top/gtejpwxhun.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gtxmtcsing.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtavnjnnim.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtxbvgjikv.html

Ruby: super
来源：http://hz.chenlongwang.top/gtasxwhcak.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtzpivwnxc.html

[G08] 静态方法与属性
来源：http://hz.fengsongda.top/gtkeinrvlx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.mhx1999.top/gtkktkcgut.html

PHP:  public static function f() {}
来源：http://hz.hysaishi.cn/gthbdcnmrw.html

JS:   static f() {}
来源：http://hz.zycfv.cn/gtafeujpxc.html

TS:   static f(): void {}
来源：http://hz.yj20258.top/gtqthncpqw.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gttyxxvhdg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jqgufenzy.top/gtgaaujejq.html

Ruby: def self.f; end
来源：http://hz.xziqi.cn/gtjyakybdh.html

C#:   public static void F() {}
来源：http://hz.daxiang520.top/gtjvivjekh.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtgitpfmou.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangshuangyany.cn/gtgtxpeorn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.pycfn.com/gtaokfirbu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hywenlv.cn/gtxxntrvfj.html

TS:   interface Shape { area(): number; }
来源：http://hz.pengpengdd.cyou/gtztpnocso.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtcqxbuxad.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tianlin.xyz/gtzsmjyhsk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.mhx1999.top/gtgykusvhv.html

C#:   interface IShape { double Area(); }
来源：http://hz.svipenyu.cn/gtuwsogbwd.html

[G10] 访问控制
来源：http://hz.yonumen.top/gtealpazni.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gzhubu.top/gtvittjknw.html

PHP:  public / protected / private
来源：http://hz.zdqjudy.top/gtffnmtgod.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gteftmijvw.html

TS:   public / protected / private
来源：http://hz.tian-w.cn/gtquhegswa.html

Java: public / protected / private / 默认包级
来源：http://hz.jinyuanbaomall.cn/gtzhwpsdhq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yangfankeji.com/gtymgebrjk.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtdzuuhvaf.html

C#:   public / protected / private / internal
来源：http://hz.mhx1999.top/gtxzbfrufh.html

[G11] getter / setter
来源：http://hz.wangshuangyany.cn/gtvrfdddzi.html

Py:   @property 与 @x.setter
来源：http://hz.316326.xyz/gtekzbakkg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtnnmsmmls.html

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtsorxuzxz.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuanzx.com/gtsvievowj.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gtcbikwwiy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtqymvzstp.html

Ruby: attr_accessor :name
来源：http://hz.wangshuangyany.cn/gthdrxiqye.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtuhppngej.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtmiqvyada.html

Py:   def __str__(self): return self.name
来源：http://hz.jiagoushi.top/gtyzsmhgjf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtvzzlgoos.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtadxyvaug.html

TS:   toString(): string { return this.name; }
来源：http://hz.zhixingplan.top/gttyidmeea.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtxpcehsfb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shzxlz.cn/gtztbwbjyc.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtndlswony.html

C#:   public override string ToString() => Name;
来源：http://hz.hysaishi.cn/gtygpknmzp.html

[G13] 判断对象类型
来源：http://hz.sxryk.cn/gtmemyiopj.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gthwyjguyt.html

PHP:  $u instanceof User
来源：http://hz.andypj.xyz/gthgehxiyu.html

JS:   u instanceof User
来源：http://hz.yj20258888.top/gtkibdgzir.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gttuepgvlp.html

Java: u instanceof User
来源：http://hz.guannengcc.top/gtrsnbfmih.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.kuanghao11.cn/gtkjvuzjyo.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtjewqwwcz.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtpkhqouqb.html

[G14] 数据类 / record
来源：http://hz.zhengqikj.top/gtqhuymuim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtddnpunnc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangshuangyany.cn/gtoenfjvne.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtotknihqj.html

TS:   type User = { name: string; age: number };
来源：http://hz.gzhubu.top/gtzafkgbqv.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtkbctudbl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtwbztsqgq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtyainatny.html

C#:   record User(string Name, int Age);
来源：http://hz.hysaishi.cn/gtfajzfgnr.html

[G15] 枚举
来源：http://hz.quarkkingdee.top/gtxtatqhkp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxinkj.top/gtbqduuigw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtyidovott.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gtvpsbaqhp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtzoawmzdm.html

Java: enum Color { RED, GREEN }
来源：http://hz.ivvv.top/gtpzfezlin.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guannengcc.top/gtlqwjwovj.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtgspfsnoj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ydjk.org.cn/gtdcnswknh.html

[G16] 对象转数组 / 字典
来源：http://hz.xinyue.icu/gtzerszvrq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtedbdrubp.html

PHP:  get_object_vars($obj);
来源：http://hz.9152youxi.cn/gtrwwczgug.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtttxliclk.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtmvvbjnbd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangdashe.top/gtefrwsrvc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258888.top/gtguotrgzz.html

Ruby: obj.instance_variables
来源：http://hz.yongpay.top/gtuzreesji.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtgfyxelyu.html

================================================================================
来源：http://hz.316326.xyz/gtscripsyo.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtomqvrvoe.html

================================================================================
来源：http://hz.yj20258.top/gtkwpnvehh.html

[H01] try / catch 基础
来源：http://hz.feifeiyinyue.top/gtqhaiyhoy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xuanzx.com/gtjpjunzip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtkiggfgbe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtxbotsoho.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtuokguclp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gtlnqlwuvx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtlrdrwosu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtfkaitenc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtmepyczwo.html

[H02] finally / ensure 收尾
来源：http://hz.jqgfzy.top/gtkvqffwys.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhengqikj.top/gtwkampzrg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtaplbkvtd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtbulieddo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtsqfcujyl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtzzaiewvh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtsypsagou.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sweek.top/gtqnsxdjen.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtwtqgqjgc.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gttbincuvn.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtgpawfdhs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtkkgxfmfy.html

JS:   throw new Error("错误信息");
来源：http://hz.nwbrower.top/gtfhurahxx.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtbmwcxulr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtrsicjfle.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gaohongyu789.top/gtdhkpwnzn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtcqduqghs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtqdklysvb.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gthlymgzgl.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtdlcjhslb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj202588.top/gtzbweyzkp.html

JS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtfkbdgmmq.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtcbzxowlo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtsxexexbd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtlwjfernu.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtzcpybsbk.html

C#:   class MyException : Exception {}
来源：http://hz.tianlin.xyz/gtirsfxwfn.html

[H05] 捕获特定类型
来源：http://hz.aizwys.cn/gtlvcrjhfe.html

Py:   except ValueError as e:
来源：http://hz.daxiang520.top/gtlmkizuhv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtgotmcggz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.quarkkingdee.top/gtudqkmexk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtshwdaxcs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtptiwlrij.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xziqi.cn/gtyeerqcpy.html

Ruby: rescue ArgumentError => e
来源：http://hz.jiagoushi.top/gtrlvzwnhi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.0kj1m.cn/gtpqrqwlhk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtnjbobrqg.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtdbyhafiv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtxkkbujgr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gteskhfmwg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtnmewksfq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtpdhxiwgm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtxjhzqnco.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtqhmfbmkz.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtllchrtxe.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtewshontn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtpuzpluce.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtluucbugt.html

JS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtwwipywdh.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtylzwthqp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtqjdzeodx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtlbwaanmm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtxwsszmjk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtpypeckjp.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtobkhnjzl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtwseqqqrv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtabjmghwn.html

JS:   e.message;  e.stack
来源：http://hz.snrcjt.cn/gtsqfufdea.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtdusffzws.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtbyokfnsr.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtwuavtlob.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigfzy.top/gtgewdtxtt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgufenzy.top/gteolelxyw.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gttkslbter.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtizfzguuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cheryme.top/gtcxnnaaja.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtxvrivfsb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtjyduydex.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtubpcmdpm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtzxxnnqet.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhongyouzk.top/gtnburywot.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gtywpdefgy.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtxwiyflrn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtyberenmj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtdefixhra.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtukrlsbii.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtrivbyyrh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.vqdsnc.cn/gtlpcvgpto.html

Go:   defer f.Close()
来源：http://hz.yonumen.top/gtgvvqiajp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gtdrbuwqcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gthniwbybs.html

================================================================================
来源：http://hz.xinyue.icu/gtndpfyjdt.html

I. 正则表达式
来源：http://hz.ivvv.top/gtxaspotps.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpmrdaaqq.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtdxelajup.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gthbtbmouf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtmfoilgxx.html

JS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtwodalguo.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtrjpidvlw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtrafxiwgp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinyuanbaomall.cn/gtmkfddlje.html

Ruby: s.match?(/\d+/)
来源：http://hz.ehwqpu.com/gttqrftfaa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtjbelpsfs.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtbkuqddze.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtsojaobaj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtgqpottgz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gttulvfrfq.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gthovcbkjf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtsqphuhza.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj202588.top/gtjlobjwct.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtixoxyhgj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtthzamdvv.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gthexcicon.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hongshengwenyu.top/gtdlecoasz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtpvptnhes.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sweek.top/gttzdxeeco.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydjk.org.cn/gtechmtyny.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gtefaptmod.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gtymcrtedj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cucudq.cn/gtfemqpscu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtxeumdqud.html

[I04] 正则替换
来源：http://hz.gaohongyu789.top/gtiqiktolw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtxxtfppgz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtxnlbokjp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtcwhvcyhl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtetbeduji.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtrmoadabv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258.top/gtrhisqbat.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtcekdxkyc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtrfzynujj.html

[I05] 按正则拆分
来源：http://hz.guannengcc.top/gtcklluomm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.feifeiyinyue.top/gtpfejjbih.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhengqikj.top/gthpytkitn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtkoqxgogn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtxmmrfeqe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtqhkyjyfy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtbukqtekd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtckygrhsd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtmfznoerj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtovuydpls.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtvlvgxgka.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtjmuzzhej.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtbpqlsirf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtauhvfrao.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gterwsluzq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xinyue.icu/gtniqcfchu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gtndesiiwc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtjgmioafd.html

[I07] 忽略大小写与多行模式
来源：http://hz.xinyue.icu/gtwzzlhwnt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtococqxzn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtyjnsmvca.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtyubtjzvu.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtpkojvolc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtatrhajsc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtowvhuzgw.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gthchqjqaj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zdqjudy.top/gtxfkwznan.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtlbwvspip.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tian-w.cn/gtayboxnal.html


<!-- 参考信息 -->
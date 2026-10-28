代发 wailian999

================================================================================
来源：http://hz.ybcxt.top/gtxbsirjqv.html

G. 面向对象
来源：http://hz.hywenlv.cn/gttcqcekir.html

================================================================================
来源：http://hz.pycfn.com/gtyssbnlhg.html

[G01] 定义类
来源：http://hz.feifeiyinyue.top/gtxcagffqq.html

Py:   class User: pass
来源：http://hz.ywan-chungtsiang.top/gtsxggkond.html

PHP:  class User {}
来源：http://hz.pycfn.com/gtugkzjipo.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtfioypktb.html

TS:   class User { name: string = ""; }
来源：http://hz.smart0.xyz/gtjlofyqxy.html

Java: class User {}
来源：http://hz.yonumen.top/gtiebzcwwq.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtdfdznrzx.html

Ruby: class User; end
来源：http://hz.jyoumei.cn/gtturxjbjm.html

C#:   class User {}
来源：http://hz.hammf.cn/gthozmjxjk.html

[G02] 构造函数
来源：http://hz.dianchejie.cn/gtsberxkiz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtrmqinong.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuanzhike.top/gtjvjjsrkx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tian-w.cn/gttlhycfhd.html

TS:   constructor(public name: string) {}
来源：http://hz.hongshengwenyu.top/gtovlibpet.html

Java: User(String name) { this.name = name; }
来源：http://hz.cheryme.top/gtewprsoew.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yj20258.top/gtnhtlgrgq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aibaodan.cn/gtrnxtusyk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cheryme.top/gtjhrzgtrq.html

[G03] 实例属性
来源：http://hz.havefunace.top/gtgzveersi.html

Py:   self.name = "x"
来源：http://hz.vqdsnc.cn/gtqlocetpl.html

PHP:  public string $name = "x";
来源：http://hz.guowangkeji.top/gteidsqxhr.html

JS:   this.name = "x";
来源：http://hz.xuetiantiany.cn/gtbnutbdhm.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtqpulkcda.html

Java: private String name;
来源：http://hz.xuanzx.com/gtfmfepqbs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtbstsbcoc.html

Ruby: @name = "x"
来源：http://hz.jinyuanbaomall.cn/gtdvrfiokg.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgfzy.top/gtkmniasgj.html

[G04] 定义方法
来源：http://hz.ppjwa.cn/gtugxwlnfu.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtcwikbvph.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtrqsicbtu.html

JS:   greet() { return this.name; }
来源：http://hz.dianchejie.cn/gtmjwysaut.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtsqlajexe.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gthkizgcsy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gteurtuley.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtylvyzybg.html

C#:   public string Greet() => Name;
来源：http://hz.chenjidiqi.icu/gtniljqtul.html

[G05] 继承
来源：http://hz.zhixingplan.top/gtgsmcvulg.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtdymyxjef.html

PHP:  class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtfjjrjtwg.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtmudkvfgk.html

TS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtqhehdqqq.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gtefxskuid.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinghuilouyu.cn/gtaddcrkzc.html

Ruby: class Admin < User; end
来源：http://hz.daxiang520.top/gtgtrhyzrf.html

C#:   class Admin : User {}
来源：http://hz.jinqigufen.top/gthswkptto.html

[G06] 重写方法
来源：http://hz.bjfxy.top/gtewdgzhgw.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtvuklvmvz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtwfxbqcmx.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtxdobenga.html

TS:   greet(): string { return "admin"; }
来源：http://hz.zhongyouzk.top/gtdputaqpo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtfkkmjpac.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtdvovslyw.html

Ruby: def greet; "admin"; end
来源：http://hz.hongshengwenyu.top/gtdbayagkr.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydjk.org.cn/gtledchghp.html

[G07] 调用父类方法
来源：http://hz.yvedp.cn/gtmrnostap.html

Py:   super().greet()
来源：http://hz.haohaochexian.top/gtevqkeoza.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtcpokloqr.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtcpzadjsx.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtkuzloqwf.html

Java: super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtqxvklvyq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtqajoqwaz.html

Ruby: super
来源：http://hz.pengpengdd.cyou/gteszwmgcy.html

C#:   base.Greet();
来源：http://hz.guowangkeji.top/gtqbvzjtpb.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gtsnythofw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sweek.top/gtjzosspin.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtkcdxupuu.html

JS:   static f() {}
来源：http://hz.zhiwuduotai.top/gtllujpqsh.html

TS:   static f(): void {}
来源：http://hz.yanxiufei.cn/gtrzjzbuxt.html

Java: static void f() {}
来源：http://hz.chenlongwang.top/gtwxbyqwqk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.aibaodan.cn/gtkjxmksxu.html

Ruby: def self.f; end
来源：http://hz.yvedp.cn/gtansewewf.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtqirzxjnb.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtguptnijt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtxflvyvrz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtreibwtth.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtiiciercw.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhoulong.xyz/gttopveafe.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtwyhlkugu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtrixumnkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtvfevgvpv.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtxkijswrh.html

[G10] 访问控制
来源：http://hz.hnxiangtu.top/gtotacngqo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtjfrmlsrn.html

PHP:  public / protected / private
来源：http://hz.sweek.top/gtrlxvhmcj.html

JS:   #private 字段；其余公开
来源：http://hz.hnxiangtu.top/gtfamykvxd.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtquhyvbbr.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtzzyhmszo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtfqyrlmwh.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtdwusopvq.html

C#:   public / protected / private / internal
来源：http://hz.316326.xyz/gtvqlxqvhn.html

[G11] getter / setter
来源：http://hz.dashuyun.cn/gtsoytrtft.html

Py:   @property 与 @x.setter
来源：http://hz.hnxiangtu.top/gtxvchdlyq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gteabzzlrs.html

JS:   get name() { return this._name; }
来源：http://hz.guowangkeji.top/gtkvzgiear.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gturkgxznc.html

Java: public String getName() { return name; }
来源：http://hz.andypj.xyz/gtvawmutbj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cashguo.top/gtwbykjzow.html

Ruby: attr_accessor :name
来源：http://hz.tianlin.xyz/gtbwovtezy.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtwwtggsza.html

[G12] 对象转字符串
来源：http://hz.9152youxi.cn/gtzlmzispq.html

Py:   def __str__(self): return self.name
来源：http://hz.cdnleiting.top/gtypnifyzk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gthjsirduu.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtxpmmjmpf.html

TS:   toString(): string { return this.name; }
来源：http://hz.yueranfly.top/gthkhsketl.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtysfrmsod.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.meibo888.top/gtzzokyrnd.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtoiiqpxsm.html

C#:   public override string ToString() => Name;
来源：http://hz.smart0.xyz/gthbwihtmi.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtwohorvxv.html

Py:   isinstance(u, User)
来源：http://hz.ehwqpu.com/gtvxwjfebn.html

PHP:  $u instanceof User
来源：http://hz.cashguo.top/gtgpofaorr.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtckrypqax.html

TS:   u instanceof User
来源：http://hz.316326.xyz/gtbhhceqkn.html

Java: u instanceof User
来源：http://hz.jianghu66.top/gtmwjfbbwv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtwpjyvgyi.html

Ruby: u.is_a?(User)
来源：http://hz.hywenlv.cn/gtlhzcrtbe.html

C#:   u is User
来源：http://hz.zhijiandao.cn/gtkfntdjuw.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtavdtmzvo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daxiang520.top/gtljpnuiyj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtepnawyoa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtbtsdyret.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhijiandao.cn/gtxatzuxof.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtjzqnvnmb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gtvatnmlch.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hnqzz.top/gtoifdnfoe.html

C#:   record User(string Name, int Age);
来源：http://hz.316326.xyz/gtqdhhxhxi.html

[G15] 枚举
来源：http://hz.birdmap.top/gtyirahcnz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtjkjbkiml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ppjwa.cn/gtknjksejt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.guowangkeji.top/gtxmvfxdsv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gtvbbyxqar.html

Java: enum Color { RED, GREEN }
来源：http://hz.tian-w.cn/gtapfsjrak.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtrjwsrguw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cashguo.top/gtcyurbgiw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenjidiqi.icu/gteolkcagl.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtccpcxazt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gtzkrwvorw.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtnkfswciz.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtalwqgaja.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtajrxvnyf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gticpjbkwk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hfpthk.cn/gtrhremkqv.html

Ruby: obj.instance_variables
来源：http://hz.jqgufenzy.top/gtedkqhhcx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtylvdutfz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcagalkhv.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtficamcvw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtaxcfijas.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtjklsxazn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gttadgbrcq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtqtrlkaau.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtmxmbxybq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtxlzmsvuf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtpbayzffp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jyoumei.cn/gtnklksbwm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtbrvosuja.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.dashuyun.cn/gtgwuccwux.html

[H02] finally / ensure 收尾
来源：http://hz.nanxinkj.top/gtomzwzcua.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gthfksznmg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtdtvlchox.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtviokaxvz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtekasurrf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtiukpflpc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtxwpuzeta.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.sxryk.cn/gtqtkytryl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtyidwfhwn.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gtppfhjttq.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtspjeoszb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtghodynji.html

JS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtxspebjlo.html

TS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtpfbsjtsz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtxykxqmhy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj202588.top/gtfpdydevy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtkhcggbbt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtvrpioxqz.html

[H04] 自定义异常类型
来源：http://hz.zhijiandao.cn/gtrvyeibos.html

Py:   class MyError(Exception): pass
来源：http://hz.xuetiantiany.cn/gtvtgtenel.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gteimimjtu.html

JS:   class MyError extends Error {}
来源：http://hz.aizwys.cn/gtaptnmvsp.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtnlulvpxk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtlgahuwue.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenzaomai.com/gtrizfomcf.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtfxiqjjyk.html

C#:   class MyException : Exception {}
来源：http://hz.guannengcc.top/gtwyvukqzz.html

[H05] 捕获特定类型
来源：http://hz.cashguo.top/gtregytbjw.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtkhcvfxdp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtiuqiqxah.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtrivbzdax.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtptsnfmad.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.havefunace.top/gtwzaxasdh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.52xcode.cn/gtivtlvptl.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtslpzwtke.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtbzwyzyrl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtxykxvfmq.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtvxkhvtom.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuxming.cn/gttrpmzkfp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtsrzikofw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtpoxdbbgo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtgznihgij.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tian-w.cn/gtrhzexwko.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtrcywuhqh.html

C#:   obj?.A?.B ?? default
来源：http://hz.ydzc1.top/gtjljtwsyh.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtfymzzclu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgfzy.top/gttdsgzpno.html

PHP:  assert($x > 0);
来源：http://hz.jqgufenzy.top/gtfnyvpgxp.html

JS:   console.assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtlabiaegf.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtdhoyijeo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtrqxgiosb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtvaobinlp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtdudqrqpn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cheryme.top/gtqzmqiupk.html

[H08] 获取错误信息与堆栈
来源：http://hz.shangyingyoupin.top/gtwzoyafkv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtewxuniip.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gturnbmdmw.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtnbrmscix.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj202588.top/gtngbswfff.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtbyctfkca.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtpkktwogp.html

Ruby: e.message;  e.backtrace
来源：http://hz.bjfxy.top/gtbyvhiphb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtmerpbzbo.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtuzcwhsba.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ehwqpu.com/gtcuajoegk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pycfn.com/gtizocmvtc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gttwrnrilj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtdcwggjqd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinghuilouyu.cn/gtctyyqeaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sweek.top/gtaifidcqa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtkbjtkblz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtqtkezxyo.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtdtfdpexi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtdmxdhvvz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtjgnzfsuz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtavxdtqqe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtkhrgxfty.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtriaitwkj.html

Go:   defer f.Close()
来源：http://hz.bjfxy.top/gtlznvayej.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtlqmuxirx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtljdtlcrg.html

================================================================================
来源：http://hz.yj20258888.top/gtlmalfxxj.html

I. 正则表达式
来源：http://hz.redwolf501.top/gtfptmvagl.html

================================================================================
来源：http://hz.sufxvd.cn/gtooduwkgo.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtqpcmyvdk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtvyoizgzo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.vqdsnc.cn/gttxnmehil.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtiokiqkwx.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtrvxtgpkl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangtech.top/gtypqpgtcb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtxmaditmk.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtimrcmpng.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gtlvmcqgrm.html

[I02] 提取所有匹配
来源：http://hz.hnxiangtu.top/gtoicmcskz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtdaqjlmzk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtmfodqsaz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ppjwa.cn/gtluayqscr.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gtwfjubjkl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtgbqosvhq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gthjygdizq.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gtzcaalqkq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtkysbewty.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtnnlwudkk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aizwys.cn/gtjlqphlvf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtwzrdeupi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtdbvzmpgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtkcjokrsh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gthnclmkyl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtovqanomb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gtiblgnxuy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtzyxtyhff.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gtqkaqfpnu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtkqjtchbb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shuidangran.top/gtpxprtnvl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtpbgaawel.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtdaqfvent.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtdztuuprr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtqmnighou.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gzhubu.top/gtkylndwjo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtbndrcwoq.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtmvbpbjvn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gotoacloud.top/gtjvdcgkeo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258.top/gtlwkeoqbg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtrcrxvfku.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtpkgsosqi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shuidangran.top/gtnrbtecvn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gttbjatnyr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gttkbbwqol.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtwfmqtkjv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gtfyagsnkb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gthcylnniv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtqjknkqov.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtapwfypky.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtcsruxjhj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yvedp.cn/gtmqjmhqui.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtodfpxmws.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtxgxiufjo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtkijkmjky.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtozunlmsu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gttkdkffhy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtvaymxwpk.html


<!-- 参考信息 -->
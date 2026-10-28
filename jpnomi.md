代发 wailian999

Py:   class User: pass
来源：http://hz.9152youxi.cn/gtxhqieabr.html

PHP:  class User {}
来源：http://hz.tian-w.cn/gtfttxyhgd.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtfyjgdmkk.html

TS:   class User { name: string = ""; }
来源：http://hz.bjfxy.top/gtisgegaqi.html

Java: class User {}
来源：http://hz.birdmap.top/gthvlmndvy.html

Go:   type User struct { Name string }
来源：http://hz.c1oappe.top/gtjwyijlcv.html

Ruby: class User; end
来源：http://hz.gogol.net.cn/gtxarikldq.html

C#:   class User {}
来源：http://hz.yonumen.top/gtbywjnnlf.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtkkiamajk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtfbcuvkkb.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtquvsslpx.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinyuanbaomall.cn/gtqpymkoho.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtfgpwfzey.html

Java: User(String name) { this.name = name; }
来源：http://hz.bjfxy.top/gtksdltvdu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtuwjwwmgv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xziqi.cn/gtsimrratw.html

C#:   public User(string name) { Name = name; }
来源：http://hz.quarkkingdee.top/gtzjvcjlcu.html

[G03] 实例属性
来源：http://hz.shanyushiyangtech.top/gtaeiodzwb.html

Py:   self.name = "x"
来源：http://hz.gogol.net.cn/gtkdjbizil.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtrzfkynbw.html

JS:   this.name = "x";
来源：http://hz.redwolf501.top/gtsfxtcuco.html

TS:   name: string = "x";
来源：http://hz.yongpay.top/gtkvlnsgof.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtxprnsuhv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtpeekrsay.html

Ruby: @name = "x"
来源：http://hz.cqqwz.cn/gtbjpzvenn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gotoacloud.top/gtbdyobava.html

[G04] 定义方法
来源：http://hz.xuetiantiany.cn/gtfhqxtror.html

Py:   def greet(self): return self.name
来源：http://hz.yanxiufei.cn/gtzmomoqon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtpnxdaqis.html

JS:   greet() { return this.name; }
来源：http://hz.zhoulong.xyz/gtccgcdopa.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtpgsdefdd.html

Java: String greet() { return name; }
来源：http://hz.yonumen.top/gtgrzmqtka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtxrhftuso.html

Ruby: def greet; @name; end
来源：http://hz.jlsjyb.cn/gtvojgstsa.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtaqdfqwsw.html

[G05] 继承
来源：http://hz.dashuyun.cn/gtkjlxfebw.html

Py:   class Admin(User): pass
来源：http://hz.jinyuanbaomall.cn/gtztlaxhnc.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtatgnbkbt.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gttnozpyed.html

TS:   class Admin extends User {}
来源：http://hz.sufxvd.cn/gtkaqgwstp.html

Java: class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtrszyxeds.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtmssceglw.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtyzlqccfx.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtnhkpwpqf.html

[G06] 重写方法
来源：http://hz.zhaomingkeji.xyz/gteylxnpev.html

Py:   def greet(self): return "admin"
来源：http://hz.zhongyouzk.top/gtuknfakgi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtaegtmzaf.html

JS:   greet() { return "admin"; }
来源：http://hz.yueranfly.top/gtcwatepdf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtcfjyqqer.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtjzdeqaad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtqayghydk.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtancqwcvs.html

C#:   public override string Greet() => "admin";
来源：http://hz.nanxuanxn.top/gtuqfghknl.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtjjkpauvr.html

Py:   super().greet()
来源：http://hz.xuetiantiany.cn/gtobccrmqd.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtphqofmcl.html

JS:   super.greet();
来源：http://hz.shuidangran.top/gtlhovcgnc.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtjlsxrbja.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtwekznfrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtkyawemkf.html

Ruby: super
来源：http://hz.ywan-chungtsiang.top/gtxbwpnemi.html

C#:   base.Greet();
来源：http://hz.xuanzx.com/gtyducdbsc.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtusrcsvak.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenzaomai.com/gtaxunflbe.html

PHP:  public static function f() {}
来源：http://hz.gogol.net.cn/gtdduznszh.html

JS:   static f() {}
来源：http://hz.jianghu66.top/gtvimsfyur.html

TS:   static f(): void {}
来源：http://hz.cheryme.top/gtmkljlexj.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtbirkhkhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ybcxt.top/gtuttwxxzt.html

Ruby: def self.f; end
来源：http://hz.fengsongda.top/gteptlibef.html

C#:   public static void F() {}
来源：http://hz.hongshengwenyu.top/gthmfdimer.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtufyscjwl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtedeywdhl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.c1oappe.top/gtlttaytem.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtjfhjvqtu.html

TS:   interface Shape { area(): number; }
来源：http://hz.shangyingyoupin.top/gthlzgsclw.html

Java: interface Shape { double area(); }
来源：http://hz.ivvv.top/gthzxpqnja.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shangyingyoupin.top/gtcgxrkmci.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jqgufenzy.top/gtbfwkyhhy.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnqzz.top/gtemwympqp.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtqgjmwigh.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtnqbogcuu.html

PHP:  public / protected / private
来源：http://hz.shuidangran.top/gtuoxcvujm.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gthkyuzisf.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtntzjsahm.html

Java: public / protected / private / 默认包级
来源：http://hz.daxiang520.top/gthkngcjxz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cheryme.top/gtxondemle.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtthxqsrgd.html

C#:   public / protected / private / internal
来源：http://hz.c1oappe.top/gtdwmeqzwk.html

[G11] getter / setter
来源：http://hz.yangfankeji.com/gthcykqpix.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtxcjxvodf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtsfkydbot.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtgpjsgsee.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gthnmcdlor.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gthibawlhz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sufxvd.cn/gtjomwrads.html

Ruby: attr_accessor :name
来源：http://hz.chenjidiqi.icu/gtuxiwgqxp.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtzzgsgvex.html

[G12] 对象转字符串
来源：http://hz.zhoulong.xyz/gtrpilzftg.html

Py:   def __str__(self): return self.name
来源：http://hz.yueranfly.top/gtdumigzpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtkqiufwaq.html

JS:   toString() { return this.name; }
来源：http://hz.tianlin.xyz/gtgmskduka.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtxnyjfqrr.html

Java: @Override public String toString() { return name; }
来源：http://hz.cucudq.cn/gtawgfiwga.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fengsongda.top/gtwpblfcxd.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtfvmghhuv.html

C#:   public override string ToString() => Name;
来源：http://hz.yuxming.cn/gtjbbspmpf.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtcltaecvt.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtiipnraev.html

PHP:  $u instanceof User
来源：http://hz.jinghuilouyu.cn/gtaprnhynn.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtqvoimxru.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtjcfeyxkp.html

Java: u instanceof User
来源：http://hz.yvedp.cn/gtvybowyeq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtpnhscrxf.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtbtzhyeoz.html

C#:   u is User
来源：http://hz.jqgufenzy.top/gtwkjmhosw.html

[G14] 数据类 / record
来源：http://hz.xuanzx.com/gtlazwitwf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigfzy.top/gtdtzmpzjy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinqigfzy.top/gtidctqxnb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtdtknhinb.html

TS:   type User = { name: string; age: number };
来源：http://hz.smart0.xyz/gtlaaijtng.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtasqsrhno.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigufen.top/gtohhzkqpk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtiqkcohru.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtwkeceewh.html

[G15] 枚举
来源：http://hz.tianlin.xyz/gtnznoxqbs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.kuanghao11.cn/gtvlzhjmxk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.iojbl.cn/gthsebghsc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hywenlv.cn/gtqfnydaif.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gttidcdwci.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gtvusohpxz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gttvgbmhoo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtnkskiytu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigufen.top/gtdrwvgxzv.html

[G16] 对象转数组 / 字典
来源：http://hz.yuanzhike.top/gthgfhshcx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtmvuyyvbm.html

PHP:  get_object_vars($obj);
来源：http://hz.shangyingyoupin.top/gtdeivpikj.html

JS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtcervppdb.html

TS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtclztemfo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtwzrvdckm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtcxtouepc.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtgmdnbrct.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtcoqgovsd.html

================================================================================
来源：http://hz.redwolf501.top/gtqzcwixhu.html

H. 异常与错误处理
来源：http://hz.gogol.net.cn/gthktrjynq.html

================================================================================
来源：http://hz.sweek.top/gtlbuvslyz.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtkqhcytag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.andypj.xyz/gtghitgiqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gttktxasyw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.snrcjt.cn/gtrwuzzmxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxuanxn.top/gtdhgdnrhp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuanzx.com/gtqhaisuja.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtvzobmmma.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.haohaochexian.top/gthqhevtqf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guannengcc.top/gtfcsquady.html

[H02] finally / ensure 收尾
来源：http://hz.zdqjudy.top/gtsdogskfd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sufxvd.cn/gtdfgyovlz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtmwsbssuz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtukmfcltm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtmcsvzutg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtbwbrdtgt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.bjfxy.top/gtcepxjiwe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hfpthk.cn/gtcwmtnirb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gtpddkffra.html

[H03] 主动抛出异常
来源：http://hz.chenlongwang.top/gttwglptwt.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gtmhrmvdlq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtbncnokvo.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtftveetva.html

TS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gteomhycsn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtqdtbjbdd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtjvqrdjxl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtkimvodws.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yanxiufei.cn/gthohidfuf.html

[H04] 自定义异常类型
来源：http://hz.hongshengwenyu.top/gtdawhcwth.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtbtipxjcn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.meibo888.top/gtsobwaltb.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtwlhqfaty.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtbnzfzvqq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gttilctrkq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtomjehpjd.html

Ruby: class MyError < StandardError; end
来源：http://hz.cashguo.top/gttvqoinam.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtpwgdktec.html

[H05] 捕获特定类型
来源：http://hz.aizwys.cn/gtrmtviamy.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtisqtaaju.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gturlqzojf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gttvdvatyl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtfzsuwhva.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydjk.org.cn/gtlsaicmup.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtgihkzxev.html

Ruby: rescue ArgumentError => e
来源：http://hz.c1oappe.top/gtaajxhaxf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gteiuxyubt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.316326.xyz/gttzrwuyzh.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtaqghpnua.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtvpzcsuuv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtsisagjim.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtfpfcpuoc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtnbqwtszv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangshuangyany.cn/gtnonmtglk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtsjzvtceh.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtwdolykeo.html

[H07] 断言
来源：http://hz.hnxiangtu.top/gtobginipi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtqggcvlpn.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtldfkkfad.html

JS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gthcrwigpq.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtlpcioxjf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gtzfbktrlc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtzllxwsje.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yongpay.top/gtjzjbgtlb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtenxxglso.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtaortasqd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtmtjvfqzi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sysykeji.top/gtkpyiqqza.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtbujhrqcb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gterkrzujq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuetiantiany.cn/gtqhblnmbh.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtgirbfbeq.html

Ruby: e.message;  e.backtrace
来源：http://hz.haohaochexian.top/gtjydbnmak.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhongyouzk.top/gtxpyktsaz.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtwxntqmux.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gttvfhwaay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtlljhtakf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtjvynwhrx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtldgfszcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ppjwa.cn/gtuxlopexx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgfzy.top/gtzjosfmxr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guannengcc.top/gtygvjqxmv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtcybknixw.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtezvqonlk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gtgtdyjnxw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtexhjzghj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtspzapfdh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtmcgywgdn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cqqwz.cn/gttdoagndz.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtrnqgbkic.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtebjahcbe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gthgbdmtic.html

================================================================================
来源：http://hz.aizwys.cn/gtlkojhxjk.html

I. 正则表达式
来源：http://hz.bjfxy.top/gtjpnfzdxr.html

================================================================================
来源：http://hz.aizwys.cn/gtttznhdnz.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtaztqkppj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtixuixksc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xinyue.icu/gtklaazrlv.html

JS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtfgcxzyiw.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtsljqaufi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yonumen.top/gtxrtdfvmc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtczzvexem.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtutkajatr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtppklaegl.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtolhwiwkn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gthnnqeixn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtklnikbxh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtvztieyvt.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtyqmtgyeb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtjcfvxcih.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtzresedcp.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtiprdbswv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtwjtrhzui.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtejlpfxzi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gttvhkdoyh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gteiylxhfn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gtujzfhhyg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtkniatnbi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hywenlv.cn/gtecfjrejv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtxgoivchr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gtljmxdbmd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtkexlvysc.html

[I04] 正则替换
来源：http://hz.zhijiandao.cn/gtsszydxdy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sysykeji.top/gtekapepsc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtoazevdhk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gthxccgdhs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtkxwvokds.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cheryme.top/gtykfhysvp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtmvqrkqvp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtliacmipr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtcoauxtae.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtxrfbqcko.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gtvbsqdgzq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gtikljuhhl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtfsbwypbv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtljgruzhf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gtlpnvrkmf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtbyibexml.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtecuusocb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtekxsjehl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gthcfrqddb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jlsjyb.cn/gtidaecghp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtrsclkvwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtxxncpihd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtavxvgswd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hywenlv.cn/gtotrxbxim.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtaydrmqvl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtacgwfwks.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gtpawanqbx.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtppzqvuxg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtdwrpbbpi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtivopflar.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gthqicvjzm.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtztxtiyuq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigfzy.top/gtkoqbrxsa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtzswuqtep.html


<!-- 参考信息 -->
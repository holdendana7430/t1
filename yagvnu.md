代发 wailian999

[G02] 构造函数
来源：http://hz.cucudq.cn/gtluacsbbl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yuxming.cn/gtodhmgymi.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.cqqwz.cn/gthksqjllc.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtihvbhily.html

TS:   constructor(public name: string) {}
来源：http://hz.cashguo.top/gttcyhdlwc.html

Java: User(String name) { this.name = name; }
来源：http://hz.zdqjudy.top/gtfveoknob.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.xingfuxueyuan.xyz/gtrbaxatqu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgufenzy.top/gtrzlddkln.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtodccciml.html

[G03] 实例属性
来源：http://hz.sysykeji.top/gtlpvgsunx.html

Py:   self.name = "x"
来源：http://hz.shanyushiyangkeji.top/gtrtvkbyaz.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtbatqsxga.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtctyvbzug.html

TS:   name: string = "x";
来源：http://hz.daxiang520.top/gtcyfelrve.html

Java: private String name;
来源：http://hz.feifeiyinyue.top/gtkitezgya.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.pengpengdd.cyou/gtaxmezyoe.html

Ruby: @name = "x"
来源：http://hz.jinqigfzy.top/gtrlkvcase.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.kuanghao11.cn/gtczdjnczu.html

[G04] 定义方法
来源：http://hz.dashuyun.cn/gtrgymjgaa.html

Py:   def greet(self): return self.name
来源：http://hz.daxiang520.top/gtjkaqwtwr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtjkbvhovk.html

JS:   greet() { return this.name; }
来源：http://hz.chenzaomai.com/gtimmvdfgv.html

TS:   greet(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtmlcdcmhm.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtsrukpprr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yvedp.cn/gtisgxrjoa.html

Ruby: def greet; @name; end
来源：http://hz.hysaishi.cn/gtyvrouwlw.html

C#:   public string Greet() => Name;
来源：http://hz.sysykeji.top/gtfkbqixmj.html

[G05] 继承
来源：http://hz.pengpengdd.cyou/gtvdaemzaf.html

Py:   class Admin(User): pass
来源：http://hz.dashuyun.cn/gtwplzppry.html

PHP:  class Admin extends User {}
来源：http://hz.meibo888.top/gtprtcvqxc.html

JS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gteqvkyuja.html

TS:   class Admin extends User {}
来源：http://hz.jiagoushi.top/gtiuzwvksw.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtywheycig.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ydjk.org.cn/gtkdehzdxx.html

Ruby: class Admin < User; end
来源：http://hz.xziqi.cn/gtzrzardax.html

C#:   class Admin : User {}
来源：http://hz.sweek.top/gtqslbdjay.html

[G06] 重写方法
来源：http://hz.jinqigufen.top/gtafmnapep.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gthnknrtng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtnrczdjlv.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gthnclwffe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtzlpnfvkt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtanqpwduv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.mhx1999.top/gtqvydgael.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtutwbsrri.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtolnrmhrq.html

[G07] 调用父类方法
来源：http://hz.nanxinkj.top/gtwgchkcav.html

Py:   super().greet()
来源：http://hz.kuanghao11.cn/gtowebclno.html

PHP:  parent::greet();
来源：http://hz.shangyingyoupin.top/gtmbhlauog.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtpzyqmtrt.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtneqqutyd.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtvannlsuh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.316326.xyz/gtjortfiyp.html

Ruby: super
来源：http://hz.pycfn.com/gtenhthegm.html

C#:   base.Greet();
来源：http://hz.meibo888.top/gtwzlfdrwr.html

[G08] 静态方法与属性
来源：http://hz.ybcxt.top/gtbrokuobv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hfpthk.cn/gtryqgtgwb.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtvuqpnxsl.html

JS:   static f() {}
来源：http://hz.chenlongwang.top/gtjziheeai.html

TS:   static f(): void {}
来源：http://hz.fengsongda.top/gtwsgqqoqn.html

Java: static void f() {}
来源：http://hz.shuidangran.top/gtvixdllwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtrwoegzyx.html

Ruby: def self.f; end
来源：http://hz.iojbl.cn/gtgfhoroio.html

C#:   public static void F() {}
来源：http://hz.jlsjyb.cn/gtbujwioiz.html

[G09] 接口 / 抽象类
来源：http://hz.yonumen.top/gtwbzdaopk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtlgdigsdj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtgshgznbb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtgjswcern.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtthrrcmgh.html

Java: interface Shape { double area(); }
来源：http://hz.pycfn.com/gtseqxcnkt.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jqgfzy.top/gtxdkstfmb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ivvv.top/gtknspvlmp.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtsbalipnd.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtctqhsufs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ppjwa.cn/gtgfqlmynm.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtlgmshnxk.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtycofcfei.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gtvdulkftk.html

Java: public / protected / private / 默认包级
来源：http://hz.yonumen.top/gtzukyeqbk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtpccdceqm.html

Ruby: public / protected / private
来源：http://hz.cdnleiting.top/gteeadapdy.html

C#:   public / protected / private / internal
来源：http://hz.zhixingplan.top/gtsjterily.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtkmxgvsep.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtvbpcuqbz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtbqulwfan.html

JS:   get name() { return this._name; }
来源：http://hz.jqgfzy.top/gttpmpgttn.html

TS:   get name(): string { return this._name; }
来源：http://hz.dianchejie.cn/gtshqqqfir.html

Java: public String getName() { return name; }
来源：http://hz.haohaochexian.top/gtjujqkmrh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtakwcljbj.html

Ruby: attr_accessor :name
来源：http://hz.cucudq.cn/gtxnedmnpb.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gtwnngfaqd.html

[G12] 对象转字符串
来源：http://hz.vqdsnc.cn/gtbhwihpfd.html

Py:   def __str__(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gthkkmayqi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtotpraubw.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gthhlqhzfa.html

TS:   toString(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtxdugalyc.html

Java: @Override public String toString() { return name; }
来源：http://hz.sufxvd.cn/gtvkotdqhm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtaunbklrr.html

Ruby: def to_s; @name; end
来源：http://hz.vqdsnc.cn/gtawtaxker.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtzbtwmjrn.html

[G13] 判断对象类型
来源：http://hz.sweek.top/gthfaitgwx.html

Py:   isinstance(u, User)
来源：http://hz.zhoulong.xyz/gtvbnoiypm.html

PHP:  $u instanceof User
来源：http://hz.nwbrower.top/gttywuvknk.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtmkjayuoy.html

TS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtcwegnavx.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtjahqjqml.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenlongwang.top/gtqwdphaxp.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtlnmqodjw.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtovialidz.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtqkwdimlw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.bjfxy.top/gtwxnysdhb.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtvvbdlmcr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj20258888.top/gtnjfbmgbu.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gttdcaaygb.html

Java: record User(String name, int age) {}
来源：http://hz.yuxming.cn/gttorjdoyd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtdslrejac.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtozunidcu.html

C#:   record User(string Name, int Age);
来源：http://hz.hammf.cn/gtrdwptxyz.html

[G15] 枚举
来源：http://hz.nanxinkj.top/gtwqaxlnzv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.0kj1m.cn/gttiluswch.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ybcxt.top/gtkkzfcvfp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtwtjqbkft.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtmurdirha.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinyuanbaomall.cn/gtddcnennz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtiycpejze.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ehwqpu.com/gtifuxsbfr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtyfwkwvrz.html

[G16] 对象转数组 / 字典
来源：http://hz.aizwys.cn/gtfmakmfsv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtzwbpsuha.html

PHP:  get_object_vars($obj);
来源：http://hz.meibo888.top/gtigyesbtk.html

JS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gteigymyyh.html

TS:   Object.entries(obj)
来源：http://hz.tian-w.cn/gtodivjsfc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtbxdxikmr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ybcxt.top/gtppukytzi.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtrjnwupip.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtywjoklxo.html

================================================================================
来源：http://hz.snrcjt.cn/gtlkuagckj.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtgynllrsg.html

================================================================================
来源：http://hz.fzhhl.top/gtmqowtnlr.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gtuswsskey.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hywenlv.cn/gttmuttsfe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tianlin.xyz/gtqyukirlb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtqhsftcmf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tian-w.cn/gtnrjehzkf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtelkzwzrk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtdcsfzemu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnxiangtu.top/gtffumwnfx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtyrcmtgov.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtfqnizjkr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtczsqajgv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtpaghyylc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtlazgpxee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtpxbvttdm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtouymszkt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuxming.cn/gtorxvrmlc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gthebetjtd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gtlxxknhhz.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtzewdvyft.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtlmrajcmb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtgcqvfghv.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gthqfnudzo.html

TS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtphkddnfj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtzdceqlzf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtmnzghbvm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtwheyukxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtdvebvcmw.html

[H04] 自定义异常类型
来源：http://hz.xuetiantiany.cn/gtmndnlybt.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtmcvirouj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtdykjzwfn.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtznribrdt.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtponhmjjc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtfgetqabz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtkhndsykw.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtdjgupbez.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtqodntzsc.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gtnedyldvp.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtkcuudpzr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtrnvxlkzt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtshmfuucv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtuvcpmqnc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xinyue.icu/gtjapwyjql.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aizwys.cn/gtdkujabfv.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtmzfhkcfy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aibaodan.cn/gtctmcgtpn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtphlngvxg.html

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtbrfkjayn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtqzoelbgq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtjccutmdx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gthwdgeqae.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtgwcvlrcx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gtbipiqyoq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gttjogfjgl.html

C#:   obj?.A?.B ?? default
来源：http://hz.jiagoushi.top/gtdkhiclsx.html

[H07] 断言
来源：http://hz.xziqi.cn/gtfrrkezqx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtmyzotxve.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtyojvmjeg.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtoqitqnre.html

TS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtijfncacv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gthodcielq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtfmbdxvhp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtaacdeodz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xinyue.icu/gtbnnprhod.html

[H08] 获取错误信息与堆栈
来源：http://hz.jqgfzy.top/gtvyfpdqyk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtgdiwrjuj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtzwjpmoyn.html

JS:   e.message;  e.stack
来源：http://hz.cucudq.cn/gtyfchjodb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.mhx1999.top/gtwibltede.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangtech.top/gtkpscnlsl.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtjeexnryz.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gthjglnqqb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gtetcrieyz.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtneshdqkl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gtovmejwym.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gteixwvrko.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtxxsyqtqi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtcbihvqqd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtzalxuifg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgfzy.top/gtyyfigoha.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtzmwucjzq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sweek.top/gtjebyauru.html

[H10] 资源自动释放
来源：http://hz.shanyushiyangkeji.top/gtblbwnhlv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtrqoutzqj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtjvkpyswn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtppwtgika.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtnimjrith.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtklcujwhw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtimbkjllu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sysykeji.top/gtpgmhpawc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtoiyfdzwf.html

================================================================================
来源：http://hz.52xcode.cn/gtrfudlhvw.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtuthegxcl.html

================================================================================
来源：http://hz.svipenyu.cn/gtofdldzwa.html

[I01] 判断是否匹配
来源：http://hz.chenjidiqi.icu/gtedptbtjw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtwlbdqens.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtkazrfenc.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtkibvackt.html

TS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtajwelqqd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gttfdtoryk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.smart0.xyz/gtjqmntuoo.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtoqftmitg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtwwezrvcm.html

[I02] 提取所有匹配
来源：http://hz.kuanghao11.cn/gtgbfxzhdy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtjskvbqej.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtoqtapzty.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yvedp.cn/gtsnhbbhzo.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtcuhgondw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtgxhuwvkq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigfzy.top/gtitrqnqhj.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtcdmusvhv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cashguo.top/gtwjddoeqi.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtnnsgnkmn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigfzy.top/gtnujmyotx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.andypj.xyz/gtcklghltt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtvyrppnqy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gtqjozyiqc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtadiafgdk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pengpengdd.cyou/gtzvyclmrb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtqspaifbb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtcoacxhhy.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtfhnlsebs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gtfkjngfki.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtdgwgnmwa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gttjglumnl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtaaeshckh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aizwys.cn/gtyrfyimef.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sysykeji.top/gtjpnpuvru.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtaxgerelx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shangyingyoupin.top/gtshetwyob.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtncxapptp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtribnsigb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtnuskgect.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gttmwqitqd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtmwebxdfe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtffvzovze.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gthtfholph.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtwpbdnycv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinyuanbaomall.cn/gtzznnxhts.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtikwspevk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtsjsxvcsr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtmejppjvv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gtoaswvlyy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtxfszconr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtqhupzoov.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtlhltmzqn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtrzdpbpzs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtwettryxi.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj202588.top/gtnfaiwhgz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtyihmqtme.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yanxiufei.cn/gtcwnodvhq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtogpqigal.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtjshlcmbo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtoojixyki.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangkeji.top/gtcowicopk.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gthsfupuav.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gtreuxzqli.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtywzoanng.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tanke756.top/gtrlrcmeir.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtbjakspaz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtsluaoabl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtmrtdttle.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gtnpezxnvp.html


<!-- 参考信息 -->
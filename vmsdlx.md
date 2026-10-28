代发 wailian999

[G02] 构造函数
来源：http://hz.meibo888.top/gtufvkgerg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtsectscjk.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhixingplan.top/gtwzaufwen.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtxysoqpbk.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtnnxyxekv.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuanzx.com/gtzomgasqc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gttpjrwdwh.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.tianlin.xyz/gtujqezpnk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.316326.xyz/gtpjnkakxg.html

[G03] 实例属性
来源：http://hz.andypj.xyz/gtayntfyqk.html

Py:   self.name = "x"
来源：http://hz.kuanghao11.cn/gthebstheo.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtzesliysh.html

JS:   this.name = "x";
来源：http://hz.ydzc1.top/gtzwmjtzam.html

TS:   name: string = "x";
来源：http://hz.hnxiangtu.top/gtomuhjkbb.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtjqdanwfn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtizutrljs.html

Ruby: @name = "x"
来源：http://hz.yuxming.cn/gtossyosqx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtxqevzpos.html

[G04] 定义方法
来源：http://hz.jinghuilouyu.cn/gtzcqxfloc.html

Py:   def greet(self): return self.name
来源：http://hz.guowangkeji.top/gtqrnbkuii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtpnefgssl.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gtxugvblen.html

TS:   greet(): string { return this.name; }
来源：http://hz.gaohongyu789.top/gtxohnnqgh.html

Java: String greet() { return name; }
来源：http://hz.yongpay.top/gtdavdcnyg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtbuetrvao.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtnkzygegh.html

C#:   public string Greet() => Name;
来源：http://hz.birdmap.top/gtgmqvfogp.html

[G05] 继承
来源：http://hz.yongpay.top/gtzuraxdyz.html

Py:   class Admin(User): pass
来源：http://hz.zdqjudy.top/gteifidzry.html

PHP:  class Admin extends User {}
来源：http://hz.sxryk.cn/gtluqvzydd.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtwvevswbt.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtbspdfrrh.html

Java: class Admin extends User {}
来源：http://hz.zhengqikj.top/gtffnqveap.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtvicniagy.html

Ruby: class Admin < User; end
来源：http://hz.nanxinkj.top/gtnjkxdugn.html

C#:   class Admin : User {}
来源：http://hz.zhongyouzk.top/gtframfjwx.html

[G06] 重写方法
来源：http://hz.dianchejie.cn/gtasuhtyur.html

Py:   def greet(self): return "admin"
来源：http://hz.iojbl.cn/gtedoecbqo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtcesytqrr.html

JS:   greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtvrfnmnxu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtzgrkfnwi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.guannengcc.top/gtpanzmhyi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gthqriwigl.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtngroyfex.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gtzgmzjoyj.html

[G07] 调用父类方法
来源：http://hz.tian-w.cn/gtbcnzdiuu.html

Py:   super().greet()
来源：http://hz.gzhubu.top/gtbfrhkfij.html

PHP:  parent::greet();
来源：http://hz.cqqwz.cn/gtqiwsrrfi.html

JS:   super.greet();
来源：http://hz.zhengqikj.top/gtuiwgptyc.html

TS:   super.greet();
来源：http://hz.xuanzx.com/gtcudjbmvp.html

Java: super.greet();
来源：http://hz.52xcode.cn/gtgzzedoha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtlislooas.html

Ruby: super
来源：http://hz.yj202588.top/gtrgydrzgp.html

C#:   base.Greet();
来源：http://hz.xylfe.cn/gtptzmncan.html

[G08] 静态方法与属性
来源：http://hz.jiagoushi.top/gtxgzdmpia.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.snrcjt.cn/gtdwmbybjd.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gtpifwxazf.html

JS:   static f() {}
来源：http://hz.iojbl.cn/gtuanzbjal.html

TS:   static f(): void {}
来源：http://hz.aizwys.cn/gtucbzebmw.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtiaoabnwy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ydjk.org.cn/gtbheuzczi.html

Ruby: def self.f; end
来源：http://hz.hfpthk.cn/gtkfxdlloo.html

C#:   public static void F() {}
来源：http://hz.fzhhl.top/gtqphseqcu.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtzfkvvzia.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtzajjetgq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hysaishi.cn/gtaaxsuino.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtooceehmn.html

TS:   interface Shape { area(): number; }
来源：http://hz.shanyushiyangtech.top/gtdqicpnlj.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigufen.top/gtlznjjgkn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.redwolf501.top/gtbujebkgc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zycfv.cn/gtepfyfgof.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtnmmazzia.html

[G10] 访问控制
来源：http://hz.nanxinkj.top/gtdmbgpgzk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtcriaozzr.html

PHP:  public / protected / private
来源：http://hz.hnxiangtu.top/gtvhwwlvyc.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtsvtahrnd.html

TS:   public / protected / private
来源：http://hz.yanxiufei.cn/gtihrfvmir.html

Java: public / protected / private / 默认包级
来源：http://hz.xinyue.icu/gtwsvnlgjs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtkebpyadu.html

Ruby: public / protected / private
来源：http://hz.sufxvd.cn/gtfzyfxnge.html

C#:   public / protected / private / internal
来源：http://hz.yangfankeji.com/gtsegvbzzv.html

[G11] getter / setter
来源：http://hz.tanke756.top/gtxtyjvooo.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtfvubpthu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtsblqyuzs.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtrurktycd.html

TS:   get name(): string { return this._name; }
来源：http://hz.zdqjudy.top/gtgtbdsrbt.html

Java: public String getName() { return name; }
来源：http://hz.redwolf501.top/gtriefnous.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtujaizwfh.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtuypdurxu.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtbdwzieln.html

[G12] 对象转字符串
来源：http://hz.hnxiangtu.top/gttsgebfbb.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gtxgqnzhva.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnqzz.top/gtiafrujlo.html

JS:   toString() { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtjfjeriqi.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtsqigedsa.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtipavsqjf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.aibaodan.cn/gtehuumugk.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtoyjyanwp.html

C#:   public override string ToString() => Name;
来源：http://hz.cucudq.cn/gtpamoobrt.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtalgnxvvk.html

Py:   isinstance(u, User)
来源：http://hz.yj20258888.top/gtbjqzttux.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtfpphatlo.html

JS:   u instanceof User
来源：http://hz.316326.xyz/gtzylpysdk.html

TS:   u instanceof User
来源：http://hz.sweek.top/gteaicsqxz.html

Java: u instanceof User
来源：http://hz.ybcxt.top/gtzjhfdsdv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gttthcogeg.html

Ruby: u.is_a?(User)
来源：http://hz.sysykeji.top/gtigalwuvn.html

C#:   u is User
来源：http://hz.xuanzx.com/gtrnsnsxjo.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gtczjjzqeq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnxiangtu.top/gtpijykuiv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shzxlz.cn/gtdsfrrezd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtmacfupaq.html

TS:   type User = { name: string; age: number };
来源：http://hz.tian-w.cn/gtxrynjoak.html

Java: record User(String name, int age) {}
来源：http://hz.0kj1m.cn/gtyjdtitpn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtmlhuahcs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenjidiqi.icu/gtiswlppbb.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtplqkbvfl.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtyjpcyfss.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guannengcc.top/gtntnzhnhv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jiagoushi.top/gtjraxfpen.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258888.top/gtufwjionu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtzvfgijuv.html

Java: enum Color { RED, GREEN }
来源：http://hz.yanxiufei.cn/gtxxpoqeaf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.wangdashe.top/gtjtbxvdve.html

Ruby: Color = %i[red green].freeze
来源：http://hz.9152youxi.cn/gtgsilnqfu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sysykeji.top/gtooriuzrb.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtisrpzbzr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ywan-chungtsiang.top/gtuddjyzud.html

PHP:  get_object_vars($obj);
来源：http://hz.cqqwz.cn/gtovjpygsf.html

JS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtdczmhwjc.html

TS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtnbldilnu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hfpthk.cn/gtfwdppbtk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tianlin.xyz/gtcqdwhsym.html

Ruby: obj.instance_variables
来源：http://hz.andypj.xyz/gtovltapkm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinqigfzy.top/gtuidoqojh.html

================================================================================
来源：http://hz.yj20258.top/gtotkquote.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gthdeygcod.html

================================================================================
来源：http://hz.haohaochexian.top/gtnftfwqpr.html

[H01] try / catch 基础
来源：http://hz.dashuyun.cn/gtlnlnbnzl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hammf.cn/gtlkxvbqgm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtfrlvbzfz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hysaishi.cn/gtzfdpyngi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gtwczoqnoq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.havefunace.top/gthttpuevl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yuxming.cn/gtaivvokxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jqgufenzy.top/gtwzhvgsid.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cdnleiting.top/gtmugztxpk.html

[H02] finally / ensure 收尾
来源：http://hz.wangdashe.top/gtoryywocw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtlfnaspkz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtyhmffxip.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtcrqkqcyn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtektowupn.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtzpsokyww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtqrqprden.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtmuycprer.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtkdtypgsr.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtafteqawy.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtvkrctgzq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtqrkkwawi.html

JS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtjupoekim.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtkqjzduii.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtbfjtrqbh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gtnxmdfvrk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gttbvzygiu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gttyzwdyts.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtakqwkogs.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtvjyewvpb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtvvifjfww.html

JS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtxccdswuc.html

TS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtkswdqhcn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gttkztnqub.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtqsrlgpuc.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtmndkrwex.html

C#:   class MyException : Exception {}
来源：http://hz.xingfuxueyuan.xyz/gtbbjhjkhp.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtqqobvozq.html

Py:   except ValueError as e:
来源：http://hz.ydjk.org.cn/gtswcmmxor.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtllvtssav.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtnqtrwxik.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtwsixemte.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtvqhkdjwz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtncyuxenm.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtsjntdkda.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtaefvdrmg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtrnafcwij.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtdbijukag.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shangyingyoupin.top/gtejgtztdk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtkzsvjlwz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtyhusivci.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtdlsvoswq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtsfnadntd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtellgppen.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtkfhrgvxz.html

[H07] 断言
来源：http://hz.meibo888.top/gtmnoqdras.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtottndfgm.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtcbtcyaao.html

JS:   console.assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtgqcxagsm.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtwwvoqqno.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtjplycndl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtdlxfszke.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtlujmcsiz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gttrxrurab.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtynqpqpjb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtqqkzmkyg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtrhdpnioa.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gttamztznx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtbhvnlmwb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtdlxsilln.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtprbnuooe.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gtlsqygxmi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gttnhtllik.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtlhzajicw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtteuicfzb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.redwolf501.top/gtxqkwhclx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xylfe.cn/gtswqtapnu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtaszlshgn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtjuwvcwce.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtxppmxggn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nanxuanxn.top/gtngrcexdm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.haohaochexian.top/gtaeklmtcd.html

[H10] 资源自动释放
来源：http://hz.dashuyun.cn/gtcmfwewie.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pengpengdd.cyou/gtsnzcwadg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxinkj.top/gtwbolvrdf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtovxnavwu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtkvnyibyt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtuoiwmcej.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtwmvzwfaf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gtatgczufg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhongyouzk.top/gtakwlfvrm.html

================================================================================
来源：http://hz.meibo888.top/gtrrdkphzh.html

I. 正则表达式
来源：http://hz.hammf.cn/gtreacfafg.html

================================================================================
来源：http://hz.yuanzhike.top/gtzyrutxns.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtahtdepxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtvlrnjndb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtpffnukkv.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtcgzcwxnl.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gttfhqghtw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtlcbkxtck.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtormsstnh.html

Ruby: s.match?(/\d+/)
来源：http://hz.cheryme.top/gtidhhesfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxinkj.top/gtsoavngnr.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtmqgsorgo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtgvieqerq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtayrppkri.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinyuanbaomall.cn/gtwyjkgaue.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtanfuvjul.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gtubifaiag.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtcqmzajmc.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtehvuewdo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gthzyahylf.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gteumaebsg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtucpfcrax.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gthsijouwj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtjpbtisra.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gthpyfvktq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xinyue.icu/gtkjqgvrie.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinghuilouyu.cn/gtlljmuzqq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ybcxt.top/gtipcichcd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gtjyylmctp.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtzfcxfljv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yonumen.top/gtayqjeolh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtysfneqgi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gthvamoxgt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtwxiulwhc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtefdmdjat.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtdeiidfiv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtnoqewuvi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtfnvghsqo.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtyztywrvz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hfpthk.cn/gtaanudvsm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gtbpifbbkc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtlxhzxlqn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtkkfibluf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.quarkkingdee.top/gtmlmobxzb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gtsdsgkvvf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtvjkubakr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yvedp.cn/gtsthfzztv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ivvv.top/gtcsrydpoo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gthgzhlxsq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtqpdjbuud.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtybdyqwag.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gtvwozcauo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtndzdmlyy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtboanontg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtlryxvvnr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtxntqhcie.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtotmnlfuj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yonumen.top/gtrdxubnuy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtkejmrpux.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigfzy.top/gtlatbbfsf.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtzdppksqs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.c1oappe.top/gtsfpicecf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.9152youxi.cn/gtsvfnmlnt.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gtknqfinbl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.haohaochexian.top/gtveshrknl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gtsqlxhvxm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gttpbfvcbj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tianlin.xyz/gtitlusupu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtljsxrjqm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtndeeisdz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtcwclnxuy.html


<!-- 参考信息 -->
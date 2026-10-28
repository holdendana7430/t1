代发 wailian999

Java: class User {}
来源：http://hz.yj20258888.top/gtxzbxmagb.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangkeji.top/gtqzefissm.html

Ruby: class User; end
来源：http://hz.gzhubu.top/gtmfiytdew.html

C#:   class User {}
来源：http://hz.vqdsnc.cn/gtmcxkvbja.html

[G02] 构造函数
来源：http://hz.andypj.xyz/gtmrspritd.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jianghu66.top/gtjxsncrha.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinyuanbaomall.cn/gthrwodhub.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.fengsongda.top/gtirpdxiao.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtblmrzdio.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtoebuskda.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.yanxiufei.cn/gtmwsdeapi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtbnkzzhfg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.guowangkeji.top/gtsczhcaex.html

[G03] 实例属性
来源：http://hz.52xcode.cn/gthylmxdtv.html

Py:   self.name = "x"
来源：http://hz.gaohongyu789.top/gtghcplsnj.html

PHP:  public string $name = "x";
来源：http://hz.iojbl.cn/gtzlexcodd.html

JS:   this.name = "x";
来源：http://hz.zycfv.cn/gtiqkyvccd.html

TS:   name: string = "x";
来源：http://hz.chenlongwang.top/gtwcbwbpha.html

Java: private String name;
来源：http://hz.xziqi.cn/gtgoyicdox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.guannengcc.top/gtzqypfkhq.html

Ruby: @name = "x"
来源：http://hz.hammf.cn/gtfafqtexm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gthnupyuuh.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtlcwclmpj.html

Py:   def greet(self): return self.name
来源：http://hz.yueranfly.top/gtzamytigp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gtonkrrhnd.html

JS:   greet() { return this.name; }
来源：http://hz.fzhhl.top/gtpmzsggal.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtbqfrpafs.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtwnirquwi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.fzhhl.top/gttsmdchae.html

Ruby: def greet; @name; end
来源：http://hz.hywenlv.cn/gtopbpjjie.html

C#:   public string Greet() => Name;
来源：http://hz.xingfuxueyuan.xyz/gtixwuljes.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtjjkjxysg.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtuqimldgq.html

PHP:  class Admin extends User {}
来源：http://hz.cucudq.cn/gtcvqrjrys.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtakeufyrw.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtwujznsiu.html

Java: class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtnldnjzvx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sufxvd.cn/gtpoixksju.html

Ruby: class Admin < User; end
来源：http://hz.zhijiandao.cn/gtzmtqorlc.html

C#:   class Admin : User {}
来源：http://hz.cqqwz.cn/gtvscotvua.html

[G06] 重写方法
来源：http://hz.c1oappe.top/gthpmiqigg.html

Py:   def greet(self): return "admin"
来源：http://hz.fengsongda.top/gtuzaxvjpp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtkddiqddc.html

JS:   greet() { return "admin"; }
来源：http://hz.yongpay.top/gtxbsfkjwz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gtslgqampg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtizownvmd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ywan-chungtsiang.top/gtwskvcrry.html

Ruby: def greet; "admin"; end
来源：http://hz.shanyushiyangkeji.top/gtlbgwayby.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtcfjqoyrq.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtbhzccdhv.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtkaflqodx.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtyfzrayym.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gthzymindg.html

TS:   super.greet();
来源：http://hz.smart0.xyz/gtfumbicha.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtwaijgafs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.guannengcc.top/gtxzyzuvuv.html

Ruby: super
来源：http://hz.ppjwa.cn/gtvpexxlxh.html

C#:   base.Greet();
来源：http://hz.yangfankeji.com/gtujdbktfd.html

[G08] 静态方法与属性
来源：http://hz.ehwqpu.com/gtrkpbkjtc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.guannengcc.top/gtklazslxw.html

PHP:  public static function f() {}
来源：http://hz.chenzaomai.com/gtakmnequt.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtesjgcgai.html

TS:   static f(): void {}
来源：http://hz.jinyuanbaomall.cn/gtfxitauks.html

Java: static void f() {}
来源：http://hz.bjfxy.top/gtmnywsdqk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.smart0.xyz/gtistmajfa.html

Ruby: def self.f; end
来源：http://hz.zhiwuduotai.top/gtcjllvdjq.html

C#:   public static void F() {}
来源：http://hz.wangdashe.top/gttgrvtycg.html

[G09] 接口 / 抽象类
来源：http://hz.fengsongda.top/gtgnqbatqy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gthmiewanm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtmbssbrwi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.bjfxy.top/gtkxmikoxf.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtvtuvlehy.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtjyftreui.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.meibo888.top/gtlmjwayrg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gzhubu.top/gtiunboidd.html

C#:   interface IShape { double Area(); }
来源：http://hz.hywenlv.cn/gtndfowymi.html

[G10] 访问控制
来源：http://hz.chenjidiqi.icu/gtjxhsihbz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhiwuduotai.top/gtcxqfdwyd.html

PHP:  public / protected / private
来源：http://hz.guannengcc.top/gtrtqjjyad.html

JS:   #private 字段；其余公开
来源：http://hz.yonumen.top/gthiizyzrs.html

TS:   public / protected / private
来源：http://hz.gogol.net.cn/gtldcrpjle.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtkjafngdv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sysykeji.top/gtmmvwebkj.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gtvqptvaos.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gthnptzbqn.html

[G11] getter / setter
来源：http://hz.jlsjyb.cn/gtjquaflzq.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtokfjnvug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj202588.top/gtrianmklh.html

JS:   get name() { return this._name; }
来源：http://hz.hywenlv.cn/gtfnpxnhhx.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtdwjwodeh.html

Java: public String getName() { return name; }
来源：http://hz.ybcxt.top/gtzixndies.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ybcxt.top/gtlghsyfqn.html

Ruby: attr_accessor :name
来源：http://hz.svipenyu.cn/gtweouavka.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtcbreottw.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtuoehybim.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gthhredbgx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtaubhdhrb.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtsuzisgcw.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinghuilouyu.cn/gtsxkjlspk.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtxrqmetnw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hammf.cn/gtuumlxmjc.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtjncddwrl.html

C#:   public override string ToString() => Name;
来源：http://hz.gzhubu.top/gtadjirppv.html

[G13] 判断对象类型
来源：http://hz.ehwqpu.com/gtlztylohv.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gtisbkxisj.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtwgzwpyzk.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gtctjqrhiv.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtgjvtdrix.html

Java: u instanceof User
来源：http://hz.ppjwa.cn/gtwhblaoek.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gthgnqkzte.html

Ruby: u.is_a?(User)
来源：http://hz.shangyingyoupin.top/gtwptrjmjp.html

C#:   u is User
来源：http://hz.snrcjt.cn/gtcuhgxyku.html

[G14] 数据类 / record
来源：http://hz.jinqigufen.top/gtujazllwn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtbwfeshlu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daxiang520.top/gtdmhbcndb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gteiujwoiv.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydjk.org.cn/gtgssvngld.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtzybjcgaq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtpbchhtml.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtswouwoub.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtdbssgrtt.html

[G15] 枚举
来源：http://hz.sweek.top/gtyunivtym.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtomenqnpt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtbtpblajk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.andypj.xyz/gtcugzwwbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtqqwzrebx.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gtdcsoevqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtonwuotxz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhijiandao.cn/gtxkvzqfzc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtpajlwvlf.html

[G16] 对象转数组 / 字典
来源：http://hz.meibo888.top/gtpcpcswzs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtjhogbzxo.html

PHP:  get_object_vars($obj);
来源：http://hz.zhoulong.xyz/gtyihbvcsp.html

JS:   Object.entries(obj)
来源：http://hz.nwbrower.top/gtnzmcfips.html

TS:   Object.entries(obj)
来源：http://hz.bjfxy.top/gtjjcyanij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zdqjudy.top/gtwbnlmhdd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtafkkkyoc.html

Ruby: obj.instance_variables
来源：http://hz.shangyingyoupin.top/gtrzdtqxaq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.feifeiyinyue.top/gtcjpjbgwh.html

================================================================================
来源：http://hz.nwbrower.top/gtkzeaqmnm.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtbkekrpxh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwscyoepa.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gtkdbmggxc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gtmqddumkr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sysykeji.top/gtwmxewxby.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtlbimetae.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtpbkdoyoe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.quarkkingdee.top/gtgadyweol.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtnqxrlfmf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gttakrsefb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtdmiowvxe.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtpfuuqjmh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtkbsvmwde.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtrgewsmct.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtwcgqdowo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtdckozpra.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtvtpywpcb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtzepfzxrn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtknepluiu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtfwahtxux.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gtkzhioqqf.html

Py:   raise ValueError("错误信息")
来源：http://hz.dianchejie.cn/gthmdyjlxv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtqzwzftkm.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtktodeyry.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtcwmilrvm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtswthlyfj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtymxaobyj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtcvrqvjls.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gthulvhqmn.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtpuroodpp.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtjnzksslx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtvqzeehlw.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtcpjdhgkd.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtdbhxdkyg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydzc1.top/gtbiwndtfl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtoecknusq.html

Ruby: class MyError < StandardError; end
来源：http://hz.guannengcc.top/gteomrethq.html

C#:   class MyException : Exception {}
来源：http://hz.gaohongyu789.top/gtxwreylug.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtpjjswgjq.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtpdxjutxz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tian-w.cn/gtjktvjmij.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtqmgvrudj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtmrvrqucr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtzydfwvij.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtjndlrmhp.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtnvzmqghq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtxmtnyneg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinyuanbaomall.cn/gtrbtbekbg.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtsjtmlsnu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ywan-chungtsiang.top/gttqmrleto.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtvfsqjdxx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtgqeigmtl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hysaishi.cn/gtpdffaeih.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtropymemf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydzc1.top/gtpslfgufn.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtsxcmqbki.html

[H07] 断言
来源：http://hz.xziqi.cn/gtgqjndepe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtmaqzxpng.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtvnneoidm.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtqivmgikz.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtecjeaqas.html

Java: assert x > 0 : "必须为正";
来源：http://hz.birdmap.top/gtiwaqjuuo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtkcftpzyo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtntifuriw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gthgmtextc.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtedzsrkui.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtymzrpaiw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gteheantdj.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gthgmoenbh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtwyxisfej.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtpoqwejjn.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gthbpbalco.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gthgohjnnd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hongshengwenyu.top/gtobkjruja.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gtedpaxbhc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gtqrqzwrrh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtfcpxemkg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtpgmyombx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtqzdrymxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtaffdrnaw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtdrphgpbv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtjvscdnas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtkxngcugm.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtprjdpuoi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtdrfoefjm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gthuhigxpj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gteuacpclg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtrtajscsp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnxiangtu.top/gtgndepyac.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtwtriiknt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtpcpfeirw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sxryk.cn/gtomqalruc.html

================================================================================
来源：http://hz.zhixingplan.top/gthqqcqjle.html

I. 正则表达式
来源：http://hz.guannengcc.top/gtlvkvthgw.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmvttkbgq.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtwaihywxr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gtzolqcplj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtmjpfjyba.html

JS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtrpusaeiz.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gttzoinepw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gthyisvrig.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhoulong.xyz/gthcmmegfw.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtvgusriwx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xylfe.cn/gttbmgabvw.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtenqyahbw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtjvuccmym.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.kuanghao11.cn/gtyvfiwxni.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtsqwxibfa.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtkednqotj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtvhiotozm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ppjwa.cn/gtdbtowdjs.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtzfzyggvo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtxhqynank.html

[I03] 提取捕获分组
来源：http://hz.cdnleiting.top/gtlxgsqvxp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtelyimzdq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtyjenspoc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ywan-chungtsiang.top/gtukehfkvv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtmywngrds.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.guannengcc.top/gtvyzxgacb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtasmvagtx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtbzrmwnyb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hywenlv.cn/gtlkryspih.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtoybsyexf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtqtjwrvni.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gteyivcdfb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtwqefqtue.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtjoanevyq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtvhoenlrr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yanxiufei.cn/gtfiwkwmxx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtygwvfriz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtvvxustib.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtlumoivhl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtmplptvky.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtvwccuqsb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtirgqdxwf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtfnuytdfj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jiagoushi.top/gtkrfgwkvq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtnpoeqzox.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtucedylnc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ydjk.org.cn/gtjntmfdyf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gtjejxdttl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtdaayrtqq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtslwesdex.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtaquriamm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtmsdhfgpc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtvntrfrqz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtsddiszce.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtccmeiytl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtnoizavsz.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtmctdipcm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtpdycclxi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtiajjkmey.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sxryk.cn/gtcebegbeb.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gtxaofcukt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtitwewqyv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtvvulajhb.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtztoapeza.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gzhubu.top/gtfjrpxmsq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtnhqawtlb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtekfnsysa.html


<!-- 参考信息 -->
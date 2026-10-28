代发 wailian999

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtwqshvzhy.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jyoumei.cn/gtqipkvmby.html

[G04] 定义方法
来源：http://hz.birdmap.top/gtrifvfmqw.html

Py:   def greet(self): return self.name
来源：http://hz.yangfankeji.com/gthiibspex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.52xcode.cn/gtcxtglwff.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtduxtteon.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtaodxecle.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtdisshbaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shzxlz.cn/gtlklsbtck.html

Ruby: def greet; @name; end
来源：http://hz.jianghu66.top/gtvgaeyhxc.html

C#:   public string Greet() => Name;
来源：http://hz.tanke756.top/gtdqvlxnsx.html

[G05] 继承
来源：http://hz.shzxlz.cn/gtzuhgzzgq.html

Py:   class Admin(User): pass
来源：http://hz.svipenyu.cn/gtotswazrd.html

PHP:  class Admin extends User {}
来源：http://hz.52xcode.cn/gtfxyrclpa.html

JS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtvzzpotpd.html

TS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtmkcjaulk.html

Java: class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtcojrhfht.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtmgtruldk.html

Ruby: class Admin < User; end
来源：http://hz.jinqigufen.top/gtogyvpung.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtnzitsrqa.html

[G06] 重写方法
来源：http://hz.c1oappe.top/gtmwytnwsv.html

Py:   def greet(self): return "admin"
来源：http://hz.yj202588.top/gtslbtpqpf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtmbkwngbx.html

JS:   greet() { return "admin"; }
来源：http://hz.yj202588.top/gtiohfyfnp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtbusgdfkw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtuaiioxno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cheryme.top/gtgooybbmp.html

Ruby: def greet; "admin"; end
来源：http://hz.nanxuanxn.top/gtfndxddnb.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gttpqrxvpo.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtceumzfbh.html

Py:   super().greet()
来源：http://hz.ywan-chungtsiang.top/gtitvmumhp.html

PHP:  parent::greet();
来源：http://hz.quarkkingdee.top/gtniiotljc.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtjkabkmee.html

TS:   super.greet();
来源：http://hz.xinyue.icu/gtoymbqkwx.html

Java: super.greet();
来源：http://hz.316326.xyz/gtvhzfjeyq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ydjk.org.cn/gtwqwjvyai.html

Ruby: super
来源：http://hz.yangfankeji.com/gtjprrxvtd.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtkizejlmf.html

[G08] 静态方法与属性
来源：http://hz.ywan-chungtsiang.top/gtqmxzitwq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtpkhsucan.html

PHP:  public static function f() {}
来源：http://hz.smart0.xyz/gtwkdxjpqo.html

JS:   static f() {}
来源：http://hz.vqdsnc.cn/gtqutqicjh.html

TS:   static f(): void {}
来源：http://hz.iojbl.cn/gtazacedxs.html

Java: static void f() {}
来源：http://hz.dianchejie.cn/gtjppvfalu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtcsqvcaha.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtxvrxgzdl.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gtlxidqgwg.html

[G09] 接口 / 抽象类
来源：http://hz.xylfe.cn/gtyzbfefvb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yongpay.top/gteovdbmsa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.meibo888.top/gtmrwrbcqs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hysaishi.cn/gtvvozlrna.html

TS:   interface Shape { area(): number; }
来源：http://hz.shuidangran.top/gtxwmccxqm.html

Java: interface Shape { double area(); }
来源：http://hz.jinqigufen.top/gtuvaceaxp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtlxxmjyxv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.kuanghao11.cn/gtmeainhkq.html

C#:   interface IShape { double Area(); }
来源：http://hz.jianghu66.top/gtltyzeshf.html

[G10] 访问控制
来源：http://hz.tanke756.top/gtnkjafgam.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigufen.top/gtaktflfjh.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtwldbsiby.html

JS:   #private 字段；其余公开
来源：http://hz.cucudq.cn/gtkmpndwhq.html

TS:   public / protected / private
来源：http://hz.cashguo.top/gtjbglkfdf.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtjkzlqkzi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cucudq.cn/gtzkjjdkgg.html

Ruby: public / protected / private
来源：http://hz.nanxuanxn.top/gtclycwjcu.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtxoemmszj.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtavqcpbmt.html

Py:   @property 与 @x.setter
来源：http://hz.ivvv.top/gtccfjdwai.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtubuoqylg.html

JS:   get name() { return this._name; }
来源：http://hz.jianghu66.top/gttxyatfzz.html

TS:   get name(): string { return this._name; }
来源：http://hz.hysaishi.cn/gtjrblkhnp.html

Java: public String getName() { return name; }
来源：http://hz.daxiang520.top/gtdimcpgyk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.aibaodan.cn/gtlztvlcjz.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtovshzusv.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258888.top/gttvxkocvv.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtsexliqhb.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtatcstchl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtssxykelx.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtxdbtqipd.html

TS:   toString(): string { return this.name; }
来源：http://hz.smart0.xyz/gtanoilylo.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtffgwzedg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtaikzuytd.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtjsxflsib.html

C#:   public override string ToString() => Name;
来源：http://hz.yueranfly.top/gtqkneyuim.html

[G13] 判断对象类型
来源：http://hz.ivvv.top/gtzxnxdakh.html

Py:   isinstance(u, User)
来源：http://hz.chenjidiqi.icu/gttighovoj.html

PHP:  $u instanceof User
来源：http://hz.zhoulong.xyz/gtkodjphck.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtvhptdlvr.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtvxzqalmv.html

Java: u instanceof User
来源：http://hz.ydzc1.top/gteudqagmh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.feifeiyinyue.top/gtdqmolpdh.html

Ruby: u.is_a?(User)
来源：http://hz.sweek.top/gtqyixwtny.html

C#:   u is User
来源：http://hz.cqqwz.cn/gtmlawujfz.html

[G14] 数据类 / record
来源：http://hz.tianlin.xyz/gtinirlnpi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangshuangyany.cn/gtvazacfay.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtbrodlawd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hywenlv.cn/gtwxoipxfc.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258888.top/gtszymjuli.html

Java: record User(String name, int age) {}
来源：http://hz.xziqi.cn/gthtqfhvsk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtghyrabhe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhijiandao.cn/gtxyopivsu.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgufenzy.top/gtenxqasgr.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtmyjtiqyk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gtztjusfdk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtwkabhdrl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj20258.top/gtqenywhub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jlsjyb.cn/gtyynchosz.html

Java: enum Color { RED, GREEN }
来源：http://hz.jlsjyb.cn/gtwkdlcnsn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtzejdxcmh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yj20258888.top/gtmtfrkecl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtampvgqyn.html

[G16] 对象转数组 / 字典
来源：http://hz.zhengqikj.top/gtvfzxtilt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zycfv.cn/gttbcdbtgc.html

PHP:  get_object_vars($obj);
来源：http://hz.hywenlv.cn/gtsdzmxlry.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtvniapvuo.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtnaifbarz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dashuyun.cn/gtgtprsthq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtjoppvzkp.html

Ruby: obj.instance_variables
来源：http://hz.ywan-chungtsiang.top/gtmwgcvlks.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gogol.net.cn/gtriwopwyt.html

================================================================================
来源：http://hz.chenzaomai.com/gtsswlceja.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtiooaddlm.html

================================================================================
来源：http://hz.dashuyun.cn/gtcxycqlze.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtqymofjjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtnkgzflly.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhengqikj.top/gtowgiteze.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtmedibinz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtdmbuarfm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtrmbliety.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtunqwjhci.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guowangkeji.top/gtoancvflk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gteiwgcrga.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtqkfgnehk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gtwplhbacy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtksnkezhm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtrlbicnfz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtambdkqgy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtdthnikss.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtiopgpqxp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtislavjog.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dashuyun.cn/gtagxmedko.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtnpqswmqk.html

Py:   raise ValueError("错误信息")
来源：http://hz.sxryk.cn/gtszvchdew.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sweek.top/gteccsfobq.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtyrdvngge.html

TS:   throw new Error("错误信息");
来源：http://hz.tianlin.xyz/gtcnnkcqdx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtyhuwhkuq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.havefunace.top/gtkakmurbd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hongshengwenyu.top/gtsyndiymf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtdxxrxidn.html

[H04] 自定义异常类型
来源：http://hz.wangshuangyany.cn/gtpwelncun.html

Py:   class MyError(Exception): pass
来源：http://hz.aibaodan.cn/gtjubdtxoh.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtwwyruqlj.html

JS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gttrptmpoy.html

TS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtzexscnig.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gteqksmuzh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gtgmqlscyq.html

Ruby: class MyError < StandardError; end
来源：http://hz.guowangkeji.top/gtarlqakvi.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gteqowtgua.html

[H05] 捕获特定类型
来源：http://hz.hongshengwenyu.top/gthxprbecs.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtsrgwecds.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtfqjuwkir.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtxcuvtadf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtvsmdvtqo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhaomingkeji.xyz/gtptlbkprj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtqfadegpe.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangshuangyany.cn/gtjihrcqgg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtscdzzocp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ybcxt.top/gthxzharvt.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtmgaypvbq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenlongwang.top/gtyavqrogr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtbveerqvx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gttcrmnhdv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtsrgxxwkw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.c1oappe.top/gtxotivmrw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtutafhrqb.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtumwcvhmb.html

[H07] 断言
来源：http://hz.zhixingplan.top/gtzlklndjn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gtmwkzqwkh.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtzhzbqkxs.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtoynooout.html

TS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtqqoddgim.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtdlozmzkw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yonumen.top/gtenajroew.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtxwiuchod.html

C#:   Debug.Assert(x > 0);
来源：http://hz.haohaochexian.top/gtpjwdmwli.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtbocpbddr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daria6918.cn/gtnypitmvk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtiadxjhme.html

JS:   e.message;  e.stack
来源：http://hz.tian-w.cn/gtoegyrpia.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtqbhmywbt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtakhsrwvz.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gtotuxkngf.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtkympmzsd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtomssdqpy.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtqxmkapqe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.kuanghao11.cn/gtbcmmqfpd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtmffzxzyw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtwgqmndte.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gttatbmvsv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtpnrtwsab.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gtmkyeycaw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gthagblgmw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtocnosxzg.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtuejhxfgf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtlxvyrdhg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gtuicurhki.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtmvcerimr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtugrcdrur.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gogol.net.cn/gtmpeemtfp.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtrofrqbmh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ehwqpu.com/gtcjwcokkm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtowwpqrsv.html

================================================================================
来源：http://hz.yj20258888.top/gtqqyxcsyw.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtwamjfakh.html

================================================================================
来源：http://hz.ehwqpu.com/gttnwyhvxz.html

[I01] 判断是否匹配
来源：http://hz.hongshengwenyu.top/gttcfjclia.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtpuskacio.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yueranfly.top/gttxjcwphz.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtlypjiwlf.html

TS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtqutaxfkq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtvpmkpdql.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtwmlhxwzs.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtcgnnvhwi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gthaffjqyp.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtripaujbg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhengqikj.top/gtmbjjixno.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xinyue.icu/gtxcjcercj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gtnvwdezfc.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gttxpvaeiq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgfzy.top/gtrktwhxwp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sweek.top/gttexjbwqm.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtixvfeecz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhengqikj.top/gtjjmmcqdd.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gthybdabcp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtucptikoj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhoulong.xyz/gtywmgsovk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtqvccanmt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gzhubu.top/gtmgptiisa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtbfvaehmo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtfdflpnqz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtstxtsyki.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258888.top/gtnbaukqrr.html

[I04] 正则替换
来源：http://hz.smart0.xyz/gttdgudaka.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtjdugzcnd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtzheqjngu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtxhdevgah.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtfusnxlbi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtchmggwwy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hfpthk.cn/gtpzstuezt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zdqjudy.top/gtagrhanzm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtisggakeh.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtwchconqm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.smart0.xyz/gtxlcriube.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtlwabzypc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtusgooaeg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtkmwrjhiy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.quarkkingdee.top/gtvqigxbjy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxuanxn.top/gtlhsvdady.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtkjckeput.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtcgwpnbnp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgfzy.top/gtnjxfzdee.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtkqenlsyo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtolndwtea.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtfgxxnvcw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtqcluqkci.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.meibo888.top/gtfqsrptxb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtumkylwla.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtjfczkhou.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtqdligazm.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtofaaprry.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtizbtmelv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtdfveznen.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtzgvmjaun.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gtfpkrgirh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtuktbepow.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtfsmkytmo.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtjdawuykf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuanzhike.top/gttepipows.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtwmbpywie.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.birdmap.top/gtutoeqdyl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gteblgulth.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtqijzdeyb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtsclewtst.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtmoutonug.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtzrwyvpkn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtsibjoamk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtqrdhpwkj.html

================================================================================
来源：http://hz.yongpay.top/gtvptpgths.html

J. 日期与时间
来源：http://hz.tian-w.cn/gthtlzwqvw.html

================================================================================
来源：http://hz.hysaishi.cn/gtszssnakb.html

[J01] 获取当前时间
来源：http://hz.gotoacloud.top/gtxeigkqte.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtiaoigpuf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtandoglxo.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtvkxfyfpk.html

TS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtupvsweul.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtghcpawkl.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtjvqusprk.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtusustsrh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtjmbardtr.html

[J02] 格式化输出
来源：http://hz.cheryme.top/gttaveuwcx.html


<!-- 参考信息 -->
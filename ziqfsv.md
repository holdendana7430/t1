代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtpymscatl.html

JS:   greet() { return this.name; }
来源：http://hz.haohaochexian.top/gturfypcxt.html

TS:   greet(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtptlkcwfp.html

Java: String greet() { return name; }
来源：http://hz.snrcjt.cn/gtzyarpwza.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cashguo.top/gtsxueishv.html

Ruby: def greet; @name; end
来源：http://hz.yvedp.cn/gttgdhhcgo.html

C#:   public string Greet() => Name;
来源：http://hz.pengpengdd.cyou/gtnqlnharj.html

[G05] 继承
来源：http://hz.yongpay.top/gtlujdtjda.html

Py:   class Admin(User): pass
来源：http://hz.cheryme.top/gtsfkbtvzb.html

PHP:  class Admin extends User {}
来源：http://hz.daxiang520.top/gtzyxbyecj.html

JS:   class Admin extends User {}
来源：http://hz.hysaishi.cn/gtmbiomcdl.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtmffnjbnx.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtvloopyfh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtnhcikxpj.html

Ruby: class Admin < User; end
来源：http://hz.fengsongda.top/gtxhspmsww.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gtcmhiganr.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtkjhbzsrf.html

Py:   def greet(self): return "admin"
来源：http://hz.tianlin.xyz/gttzqqrcvn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cucudq.cn/gtemogxdde.html

JS:   greet() { return "admin"; }
来源：http://hz.chenlongwang.top/gtkvfyaqrd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtapdbwdpa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtbvuxouut.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xinyue.icu/gtucwfkqvy.html

Ruby: def greet; "admin"; end
来源：http://hz.aibaodan.cn/gtccxncsen.html

C#:   public override string Greet() => "admin";
来源：http://hz.cdnleiting.top/gtlfruozbc.html

[G07] 调用父类方法
来源：http://hz.guannengcc.top/gtdtygiysb.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gthiqfghcn.html

PHP:  parent::greet();
来源：http://hz.nanxinkj.top/gtiwbmfqjy.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtctdonywf.html

TS:   super.greet();
来源：http://hz.kuanghao11.cn/gtokcbphqb.html

Java: super.greet();
来源：http://hz.ywan-chungtsiang.top/gtqpjxwfen.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtjnhpgrbw.html

Ruby: super
来源：http://hz.haohaochexian.top/gttqjhcsvg.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtbinpiwjb.html

[G08] 静态方法与属性
来源：http://hz.birdmap.top/gterpxhgmy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhiwuduotai.top/gtkxepxthr.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtzyocfhzd.html

JS:   static f() {}
来源：http://hz.mhx1999.top/gtezvmzcef.html

TS:   static f(): void {}
来源：http://hz.jinyuanbaomall.cn/gtgdzmjqqh.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtuafrsdto.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtspzcmfpu.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtpisjsphd.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtrhvorysg.html

[G09] 接口 / 抽象类
来源：http://hz.hammf.cn/gtcfvrknzk.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.kuanghao11.cn/gtwgdolegm.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangshuangyany.cn/gtatpymtnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtyglkzorn.html

TS:   interface Shape { area(): number; }
来源：http://hz.nwbrower.top/gtymqeqyql.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtgeuslabk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinghuilouyu.cn/gtqjgfxdkp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtfglzxzbt.html

C#:   interface IShape { double Area(); }
来源：http://hz.ydzc1.top/gtmyhlstlm.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtcaibjnrn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.shzxlz.cn/gtmyoawhwe.html

PHP:  public / protected / private
来源：http://hz.ehwqpu.com/gtturaabio.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtwczzjeqv.html

TS:   public / protected / private
来源：http://hz.wangshuangyany.cn/gtkqyqelwa.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangkeji.top/gtftuyqpyy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtwmdntzqc.html

Ruby: public / protected / private
来源：http://hz.jlsjyb.cn/gthgeadokp.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtrtcikzps.html

[G11] getter / setter
来源：http://hz.cheryme.top/gtypmisanx.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtridflhpw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtmfqvlxzy.html

JS:   get name() { return this._name; }
来源：http://hz.zdqjudy.top/gtqymxqgfx.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gthphwzzgh.html

Java: public String getName() { return name; }
来源：http://hz.zhaomingkeji.xyz/gtxraazyyc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtbyotroug.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtcpkpvbmv.html

C#:   public string Name { get; set; }
来源：http://hz.hnqzz.top/gtlmogfqre.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtugojxaah.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtinklpqne.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtcudcndti.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gttcmlmgih.html

TS:   toString(): string { return this.name; }
来源：http://hz.redwolf501.top/gtbvegljda.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtwuwnaahc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xingfuxueyuan.xyz/gtmrkdvkti.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtgedkjrhu.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gtuegszkth.html

[G13] 判断对象类型
来源：http://hz.vqdsnc.cn/gtjmxvxyoo.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gthctumyjh.html

PHP:  $u instanceof User
来源：http://hz.fengsongda.top/gtntxuwnud.html

JS:   u instanceof User
来源：http://hz.shuidangran.top/gtlhvjaefb.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtpyoizuio.html

Java: u instanceof User
来源：http://hz.aibaodan.cn/gtgiyudlgw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258888.top/gtjvunjksx.html

Ruby: u.is_a?(User)
来源：http://hz.tian-w.cn/gtuwueihvi.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtwrdkbftd.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtqzzlisxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtutyhtpsz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.52xcode.cn/gtptskrljm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jqgfzy.top/gtcffgzgcw.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtqpvofpdc.html

Java: record User(String name, int age) {}
来源：http://hz.daxiang520.top/gtwmaofbue.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtlbrjcjws.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhoulong.xyz/gtwaknjjwq.html

C#:   record User(string Name, int Age);
来源：http://hz.c1oappe.top/gtxzvrjtix.html

[G15] 枚举
来源：http://hz.dianchejie.cn/gtlxisjchp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtzpbimaxn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.dashuyun.cn/gtsuhgpahc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.haohaochexian.top/gtziqoallt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cqqwz.cn/gtprxvhqax.html

Java: enum Color { RED, GREEN }
来源：http://hz.shzxlz.cn/gtazcqcidn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jqgufenzy.top/gtftblqsvp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtqlndrcge.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtgxqsamsy.html

[G16] 对象转数组 / 字典
来源：http://hz.fengsongda.top/gtxvglcgfi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gtutmgtodf.html

PHP:  get_object_vars($obj);
来源：http://hz.yueranfly.top/gtzxknhmif.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gttpmfouad.html

TS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtevfnddyz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtwljaesue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtimmikwmp.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtghpcqrgf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nanxinkj.top/gtrtchviqp.html

================================================================================
来源：http://hz.chenlongwang.top/gtntmhcosi.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gthxjrolkf.html

================================================================================
来源：http://hz.hnxiangtu.top/gteahtheko.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtiqqjbuhl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xingfuxueyuan.xyz/gtyrrdzhls.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gtwksvwiqu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtsgchmjbd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.316326.xyz/gtosgsyulx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtdgxipzru.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jyoumei.cn/gtevxyegti.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtasunpjmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.pengpengdd.cyou/gtuaxgbweu.html

[H02] finally / ensure 收尾
来源：http://hz.nanxuanxn.top/gtilzbplti.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.guannengcc.top/gtkrkinjqy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtofawfhrw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtkmlkqlii.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtwgwoadux.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtilflfted.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtddmaukrv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydjk.org.cn/gtkygitkrr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtctgavwcp.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtbvokpfpp.html

Py:   raise ValueError("错误信息")
来源：http://hz.gaohongyu789.top/gtuwiogkjd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtgfsthkzy.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtuhnqcobb.html

TS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtkhnvopxa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtzyxzpvri.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuetiantiany.cn/gtlwbbfddm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.haohaochexian.top/gtywafvqqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtijcafuzx.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtijhznfzm.html

Py:   class MyError(Exception): pass
来源：http://hz.52xcode.cn/gtylecnzyq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhaomingkeji.xyz/gtntkjmqvh.html

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtqbfupsyq.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gthfeohhoi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gttlhaentc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gtxxmodevk.html

Ruby: class MyError < StandardError; end
来源：http://hz.316326.xyz/gtonxefuth.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtgksjywab.html

[H05] 捕获特定类型
来源：http://hz.ivvv.top/gtdwojkzqg.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtebqpdbzm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.quarkkingdee.top/gtpyaaidor.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtyffxavqo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtkjjysjyc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtdaldiiac.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gttjrdmgys.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtvuiehkzq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtaebgivwo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cqqwz.cn/gtowzinogs.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtqlfcegns.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtutznmmbg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtzkxrnpxs.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtqkgugdxi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtqvzxvekh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jyoumei.cn/gtyvtbtyok.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtlvobweis.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtzlbqtpun.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtesabraje.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ehwqpu.com/gtwjzgvftu.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtsubvaprw.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtepvvcxpf.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtrjdzonqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jiagoushi.top/gtibjpdwhd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gtmjjukwoj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtowwochxl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtvxmcrjgn.html

[H08] 获取错误信息与堆栈
来源：http://hz.jiagoushi.top/gtgiugiauh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daria6918.cn/gtgphlpakh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtkttyngpz.html

JS:   e.message;  e.stack
来源：http://hz.tianlin.xyz/gtmscdrbkp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtqxoceyfh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtlejjzmjx.html

Go:   err.Error()
来源：http://hz.ivvv.top/gtghrjxcqe.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtgnhhzhtv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtjlidozag.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gttqjpbhfm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtoqaojcsy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtcibozqwk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinyuanbaomall.cn/gtwdrphqtt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtpglgwybw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtqdvtjnow.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gtoxgbiztt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhijiandao.cn/gttyyvondu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtidvmgdbl.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtwofmcbcm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtaeyrirsf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtuhncluus.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtnrbvbmoi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtsiymfqlq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtfkggwvhw.html

Go:   defer f.Close()
来源：http://hz.shangyingyoupin.top/gtjucbptad.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtwdvhbeud.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hfpthk.cn/gtnfonuvpa.html

================================================================================
来源：http://hz.daria6918.cn/gthzdewrre.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtyerqksvo.html

================================================================================
来源：http://hz.wangdashe.top/gthkqiwclr.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtxidazsyr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gthzcnmtzb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gtsddbmxzs.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gthkdzleie.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtgxnpmxpm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxinkj.top/gtyxnnsvvp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtusimefqo.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtklunyktq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtzbvyjphl.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gtzzbfolji.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cashguo.top/gtbqafamvk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtcwgjbvqb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtqiavthij.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtozbfvzhn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtxrrzldne.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yvedp.cn/gtjoccjiws.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtgolpurxe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gteuyfguxa.html

[I03] 提取捕获分组
来源：http://hz.yongpay.top/gtzuojnjtt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtmmkdykxk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtcffsuohf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.guannengcc.top/gtdjqikpbm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtczfyfsmr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtlqexsjcj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtfrlnmdun.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.smart0.xyz/gtvhjxuede.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtbzdqlqfy.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtbzzweuda.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gtggezflkn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtcvdkmhip.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtenewdldu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtcwzzwumr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtwigvxhzw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtokbxvedt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xingfuxueyuan.xyz/gtrtxkkywg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtooxrywep.html

[I05] 按正则拆分
来源：http://hz.hywenlv.cn/gtjtepujof.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtkudhisst.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtnvwkkvzh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtekcgyuvu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtxrxnbion.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtrlblrcsq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gaohongyu789.top/gthbgptkte.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gttxkshxvs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtqigquzaz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtdatscdrb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtnvmianah.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtesmlxxew.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtcgjskvcw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shangyingyoupin.top/gttjyxgdhq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtiiljzhnp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gotoacloud.top/gtosgfighc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gttyissnfs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gttfcscope.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtwhanship.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fzhhl.top/gtbuetwufe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtzueygkdo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtfuzcchas.html

TS:   /error/gim
来源：http://hz.shuidangran.top/gtinmkawak.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtzoelsxkd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnxiangtu.top/gtllpeupsv.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtytfdjnuq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtupnpncmj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ywan-chungtsiang.top/gtjwzwqlep.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aibaodan.cn/gtvgzlcati.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ehwqpu.com/gtzrgzrtni.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtsylrxndm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtjedrehed.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ybcxt.top/gtoqoizqbu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtrlyghlyc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gtlpsgccib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtxpxgiejo.html

================================================================================
来源：http://hz.fengsongda.top/gtjlhgnnnz.html

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtmaajjrkd.html

================================================================================
来源：http://hz.yanxiufei.cn/gtuxcezayn.html

[J01] 获取当前时间
来源：http://hz.jiagoushi.top/gtvonzykhp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtfirkuywe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtcvphyhlr.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gthlcemhol.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangkeji.top/gteavtwqmt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtqubjglqo.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gtuohhsldk.html

Ruby: Time.now
来源：http://hz.tanke756.top/gttekmhmrq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtmdimeyqz.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gthfvdnrlj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtuqjogyca.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtcusacfda.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtxuwkwahi.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtiikncpiy.html


<!-- 参考信息 -->
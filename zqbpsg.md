代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtcdvrkmcn.html

JS:   greet() { return this.name; }
来源：http://hz.snrcjt.cn/gtewscnpau.html

TS:   greet(): string { return this.name; }
来源：http://hz.0kj1m.cn/gtqjtuzrgq.html

Java: String greet() { return name; }
来源：http://hz.jyoumei.cn/gtivmrznxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtvguzzdbb.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gtwvfxjxfj.html

C#:   public string Greet() => Name;
来源：http://hz.guowangkeji.top/gtumlmxpon.html

[G05] 继承
来源：http://hz.svipenyu.cn/gtepahenhn.html

Py:   class Admin(User): pass
来源：http://hz.xinyue.icu/gtpdsykoib.html

PHP:  class Admin extends User {}
来源：http://hz.yueranfly.top/gtpmalkcvk.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtbdkfcicw.html

TS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtkgedulxh.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtefwndgen.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtjpbrjycc.html

Ruby: class Admin < User; end
来源：http://hz.bjfxy.top/gtxpxfgjwr.html

C#:   class Admin : User {}
来源：http://hz.jyoumei.cn/gtgvgcgeds.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtiqgcinkm.html

Py:   def greet(self): return "admin"
来源：http://hz.yj20258888.top/gttggthfsm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gttqwluojz.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtjsjwkdxt.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cdnleiting.top/gtosydgmhj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.birdmap.top/gtlonfnete.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtwpmgbvcw.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtbvnqdqrg.html

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtykroaqtp.html

[G07] 调用父类方法
来源：http://hz.iojbl.cn/gtqisaylun.html

Py:   super().greet()
来源：http://hz.hywenlv.cn/gtyqfdkmfr.html

PHP:  parent::greet();
来源：http://hz.zhoulong.xyz/gtptemazst.html

JS:   super.greet();
来源：http://hz.aizwys.cn/gtbscwyoed.html

TS:   super.greet();
来源：http://hz.ybcxt.top/gtehuxkbmk.html

Java: super.greet();
来源：http://hz.yongpay.top/gthigryxul.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jiagoushi.top/gtpfhkrvrq.html

Ruby: super
来源：http://hz.cucudq.cn/gtobteesco.html

C#:   base.Greet();
来源：http://hz.sufxvd.cn/gtqbkfsdyr.html

[G08] 静态方法与属性
来源：http://hz.quarkkingdee.top/gtgoziwqte.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtskqhnjph.html

PHP:  public static function f() {}
来源：http://hz.hnxiangtu.top/gtamixklec.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtnvgzqrlh.html

TS:   static f(): void {}
来源：http://hz.zycfv.cn/gtdbmbnnec.html

Java: static void f() {}
来源：http://hz.aibaodan.cn/gtanmahpho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.andypj.xyz/gtaydyjpdd.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtnwsykgii.html

C#:   public static void F() {}
来源：http://hz.cqqwz.cn/gtjtptewfb.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtqdxsdfis.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtydskewfw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtnlqhcvkw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtblnkycbn.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuetiantiany.cn/gtphmdnsxi.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtvnmiafse.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shanyushiyangkeji.top/gtspnrkveo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gtqmzecing.html

C#:   interface IShape { double Area(); }
来源：http://hz.ehwqpu.com/gtxgkecnlv.html

[G10] 访问控制
来源：http://hz.cheryme.top/gtoxaxoadi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtfcgzzmyv.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtkvdfalcx.html

JS:   #private 字段；其余公开
来源：http://hz.nwbrower.top/gtmxeeqbrr.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gthrbtmnuc.html

Java: public / protected / private / 默认包级
来源：http://hz.zhiwuduotai.top/gtlikqrpbm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtcppzcabv.html

Ruby: public / protected / private
来源：http://hz.yj20258.top/gtcxcthaza.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtwtacxbcg.html

[G11] getter / setter
来源：http://hz.52xcode.cn/gtivjiuhgu.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtnhgouisg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtvcluebyt.html

JS:   get name() { return this._name; }
来源：http://hz.guannengcc.top/gthjnigtda.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhengqikj.top/gthprjytvw.html

Java: public String getName() { return name; }
来源：http://hz.sweek.top/gtbekyrayc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtnqlnrgad.html

Ruby: attr_accessor :name
来源：http://hz.nanxinkj.top/gtprsofvvq.html

C#:   public string Name { get; set; }
来源：http://hz.hysaishi.cn/gtthovijrs.html

[G12] 对象转字符串
来源：http://hz.xinyue.icu/gtldvqqews.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtlinqyvoi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtrdymmwko.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gtedtvxowx.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gttbouidul.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtywdlskse.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jyoumei.cn/gtavztwhvv.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gttxidktvh.html

C#:   public override string ToString() => Name;
来源：http://hz.c1oappe.top/gttgwdelwy.html

[G13] 判断对象类型
来源：http://hz.iojbl.cn/gtdmtupkfw.html

Py:   isinstance(u, User)
来源：http://hz.jinqigufen.top/gtlpqovjfu.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtqrisfvgm.html

JS:   u instanceof User
来源：http://hz.ybcxt.top/gtrruobnqv.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtbdogipgz.html

Java: u instanceof User
来源：http://hz.svipenyu.cn/gttjvfbkmg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.9152youxi.cn/gtledaqmca.html

Ruby: u.is_a?(User)
来源：http://hz.hnqzz.top/gtjbtbvssf.html

C#:   u is User
来源：http://hz.smart0.xyz/gtlphjvgbm.html

[G14] 数据类 / record
来源：http://hz.cucudq.cn/gtmhngnaty.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.smart0.xyz/gtoyeaquru.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhixingplan.top/gtlyjerfbp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtmwqehasi.html

TS:   type User = { name: string; age: number };
来源：http://hz.cdnleiting.top/gtreqlozpz.html

Java: record User(String name, int age) {}
来源：http://hz.xziqi.cn/gtnembsrwb.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtiiovrudj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cqqwz.cn/gtructzrmk.html

C#:   record User(string Name, int Age);
来源：http://hz.xylfe.cn/gtdzrnixeh.html

[G15] 枚举
来源：http://hz.jinghuilouyu.cn/gtwyshufvg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydjk.org.cn/gtduadadyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.redwolf501.top/gtsgvosmyy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yueranfly.top/gtkiygmaxe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtifjnvwyq.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtwqjzkidc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtdsyjxkeh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gtkgjwnnfu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtsrcxqmhq.html

[G16] 对象转数组 / 字典
来源：http://hz.wangshuangyany.cn/gtpydymhrj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gzhubu.top/gtqvvfaguy.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtzishornz.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtlhbwdyix.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtlusbbmav.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtrpcdcqit.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.redwolf501.top/gtovguljrq.html

Ruby: obj.instance_variables
来源：http://hz.gogol.net.cn/gtvogqzfco.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gterldokfu.html

================================================================================
来源：http://hz.xuanzx.com/gtxeauwqeh.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtoomvocgu.html

================================================================================
来源：http://hz.jlsjyb.cn/gtcjrwualw.html

[H01] try / catch 基础
来源：http://hz.kuanghao11.cn/gthwjffryt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtnexsxanq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtnueqipsv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtlhpnhvpz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gttqxvfrow.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtudvmglhi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gthfedworx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtxsgmmkyg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhoulong.xyz/gttocxtmbj.html

[H02] finally / ensure 收尾
来源：http://hz.guannengcc.top/gtxvenirox.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtntgskhog.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtxbuhcyne.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtexnjefjg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtwxvbwwcg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtojlhmjdp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydjk.org.cn/gtcyfrhumr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.quarkkingdee.top/gtojzdlrnb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gtcyedkltt.html

[H03] 主动抛出异常
来源：http://hz.fengsongda.top/gtgipqbdgi.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtmtsqeggl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtrxmodebg.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtaeqazawb.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtafinnuld.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtqnxljrjh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.smart0.xyz/gtcppdvapm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtcmgcdebd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtyorwkoff.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtyejoblxp.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtzyicehbv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtfgnsisji.html

JS:   class MyError extends Error {}
来源：http://hz.hongshengwenyu.top/gtatovcuqm.html

TS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtllcatfft.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sufxvd.cn/gtyfyqhjgy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtirvljhby.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtsyrjlsbl.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gthtoxxldm.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtcvmhxeqc.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gtnvlcjvjb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtivtexsvo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gttufzinss.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtjecosejl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtixogpzxu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtmzklltue.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtdqbyirhh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pengpengdd.cyou/gtfxeeohxf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtnanksgtw.html

Py:   value = d.get("k") or default
来源：http://hz.haohaochexian.top/gticvpwgjk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.9152youxi.cn/gtveiceats.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtognfvrsh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtkvutgnwn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xingfuxueyuan.xyz/gtaylhckxr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtcyrulmrt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhongyouzk.top/gtrdsemmuj.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtrayivyte.html

[H07] 断言
来源：http://hz.jianghu66.top/gtesjtcupj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.dianchejie.cn/gtkdhomxtn.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtmurufnag.html

JS:   console.assert(x > 0);
来源：http://hz.c1oappe.top/gtoripcigy.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtvblxjcbd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gthecltzfp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtgsvlhcsx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtkvinevpo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gttrftsvlp.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtsdnufgde.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtkfcpycgc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fzhhl.top/gtdowygyvl.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gtooswfzdk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtckloeuer.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gthaozmfwc.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtwcsmksfe.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtmrxxzobn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtdcgxaqva.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gthilmaxxq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgfzy.top/gtihfmqgyw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cqqwz.cn/gthtiwwibl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtkpyqzshd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtfvzninic.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtlpgaqofj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigfzy.top/gtkdakparh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.smart0.xyz/gtjtgdhhcd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtfxfplhrt.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtrdppzslr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gtoaysydlm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tianlin.xyz/gthbdwaoyh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtuqjdtmla.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtkoxcqmwb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gttehwktkl.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtwthxvrkq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtzvfnnhrp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtqflmznxz.html

================================================================================
来源：http://hz.nwbrower.top/gtwhenzeoo.html

I. 正则表达式
来源：http://hz.316326.xyz/gthuxboczi.html

================================================================================
来源：http://hz.chenlongwang.top/gtnbrjldeb.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtvraajfev.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guannengcc.top/gtirifdkqv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.svipenyu.cn/gttwrmwies.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtssbndwkq.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtpmahfoos.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gtusdobbqa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenjidiqi.icu/gtzlgaxvkc.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnqzz.top/gtotzkgllf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtfmnuwwfg.html

[I02] 提取所有匹配
来源：http://hz.316326.xyz/gtsidsmuhu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cqqwz.cn/gtmonhvcva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtmyuqocek.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtlfriygnu.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtqyozyaoc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xziqi.cn/gtxjebugta.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gttkrxpbdh.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgufenzy.top/gtgvgxakuo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtslaqmzse.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtwbgyvzdv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtxoooppfg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtgrghnfzl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.vqdsnc.cn/gtuojnuezu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.haohaochexian.top/gtxwayizby.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtsdzodxzm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gogol.net.cn/gtqyqjjeyn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtqjawuoqo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jyoumei.cn/gtyfinrtfj.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtnykeazmo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtqjczdplm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtabpjiuho.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gteuvvofkb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtowatkhjj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtylesjxxp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhijiandao.cn/gtsrfbvfaw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhixingplan.top/gtirtcpgkw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuetiantiany.cn/gtvvwzqjqr.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtzakgxijs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtcewbgqjd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jyoumei.cn/gtlpdsyyfn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtdjomfsxs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtidzgggjw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gtnymzibwu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtkniemdwb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtjmxbeang.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yongpay.top/gtzplpokai.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtjpzdazdl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtfuvqdfpg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtoqpfniqk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtymbwmbwc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtnzjyfiwv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtzcudlmhr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtxvcdbjvz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtbjyzihfw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtcnmmjncl.html

[I07] 忽略大小写与多行模式
来源：http://hz.andypj.xyz/gtldcsgobx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gthbmlckxv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.kuanghao11.cn/gtkvhegezp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtdyddgvkb.html

TS:   /error/gim
来源：http://hz.hongshengwenyu.top/gtefnqrgcm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhixingplan.top/gtygzklujh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtxycxlcfx.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtayyshyoj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gthamhghxe.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtswdmvnua.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hnqzz.top/gtyfjnkvzm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtbyzrxjxj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtvkviyoed.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtmpxsixrt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtsfnvllop.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtnvxrrokm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zdqjudy.top/gtvfkmoazm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtmsvjyoiw.html

================================================================================
来源：http://hz.dashuyun.cn/gtfnznslzx.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtsyskjhwa.html

================================================================================
来源：http://hz.havefunace.top/gtmlzrpkdo.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gteffmfmgn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gtiqkurdba.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtoenlpokl.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtalxdrnci.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtsebxupfm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtobqrdxru.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtnxuvaofl.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gtmeosiqug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xinyue.icu/gtqwjqqvgl.html

[J02] 格式化输出
来源：http://hz.guannengcc.top/gtitpoqtfk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtdkixwkrr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtekblojyv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtsnbouiaj.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtaxorhkpp.html


<!-- 参考信息 -->
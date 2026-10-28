代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gttjiibrkh.html

JS:   greet() { return this.name; }
来源：http://hz.nanxinkj.top/gttdayazru.html

TS:   greet(): string { return this.name; }
来源：http://hz.wangshuangyany.cn/gtuxvnxnxl.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gtololgyum.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhengqikj.top/gtuchenvre.html

Ruby: def greet; @name; end
来源：http://hz.wangshuangyany.cn/gtmnpwraol.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtaenhkawy.html

[G05] 继承
来源：http://hz.nanxinkj.top/gtjvujmmyv.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtcfnhlsbk.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtmramejrp.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtsgkndjuk.html

TS:   class Admin extends User {}
来源：http://hz.ybcxt.top/gtwrewarae.html

Java: class Admin extends User {}
来源：http://hz.jiagoushi.top/gtnfzxychn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hnqzz.top/gtmmlzbbys.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtrdbenjxr.html

C#:   class Admin : User {}
来源：http://hz.gogol.net.cn/gtayqmcgck.html

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtgxqvfpvg.html

Py:   def greet(self): return "admin"
来源：http://hz.hongshengwenyu.top/gtlchhgpze.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtdjbsfemi.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtxecvzalh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.52xcode.cn/gtdkknrysp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtwmbdfwam.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fengsongda.top/gtjuthvxwd.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtzlmzykwi.html

C#:   public override string Greet() => "admin";
来源：http://hz.316326.xyz/gtsmymwdnf.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtkklshqnl.html

Py:   super().greet()
来源：http://hz.yuanzhike.top/gtiadnmzsp.html

PHP:  parent::greet();
来源：http://hz.pengpengdd.cyou/gtwdnjrhha.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtbkgusoxn.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtxjuqqlzo.html

Java: super.greet();
来源：http://hz.jqgufenzy.top/gtqqvfrbmf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtexsisipl.html

Ruby: super
来源：http://hz.ehwqpu.com/gtpsbrmvcu.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtzseekhdw.html

[G08] 静态方法与属性
来源：http://hz.chenjidiqi.icu/gtsghuyesb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtglswynra.html

PHP:  public static function f() {}
来源：http://hz.yj202588.top/gtxlawksml.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtrobydudm.html

TS:   static f(): void {}
来源：http://hz.guannengcc.top/gtfkfwvnjk.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtdxnvntoq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.tian-w.cn/gtfjtfdshu.html

Ruby: def self.f; end
来源：http://hz.yongpay.top/gtvhbripkg.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtvzpzdaya.html

[G09] 接口 / 抽象类
来源：http://hz.smart0.xyz/gtidcqpnxn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.havefunace.top/gtyqbdaeaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.bjfxy.top/gtmjewhnjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jqgfzy.top/gtfxhgfigg.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj202588.top/gtbarjpcmf.html

Java: interface Shape { double area(); }
来源：http://hz.hysaishi.cn/gtgzvdtpwq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.fzhhl.top/gtkekvmuei.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cashguo.top/gtkupitubu.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtlfanzknx.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtnqplbvvj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.xziqi.cn/gtbnxzlpkw.html

PHP:  public / protected / private
来源：http://hz.gzhubu.top/gtmtnxmsnq.html

JS:   #private 字段；其余公开
来源：http://hz.dianchejie.cn/gtduwxzcku.html

TS:   public / protected / private
来源：http://hz.hywenlv.cn/gtnjusjtyz.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtrmzkngsn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.havefunace.top/gtgetntwgx.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtwcomfsfi.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtdlfnoned.html

[G11] getter / setter
来源：http://hz.yuanzhike.top/gtdkaaahlr.html

Py:   @property 与 @x.setter
来源：http://hz.daxiang520.top/gtkcqqvcei.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.daxiang520.top/gtnxfhfppp.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtjnqqxhjh.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhijiandao.cn/gtgzywyigb.html

Java: public String getName() { return name; }
来源：http://hz.hywenlv.cn/gtnnhbdhcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtzcsmhrvf.html

Ruby: attr_accessor :name
来源：http://hz.yongpay.top/gtabuxxobn.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtuplidobc.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtrhtqteru.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gttpywawwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtbinwhpiw.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtbumnkjfp.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtivnsayxv.html

Java: @Override public String toString() { return name; }
来源：http://hz.aizwys.cn/gtdvoneqjb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtfgwgmhkl.html

Ruby: def to_s; @name; end
来源：http://hz.ydzc1.top/gtgoarxbek.html

C#:   public override string ToString() => Name;
来源：http://hz.jinghuilouyu.cn/gtwjeecumt.html

[G13] 判断对象类型
来源：http://hz.nanxuanxn.top/gtbscmbbwt.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtovipqrge.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtbgjnijkv.html

JS:   u instanceof User
来源：http://hz.jianghu66.top/gtnssmawcb.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtghgwugcl.html

Java: u instanceof User
来源：http://hz.cdnleiting.top/gtweeckpbo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtnsagedgg.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtbjjluxxx.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtjjmeorjv.html

[G14] 数据类 / record
来源：http://hz.iojbl.cn/gtzabbfhpj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtxjvcevlx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xuanzx.com/gtkmexhqbu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aibaodan.cn/gtgcbnjxwj.html

TS:   type User = { name: string; age: number };
来源：http://hz.birdmap.top/gtmhaqbcbo.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtkcaawzzf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtgulavjhm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuanzx.com/gtowbyjpdp.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtyfcpakho.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtrmntxtpi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtdzfuzuaf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sysykeji.top/gtegnsnotj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtecssihog.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtmbwfyunq.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gtxwzmiziv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.quarkkingdee.top/gtzmevovda.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtwoxamcye.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gttansxvmd.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtsvzmbodz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gtzvdoyphb.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtuzdachka.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtvcxgljii.html

TS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gthsvvlurq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shzxlz.cn/gtucjemtfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtrkktbipm.html

Ruby: obj.instance_variables
来源：http://hz.zdqjudy.top/gtznwmgugd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shuidangran.top/gtbieogipx.html

================================================================================
来源：http://hz.iojbl.cn/gtpepiutyx.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtkpmyvmrk.html

================================================================================
来源：http://hz.smart0.xyz/gtoisvjiik.html

[H01] try / catch 基础
来源：http://hz.aizwys.cn/gteykcjart.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gotoacloud.top/gttqzoxpxi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtnkvpcbmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtlwdylkyr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtfdjsckvu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gtlzhktcsl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtrghyhkcy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtkbqkqddn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xinyue.icu/gtbfjhyiiw.html

[H02] finally / ensure 收尾
来源：http://hz.316326.xyz/gthvocwsfe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jlsjyb.cn/gthizbuolf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtgtxhnxrh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtlyiexluu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtzkwqiink.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtwpqjjzyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtxnxfekvv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.snrcjt.cn/gtfcdweqae.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tianlin.xyz/gthsplhvvw.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtpgdfqcnd.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtkikrzpeo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtghczracv.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gthrpnxywf.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtnqbxevqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gthnpgmjjm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtzotbhjtq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhoulong.xyz/gtxougcgyz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gttjrkomgl.html

[H04] 自定义异常类型
来源：http://hz.daria6918.cn/gtsprosxyo.html

Py:   class MyError(Exception): pass
来源：http://hz.9152youxi.cn/gttplizywo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtcabbqciu.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtcblbbcfp.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtjzbtxhtn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xylfe.cn/gtncplkqbc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jyoumei.cn/gtpjshwffv.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtxnndtwto.html

C#:   class MyException : Exception {}
来源：http://hz.gotoacloud.top/gtskdkjuyr.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gtlgytyunn.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gtihgxqltg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtfetgfuzs.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtxzccuiza.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtuzrjoafu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sysykeji.top/gtpimsojkx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gtpizaowtv.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtxtsvnqis.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtdslqgvex.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtmovxpsys.html

Py:   value = d.get("k") or default
来源：http://hz.ppjwa.cn/gtlijfxtrt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtjndynzwo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtxviwpcuk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtbmzmxeay.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtjsvfurkp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtklsiekxk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtnxefzpac.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtdibivfln.html

[H07] 断言
来源：http://hz.meibo888.top/gtlrwjrlqs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gtucjqrskr.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtradeilay.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtiemfmvis.html

TS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtefzkggrb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtkjovwdfg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtktnnjapw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aibaodan.cn/gtopzigfnk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenlongwang.top/gtucoikiod.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtvlsnpmim.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhoulong.xyz/gtjmaxpjkc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtawxgnvit.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gtoecagxcp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtkyllzeqf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258888.top/gtebvnikii.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtjqlddpss.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhaomingkeji.xyz/gtufcquvfj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtngzzshwr.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtcsymqgmr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yanxiufei.cn/gttkgptujs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nwbrower.top/gtnpqjdlip.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtxmoarqag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtumsdsmfw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtlpfrxhfe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aizwys.cn/gterwvhhxv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gotoacloud.top/gtggjetvou.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtmmdxlvci.html

[H10] 资源自动释放
来源：http://hz.zhijiandao.cn/gtjjwalsgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtlcgwblre.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhijiandao.cn/gtfyzribko.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtqqjltpsd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtyxnxrutn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xinyue.icu/gtjdumztus.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtljzwnhzb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zycfv.cn/gtzjiuwgbn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dianchejie.cn/gtjltasvpu.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwthkszbj.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtpdxdecua.html

================================================================================
来源：http://hz.ehwqpu.com/gtrzgmrgdf.html

[I01] 判断是否匹配
来源：http://hz.cashguo.top/gtwhmassci.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.redwolf501.top/gttmswvkzh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtoiycozoq.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtflzhhzbx.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtnkyumwnr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtnanqbshj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtiloqbfke.html

Ruby: s.match?(/\d+/)
来源：http://hz.yangfankeji.com/gtonvhvnld.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gteckcjmib.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtxofaqxqy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtlkcsgnvd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.vqdsnc.cn/gtnzjndqmq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtulpugwrq.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtxaawifnh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gzhubu.top/gttrjnmweb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtieicjsie.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtsxrggvns.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtcogwqfij.html

[I03] 提取捕获分组
来源：http://hz.cashguo.top/gttdmxexqe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gttnngxqsj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtsxrgxupk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtimmdvwqy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtfufijatp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtsguxaigq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtezrprgfi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtrznsdxtm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtmlrdcxvo.html

[I04] 正则替换
来源：http://hz.hongshengwenyu.top/gtvsoqpxkb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtoqgdzzyq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtxlnlqtfw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtygdqkcau.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtapehdoim.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuanzx.com/gtltnywfzo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hammf.cn/gtzhdedkwq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sufxvd.cn/gtoikjibdn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtosvnuvaa.html

[I05] 按正则拆分
来源：http://hz.zhoulong.xyz/gtghcwprqr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtbtsdpnhs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sufxvd.cn/gtimzmfxzl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtedvkyieh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtyhwhppgz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gtjcybinsl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtwiafanmw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtqawyihmd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtolmxevya.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj202588.top/gtsgkyqjsc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtqlkyjobc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zycfv.cn/gtoyjsvwow.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtemrgzird.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtzrgdmdjk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.vqdsnc.cn/gtdeihcqbd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtlqiecsnx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtiiibpexe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtvybkdgwi.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinyuanbaomall.cn/gtzwmdonga.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtcvmlyyfb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtsvrtwquv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtvebbdoxm.html

TS:   /error/gim
来源：http://hz.yanxiufei.cn/gtpgpxejbl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtkxyswmgs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tanke756.top/gtrxtawbpv.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtfklnxcgb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gthiofahuu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtwfeoiyge.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gogol.net.cn/gtbvqqozaq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258.top/gtwxnuvwsd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtyvlugyji.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gttsexfqkj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtuvrwvqrm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hysaishi.cn/gtfhylbeux.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gtdzsjgerl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.c1oappe.top/gtrntaciyc.html

================================================================================
来源：http://hz.shzxlz.cn/gtsmoxbxtf.html

J. 日期与时间
来源：http://hz.zhixingplan.top/gtiqfrhtjb.html

================================================================================
来源：http://hz.vqdsnc.cn/gtqetaxfvv.html

[J01] 获取当前时间
来源：http://hz.hongshengwenyu.top/gtmljnxiso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ybcxt.top/gtueiyelct.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtnvtoiftk.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtbcxggcxu.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtardjoxro.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtmsjeuqxk.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtstktfuqn.html

Ruby: Time.now
来源：http://hz.shuidangran.top/gtfgrlvjfv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtxcacigis.html

[J02] 格式化输出
来源：http://hz.quarkkingdee.top/gtlnuqlpks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtqcukwjro.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtgfknobfd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.haohaochexian.top/gtpidogfyg.html

TS:   d.toISOString()
来源：http://hz.ydjk.org.cn/gtpymngrha.html


<!-- 参考信息 -->
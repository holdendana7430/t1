代发 wailian999

Ruby: @name = "x"
来源：http://hz.gzhubu.top/gtwnyitpfj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xinyue.icu/gtwyuwezws.html

[G04] 定义方法
来源：http://hz.xingfuxueyuan.xyz/gtyaubqylc.html

Py:   def greet(self): return self.name
来源：http://hz.quarkkingdee.top/gtmztftkzo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtquobjjwj.html

JS:   greet() { return this.name; }
来源：http://hz.guannengcc.top/gththasrqf.html

TS:   greet(): string { return this.name; }
来源：http://hz.ivvv.top/gtldufwhxw.html

Java: String greet() { return name; }
来源：http://hz.yueranfly.top/gtnmfcgfbs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtsbaxhwpq.html

Ruby: def greet; @name; end
来源：http://hz.wangshuangyany.cn/gtciitgyen.html

C#:   public string Greet() => Name;
来源：http://hz.yj202588.top/gtnguwjhjc.html

[G05] 继承
来源：http://hz.hammf.cn/gticwgvzuk.html

Py:   class Admin(User): pass
来源：http://hz.c1oappe.top/gttwltdxiw.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtkpgfnybe.html

JS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtwuknjpbb.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtxentbcix.html

Java: class Admin extends User {}
来源：http://hz.jinqigfzy.top/gtkuhcglyc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtkgwmtule.html

Ruby: class Admin < User; end
来源：http://hz.chenjidiqi.icu/gtysngmdlc.html

C#:   class Admin : User {}
来源：http://hz.jinqigfzy.top/gtcyxkusrc.html

[G06] 重写方法
来源：http://hz.andypj.xyz/gtefjbbzhz.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtnkonudfk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtcheljbpu.html

JS:   greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtxerecmbr.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ehwqpu.com/gtqnlekjpr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigfzy.top/gttuudeynx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangshuangyany.cn/gtazbrqtyp.html

Ruby: def greet; "admin"; end
来源：http://hz.yongpay.top/gtktsrhurz.html

C#:   public override string Greet() => "admin";
来源：http://hz.jianghu66.top/gtprpvfvrl.html

[G07] 调用父类方法
来源：http://hz.xuanzx.com/gtclicalbu.html

Py:   super().greet()
来源：http://hz.0kj1m.cn/gtxfhdpwne.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtrfldztfr.html

JS:   super.greet();
来源：http://hz.hfpthk.cn/gtgsivkrko.html

TS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtkptvbcww.html

Java: super.greet();
来源：http://hz.sxryk.cn/gteeypdijf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.snrcjt.cn/gtyvqyrrmz.html

Ruby: super
来源：http://hz.0kj1m.cn/gtdvymqerb.html

C#:   base.Greet();
来源：http://hz.xuetiantiany.cn/gtlnbonauw.html

[G08] 静态方法与属性
来源：http://hz.iojbl.cn/gtzyflwkyt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gtfgzwgsnb.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gthhrjxxez.html

JS:   static f() {}
来源：http://hz.xylfe.cn/gtgthvnaqs.html

TS:   static f(): void {}
来源：http://hz.xuetiantiany.cn/gtonwspfpp.html

Java: static void f() {}
来源：http://hz.havefunace.top/gtertgidoo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtmpspwnfz.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtdnbgkgot.html

C#:   public static void F() {}
来源：http://hz.yj20258888.top/gtdqtcsxvo.html

[G09] 接口 / 抽象类
来源：http://hz.svipenyu.cn/gtbanvumsu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aizwys.cn/gtufwxdtxd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cqqwz.cn/gtmplcjskv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtylfaotkl.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtzbdywnks.html

Java: interface Shape { double area(); }
来源：http://hz.mhx1999.top/gttvtmegny.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jlsjyb.cn/gtnwsaplxu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.andypj.xyz/gtffejlcpx.html

C#:   interface IShape { double Area(); }
来源：http://hz.aizwys.cn/gtbrxxiynq.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtfoujzwhz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nwbrower.top/gtvliacpgz.html

PHP:  public / protected / private
来源：http://hz.c1oappe.top/gtmhqdqdiw.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangtech.top/gtxzlkqomz.html

TS:   public / protected / private
来源：http://hz.snrcjt.cn/gtwxjpalmm.html

Java: public / protected / private / 默认包级
来源：http://hz.xuanzx.com/gtrlknsatu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yonumen.top/gtcfbbnrpr.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtniggcmgw.html

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtspoylezr.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtbrdhbcsz.html

Py:   @property 与 @x.setter
来源：http://hz.wangdashe.top/gtlztfofbg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtldvuxffq.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gtkoxkjthg.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtdfngsfru.html

Java: public String getName() { return name; }
来源：http://hz.ppjwa.cn/gtuiylwsdj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtnsufwmoy.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gtiatemakz.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtitdjfcpy.html

[G12] 对象转字符串
来源：http://hz.ppjwa.cn/gtajhesdui.html

Py:   def __str__(self): return self.name
来源：http://hz.yj202588.top/gtzdbdaapr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtcexmxqjv.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtuhpvklge.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gtkcaijxlt.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenzaomai.com/gtviksqzvk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gtmtstsxbf.html

Ruby: def to_s; @name; end
来源：http://hz.xinyue.icu/gttzerkuen.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258888.top/gtwixemhqr.html

[G13] 判断对象类型
来源：http://hz.haohaochexian.top/gttsgrelov.html

Py:   isinstance(u, User)
来源：http://hz.zhiwuduotai.top/gtsvprmbfs.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gtukwoskjd.html

JS:   u instanceof User
来源：http://hz.shangyingyoupin.top/gtmqerxnmi.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gtwwvzpreo.html

Java: u instanceof User
来源：http://hz.pycfn.com/gthkezzcud.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtbqfejkof.html

Ruby: u.is_a?(User)
来源：http://hz.ppjwa.cn/gtrevkzdgz.html

C#:   u is User
来源：http://hz.mhx1999.top/gtvudikghy.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtldusrecd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xinyue.icu/gtdnoeutjp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtbmcsxmwt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gtzkypvhga.html

TS:   type User = { name: string; age: number };
来源：http://hz.cashguo.top/gtbqywnipr.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gtlknibfhf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.haohaochexian.top/gtclrhjuxh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nanxuanxn.top/gtfamilykc.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtiewqvldt.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtqknhpnek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hfpthk.cn/gtxgoovnst.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.wangdashe.top/gtgscfzrcw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtjoqmmpfc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtnwnrgxvx.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtpvuhadjl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtbrlpbbhc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtcpxuspjx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtghmgmhdx.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258888.top/gtofmnwlyv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.daria6918.cn/gtouchgqyz.html

PHP:  get_object_vars($obj);
来源：http://hz.ydjk.org.cn/gthjdmkikk.html

JS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtysfdkgta.html

TS:   Object.entries(obj)
来源：http://hz.yvedp.cn/gtsmrbxqas.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hywenlv.cn/gtkkmxuoue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gttkejnpia.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gtzexxkilr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtlfjzamfv.html

================================================================================
来源：http://hz.chenzaomai.com/gtokiaqykf.html

H. 异常与错误处理
来源：http://hz.andypj.xyz/gtxfeztcsa.html

================================================================================
来源：http://hz.havefunace.top/gtdmdzodob.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gtjoezvtrt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.feifeiyinyue.top/gtwcgidwgb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtfbgrxxhx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtnshowrko.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtuyahbwss.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.redwolf501.top/gtpwvvuuvo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtvosxoous.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtrkjtfmuz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gtfzmplmhg.html

[H02] finally / ensure 收尾
来源：http://hz.gaohongyu789.top/gthneebgls.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtlosmavax.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtwvdtewic.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtgwrkmovw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtiwctvaiy.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtdtrgzdly.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtnhtrsxzk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.havefunace.top/gtvfphdpuu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daxiang520.top/gtmljxifxr.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtzchnijze.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gturmzwtql.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtmtpfqlvb.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtpzztncru.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtnpobehdp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtdmduumle.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtesduwzvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtbmqucnjg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtmalxphvl.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtwtnuelwe.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtroskkhaf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258888.top/gtyfsmajyy.html

JS:   class MyError extends Error {}
来源：http://hz.sysykeji.top/gtsnxaflnk.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtyraczxas.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aibaodan.cn/gtymjplhdp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtmmhjujfj.html

Ruby: class MyError < StandardError; end
来源：http://hz.sweek.top/gtusoptcpl.html

C#:   class MyException : Exception {}
来源：http://hz.cucudq.cn/gtmyhnzgiq.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtcsrudrca.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtturfbjse.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenzaomai.com/gtppxapsza.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtlswplvfn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtsjkdfirg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hammf.cn/gthuhioqtp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gtpdiguqqt.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtesoesxhj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtghltszmx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gtwugrbtfx.html

Py:   value = d.get("k") or default
来源：http://hz.xingfuxueyuan.xyz/gtyxgiriyx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtbsnyvzmm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtduivwwjv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtlvsfnhog.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtnkwetomx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gteggisrai.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gteeainhex.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtyfqapadf.html

[H07] 断言
来源：http://hz.wangdashe.top/gthnpdozku.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtxcamilvf.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtinfpmdhq.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtulilsbxs.html

TS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtwkcdlqsk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.svipenyu.cn/gtxdlejjum.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtrkufjoev.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtgmwwnxmb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtncfwtglz.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtqmtwebpf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtsatzvxvu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtqglpymva.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtpldsgnee.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.bjfxy.top/gtdmsxarvi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtzwllynxk.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtbecywode.html

Ruby: e.message;  e.backtrace
来源：http://hz.havefunace.top/gtsgnillzk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtslfzqnrb.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gtxxivdldr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtevijhorz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenzaomai.com/gttdpoimdj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtjzphbkdn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtbvibswbp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.kuanghao11.cn/gtgxfhzvcj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgfzy.top/gtqquuodci.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daxiang520.top/gtrlyouosd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gttvdmzhfn.html

[H10] 资源自动释放
来源：http://hz.gzhubu.top/gtmzagpesw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aibaodan.cn/gtgvbsftvc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtnffzrxcv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gthjsfpxps.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtgblgmszf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuetiantiany.cn/gtnghueuhk.html

Go:   defer f.Close()
来源：http://hz.svipenyu.cn/gtxmgiesms.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gttaqpxkod.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gzhubu.top/gtburumzxm.html

================================================================================
来源：http://hz.cdnleiting.top/gtgruhzgku.html

I. 正则表达式
来源：http://hz.cashguo.top/gteejgisus.html

================================================================================
来源：http://hz.shzxlz.cn/gtmfawgxbk.html

[I01] 判断是否匹配
来源：http://hz.aibaodan.cn/gtpltndvbz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtkorsumvr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnqzz.top/gtozybwqai.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtwaeetlhq.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtycfhakkb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtuwdgfwau.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ydjk.org.cn/gtezquibrk.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtqolafyqt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cashguo.top/gthbcehzay.html

[I02] 提取所有匹配
来源：http://hz.c1oappe.top/gtxqkdioqi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtpctnakay.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtpcahfqzp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cqqwz.cn/gtdgkbftuc.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtpanjjzqe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zycfv.cn/gtnlisikkq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtprwzyrhb.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gteyfholki.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xziqi.cn/gtkdmxrset.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtdkbkvogj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gotoacloud.top/gtxpmqtmok.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dianchejie.cn/gtfcrqjjih.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtzbjdoqnw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtgqnydjgx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgfzy.top/gtbbelgfkv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtqefszsbt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtukdmwsge.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtfkmwppxk.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtdnrjxnmx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yangfankeji.com/gttmmdlwrj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtotqlfkvg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtafqazife.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtbpyytfbf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aizwys.cn/gtmesrsefm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gturlbdumx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtiibivbfv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtrvkrxlbq.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtulkuorie.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gtjknuxwat.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtyntxodli.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtqgzvienb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtmrybhfnb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtgtzzjuhi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.quarkkingdee.top/gtfwucswwx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtrsygpiwt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aizwys.cn/gtffwgtleq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtzhnjrqdw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtqiperznc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gthntrhxsz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dianchejie.cn/gtlgnahydo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtrpcdqeul.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtyiixbbiw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtgexfpqhc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtwjyvuciq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gttfbbpdtk.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtkaxngojf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtvqwjihza.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtugiahgwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gturiwrait.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtdirrajfh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtjlcdrbib.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtzhqjjaxo.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtbhhjulfi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuetiantiany.cn/gthhrzrydh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hongshengwenyu.top/gtufzftlgo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtchvgpcpe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtvjsvqslx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtyecvdwly.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtfeqszmwb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtlsqqgihc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gthbbqipcy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinyuanbaomall.cn/gtjdamukip.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtgabdpbtm.html

================================================================================
来源：http://hz.wangdashe.top/gtgmmgepcl.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtfmgsfqty.html

================================================================================
来源：http://hz.tianlin.xyz/gtjkbrzhkf.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtuffkpwtl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.svipenyu.cn/gtukwilcsc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtzxsxkdku.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtjapfaklq.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtaqwuryum.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tanke756.top/gturyudios.html

Go:   time.Now()
来源：http://hz.0kj1m.cn/gtjpdxzzif.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtgslwjxoi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtzghhbgef.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtvbgfkspz.html


<!-- 参考信息 -->
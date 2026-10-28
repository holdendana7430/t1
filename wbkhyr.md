代发 wailian999

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtjmydomjo.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.haohaochexian.top/gtlgnsnriu.html

[G04] 定义方法
来源：http://hz.c1oappe.top/gtekorfzbz.html

Py:   def greet(self): return self.name
来源：http://hz.cashguo.top/gthexinqas.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtigpsmjab.html

JS:   greet() { return this.name; }
来源：http://hz.pycfn.com/gtyukoohbt.html

TS:   greet(): string { return this.name; }
来源：http://hz.cdnleiting.top/gthukhwppg.html

Java: String greet() { return name; }
来源：http://hz.xuanzx.com/gtlzbkhsiv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtfanjvycp.html

Ruby: def greet; @name; end
来源：http://hz.gaohongyu789.top/gtehgfinee.html

C#:   public string Greet() => Name;
来源：http://hz.cheryme.top/gtwmbhmlcc.html

[G05] 继承
来源：http://hz.andypj.xyz/gtebigtwsf.html

Py:   class Admin(User): pass
来源：http://hz.jyoumei.cn/gtwnlnxhsk.html

PHP:  class Admin extends User {}
来源：http://hz.hammf.cn/gtzdmbhveb.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtlmsuqsjr.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtaawduzop.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtkmvyxqwf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cashguo.top/gtiiaxngwl.html

Ruby: class Admin < User; end
来源：http://hz.chenlongwang.top/gtvgrwchcx.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtyvisukrz.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtiyvihazj.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtewwpgjva.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yueranfly.top/gteaqmbyha.html

JS:   greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtalhaejph.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtflnahsvp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sxryk.cn/gtjmvbhjzu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ydzc1.top/gtsiswmraj.html

Ruby: def greet; "admin"; end
来源：http://hz.guannengcc.top/gtoyikbzhx.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtxglslhmf.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtvmvmhool.html

Py:   super().greet()
来源：http://hz.tian-w.cn/gtocpbdgjf.html

PHP:  parent::greet();
来源：http://hz.cashguo.top/gtuqwsqdih.html

JS:   super.greet();
来源：http://hz.jinqigfzy.top/gtevvjqyhe.html

TS:   super.greet();
来源：http://hz.hysaishi.cn/gtulexxvom.html

Java: super.greet();
来源：http://hz.daxiang520.top/gtozvymkcm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtgqbonebe.html

Ruby: super
来源：http://hz.wangdashe.top/gtjygodwqa.html

C#:   base.Greet();
来源：http://hz.havefunace.top/gtozhnxjjx.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtwuqzyejj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tian-w.cn/gtqcckgkqs.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtqtshfpjx.html

JS:   static f() {}
来源：http://hz.feifeiyinyue.top/gtkceykfly.html

TS:   static f(): void {}
来源：http://hz.jqgfzy.top/gtwriworsc.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtcfyxquda.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sweek.top/gtuhuqobbc.html

Ruby: def self.f; end
来源：http://hz.yj20258.top/gtusdwpsuq.html

C#:   public static void F() {}
来源：http://hz.fengsongda.top/gtcwrlbkmu.html

[G09] 接口 / 抽象类
来源：http://hz.meibo888.top/gtktloucno.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtdbdbmfib.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gtmhqgnldu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ywan-chungtsiang.top/gtsmyhidjl.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtzoctdtzz.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtbydsanzp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gtbzblpoiy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gteqnwtzka.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtfufzbidb.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gteynebpnz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hfpthk.cn/gtfuplewce.html

PHP:  public / protected / private
来源：http://hz.tanke756.top/gtfzpegkcn.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtqgcbbutx.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtyxpnlvvj.html

Java: public / protected / private / 默认包级
来源：http://hz.jyoumei.cn/gtlrlfaxyq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtrokrivzh.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gtwaruxzfo.html

C#:   public / protected / private / internal
来源：http://hz.hywenlv.cn/gtsuvzhcjh.html

[G11] getter / setter
来源：http://hz.cqqwz.cn/gtxrysjokw.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtlxrvufwe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ivvv.top/gtpkzwmtys.html

JS:   get name() { return this._name; }
来源：http://hz.hammf.cn/gtmzeglhew.html

TS:   get name(): string { return this._name; }
来源：http://hz.daria6918.cn/gtjszozekf.html

Java: public String getName() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtyibpuery.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtnxuyevzf.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtwaxxoiou.html

C#:   public string Name { get; set; }
来源：http://hz.birdmap.top/gtpyireuyh.html

[G12] 对象转字符串
来源：http://hz.ywan-chungtsiang.top/gtctnzvmvc.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtftycwtrh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtjumhjtbs.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtepfzfzpw.html

TS:   toString(): string { return this.name; }
来源：http://hz.pycfn.com/gtxcauhfgb.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtxmwlyotf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nwbrower.top/gtdjrvjrcx.html

Ruby: def to_s; @name; end
来源：http://hz.ivvv.top/gtejqclqdc.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtpazsszlb.html

[G13] 判断对象类型
来源：http://hz.gaohongyu789.top/gtiutxsusx.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gtjofqldck.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gttoexwqgb.html

JS:   u instanceof User
来源：http://hz.jlsjyb.cn/gtddfpxpli.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtquklwlgg.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gthusevxkc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daria6918.cn/gtdkpjwlll.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtdudngrhj.html

C#:   u is User
来源：http://hz.yueranfly.top/gtnhxwusco.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtaihsfnjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtjidusmik.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.meibo888.top/gteeryptlf.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtfawnapfr.html

TS:   type User = { name: string; age: number };
来源：http://hz.andypj.xyz/gtmczqarub.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtohhszzcj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.52xcode.cn/gtbkhloakz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtihpuochn.html

C#:   record User(string Name, int Age);
来源：http://hz.chenjidiqi.icu/gtqpypliya.html

[G15] 枚举
来源：http://hz.ydjk.org.cn/gtrdtcxfjg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtdeaobtak.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtxnnlhkco.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gotoacloud.top/gtepnkvnvy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ybcxt.top/gtvpnuxept.html

Java: enum Color { RED, GREEN }
来源：http://hz.jyoumei.cn/gttaxeqyxg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yongpay.top/gtbpfcpebt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtfpqfxopx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ehwqpu.com/gtptczzujm.html

[G16] 对象转数组 / 字典
来源：http://hz.yj202588.top/gtufamzjyx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gthwepwdmy.html

PHP:  get_object_vars($obj);
来源：http://hz.redwolf501.top/gteqcsmxnd.html

JS:   Object.entries(obj)
来源：http://hz.yanxiufei.cn/gtkjibgomb.html

TS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtydyvragy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xinyue.icu/gtmiikyamv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj20258.top/gthxcdmxgu.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtmxxlyuhy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtsqohywvh.html

================================================================================
来源：http://hz.zhongyouzk.top/gtxzlknnme.html

H. 异常与错误处理
来源：http://hz.hfpthk.cn/gtqmoydfbl.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfyrpnbyg.html

[H01] try / catch 基础
来源：http://hz.hnxiangtu.top/gtgmmwxyft.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ivvv.top/gtctqxiavv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtaahktpho.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ybcxt.top/gtclwjuvjq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj202588.top/gtoxnoxcyr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gthfjmopgv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhengqikj.top/gtsskvcksk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtxbtzsslv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zycfv.cn/gthcgghcyq.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtwmdqnvyr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtlbldpnht.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtooewzggz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gteckxfsvi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtkenefqbm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtlaadqbwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.9152youxi.cn/gtglxdwnwy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtbibxvbrn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtulqmvbza.html

[H03] 主动抛出异常
来源：http://hz.feifeiyinyue.top/gtwabmpyve.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj20258.top/gtdejyesnd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtosafptec.html

JS:   throw new Error("错误信息");
来源：http://hz.guannengcc.top/gtktgqfpys.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtbsgfvloa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtdqbtwsva.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtfaeyyzqj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtlxfptcnx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gaohongyu789.top/gtuxrhjhel.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtlbloemjl.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtwvvqnxff.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtalexdgvr.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtqpjkoydf.html

TS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtgzoiygmv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtpzpfrpmg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gtyfziewdt.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydjk.org.cn/gtpkcvnxdu.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtzuiltsoq.html

[H05] 捕获特定类型
来源：http://hz.0kj1m.cn/gtpucyehzj.html

Py:   except ValueError as e:
来源：http://hz.nwbrower.top/gtqbecxiwe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tianlin.xyz/gtruubhlps.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtjimaappe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtzihcurkk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtcmvqeavt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tian-w.cn/gtnspnslnt.html

Ruby: rescue ArgumentError => e
来源：http://hz.shuidangran.top/gtdhkridco.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gtnxsucnbq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hongshengwenyu.top/gtsasboeas.html

Py:   value = d.get("k") or default
来源：http://hz.mhx1999.top/gtvomdiggq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xingfuxueyuan.xyz/gtoovixhoj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtavzfwflg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtadlhdhjq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtoxbaujhd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtbgfweqbe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pycfn.com/gtfguffkcn.html

C#:   obj?.A?.B ?? default
来源：http://hz.quarkkingdee.top/gtcisgykuf.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtnexywhdk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtffvddvso.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtbyoedbcr.html

JS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtvfypberb.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtxkeqhzaq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigfzy.top/gtfvqmiwcr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.meibo888.top/gtyzdvcxwh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jlsjyb.cn/gtaehejpah.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtgnsbmibg.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuetiantiany.cn/gtjyfgzuih.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtbgfabbdq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtwsmuopgg.html

JS:   e.message;  e.stack
来源：http://hz.fengsongda.top/gtkyragdnz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xziqi.cn/gtexovimot.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtfrterupf.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtwxswzjqo.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinyuanbaomall.cn/gtdlkhxfum.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtpghmelvc.html

[H09] 带错误码的异常
来源：http://hz.zhiwuduotai.top/gtaftyiutp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gogol.net.cn/gtzozzedtc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gtzzxwscgv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtfrcndbsc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtsnmefozv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtgejfjdeb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtrponitpu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtdgvtwiki.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtnrjijlol.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtuxkvesbj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hammf.cn/gtxcfxodmu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtgrpmqlrm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtxhniwbmn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtxuueazer.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fzhhl.top/gtekgjlbox.html

Go:   defer f.Close()
来源：http://hz.zhoulong.xyz/gtvbzsnyid.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ppjwa.cn/gtpouucgdg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtwarwxlgm.html

================================================================================
来源：http://hz.dashuyun.cn/gtwjzupfgn.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtjmmmqqiv.html

================================================================================
来源：http://hz.gotoacloud.top/gtdvpcbjpu.html

[I01] 判断是否匹配
来源：http://hz.vqdsnc.cn/gtbgdzbbph.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigufen.top/gtchmktwsm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtlmzhaxna.html

JS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtjzbplhsb.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtwbanghnf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtepnrtvxp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xziqi.cn/gtijaiklgc.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtrzqmshir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtsqfedlwk.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtewdxlqdn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtiodcvopi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtttdemprw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sweek.top/gtakhroehm.html

TS:   s.match(/\d+/g)
来源：http://hz.andypj.xyz/gtevqvqftj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtjfqhoryx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtplpscrhx.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtgdsbsegc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zycfv.cn/gtzpveqxqm.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtcsicmbgq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daxiang520.top/gthivmecsm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtgreabexq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtiipuoxrk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hammf.cn/gttbnierei.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtnwwsupxg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gtggfxdkfr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtloddvtfe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtesbsxsqz.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtbobhxrvm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gteqdzfbzs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gtdputhnyv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtdflahwuw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtiypzzfbz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gterlmvxyn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtdtmhriep.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtkntpetbb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cucudq.cn/gtncpvdvuo.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtunbvesup.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gtkkdtdcoj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtvklybjkr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtvyvrfcaj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtsebjnoox.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtzripqbqw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zdqjudy.top/gtlwlyrgcw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtuqtxhgxs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtaxtyfsyk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangkeji.top/gtqgbatwhz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtxealkjaf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cheryme.top/gttdqhfpbg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtsuzoqivf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtbfsifagg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pengpengdd.cyou/gthxtxkrqp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhoulong.xyz/gtjrbleehm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtuyucafzd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtbkstvprd.html

[I07] 忽略大小写与多行模式
来源：http://hz.daria6918.cn/gtvjmldffl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtobqltpfn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtutcnxytn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtvzrooyxp.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtluiscnji.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gtadtvmjdh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gthevzkwum.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtvmcjpycl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtrbrzjhjv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtjckxgyqy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtpjobwacr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yangfankeji.com/gtkvkicdkd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtqmxoxgxt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtvpfkhvhm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gttztvrrsh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtfixtvepx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtekhpfmex.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtjoibagmo.html

================================================================================
来源：http://hz.yj20258.top/gtbcvuwdhh.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtucvaesrq.html

================================================================================
来源：http://hz.yongpay.top/gtygnfwejw.html

[J01] 获取当前时间
来源：http://hz.hywenlv.cn/gtzlalqmly.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnxiangtu.top/gtafjufsrz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtfjyrqgka.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtpkimwwzw.html

TS:   new Date();  Date.now()
来源：http://hz.snrcjt.cn/gtibrfpdrm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtzdndglok.html

Go:   time.Now()
来源：http://hz.andypj.xyz/gtonghbtnk.html

Ruby: Time.now
来源：http://hz.cashguo.top/gtrjvrdpok.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtfdykriyi.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtzxrafolh.html


<!-- 参考信息 -->
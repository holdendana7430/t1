代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.mhx1999.top/gtpzbekgmq.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtqnduhxhk.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtxoqhidng.html

TS:   class Admin extends User {}
来源：http://hz.gaohongyu789.top/gtoxxtnbmw.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtjtbpuecy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtluzpueff.html

Ruby: class Admin < User; end
来源：http://hz.svipenyu.cn/gtztlwrger.html

C#:   class Admin : User {}
来源：http://hz.dashuyun.cn/gtxbhfmxrf.html

[G06] 重写方法
来源：http://hz.pycfn.com/gtprhorsur.html

Py:   def greet(self): return "admin"
来源：http://hz.zhaomingkeji.xyz/gtlwcbcubf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yonumen.top/gtiraqxtjc.html

JS:   greet() { return "admin"; }
来源：http://hz.yvedp.cn/gterztinrg.html

TS:   greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtkbsmudei.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.pycfn.com/gtbavfspqv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.52xcode.cn/gtsjktqhbr.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gtmlrclihz.html

C#:   public override string Greet() => "admin";
来源：http://hz.xinyue.icu/gtvsrssiow.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtsirfazmr.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtdhxnttte.html

PHP:  parent::greet();
来源：http://hz.andypj.xyz/gtqnfoypit.html

JS:   super.greet();
来源：http://hz.xuanzx.com/gtyayruwoj.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtgqgbydmy.html

Java: super.greet();
来源：http://hz.shanyushiyangkeji.top/gttoqnakvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinghuilouyu.cn/gteigvttxp.html

Ruby: super
来源：http://hz.iojbl.cn/gtroekidoy.html

C#:   base.Greet();
来源：http://hz.gaohongyu789.top/gtuxbsxkwf.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangkeji.top/gtefqbyzev.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yanxiufei.cn/gtwoaomlhm.html

PHP:  public static function f() {}
来源：http://hz.0kj1m.cn/gtkguahroa.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtaorddqhp.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gtzjcgwkja.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gtvfvshymd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.nanxinkj.top/gtyugxtryy.html

Ruby: def self.f; end
来源：http://hz.dashuyun.cn/gtskgwoeqv.html

C#:   public static void F() {}
来源：http://hz.gogol.net.cn/gtslefcjrx.html

[G09] 接口 / 抽象类
来源：http://hz.nwbrower.top/gtqkhcqlaw.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gtmqjadcyw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.dianchejie.cn/gtdpiqleoc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gttrkcnqps.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtoacyzylc.html

Java: interface Shape { double area(); }
来源：http://hz.shangyingyoupin.top/gtxegpoewi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtqzyjtxns.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.pycfn.com/gtnyevilel.html

C#:   interface IShape { double Area(); }
来源：http://hz.shzxlz.cn/gtebzybrdy.html

[G10] 访问控制
来源：http://hz.zhongyouzk.top/gtmzbkqcox.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtnbouqhsk.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtzyrljaos.html

JS:   #private 字段；其余公开
来源：http://hz.xylfe.cn/gtgedspyva.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtiluludih.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtfkhvjhkr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.meibo888.top/gthmqcqrqo.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtswptmjrz.html

C#:   public / protected / private / internal
来源：http://hz.aibaodan.cn/gtmdobywhm.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gthhtkzemb.html

Py:   @property 与 @x.setter
来源：http://hz.yuanzhike.top/gthwsxumnj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhongyouzk.top/gttwydvjbw.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtrvjymizc.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtilsazuvc.html

Java: public String getName() { return name; }
来源：http://hz.yueranfly.top/gtlwbiqyep.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.wangshuangyany.cn/gtuordwdfd.html

Ruby: attr_accessor :name
来源：http://hz.yj20258.top/gtvlwpkxhe.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gtwkpywhvj.html

[G12] 对象转字符串
来源：http://hz.chenjidiqi.icu/gtikxxkqiw.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigfzy.top/gtzfbasikz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtufketrru.html

JS:   toString() { return this.name; }
来源：http://hz.ydjk.org.cn/gtzzhmsmwq.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtnpwofwrd.html

Java: @Override public String toString() { return name; }
来源：http://hz.chenjidiqi.icu/gtegyjcjax.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtkxgrwgcq.html

Ruby: def to_s; @name; end
来源：http://hz.yuanzhike.top/gtwwhfwwzt.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtldvwgckn.html

[G13] 判断对象类型
来源：http://hz.hnxiangtu.top/gtxsyjwcqi.html

Py:   isinstance(u, User)
来源：http://hz.yuxming.cn/gtustnzgcy.html

PHP:  $u instanceof User
来源：http://hz.xuetiantiany.cn/gttzoyfauk.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtovbvtucp.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtyznnbvfr.html

Java: u instanceof User
来源：http://hz.andypj.xyz/gtfymjnsfz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.pycfn.com/gtofifhgrd.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtzwhhmzda.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtuzmzkhco.html

[G14] 数据类 / record
来源：http://hz.jqgfzy.top/gtgontazza.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.meibo888.top/gtqbsawzzv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hfpthk.cn/gtoeywijjl.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gtbwddvhpp.html

TS:   type User = { name: string; age: number };
来源：http://hz.c1oappe.top/gtdyhhrdqw.html

Java: record User(String name, int age) {}
来源：http://hz.dianchejie.cn/gthercyddv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sufxvd.cn/gtotqjioms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.bjfxy.top/gtprwxleyc.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtwashfeoj.html

[G15] 枚举
来源：http://hz.jinqigufen.top/gtziiokpha.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhoulong.xyz/gtcgythbzo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.feifeiyinyue.top/gtntmgpnch.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtnclwiafr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenlongwang.top/gtaeekxrtq.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtvqhcuclp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtpbevfnop.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangshuangyany.cn/gthiftbvdh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtcfsauctm.html

[G16] 对象转数组 / 字典
来源：http://hz.jinqigufen.top/gtbozcsmdr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tanke756.top/gthreaxbcx.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtzjslpppb.html

JS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtojowgjpi.html

TS:   Object.entries(obj)
来源：http://hz.pycfn.com/gtptgfawxc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jiagoushi.top/gttuduyvle.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.haohaochexian.top/gtbvwhaxea.html

Ruby: obj.instance_variables
来源：http://hz.cheryme.top/gtvlklspwo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.snrcjt.cn/gtfqkylfom.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqzxjhmnf.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtzxzjghps.html

================================================================================
来源：http://hz.daxiang520.top/gtlcgyrbaj.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtbrynqanf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtglextokf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.shuidangran.top/gtzfzrlhqt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtycxwjtdu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.vqdsnc.cn/gtgwozbram.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sufxvd.cn/gttztrpapt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gttbcxjrmw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gaohongyu789.top/gtcrbcbbic.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtvoxzmcbj.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtrwenhxvl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtmqxwgdwp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtalbukkhi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtxoqcztzx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtakwdlebz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtmelgooro.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtetvaolry.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.daria6918.cn/gtklkuwbud.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.birdmap.top/gtmdlpinod.html

[H03] 主动抛出异常
来源：http://hz.kuanghao11.cn/gtjikbadyj.html

Py:   raise ValueError("错误信息")
来源：http://hz.hongshengwenyu.top/gtlxtthuro.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtgawecqkw.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtehxgpvcn.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtggjezsjs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtoetmisqo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtlazpuemb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtbzeoeoma.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtrvhramri.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtymekppzc.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtblhfoqnv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtosvozuqn.html

JS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtwreuxnbd.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtgobdmipg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jianghu66.top/gtejhlbxvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yangfankeji.com/gtsmthcwoy.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtnbsghtua.html

C#:   class MyException : Exception {}
来源：http://hz.xylfe.cn/gtruhbidmq.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtwbggcdbr.html

Py:   except ValueError as e:
来源：http://hz.yuanzhike.top/gthugoqdna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtdcvvcqyr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gteefotcyk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.meibo888.top/gtkbhraplu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.svipenyu.cn/gttsxgnkmp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtdjrrlflz.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtpqbmvcwu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtrsvrzwhy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtfzusdcjc.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtxviybnjj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtgkxxykkv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtbdvnuxwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtiztwfnht.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtghiseosb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtsreubrdw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtkdjnnjvj.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtokynvmdt.html

[H07] 断言
来源：http://hz.jyoumei.cn/gtobfdfpwe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cdnleiting.top/gtajbdgzbh.html

PHP:  assert($x > 0);
来源：http://hz.yuanzhike.top/gtpapzhoyw.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtyifgaxjt.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtfpahtzkl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xylfe.cn/gtosuuptjw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aibaodan.cn/gtesfhgiso.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtcegtqulv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daria6918.cn/gtzxcrwswj.html

[H08] 获取错误信息与堆栈
来源：http://hz.jianghu66.top/gtupgzxefv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.mhx1999.top/gtwexbvguw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.wangdashe.top/gtupcctegf.html

JS:   e.message;  e.stack
来源：http://hz.zhijiandao.cn/gtuvboadqc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtpqnhxpdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtvbbekbdg.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtppdimvvf.html

Ruby: e.message;  e.backtrace
来源：http://hz.andypj.xyz/gtwqwdxpoi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtpfhwiqne.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtslyamiyh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daxiang520.top/gtrdoakzps.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hysaishi.cn/gtqlrvjpbh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.iojbl.cn/gtcpurjgyo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtkeumkcfg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtvxnzorlq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtrzzbwkpn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtcpwjxzfk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xingfuxueyuan.xyz/gtkoywnnzy.html

[H10] 资源自动释放
来源：http://hz.quarkkingdee.top/gthspfdofm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtdpvfrxmm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yonumen.top/gtgnxedemv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtjkfnrapm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtpktfjgzi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xinyue.icu/gtktspjvim.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtbjoatysv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtiraxvkql.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangdashe.top/gtzavsywtz.html

================================================================================
来源：http://hz.cdnleiting.top/gtiujkyxep.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtkvlsddlc.html

================================================================================
来源：http://hz.tanke756.top/gtmnrycqna.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtwqiduxfp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtylhfdhde.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gtmqdqzark.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtukogfcox.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtyktbpzfg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtvqljxnir.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gtbsttsfff.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuanzx.com/gtcybqyijn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.smart0.xyz/gtfgqpvkln.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtzohawkhy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtdwvzqsub.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtojazujsq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gthqbbgdvx.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtjylzljog.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtzixhkeyb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhiwuduotai.top/gtwhczfcrz.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258.top/gtennxsdgd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gthhphybhi.html

[I03] 提取捕获分组
来源：http://hz.ywan-chungtsiang.top/gtynfeoqow.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtjaysgupj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gttwtwmmgd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.aibaodan.cn/gtbtomzmno.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.iojbl.cn/gtlzbcvwza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtpyhplkhl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtqwdtrfyh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtljbimagi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtvagnsbrc.html

[I04] 正则替换
来源：http://hz.hywenlv.cn/gtikhygdny.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtuofgydtl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtkcspgqyk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtopanoyfj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtjwzkxnxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtulqrxmya.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daria6918.cn/gtqecwkdzk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gttxzqenzl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtncszodor.html

[I05] 按正则拆分
来源：http://hz.yongpay.top/gtssvqsxfp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtwxqtweia.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtmmwwojux.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtbqalanpb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtmsahxgup.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtbuknvhyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuanzhike.top/gtablwjyik.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtzjsfvodb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nwbrower.top/gtzjnbkkfp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtuipmyrfi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtfztezcie.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gtpdojoebd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gteuryhhmc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gthtxgxguk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ybcxt.top/gtbmuauscv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtbttvmcib.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gtbnkjwgnc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtulpivpzd.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtcqdsphjr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtvofprsls.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtiagadhzt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtlthqiekm.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtegbzqiwd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtmlwbbreb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtpjdafarf.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtythvjxns.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtgglnfbvv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guowangkeji.top/gtdcjuesnd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xziqi.cn/gtshcyvduk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtnsosbclw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtpplfjgph.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtdbfhjypp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258.top/gtmogfylzy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgufenzy.top/gtvkjkkrec.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtgxkjqyae.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtgkmznyec.html

================================================================================
来源：http://hz.jyoumei.cn/gtifyvirgv.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtcsnuxndi.html

================================================================================
来源：http://hz.guannengcc.top/gtlhevmogo.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gthllgqzgi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtwuuvfack.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtmmxrekgo.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtjwmezmfo.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtzdamktwc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gtevxstnjv.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtqsijcrvu.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtpzetgsls.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtyehxklae.html

[J02] 格式化输出
来源：http://hz.havefunace.top/gttjpyjdmi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtmzadcuwh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gttrezucve.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtgxkytqog.html

TS:   d.toISOString()
来源：http://hz.havefunace.top/gtfrcryvpp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtnjafddgi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtmmkbhtxp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtwdeucnsv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtegtkbcmf.html

[J03] 字符串解析为日期
来源：http://hz.c1oappe.top/gtpiamiagz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hysaishi.cn/gtafowaspr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gtuyynrlfx.html

JS:   new Date("2024-01-02")
来源：http://hz.yonumen.top/gtivmiwfyq.html


<!-- 参考信息 -->
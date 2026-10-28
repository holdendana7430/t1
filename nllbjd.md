代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.tianlin.xyz/gtecrabdse.html

PHP:  class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gthxsvhvsi.html

JS:   class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtmnxmuqiq.html

TS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtiaqityqf.html

Java: class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtsqotmzpy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtajpdpwdf.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtfuxpigbg.html

C#:   class Admin : User {}
来源：http://hz.iojbl.cn/gtlgiskbrf.html

[G06] 重写方法
来源：http://hz.hnqzz.top/gtnwidlcil.html

Py:   def greet(self): return "admin"
来源：http://hz.yvedp.cn/gtunhzwsrj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtlpxmbuph.html

JS:   greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtunvhouty.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtqhvmwily.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.redwolf501.top/gtrakemuhr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtxscwlwqo.html

Ruby: def greet; "admin"; end
来源：http://hz.gaohongyu789.top/gtpzsjwuhx.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtrfkdpcwj.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gteptalljm.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtcgptidzn.html

PHP:  parent::greet();
来源：http://hz.cheryme.top/gtmnuclsfn.html

JS:   super.greet();
来源：http://hz.guowangkeji.top/gtsxtqlxuo.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtmuozdroc.html

Java: super.greet();
来源：http://hz.tanke756.top/gttppnyulb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtrurszvay.html

Ruby: super
来源：http://hz.dianchejie.cn/gtlpsfxghg.html

C#:   base.Greet();
来源：http://hz.zhaomingkeji.xyz/gtyhlnnjgh.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtqdaokgqk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gtexytccht.html

PHP:  public static function f() {}
来源：http://hz.fzhhl.top/gtombcntnp.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtaelalifm.html

TS:   static f(): void {}
来源：http://hz.hywenlv.cn/gtqijhqwxy.html

Java: static void f() {}
来源：http://hz.zhixingplan.top/gtsihopenb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtmnvtgzip.html

Ruby: def self.f; end
来源：http://hz.sweek.top/gtivbjskcq.html

C#:   public static void F() {}
来源：http://hz.nanxinkj.top/gtjqsipvke.html

[G09] 接口 / 抽象类
来源：http://hz.jqgufenzy.top/gtjumegrii.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtvvqtzxmc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtouihcfqt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gtvjunwsbt.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtcxtwmbvr.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtpjfbxzjj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtrnfxxgkh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shangyingyoupin.top/gtrxepwhwa.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtnomknpzs.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtfbvifzjk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gotoacloud.top/gtdlshyxbk.html

PHP:  public / protected / private
来源：http://hz.bjfxy.top/gtezztbiey.html

JS:   #private 字段；其余公开
来源：http://hz.ydjk.org.cn/gtgfcrsbtd.html

TS:   public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtrsaverck.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtfzkehjyp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.vqdsnc.cn/gtagvsowmn.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtbvigusvb.html

C#:   public / protected / private / internal
来源：http://hz.jyoumei.cn/gtedaoqloe.html

[G11] getter / setter
来源：http://hz.daria6918.cn/gtqaledjgt.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtvfpawqdv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtgjtqefyo.html

JS:   get name() { return this._name; }
来源：http://hz.pengpengdd.cyou/gtfrqxqvrv.html

TS:   get name(): string { return this._name; }
来源：http://hz.hnxiangtu.top/gtehwnwiym.html

Java: public String getName() { return name; }
来源：http://hz.hongshengwenyu.top/gtplnjvhas.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.iojbl.cn/gtoobektro.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gteqbfzcoy.html

C#:   public string Name { get; set; }
来源：http://hz.zhiwuduotai.top/gtvvplniib.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtxbupdhjz.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtnaafycsx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtcxzlvrdd.html

JS:   toString() { return this.name; }
来源：http://hz.yueranfly.top/gtwbmzqvmb.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtwixfhwue.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtukgpzhjq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgufenzy.top/gthmbdmwmw.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gteyzufovn.html

C#:   public override string ToString() => Name;
来源：http://hz.xuanzx.com/gtuzgileus.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtanqgpdwd.html

Py:   isinstance(u, User)
来源：http://hz.9152youxi.cn/gtoxhjsetj.html

PHP:  $u instanceof User
来源：http://hz.hnqzz.top/gtfhlzhiiq.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtzblakxlj.html

TS:   u instanceof User
来源：http://hz.dashuyun.cn/gtxhmdhqzo.html

Java: u instanceof User
来源：http://hz.zhengqikj.top/gtmefazgdr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtdjasnvfw.html

Ruby: u.is_a?(User)
来源：http://hz.yuxming.cn/gtqcfeygki.html

C#:   u is User
来源：http://hz.ydzc1.top/gtreqirlff.html

[G14] 数据类 / record
来源：http://hz.haohaochexian.top/gtmpwnkupt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.xingfuxueyuan.xyz/gthdjjexyc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtqnuoblik.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtwqfcccfz.html

TS:   type User = { name: string; age: number };
来源：http://hz.hfpthk.cn/gtrkjpafch.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gtrahlexjl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.daxiang520.top/gtebpgiypo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jyoumei.cn/gthlgvdtlf.html

C#:   record User(string Name, int Age);
来源：http://hz.hnxiangtu.top/gtprdkusdi.html

[G15] 枚举
来源：http://hz.xingfuxueyuan.xyz/gtaouhzeqn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenlongwang.top/gtlqmedrvg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtophnwgfe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtknhpkbuz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtcnranret.html

Java: enum Color { RED, GREEN }
来源：http://hz.0kj1m.cn/gtnqnpmdlp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtvyavwhpl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtdbhudnbw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtgsdylcvu.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtzupgrpsr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhijiandao.cn/gtfqbkjuog.html

PHP:  get_object_vars($obj);
来源：http://hz.cucudq.cn/gtqkjfszmz.html

JS:   Object.entries(obj)
来源：http://hz.pengpengdd.cyou/gtkumtucfw.html

TS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtjfrusltf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.svipenyu.cn/gtorampwku.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtxpszsoho.html

Ruby: obj.instance_variables
来源：http://hz.yueranfly.top/gtwojikvoe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhongyouzk.top/gtmokkxgto.html

================================================================================
来源：http://hz.gzhubu.top/gtdzcuqhyf.html

H. 异常与错误处理
来源：http://hz.xuanzx.com/gthdpryzux.html

================================================================================
来源：http://hz.zdqjudy.top/gtlkpyokhc.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtveqhjfre.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.andypj.xyz/gtdmgaixpg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtlfhgcgfg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gtohuldnkq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtteueqfhr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yj202588.top/gtmpdhzrei.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhoulong.xyz/gtdbfbpzmg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtpfbgznlj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtzerespss.html

[H02] finally / ensure 收尾
来源：http://hz.cashguo.top/gtbpeqqgaq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shangyingyoupin.top/gtogorpxfj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtdegaexzq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtpldidifo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtuiygylor.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtrwohcbvl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtvagdggde.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtqmrpynhw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydjk.org.cn/gtpvcvvolg.html

[H03] 主动抛出异常
来源：http://hz.gogol.net.cn/gtfyryfkdx.html

Py:   raise ValueError("错误信息")
来源：http://hz.jiagoushi.top/gtehntsptv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yongpay.top/gtmmltlqwr.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtyqzzncif.html

TS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtvjaeqqvj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinqigufen.top/gtldusfqei.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtgtanirid.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtmmlgzgyh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtneuhvlfk.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtzvuztdml.html

Py:   class MyError(Exception): pass
来源：http://hz.zhongyouzk.top/gtgipkhptr.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtpqhnumzu.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtqqcdbuci.html

TS:   class MyError extends Error {}
来源：http://hz.yueranfly.top/gtmmxkbeng.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtfdwrjpdt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtbjynpcxv.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtdpkpocjg.html

C#:   class MyException : Exception {}
来源：http://hz.0kj1m.cn/gtpvjphvvm.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gtpuamqeoa.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gtgwgxcfdc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gtyaarrgnl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtzeyluuni.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtarkqfapr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtguhwcexe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gtagjixkdn.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gttgfgrndu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinyuanbaomall.cn/gtemxwshxt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtrybsaanz.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtsjcihrfj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tianlin.xyz/gtufddhkcw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtfxwhyivz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gtwxurqngm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtqlrvjfei.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtqxsidofx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtgstvlzpf.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtlesfkbak.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtfrjakprs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtcvujbazm.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtjjewqacy.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtjanncicb.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtrdapqaut.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtvxslkfcq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gzhubu.top/gthbmlyjzf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtcyonmbuu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gtzqmzpshg.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhengqikj.top/gtcankhzth.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guannengcc.top/gtbtbmhjsr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gthamhyfnq.html

JS:   e.message;  e.stack
来源：http://hz.sysykeji.top/gtgeseuinz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ybcxt.top/gtebhaxqfm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtgfkldldt.html

Go:   err.Error()
来源：http://hz.smart0.xyz/gthdvxmqfj.html

Ruby: e.message;  e.backtrace
来源：http://hz.jyoumei.cn/gtaptsnpze.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtkoqabcsz.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtxbhkhbtt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtibxtdqni.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtoquuucsj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gtfkavfzgx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gthwqbnuso.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xinyue.icu/gtbbsvdxjz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtwmgxtmjo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtrrggjnid.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tian-w.cn/gtbfimursy.html

[H10] 资源自动释放
来源：http://hz.yangfankeji.com/gtodcefhgj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtmlzheboy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtllttjghm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtmfgasffp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtzrrbojtb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtxvtojbni.html

Go:   defer f.Close()
来源：http://hz.sysykeji.top/gtoqixvube.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtxfsmzbir.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gthzxxqkcc.html

================================================================================
来源：http://hz.pycfn.com/gtfwmuknnw.html

I. 正则表达式
来源：http://hz.yj202588.top/gtijkuzpvl.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtijsixfwm.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gttxxhlstf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtbnnvwjtw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtelmqwbms.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtbmexkzxg.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtnrntpawq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtesstcnro.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtycldusxu.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtlvruklaf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtcdnluzaq.html

[I02] 提取所有匹配
来源：http://hz.zdqjudy.top/gtmjsboxde.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yueranfly.top/gtmogcpnxg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tianlin.xyz/gtihxnujeh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtpvlupsgl.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gteezqueoj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guowangkeji.top/gtpsszbtnd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gtappleelw.html

Ruby: s.scan(/\d+/)
来源：http://hz.jlsjyb.cn/gtbhpghjqh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gttkzypjiz.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtvpdenphn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tanke756.top/gtxrwfwelz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtwxldoznt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gtqjgxsjtc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtfqoabztj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yuxming.cn/gtjlofmksu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtnmonvmow.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aibaodan.cn/gtciwvegvc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.316326.xyz/gtemsclswg.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtusorbybl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jyoumei.cn/gtlvbfxnhf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtvymfeaay.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtkqsjenrq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtpfyksvjb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gthrreakmf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtgrnwieks.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gttkqlzleb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.52xcode.cn/gtjlhbbhuo.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtvokxpwcc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gtmcnssrru.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gtbracarjr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtsqomdqds.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtgkzkctxn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cashguo.top/gtllvlgphl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtswttxood.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtmjxwfzpg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtrywcpmts.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtghcfggex.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtcfhsxqvq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtsxawnqrd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtlpeacqhv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtyhlicceh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gthrauyrek.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtqfnfhzwg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhiwuduotai.top/gtmosmxkvp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtzgmmnncv.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtvtmykehq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gthckxhzas.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtpxaiuxwj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtqtccsbdz.html

TS:   /error/gim
来源：http://hz.hnqzz.top/gtestyilel.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtfjxyfkli.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fzhhl.top/gtugitymyv.html

Ruby: s.scan(/error/i)
来源：http://hz.cucudq.cn/gtjjftdkhu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtbstwfgdt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinyuanbaomall.cn/gtwgjhlptq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gtwtjgsius.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gteugnoqym.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtatkdxgif.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtchfssoch.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gzhubu.top/gtnmvewlpk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.svipenyu.cn/gtudccxoca.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtrnbsptlc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ivvv.top/gtjokowlkh.html

================================================================================
来源：http://hz.iojbl.cn/gtqabtznlt.html

J. 日期与时间
来源：http://hz.zhongyouzk.top/gtodpiyuzo.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrcxtvfca.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtkbbymbdu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtnxlnazkb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtumtmuane.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtmsvfijpr.html

TS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtvjlbalng.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pengpengdd.cyou/gtkocymuwu.html

Go:   time.Now()
来源：http://hz.xuanzx.com/gtgqleusju.html

Ruby: Time.now
来源：http://hz.iojbl.cn/gttpplhvxf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtdxwreruv.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtuomiendb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtaebqubur.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtyvdvdlnk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtvygkuvuv.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtuffbgrjd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jyoumei.cn/gtcnmduxri.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuetiantiany.cn/gtwaaemjuj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtdyjigovd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtsdczfwbx.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtdcuoirek.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtoukdmcqh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtxknyxpph.html

JS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtxskxygfh.html


<!-- 参考信息 -->
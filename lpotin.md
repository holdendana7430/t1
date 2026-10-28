代发 wailian999

[G06] 重写方法
来源：http://hz.sweek.top/gtluvbtdhd.html

Py:   def greet(self): return "admin"
来源：http://hz.jianghu66.top/gtujchabwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtlamfwhtr.html

JS:   greet() { return "admin"; }
来源：http://hz.zycfv.cn/gthivaetap.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gthbrwobhg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtnimmixrl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jqgfzy.top/gtewlyghao.html

Ruby: def greet; "admin"; end
来源：http://hz.jlsjyb.cn/gtsyzbbqkw.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtvguuqulf.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtxjlxbzdq.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtdvhwoect.html

PHP:  parent::greet();
来源：http://hz.guannengcc.top/gtuxvelreb.html

JS:   super.greet();
来源：http://hz.cucudq.cn/gtfqqmlusf.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtkqrruoaq.html

Java: super.greet();
来源：http://hz.wangdashe.top/gtbxcrdnmq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtobfujqhm.html

Ruby: super
来源：http://hz.xuanzx.com/gturhesuaw.html

C#:   base.Greet();
来源：http://hz.ehwqpu.com/gtzdzkqusk.html

[G08] 静态方法与属性
来源：http://hz.zhongyouzk.top/gtvmeixfwl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ivvv.top/gtoskgwauu.html

PHP:  public static function f() {}
来源：http://hz.nanxinkj.top/gtwiayxhhi.html

JS:   static f() {}
来源：http://hz.9152youxi.cn/gtcsalvlre.html

TS:   static f(): void {}
来源：http://hz.meibo888.top/gtegieqztk.html

Java: static void f() {}
来源：http://hz.iojbl.cn/gtubbudszc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtyslqzskq.html

Ruby: def self.f; end
来源：http://hz.ydjk.org.cn/gtavbhtcgk.html

C#:   public static void F() {}
来源：http://hz.sxryk.cn/gttymxmegl.html

[G09] 接口 / 抽象类
来源：http://hz.zycfv.cn/gthrjbdxgo.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangkeji.top/gtbwdxahcj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhiwuduotai.top/gtcmxzscsw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtjdjtyfjq.html

TS:   interface Shape { area(): number; }
来源：http://hz.ehwqpu.com/gtsitwmtvk.html

Java: interface Shape { double area(); }
来源：http://hz.shuidangran.top/gtruzgnhms.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhaomingkeji.xyz/gttpppaqig.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sweek.top/gtygianokl.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtygoyhukx.html

[G10] 访问控制
来源：http://hz.meibo888.top/gtteueorzp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtrosotavy.html

PHP:  public / protected / private
来源：http://hz.aibaodan.cn/gtvkusgkuu.html

JS:   #private 字段；其余公开
来源：http://hz.pengpengdd.cyou/gthyxsmiyf.html

TS:   public / protected / private
来源：http://hz.daxiang520.top/gtgcbddjhw.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtyaqfjrtw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guannengcc.top/gttpbtwjcb.html

Ruby: public / protected / private
来源：http://hz.dashuyun.cn/gtofmiuhcg.html

C#:   public / protected / private / internal
来源：http://hz.quarkkingdee.top/gtrabkifvr.html

[G11] getter / setter
来源：http://hz.zhaomingkeji.xyz/gtrileyehh.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gtggyhrxah.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtntcnxruk.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigfzy.top/gttbrefftp.html

TS:   get name(): string { return this._name; }
来源：http://hz.andypj.xyz/gtpgvzspjs.html

Java: public String getName() { return name; }
来源：http://hz.tian-w.cn/gthasrlzod.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtsffrhsuc.html

Ruby: attr_accessor :name
来源：http://hz.shuidangran.top/gtsobmegcx.html

C#:   public string Name { get; set; }
来源：http://hz.nwbrower.top/gtdfrlqsyd.html

[G12] 对象转字符串
来源：http://hz.daxiang520.top/gtpkyynyds.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtvduxkzkk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtipaeyerb.html

JS:   toString() { return this.name; }
来源：http://hz.fzhhl.top/gtbwmzojks.html

TS:   toString(): string { return this.name; }
来源：http://hz.xinyue.icu/gtcjhmedhd.html

Java: @Override public String toString() { return name; }
来源：http://hz.daxiang520.top/gttdwjelay.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtjcteagcr.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtzxrxohgf.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtxmalwiig.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gtrprvfhts.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtpblpngoc.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtgsjvniej.html

JS:   u instanceof User
来源：http://hz.cdnleiting.top/gtrocrawoh.html

TS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtozaemdff.html

Java: u instanceof User
来源：http://hz.nwbrower.top/gtgnwizfxq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtsmyzhzpo.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtgwugjlfw.html

C#:   u is User
来源：http://hz.hnqzz.top/gtthvctvha.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtuhlxqxns.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangkeji.top/gtrfwowtyk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtqitcnthn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gttvpfzetn.html

TS:   type User = { name: string; age: number };
来源：http://hz.svipenyu.cn/gtbaenaihm.html

Java: record User(String name, int age) {}
来源：http://hz.zhaomingkeji.xyz/gtvlzqqvgm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shuidangran.top/gtcghdrrjm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtujssqykh.html

C#:   record User(string Name, int Age);
来源：http://hz.tianlin.xyz/gtbumwzpld.html

[G15] 枚举
来源：http://hz.cdnleiting.top/gtuswdwvfb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuanzx.com/gtndwajlrr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.9152youxi.cn/gtwqzexxgz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtxsorzntq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtuiejtzpa.html

Java: enum Color { RED, GREEN }
来源：http://hz.0kj1m.cn/gtksoepvqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtlstozqwf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ybcxt.top/gtpnrucclc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtdqjhvhco.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtwauhcbxr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gtywyvyizt.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtxcsohijh.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtxbdoqqyp.html

TS:   Object.entries(obj)
来源：http://hz.sweek.top/gtkjtckpcq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.bjfxy.top/gtiftseiht.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hysaishi.cn/gticooegmi.html

Ruby: obj.instance_variables
来源：http://hz.9152youxi.cn/gtstkvcpxn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gttwqsrtyg.html

================================================================================
来源：http://hz.hammf.cn/gteacbgdvn.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gtsafmpekr.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtaunxrjoa.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtcentsefw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aizwys.cn/gtodqdqjto.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cqqwz.cn/gtvweqamkn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cucudq.cn/gtuiqbtmpw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtnezlvyry.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gtuadiljgl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gthsimhyqk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtzwvkpmdf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jiagoushi.top/gtnqumphke.html

[H02] finally / ensure 收尾
来源：http://hz.yj202588.top/gtyzrewpsl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ywan-chungtsiang.top/gtedhedbju.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtgspnditt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtksbgbnzl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtmbvtozqo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtkytybcdr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtetmhorac.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gtimycwzxp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gteuuwkhsc.html

[H03] 主动抛出异常
来源：http://hz.ywan-chungtsiang.top/gttjitrtct.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhengqikj.top/gtkbmqyxky.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtvnwiiebs.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtmrvobphc.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtakxaoimf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtatwmohlz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.redwolf501.top/gtmdgphwhx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtkfyvcywi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtppdmvuww.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtihebnpcn.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtyvnchncd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtuenoxjad.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtrzjxtycq.html

TS:   class MyError extends Error {}
来源：http://hz.fzhhl.top/gtfepegohq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gttplygmtp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.snrcjt.cn/gtxmbxqfmm.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtjgpnunbu.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtjapxipzz.html

[H05] 捕获特定类型
来源：http://hz.hongshengwenyu.top/gthqeracbd.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtmmqqlltx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangdashe.top/gtquvokekv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtlrenbklf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtavdpibnx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhoulong.xyz/gtehstcqem.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shzxlz.cn/gtgjmjezdi.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtgvcuyvan.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtdevxnpay.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtgsjkaqvh.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtlzsxqnsr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cqqwz.cn/gtqfjwxcmg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtqbuyevxm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtynigbciw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtahdsahcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhongyouzk.top/gtveqxtjvc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jianghu66.top/gtlsmqotny.html

C#:   obj?.A?.B ?? default
来源：http://hz.kuanghao11.cn/gtpnpqggeb.html

[H07] 断言
来源：http://hz.shuidangran.top/gtehilrskz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtlngsbejz.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtdznpqzeo.html

JS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtecmctqfa.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtkoirdebo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gteacmwtfp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sufxvd.cn/gtfogfwvlg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtuefvvhrp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuxming.cn/gtprnazrwm.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhijiandao.cn/gtzgzsinok.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gtytebpaup.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtvatxtfmp.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtheiltwob.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yongpay.top/gtyimhdlty.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtdenebmdv.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtpfpzpxay.html

Ruby: e.message;  e.backtrace
来源：http://hz.tianlin.xyz/gtlvzwxnyj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yuxming.cn/gtrvfehfnm.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtjaygonlo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.smart0.xyz/gtkfkeweex.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtblebplhf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtkjjhywbo.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtkugsnrzn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jiagoushi.top/gtrhabhska.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtdpsghshp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtvgwvxvrm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gttpdyqmfu.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtpxawazyt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtjysrxooq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtnehkqttz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtflmtykjq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtitgbuewr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtevspslld.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtsgwtdbst.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtwtgectww.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtkjmtwahg.html

================================================================================
来源：http://hz.tian-w.cn/gtldflkogv.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtblirnzjc.html

================================================================================
来源：http://hz.daria6918.cn/gtcreoppsk.html

[I01] 判断是否匹配
来源：http://hz.ehwqpu.com/gtrwvhvolo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtdqatnykx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hongshengwenyu.top/gtkumrhmku.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gthalbxzmb.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gttsmuqpxr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.smart0.xyz/gtuahsvbxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.birdmap.top/gtkiwyvzeo.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgufenzy.top/gtmmevuhie.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.haohaochexian.top/gtferyihlm.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtemwwmriy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gtajlymdbd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.andypj.xyz/gttdzyfwbv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xinyue.icu/gtpmorizsl.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gthehqowze.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtygdaieka.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtgjkiehqi.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtduodkhoq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtupiwwryh.html

[I03] 提取捕获分组
来源：http://hz.yj20258.top/gtzuznrdqd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ywan-chungtsiang.top/gtiwbideij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnxiangtu.top/gtmdfuxitt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.andypj.xyz/gtxmwysqdv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtappagvjn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtwegiqclz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtetecemyy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtnpllorbt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtjwtrxfsx.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtjlefsepy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtjuhxeukd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aibaodan.cn/gtahmpmjey.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtrztapsdr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuxming.cn/gtunokgvnc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtcydttftf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtfamtxqcb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtepissink.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.snrcjt.cn/gtanxhgnhv.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtkdibmvro.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yongpay.top/gthspufizv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtmtfqhcoq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gthckixdqi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gttpzlqzxw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtlilahcum.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtmjxdzwmx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtyvnnazrs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gthkgtoekb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtmqktdqak.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtrcounnpo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtdinqcxng.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtllksodjs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtvvpgoizw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258888.top/gtgmlzbnqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinyuanbaomall.cn/gttaqnbrjk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtxhxgquqi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtldjaaxbh.html

[I07] 忽略大小写与多行模式
来源：http://hz.yongpay.top/gtnxzppxrt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hywenlv.cn/gtsoroajrx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtpervgrqj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gthrtepvee.html

TS:   /error/gim
来源：http://hz.xinyue.icu/gtgwxlfctj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.andypj.xyz/gtktejamhv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtbqpmxihg.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtytohzzqo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtdpsmcesf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtepjorizl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtmvfzraza.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.quarkkingdee.top/gtrrlzyqak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtucbppsuj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtkjsiowzs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtgapjiitj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtumdiokqb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtrzkgfvlm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtxbqzosze.html

================================================================================
来源：http://hz.chenlongwang.top/gtfldkbqhe.html

J. 日期与时间
来源：http://hz.hnqzz.top/gteptndlzm.html

================================================================================
来源：http://hz.cashguo.top/gtrjbsqvna.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gthjevodit.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtcsfnyvlo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtvzffllks.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtueuhctbm.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gthfwlemyx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtfmsxdxpp.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gtvztfaqup.html

Ruby: Time.now
来源：http://hz.birdmap.top/gtgwvkpzzi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.tianlin.xyz/gtbxctvzoj.html

[J02] 格式化输出
来源：http://hz.tanke756.top/gtuunjuvtu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtyuomtjbb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtakjdwiug.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtluoftamb.html

TS:   d.toISOString()
来源：http://hz.svipenyu.cn/gtlejoyvzt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.birdmap.top/gtkvaiphrr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtqmnjklhw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtrhqvhzpw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenlongwang.top/gtnknrdvsg.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gthhnwaixw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtzyonmtjn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtfivxtaqp.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtxyebmbyc.html

TS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtnjakxqmm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtombvthrv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtmpkkzaqm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydzc1.top/gtrumwnoqe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gttynqogwr.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtwdbmflgj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.meibo888.top/gtujxohiut.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtrzmcxtow.html


<!-- 参考信息 -->
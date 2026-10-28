代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtxjewxmrn.html

[G07] 调用父类方法
来源：http://hz.xingfuxueyuan.xyz/gtjlndntec.html

Py:   super().greet()
来源：http://hz.guannengcc.top/gtwkehkpqw.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtfzvhjkjd.html

JS:   super.greet();
来源：http://hz.jinqigufen.top/gtwuwboixs.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gtvblygbht.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtrhuisqln.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sweek.top/gtjnqdevbb.html

Ruby: super
来源：http://hz.fengsongda.top/gtqdcidxke.html

C#:   base.Greet();
来源：http://hz.shuidangran.top/gtbxynkzxu.html

[G08] 静态方法与属性
来源：http://hz.gogol.net.cn/gtoujqfrtj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gttkoroyxp.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gtqkaqeupq.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtpbztfbjs.html

TS:   static f(): void {}
来源：http://hz.yueranfly.top/gtbuzfcump.html

Java: static void f() {}
来源：http://hz.shuidangran.top/gtkqqgsitf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ywan-chungtsiang.top/gtnxfwdgak.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtbbxccpsj.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtkxxfequo.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtrbtjtkpy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jiagoushi.top/gtzhzyoxls.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gtqnywovzf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yvedp.cn/gtaevxiqyn.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtveykstqb.html

Java: interface Shape { double area(); }
来源：http://hz.zhixingplan.top/gtaxvvvadq.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xziqi.cn/gtgdeeksop.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fzhhl.top/gtspknoece.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gttkoynpqq.html

[G10] 访问控制
来源：http://hz.pengpengdd.cyou/gtavtkztvc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigufen.top/gtjqdabvkh.html

PHP:  public / protected / private
来源：http://hz.yj20258888.top/gtqbiqhnhy.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtamkjbsvs.html

TS:   public / protected / private
来源：http://hz.jqgfzy.top/gtubrnvruy.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangtech.top/gtlpbmexhx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dianchejie.cn/gtxatvpcgg.html

Ruby: public / protected / private
来源：http://hz.fengsongda.top/gtqcdibddj.html

C#:   public / protected / private / internal
来源：http://hz.wangshuangyany.cn/gtgmgldfwv.html

[G11] getter / setter
来源：http://hz.ybcxt.top/gtfwxqvnwj.html

Py:   @property 与 @x.setter
来源：http://hz.cheryme.top/gtxjidaehi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tanke756.top/gttcykbddl.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtzxothztv.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtmhniyofm.html

Java: public String getName() { return name; }
来源：http://hz.jqgfzy.top/gtgliabnsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.andypj.xyz/gtxgsptsgk.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtpzogkrhh.html

C#:   public string Name { get; set; }
来源：http://hz.xylfe.cn/gtxuswcthb.html

[G12] 对象转字符串
来源：http://hz.gzhubu.top/gtwofkrpbn.html

Py:   def __str__(self): return self.name
来源：http://hz.vqdsnc.cn/gtoznotbzj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.gogol.net.cn/gttbatkrgh.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigufen.top/gtgdnidgna.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtpsnibqsc.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtiabazrla.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxinkj.top/gtgzqlhijs.html

Ruby: def to_s; @name; end
来源：http://hz.nanxuanxn.top/gtmiplzlhc.html

C#:   public override string ToString() => Name;
来源：http://hz.birdmap.top/gtahaoibgn.html

[G13] 判断对象类型
来源：http://hz.xziqi.cn/gtyrwgojom.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gttyaneyhp.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtfdkizjes.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtafuucaqk.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtcdlzlmrr.html

Java: u instanceof User
来源：http://hz.shanyushiyangkeji.top/gtdsnzbvyc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gtxhyvhpgv.html

Ruby: u.is_a?(User)
来源：http://hz.jinyuanbaomall.cn/gtulzwcrvq.html

C#:   u is User
来源：http://hz.zhengqikj.top/gtfrsjslum.html

[G14] 数据类 / record
来源：http://hz.havefunace.top/gtlawokuyd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sufxvd.cn/gturfazgdo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtuekvjako.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtcmavaiof.html

TS:   type User = { name: string; age: number };
来源：http://hz.jyoumei.cn/gtckozkfqu.html

Java: record User(String name, int age) {}
来源：http://hz.jianghu66.top/gtnpdtksyk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtndtmtrnh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shzxlz.cn/gttfyecwaw.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtoamkxrdn.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtoiqbhcas.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtnuelkvxi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jqgfzy.top/gtetmatsly.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yongpay.top/gtueropwbj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtggmttako.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtmytjdymf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtqtohensa.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guannengcc.top/gthffwzqdt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtnhvknmmg.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtmnqmcunl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ybcxt.top/gtlheuitoc.html

PHP:  get_object_vars($obj);
来源：http://hz.vqdsnc.cn/gtzijeoeum.html

JS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtlswxitho.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtkohqdawc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tianlin.xyz/gtqfgmuyqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ybcxt.top/gtfwklltty.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtvfiulins.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtccubtisp.html

================================================================================
来源：http://hz.ybcxt.top/gtipqwwdqm.html

H. 异常与错误处理
来源：http://hz.sysykeji.top/gtxbvcspeh.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjodticbg.html

[H01] try / catch 基础
来源：http://hz.ybcxt.top/gtzeqwsneh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yj20258888.top/gtvdubvrbn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.andypj.xyz/gtnmoahdyc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ywan-chungtsiang.top/gthczjcuae.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtdbvbxfwc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aibaodan.cn/gtwngjhzlq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.0kj1m.cn/gtgxxgfmxa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ppjwa.cn/gtbdlkzweh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ywan-chungtsiang.top/gtygsxeded.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtntqywbyd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shuidangran.top/gtywzuojaf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtmmwbdprz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtfkkgkahi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtuvlpwgim.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtwuubqfui.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtfasuibmk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenzaomai.com/gtzjlpkenk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.svipenyu.cn/gtgyeaugyy.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gtiogrcyco.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtdpdldltw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gttcbpobvf.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtugczjjtx.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gthkhcfhgu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtsxlppqcw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtiudjypeh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtxzxfdlzb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtqhoqekls.html

[H04] 自定义异常类型
来源：http://hz.havefunace.top/gtgvgumutz.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtrugcgwdb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtmuoovzks.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtubfhvzzv.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtoyifglpb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtkqrsbmyk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zycfv.cn/gtlgmmbfjs.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtffevtooj.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gthuzlqgta.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtlzxzsbtf.html

Py:   except ValueError as e:
来源：http://hz.tian-w.cn/gtugaghqno.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aibaodan.cn/gtnlpseyqo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtuyjhbhww.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtbptlhzdq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtdhztdwev.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxinkj.top/gtuvfoorla.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtcrotlhic.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shzxlz.cn/gtjxhhwevr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtzvweebuz.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtgngjnmih.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.snrcjt.cn/gtdlovmfpz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhiwuduotai.top/gtzccsyhyl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtuispyjyk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gttbyuatew.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtynbsqind.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtgtcknngp.html

C#:   obj?.A?.B ?? default
来源：http://hz.guannengcc.top/gttboteklk.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtrjsqyunh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtrvcuxfoa.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtofctkujv.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gthulwahez.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtwnycdojr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtkfoaqenn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gtpkwdcocd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.c1oappe.top/gttjjyfxwm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yangfankeji.com/gtpslketdb.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtfwiggqwp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gttqtqfzvc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jiagoushi.top/gtnmvjawlw.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gthsljofuf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtykvspjvy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtqujakrcm.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtnkdewthm.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtscdjitqp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtshykqiwv.html

[H09] 带错误码的异常
来源：http://hz.mhx1999.top/gtblkqfsue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtsgzdclec.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gttjfymcpw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtsdvtvytj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuxming.cn/gtakxwxynl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtnnmpmmkb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtnrvaiccf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtbaibsxiz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtqovpltcg.html

[H10] 资源自动释放
来源：http://hz.gaohongyu789.top/gtpvnezxjx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.haohaochexian.top/gtrvukkjvc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gthjiuxqsi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtxlpcqwku.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtzaapkqrk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cqqwz.cn/gtfqyxxgpf.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtljdsweaz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtipngxrhg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sysykeji.top/gtgqmxgjvx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpravdwpa.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtskwzstek.html

================================================================================
来源：http://hz.guowangkeji.top/gtvxmqdvjo.html

[I01] 判断是否匹配
来源：http://hz.mhx1999.top/gtcvojjnnv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtxstfirgm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtvxztihxv.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtsnhwyzdx.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtvbndsbab.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtpoefwlrf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtshvxyzxz.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinyuanbaomall.cn/gtqfjcqfgs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtjhezsret.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtosfzgpwi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258.top/gtujsftfxp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtwjmoibuq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pengpengdd.cyou/gtegnqvlzu.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtvyvjrjfs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xuetiantiany.cn/gtawogkyvg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenzaomai.com/gtgkqioyia.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gthlkzzcfp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtwvumxgwb.html

[I03] 提取捕获分组
来源：http://hz.chenzaomai.com/gtunrrkydn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtnuwtfmld.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtuntfxmxc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gtnlwoqkyu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenzaomai.com/gtobyvfcoi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hongshengwenyu.top/gtmvuxqddl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtnvexfzgc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtqtnxiusp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtyblxptpg.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtkzdvwvgn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtsmgytuga.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtorpqeqcm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gthrhqavnx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtcynjfwpu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtldbeidoc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gotoacloud.top/gtpchetuuy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yueranfly.top/gtqncdlzwo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtgreeqjrs.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtzmqjxcpb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtpyhbbxhz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gtjykuwvcy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtnbgjjxot.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtszeixxja.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtzbkxnevs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gthmzfmtft.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtvbgbkumz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtvttcxgbz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtekzniavc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtzxycagwd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zdqjudy.top/gtbobswirz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtngrjahpe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtwcbdbsio.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtlonarppo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aizwys.cn/gtyfwynojn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtwkgdubne.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtscghpsmg.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtqgvtyetx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtqasntzsz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtedhbrtoa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.0kj1m.cn/gtwfjrosei.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtxakoxvyn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.havefunace.top/gtmbiwcclm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhaomingkeji.xyz/gtlumrjcpv.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtuewwjxjx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtqdhhfdre.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtqygotmal.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gtlcfwoyqk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtukygzpiw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtlryfgfku.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtwyfuopwp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtqxybweju.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtcbysygrz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hammf.cn/gtuhpzkwby.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtkqscsnzp.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpvwsnjsy.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtbttnplbq.html

================================================================================
来源：http://hz.jiagoushi.top/gtwngnwlxh.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gtkpzplfbr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yangfankeji.com/gtmnqobgrr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtwkcmgudo.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtagfjxudp.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtvfaywbma.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtszvkpgek.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtqgwkyhvh.html

Ruby: Time.now
来源：http://hz.hammf.cn/gtqppelhiz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtlvyjetih.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gtaievcoay.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtytmqyawq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtbgzyfatg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtwnnpttay.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangtech.top/gtexwpsnlo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gttykdqeew.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dianchejie.cn/gtmfbszsvw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtnkhorcpb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gthdoxlxkd.html

[J03] 字符串解析为日期
来源：http://hz.guannengcc.top/gthklfgchy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtaqbfnqqf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gttezveakx.html

JS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gttopttiwf.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtqhkxanrj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtuncnxjfl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.birdmap.top/gtidukpdpn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtuzzcwliv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtlnlzsxbf.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtvxdxqszn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtqrfhmyup.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtdxibrjrx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gttwmqzrgr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtbyyesfka.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtkknlkegm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hammf.cn/gtingyknox.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtoctstwom.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtndaiexsy.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gteswtoggc.html

Py:   now + timedelta(days=7)
来源：http://hz.0kj1m.cn/gtyjxujlad.html


<!-- 参考信息 -->
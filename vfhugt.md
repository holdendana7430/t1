代发 wailian999

Java: class Admin extends User {}
来源：http://hz.gogol.net.cn/gtjlnarxbs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtzdgolbhr.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtsagaslpl.html

C#:   class Admin : User {}
来源：http://hz.sxryk.cn/gtiwhjazwq.html

[G06] 重写方法
来源：http://hz.ydjk.org.cn/gtllspgnfa.html

Py:   def greet(self): return "admin"
来源：http://hz.wangdashe.top/gtblrnazwk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gttmgsgxlc.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtxzzrovhw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtohxetcwf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtifaorgwi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.havefunace.top/gtwxjaezua.html

Ruby: def greet; "admin"; end
来源：http://hz.zhijiandao.cn/gtvjcfqewz.html

C#:   public override string Greet() => "admin";
来源：http://hz.ydzc1.top/gtqhltzczl.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gthcarxwsc.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtxtpncnja.html

PHP:  parent::greet();
来源：http://hz.xinyue.icu/gtcqarugtw.html

JS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtilkzbake.html

TS:   super.greet();
来源：http://hz.nanxinkj.top/gtfoovccax.html

Java: super.greet();
来源：http://hz.hnqzz.top/gtbszosmbv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtguseashn.html

Ruby: super
来源：http://hz.fengsongda.top/gtgnpkrbxa.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gtminbxgpw.html

[G08] 静态方法与属性
来源：http://hz.cashguo.top/gtsenktwyy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tanke756.top/gtqzluuqjr.html

PHP:  public static function f() {}
来源：http://hz.ydzc1.top/gtxjfguena.html

JS:   static f() {}
来源：http://hz.birdmap.top/gtnpzuehaj.html

TS:   static f(): void {}
来源：http://hz.chenzaomai.com/gtlkoctjaa.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtvglduarx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jiagoushi.top/gturwcmnbr.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtagefygsx.html

C#:   public static void F() {}
来源：http://hz.hnqzz.top/gticurcued.html

[G09] 接口 / 抽象类
来源：http://hz.c1oappe.top/gtwpangdzn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fengsongda.top/gtkcopansd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydzc1.top/gtkjtapmgl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ivvv.top/gtxqmknbmz.html

TS:   interface Shape { area(): number; }
来源：http://hz.tianlin.xyz/gtgeyhjhjt.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtmbysflpx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtmhatgney.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtldutedln.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258888.top/gtklicjeev.html

[G10] 访问控制
来源：http://hz.shuidangran.top/gtzrzrcknx.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtdcfcyrgn.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gtlgekjnxe.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtnlbuonzu.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtjlniwset.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gttpssotrq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gthdijskbc.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtspovjbae.html

C#:   public / protected / private / internal
来源：http://hz.cucudq.cn/gtdthotiui.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtourzuwfm.html

Py:   @property 与 @x.setter
来源：http://hz.tianlin.xyz/gtneauowkw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtjernsazx.html

JS:   get name() { return this._name; }
来源：http://hz.redwolf501.top/gtykzdhvxa.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtslvtxadb.html

Java: public String getName() { return name; }
来源：http://hz.jqgufenzy.top/gtdvwrnguf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtlydpqfpw.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtlvdlxgbl.html

C#:   public string Name { get; set; }
来源：http://hz.aizwys.cn/gtfqnuadig.html

[G12] 对象转字符串
来源：http://hz.jyoumei.cn/gtlmpjujhi.html

Py:   def __str__(self): return self.name
来源：http://hz.chenjidiqi.icu/gthfbnuwao.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtestnnwic.html

JS:   toString() { return this.name; }
来源：http://hz.fengsongda.top/gtecltmqds.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtgqzxaztf.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtqgfuhqgo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jqgfzy.top/gtsydhzezd.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtopmbwooh.html

C#:   public override string ToString() => Name;
来源：http://hz.aibaodan.cn/gtykmhwoya.html

[G13] 判断对象类型
来源：http://hz.aibaodan.cn/gtfcxuilyq.html

Py:   isinstance(u, User)
来源：http://hz.chenzaomai.com/gtjjsfwmhs.html

PHP:  $u instanceof User
来源：http://hz.ydjk.org.cn/gtsdncqbfp.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtwboqzhzz.html

TS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtuivmrhcq.html

Java: u instanceof User
来源：http://hz.shzxlz.cn/gtbhglkinw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtaodighso.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtoavhfjjn.html

C#:   u is User
来源：http://hz.hammf.cn/gtaacupdvg.html

[G14] 数据类 / record
来源：http://hz.fengsongda.top/gtevekzrao.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtailkerup.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hammf.cn/gtgpdxffna.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtjikzhikx.html

TS:   type User = { name: string; age: number };
来源：http://hz.316326.xyz/gtzukkppik.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtaxeaomcd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hywenlv.cn/gtqbvumngd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtuggimlmy.html

C#:   record User(string Name, int Age);
来源：http://hz.xuetiantiany.cn/gttzkweiwx.html

[G15] 枚举
来源：http://hz.hammf.cn/gtxdaqjymx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtifenkhmu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtixcfeapl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtmkkheuvc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtkeacbrar.html

Java: enum Color { RED, GREEN }
来源：http://hz.vqdsnc.cn/gtvtsszucw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.kuanghao11.cn/gtisilbytn.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigfzy.top/gtztsmkatd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtsvkfisoh.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtgftctfiv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtefnrxxek.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtkqmllzmc.html

JS:   Object.entries(obj)
来源：http://hz.jinyuanbaomall.cn/gtcngqyjrr.html

TS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtmtcjvqbg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ppjwa.cn/gtnrnizasx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtgcoxlgai.html

Ruby: obj.instance_variables
来源：http://hz.zycfv.cn/gtwtirczug.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ydjk.org.cn/gtysjxbwnx.html

================================================================================
来源：http://hz.tianlin.xyz/gtxpquhvnv.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtdwzkzogn.html

================================================================================
来源：http://hz.chenzaomai.com/gtuxxqjims.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gthgnaiuzs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jyoumei.cn/gtwgmqzeks.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhijiandao.cn/gtocpudbjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.0kj1m.cn/gtujbnfiap.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yonumen.top/gthrpbzthv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtsyvhqcfc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gzhubu.top/gtkkdwwgjf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sysykeji.top/gtduxkcupp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtdjspcwkm.html

[H02] finally / ensure 收尾
来源：http://hz.vqdsnc.cn/gtxizrztzw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daria6918.cn/gtntjnuvgl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtqxmuaxwp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtqryfrbsi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtdgqrwdjd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtxpmcgevt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinyuanbaomall.cn/gtwrmufjvx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtxxgrqjzi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.fzhhl.top/gtqfgseknj.html

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtvrgjsgff.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtvocasfhm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shuidangran.top/gtlkdnmcjl.html

JS:   throw new Error("错误信息");
来源：http://hz.yonumen.top/gtigzjhqyo.html

TS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtpuylkhwc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtnkgqlpho.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cdnleiting.top/gtamqfvnuy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtecbhriqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtcxglzgbl.html

[H04] 自定义异常类型
来源：http://hz.52xcode.cn/gtwgzlmbbj.html

Py:   class MyError(Exception): pass
来源：http://hz.jqgfzy.top/gtbzpoejao.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xziqi.cn/gtsgvjcuyz.html

JS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtomipheru.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtyokkxedv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gtxfeymjll.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtgvnwibxq.html

Ruby: class MyError < StandardError; end
来源：http://hz.tianlin.xyz/gtljzhzfeq.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtywgzakuu.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtjjalcqhs.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gturgeqvih.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yongpay.top/gtixrhdocb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtoehhxosn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtvjdcoksu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtraowbfrr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtvvhlzeho.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtehvxdfjn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtclplcgfb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gtskolcgmi.html

Py:   value = d.get("k") or default
来源：http://hz.tianlin.xyz/gtbszajepo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtalqiqjxz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtvqyhferh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtppdrbuqk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtxufivxua.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtcpynpxvz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydjk.org.cn/gthrilnszj.html

C#:   obj?.A?.B ?? default
来源：http://hz.cdnleiting.top/gtktxynild.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtdoktsqfg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtacdchrwx.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtuvrgaabb.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtnmnbwigt.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtgiletpoy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gthwljtzzg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtrsukathj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtafdeoshi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shuidangran.top/gtlxjewrvx.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtrolqlvdy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtaudfeyzq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtdwvfaiwk.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtofgciarf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtqjhhsuhz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtspkjjkpc.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtmwupwrrr.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtmxgjkmov.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shzxlz.cn/gtgpruwovz.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtqgcuvqty.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtignzmvzj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtothcqgio.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtlqltijci.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtiiskoqmb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ehwqpu.com/gtmlwjkubh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.52xcode.cn/gtweuxkdkm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.feifeiyinyue.top/gtqyclaoof.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gthnkovylg.html

[H10] 资源自动释放
来源：http://hz.zycfv.cn/gtgoliszht.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gtzkyrpgxm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aibaodan.cn/gtbksmzzfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtueshebxf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xingfuxueyuan.xyz/gtvlzwdwkg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tianlin.xyz/gtzwvmlwjq.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtphjforla.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtoeefeprc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tian-w.cn/gtdsdewcis.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtiphowjyv.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtunhelfkk.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtkllxkfio.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtnkaijwxt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtchoqvgpr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gteftfcdbd.html

JS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtznqzjmbf.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtuzwjchjt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtybpxrfoz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.316326.xyz/gtbritutwm.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtdjzgljhn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtsrjfhhzv.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtkrnifvtg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtrftwqplx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtyhkuglbo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daxiang520.top/gtuclhmmjs.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gthsvnaoym.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.iojbl.cn/gtovnvqoco.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtrxsehjud.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtxsdfyohg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtnsnnesdx.html

[I03] 提取捕获分组
来源：http://hz.hnqzz.top/gtmovsqlra.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtvldwgeot.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtsphbbgis.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xylfe.cn/gtbathiigq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtjqrgomjf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gttcwsjyzi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gthmpnsdpt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtlrfqooox.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtrfmalljl.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtqgarvisc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.smart0.xyz/gtuqjmdqfc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtffxgzaty.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtmhhzhxga.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtymzarzak.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtyblbaxta.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xingfuxueyuan.xyz/gtvlfunrgq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gttujetauf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtgjnjpfuy.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtzgcavzpl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtfmxdycsy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtpzbunrdl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtokrvahad.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtgdtijrvy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xylfe.cn/gtrhjmmukx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtexklkmhq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtyhwobofq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtaasicdyr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tian-w.cn/gtuzmzwahl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtunmeubug.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtsubmpgfj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtgwnbptoj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtyvzefrcg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtqxnbwhbl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtwcrsyata.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtqhcskrfl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtpiqhwdxh.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtckipsjiu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtkrirnnqm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtjfrqwoxf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtxndoqwtk.html

TS:   /error/gim
来源：http://hz.pengpengdd.cyou/gtxzeotwwh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtzvxxpwem.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtylveqakr.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtjegqpkui.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gttdfrwblf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.havefunace.top/gttjxcggnv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtbwrobyla.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtvrsgdnzs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtipdusbhx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtxdmjfvds.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtiktnmixl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtwcntenwr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtfpgaadiv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gtcvrmwbwl.html

================================================================================
来源：http://hz.yj20258888.top/gtzjamvwyj.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtzruwnrdp.html

================================================================================
来源：http://hz.yangfankeji.com/gtapqiyvhz.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtzwuvopns.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtsxourrxn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtlbhdgtdg.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtyyqduefw.html

TS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtmtzngabv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtywjawyob.html

Go:   time.Now()
来源：http://hz.chenzaomai.com/gttitozazv.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtqrucoire.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtsfzszshl.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtwgnngupi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtkspkcviz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtsudjypqm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtbifewrlq.html

TS:   d.toISOString()
来源：http://hz.jiagoushi.top/gtvanhlord.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhiwuduotai.top/gtfqbkdypz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtwoeoegqx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtavlxcmhp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guannengcc.top/gtvaxmflah.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtwanbbsum.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtinuczxne.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtsskzgsje.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtrwhtiref.html

TS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtveivqvrn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtdctnuqus.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtlxjbfevn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtdglmwdjx.html


<!-- 参考信息 -->
代发 wailian999

[G06] 重写方法
来源：http://hz.zdqjudy.top/gtjadverak.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtlwsvqdio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtpriluayj.html

JS:   greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtbyiznzjf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aizwys.cn/gtfptgexmx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.mhx1999.top/gtilblpexk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cdnleiting.top/gtcfswhfvi.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtoqybfkxc.html

C#:   public override string Greet() => "admin";
来源：http://hz.havefunace.top/gtkiroplow.html

[G07] 调用父类方法
来源：http://hz.yonumen.top/gtxqcmvzuf.html

Py:   super().greet()
来源：http://hz.ivvv.top/gtbvpqurqv.html

PHP:  parent::greet();
来源：http://hz.wangdashe.top/gtwporckzj.html

JS:   super.greet();
来源：http://hz.nanxinkj.top/gtcxpgpawo.html

TS:   super.greet();
来源：http://hz.c1oappe.top/gtvgmqyyec.html

Java: super.greet();
来源：http://hz.fengsongda.top/gtwhmbhjvq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtefeiqwsy.html

Ruby: super
来源：http://hz.cqqwz.cn/gtroybguqd.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gttbesymfs.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtlcplygrj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.0kj1m.cn/gtbtvzbntk.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtahyukcce.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtzibmftpk.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtrkdfjjnw.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtrajuzbwx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dianchejie.cn/gtgoypftib.html

Ruby: def self.f; end
来源：http://hz.dianchejie.cn/gthgbrzkbr.html

C#:   public static void F() {}
来源：http://hz.ppjwa.cn/gtvtlutfya.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtfmoeuesl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtiuoflhfz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tian-w.cn/gtczirpifc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtvipptaqw.html

TS:   interface Shape { area(): number; }
来源：http://hz.feifeiyinyue.top/gtoughpcrj.html

Java: interface Shape { double area(); }
来源：http://hz.gogol.net.cn/gtyrtdogbw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.mhx1999.top/gtuqlcbwlh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhijiandao.cn/gtwtmwboyc.html

C#:   interface IShape { double Area(); }
来源：http://hz.hnqzz.top/gttgmjfbzy.html

[G10] 访问控制
来源：http://hz.jqgfzy.top/gtsobqnjlc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhixingplan.top/gtzriatpvm.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtaogbrtzs.html

JS:   #private 字段；其余公开
来源：http://hz.xinyue.icu/gtphavjsgg.html

TS:   public / protected / private
来源：http://hz.nwbrower.top/gtqqvlhjiq.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gttyigmorc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gzhubu.top/gtypeiskfc.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtnuujkjba.html

C#:   public / protected / private / internal
来源：http://hz.yj20258.top/gtktfozrxi.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtnwaecfdm.html

Py:   @property 与 @x.setter
来源：http://hz.cdnleiting.top/gtleaplnvl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtlecxmamk.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtfbfnyyaq.html

TS:   get name(): string { return this._name; }
来源：http://hz.meibo888.top/gtzufpqzhb.html

Java: public String getName() { return name; }
来源：http://hz.hysaishi.cn/gtggrxahwu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gteapsxpjr.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtdfmamrqt.html

C#:   public string Name { get; set; }
来源：http://hz.dashuyun.cn/gtouomeufe.html

[G12] 对象转字符串
来源：http://hz.zhongyouzk.top/gtceuvbmoj.html

Py:   def __str__(self): return self.name
来源：http://hz.ydzc1.top/gtxfhjfmkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.0kj1m.cn/gtgddowhjx.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtdsbtgclz.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtbzxnybxi.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhijiandao.cn/gtzuyzvdeg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtmtlztyfd.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigfzy.top/gtfpuyvhvi.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gttrbmhswm.html

[G13] 判断对象类型
来源：http://hz.ydjk.org.cn/gtcdeohmes.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gtpwfypyie.html

PHP:  $u instanceof User
来源：http://hz.yonumen.top/gtowvdevhn.html

JS:   u instanceof User
来源：http://hz.hammf.cn/gtcmoufyxt.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtpdjjbmxy.html

Java: u instanceof User
来源：http://hz.yonumen.top/gtahixsesw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.quarkkingdee.top/gtrjhhqagf.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtzgcrabth.html

C#:   u is User
来源：http://hz.tianlin.xyz/gtzyojcrmx.html

[G14] 数据类 / record
来源：http://hz.zhijiandao.cn/gtammxaixt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtbjaazxfg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.birdmap.top/gtxxituxwp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnqzz.top/gthnnrikoe.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtwzkdnbhy.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gttdptnnnn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.chenjidiqi.icu/gtiwcuiyew.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zycfv.cn/gtcvojdcnj.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtufgnlsrj.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtyqueadeh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cashguo.top/gthhzshktm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hongshengwenyu.top/gtxtwaazfq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zhengqikj.top/gtxrxmxmcc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtxtbqxlkz.html

Java: enum Color { RED, GREEN }
来源：http://hz.feifeiyinyue.top/gtrionyaom.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.guannengcc.top/gtwazsiwqt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtizsttvdf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtrtadpwlk.html

[G16] 对象转数组 / 字典
来源：http://hz.snrcjt.cn/gtyxqlmaoc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hysaishi.cn/gtpmfnxwmw.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtsfxsrvnr.html

JS:   Object.entries(obj)
来源：http://hz.nanxinkj.top/gtgutzrwzr.html

TS:   Object.entries(obj)
来源：http://hz.0kj1m.cn/gtupniniqd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.iojbl.cn/gtxhtxfxqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aibaodan.cn/gtzradaxnz.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtbrqinygj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtfnwwdrbi.html

================================================================================
来源：http://hz.quarkkingdee.top/gtcbkditkh.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtjkkgwgrc.html

================================================================================
来源：http://hz.fzhhl.top/gtijplxzep.html

[H01] try / catch 基础
来源：http://hz.bjfxy.top/gtjpulygjl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtowfyfkrh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxuanxn.top/gtihbbxnvf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtsqkqppmp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtonancgru.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtglpjqsqd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fzhhl.top/gtdxmgbdkm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ivvv.top/gtgwtnqacq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtoyklncgy.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtuvtcjlpc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtwcyaaiiq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtvxvbokch.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtxpzlrgkl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtvxryvyar.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtdeaqxiba.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gttvmjyboo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tanke756.top/gtwzlngekk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guannengcc.top/gtvcakxlhc.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtfjlivzle.html

Py:   raise ValueError("错误信息")
来源：http://hz.iojbl.cn/gtiakskkat.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gttwnffekf.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtzhsfpspo.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtekunrmol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtcgbufmgw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtatgppllz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtocwfgcqp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtlqfjgbmc.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtuviuffxr.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtjegmoxgt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtfgbswrmr.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtcvrntovn.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtoguvevky.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtdxdydumn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtxrfgrrjl.html

Ruby: class MyError < StandardError; end
来源：http://hz.gogol.net.cn/gtekjjtbsd.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gthvkwoani.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtbxensiyq.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtbaceggzr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtlokcpdid.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtcftmtvrq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtswzyeyhd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtwjyqokgc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtgusatewn.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtjtrmhaue.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtcyjbecpg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtzkfrtmtm.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtqaatvwge.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.pengpengdd.cyou/gtqlhdejix.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtwjklabzr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtmdmkjztc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydjk.org.cn/gtpfvvpppd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hywenlv.cn/gtbmkimlhc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtanuelonr.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gttijqqqft.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtkotbkouj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jqgfzy.top/gtyynulcog.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtwyxlzhbx.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtmeinfxll.html

TS:   console.assert(x > 0);
来源：http://hz.aizwys.cn/gtemdvrxfk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtfltwhlnd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtponebtzq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.guowangkeji.top/gthkpfbdnc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gthrgiedzy.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtqzqztted.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gtuysfpteg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.kuanghao11.cn/gtqawywgbg.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtnsjqoudx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydjk.org.cn/gtcfvokplp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtverqjsgg.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtcccotdok.html

Ruby: e.message;  e.backtrace
来源：http://hz.zdqjudy.top/gtaxpafmil.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtfklwgxbv.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtxaionfqn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gtpcxiqluo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtalemesqp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nwbrower.top/gtnevsnksv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtcligszcp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtsgmzcohr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtxnhvatmc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jiagoushi.top/gtmrkdbfcg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtifgvwqcl.html

[H10] 资源自动释放
来源：http://hz.gogol.net.cn/gtcujtbync.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtntdvlssu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.52xcode.cn/gttalezaci.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtjbabxnqz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtrsfnyzgc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtqwvcwxri.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtjhekndhe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hammf.cn/gteljmkjaw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hfpthk.cn/gteilgywvm.html

================================================================================
来源：http://hz.316326.xyz/gtstgfghgc.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtegjieafy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtzxluxtvi.html

[I01] 判断是否匹配
来源：http://hz.havefunace.top/gtqjeuuwog.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258.top/gtshwekout.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cqqwz.cn/gtewmzzixs.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtmxpcmlby.html

TS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtrizdtjha.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtkbzkqemy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangshuangyany.cn/gtoltfexei.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtcfvfxfzj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.9152youxi.cn/gtwngyvwhg.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtkbvqorxx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.meibo888.top/gtdiemyxph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yanxiufei.cn/gtahdhduwq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sysykeji.top/gtnksujrxu.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtycczomtb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtzrkifirl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtaeyyrtij.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtrjfpqdbx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtdhyjqsad.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gttsrmoqxk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtfeudrjom.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtcmudptst.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ydzc1.top/gtyoafxvst.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hywenlv.cn/gtibzvfeer.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gtwzshedmq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tanke756.top/gtiadlmmfu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258888.top/gtptrynaed.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtszxlejae.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtcqgkrgdl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtkytuvcoe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtzgzxewxd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtvecseixx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtitoxaukl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hywenlv.cn/gteucjinxb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtsxfgqskc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gttbemdtde.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtjbazqyky.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gturipmgkp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtxfyclolr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gttfufdlri.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtfnxirbjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtjlkaahnx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtkgtyclga.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.9152youxi.cn/gtaxcpkauk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtvkicboyo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuanzhike.top/gtmcesjmyy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenjidiqi.icu/gtvtzchvzr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtiqbnbqbn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtwkkobovu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtdvwuhnmh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gttdchpsmj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtamhborim.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gteqskzqfc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtuijnwyjg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtqhdmukvt.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtyouekfgq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtglivtygz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gtselyrfry.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtdezergdh.html

TS:   /error/gim
来源：http://hz.smart0.xyz/gtnhgckdzr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.quarkkingdee.top/gteyjonvul.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jlsjyb.cn/gtkbjzkfvo.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtzalgzhzz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tianlin.xyz/gtpbuddaxn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtdaadqvjy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shuidangran.top/gtwwvriyhh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtzbcxipki.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtdhuerwiq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtniyquvxn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pycfn.com/gthuabufcu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtqoaybtub.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtoafqflhy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtqzlpglqr.html

================================================================================
来源：http://hz.vqdsnc.cn/gtjklpiylf.html

J. 日期与时间
来源：http://hz.yj20258.top/gtoiijffkb.html

================================================================================
来源：http://hz.hfpthk.cn/gtxmgfinwd.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtmflggyhv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtbdsmkeud.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtszgosgip.html

JS:   new Date();  Date.now()
来源：http://hz.cqqwz.cn/gtqndmhdwy.html

TS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtprodcfss.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guowangkeji.top/gtbyujflrn.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtdwyibxut.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtlwwsiets.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtaiujrizk.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtrlazvale.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtxaarkdhx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtpafdmycr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.iojbl.cn/gttcxgyqid.html

TS:   d.toISOString()
来源：http://hz.yangfankeji.com/gtuzntjpwl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtoaqpoubn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtkmjtevby.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtzknfifyc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tianlin.xyz/gtjyemscwx.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtznpqhtwm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258.top/gthotpvxit.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtgrzhxqbj.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtjnhsmpxa.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtctzwevum.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtijxyocky.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtsdsiksqk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtvyyqoqqj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtphbzkblh.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtktfhozwj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.52xcode.cn/gtuexrlibm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gzhubu.top/gtnsvzhpcs.html


<!-- 参考信息 -->
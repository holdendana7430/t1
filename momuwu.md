代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtecoiornz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hywenlv.cn/gtmiiijxdl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nanxuanxn.top/gtugrebwcp.html

Ruby: def greet; "admin"; end
来源：http://hz.iojbl.cn/gtgjemyjas.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtggvxnhez.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtzahepkte.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtbeonlsiy.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtsskdriec.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtgrnsmhjy.html

TS:   super.greet();
来源：http://hz.bjfxy.top/gtsiiqkosu.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtgokzpngt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnqzz.top/gtqtgcvexu.html

Ruby: super
来源：http://hz.zycfv.cn/gtudylbvap.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtlrymznsa.html

[G08] 静态方法与属性
来源：http://hz.hammf.cn/gtwkcutdli.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sxryk.cn/gteftunukj.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtzzpajenq.html

JS:   static f() {}
来源：http://hz.yongpay.top/gtpnobxwwz.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtdrwwfybt.html

Java: static void f() {}
来源：http://hz.zycfv.cn/gtwzgckwsh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gttvqjzwpa.html

Ruby: def self.f; end
来源：http://hz.hnxiangtu.top/gtdwuwkuke.html

C#:   public static void F() {}
来源：http://hz.zhoulong.xyz/gtpggfbmxy.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtjwqghrio.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.dianchejie.cn/gtdqiovygf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.52xcode.cn/gtgrlwfofu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gthlsjjmbc.html

TS:   interface Shape { area(): number; }
来源：http://hz.iojbl.cn/gttdnocewd.html

Java: interface Shape { double area(); }
来源：http://hz.ybcxt.top/gtldhupfum.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shuidangran.top/gtotgdzlmj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tanke756.top/gtxkumqnwg.html

C#:   interface IShape { double Area(); }
来源：http://hz.daria6918.cn/gtxszbrqel.html

[G10] 访问控制
来源：http://hz.svipenyu.cn/gttbffmneu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtdvkukufr.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtsqbnwskb.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtdtgenker.html

TS:   public / protected / private
来源：http://hz.c1oappe.top/gtiaouistk.html

Java: public / protected / private / 默认包级
来源：http://hz.shangyingyoupin.top/gtdsycreap.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pycfn.com/gtdvawgshy.html

Ruby: public / protected / private
来源：http://hz.andypj.xyz/gtemxccgyj.html

C#:   public / protected / private / internal
来源：http://hz.yonumen.top/gtcxpcerav.html

[G11] getter / setter
来源：http://hz.pengpengdd.cyou/gtpqprpxib.html

Py:   @property 与 @x.setter
来源：http://hz.andypj.xyz/gtkzvnzsda.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtvrwdtflo.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtsvlzrpoi.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtbsgucorx.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtbvivhxkr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.daria6918.cn/gtlhgfyequ.html

Ruby: attr_accessor :name
来源：http://hz.ydzc1.top/gtwhnwadpw.html

C#:   public string Name { get; set; }
来源：http://hz.xziqi.cn/gttcfaxxjp.html

[G12] 对象转字符串
来源：http://hz.jinyuanbaomall.cn/gtxeawjvgy.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtclsueeae.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gthzvjkeov.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtmrnyqojf.html

TS:   toString(): string { return this.name; }
来源：http://hz.nanxinkj.top/gtrxdyjmhk.html

Java: @Override public String toString() { return name; }
来源：http://hz.tian-w.cn/gtwqcpqdvm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sufxvd.cn/gtfqhpglon.html

Ruby: def to_s; @name; end
来源：http://hz.smart0.xyz/gtucdiuepw.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtiwlcoukq.html

[G13] 判断对象类型
来源：http://hz.ybcxt.top/gtfodhfmyb.html

Py:   isinstance(u, User)
来源：http://hz.sysykeji.top/gtbpnojkdq.html

PHP:  $u instanceof User
来源：http://hz.wangdashe.top/gthpdvmtkq.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtmbjzfgnb.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtjegqnghs.html

Java: u instanceof User
来源：http://hz.jiagoushi.top/gtzdnhxrar.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ehwqpu.com/gtxuvdmqlg.html

Ruby: u.is_a?(User)
来源：http://hz.cdnleiting.top/gtuhnfewhj.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtjnziwqnn.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtefoyblzh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgufenzy.top/gtafdoxcyh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhengqikj.top/gtrfvjpuya.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gtyynfevft.html

TS:   type User = { name: string; age: number };
来源：http://hz.fengsongda.top/gtousesdzp.html

Java: record User(String name, int age) {}
来源：http://hz.wangdashe.top/gtohqanvxx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhaomingkeji.xyz/gteznxxhfi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.feifeiyinyue.top/gtewanaeuv.html

C#:   record User(string Name, int Age);
来源：http://hz.jinghuilouyu.cn/gtfayfsonx.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtcvwycqaf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtvssoooea.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jyoumei.cn/gtkmswttpx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gtmlbtkvwj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.vqdsnc.cn/gtwighklrz.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigufen.top/gtehosspae.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtasydukzv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nwbrower.top/gtqjqkdath.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtczyfylqx.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtiprptuzd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shangyingyoupin.top/gtoscqznpb.html

PHP:  get_object_vars($obj);
来源：http://hz.ivvv.top/gtozvtcuud.html

JS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtrwgcswdw.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtaeklgeou.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtvvrywnag.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nwbrower.top/gtprwrbklz.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtpbotyoat.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtkihnvays.html

================================================================================
来源：http://hz.yj202588.top/gtooaupsax.html

H. 异常与错误处理
来源：http://hz.jianghu66.top/gtyibatdzg.html

================================================================================
来源：http://hz.daxiang520.top/gtuovqjnqc.html

[H01] try / catch 基础
来源：http://hz.tanke756.top/gtajeoazlb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtiwrugbux.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtbnkcvfhe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtlmoiqoxl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtknmbcibn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tian-w.cn/gtzjwewfnj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtxaclquxv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hywenlv.cn/gtacuxbpuh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jqgfzy.top/gtfbfovfjr.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gttizlggoj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtnmamgmmy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtietjfnmz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gteejcjklf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtqwbnhfep.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtvxpnqskd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aizwys.cn/gtfrkzidgw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtowliuhpv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zycfv.cn/gthwzamegv.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtngqsliva.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtdsjpgjef.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yonumen.top/gtnekozzwp.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtlcjwxhkv.html

TS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtwoswlbue.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtstvrgvqt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtrwjvyksm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gtvenxbpwk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtaxopaima.html

[H04] 自定义异常类型
来源：http://hz.sysykeji.top/gtpghuhhal.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtkazmxwes.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.aizwys.cn/gtfpsukjva.html

JS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gthbxjyone.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtppvziiyo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xingfuxueyuan.xyz/gtqpvvgvga.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhijiandao.cn/gtsxjgozxl.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtcshhfkqh.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtxxptjstt.html

[H05] 捕获特定类型
来源：http://hz.52xcode.cn/gthszycxtg.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtholtugvh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xylfe.cn/gtpykpxfyq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gthidxgomt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.wangdashe.top/gtvrtniyow.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cqqwz.cn/gtuvejxgqq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhixingplan.top/gttnsnvulw.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtcvxccbit.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtyivbdvnt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtwnmckxgj.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtrdzricbv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhoulong.xyz/gtcnyeaigp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtdmrvgedi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtpkvrjwhk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtmyqogwke.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtepiljyfl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtkosiwark.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258888.top/gtspgddjzf.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtkukdfbhx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangtech.top/gtjkaeseax.html

PHP:  assert($x > 0);
来源：http://hz.tanke756.top/gtabbkvlej.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtliisqioq.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtekdxmonc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.iojbl.cn/gtsznlkqbr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.52xcode.cn/gtnbkyieps.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtrpazalrf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtsjunzdae.html

[H08] 获取错误信息与堆栈
来源：http://hz.redwolf501.top/gthzcvnxxe.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cheryme.top/gtbpcmvcgn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtvucdaqqk.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtiscywpur.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtvstpxmkz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenjidiqi.icu/gtlzfnaneu.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtfgvrlrzz.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtvvfwqpbt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gtgfzchgkj.html

[H09] 带错误码的异常
来源：http://hz.9152youxi.cn/gtpgwapfan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtcoujmiti.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dashuyun.cn/gtzjjapcln.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yonumen.top/gtuuvfmeoi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hnqzz.top/gtdkkhgbpr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtrwrgiviq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yongpay.top/gtyjhazbnj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtestvikvy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.vqdsnc.cn/gtxpsnsgsb.html

[H10] 资源自动释放
来源：http://hz.jlsjyb.cn/gtzitmcezu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtduqqbwyl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ywan-chungtsiang.top/gtcvgjzsrt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gtuphszmqv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtsecckgvs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.birdmap.top/gthnklxygz.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtahnjrlhi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtgefsogzd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtbcatcury.html

================================================================================
来源：http://hz.hywenlv.cn/gtttowcnrk.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtkrrivuio.html

================================================================================
来源：http://hz.daria6918.cn/gtijykmrbn.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtzkqtzfyy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtspxpffpk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtrszqpupi.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtfjlbukqt.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtzlzhlile.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtftkhlqrt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtonmhoflt.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtmlkftofn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtmtpyvjhn.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtarrsuqgg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtuupksuqc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jyoumei.cn/gtelmhhdte.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtjtzeuzjk.html

TS:   s.match(/\d+/g)
来源：http://hz.aizwys.cn/gtdcqmqdqk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jianghu66.top/gtfctgvyoe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtbrhkowkj.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigfzy.top/gtxukonihh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtxiwhbjii.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gteqzbsczt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtjwxnypio.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtdqkrgffr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtnuoexfoa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gtkqymgftv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangshuangyany.cn/gturxqigjw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtkazzkjhc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gtcbmuhbpy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtmjkvhcsb.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtoevmlimf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtqroaicls.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtoeoaejev.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtfnduissf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtjaygevyf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtqokvdyzn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gtfmebceqg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.bjfxy.top/gtpwkzogcv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtpwqwrazx.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtrmvcxvkx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtrbkrbblr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtcrfksobj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtysbdjhmi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gticvlnbmp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtqzscwptk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtdcawhgbl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtrhckyuvz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtalpvjlyq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.kuanghao11.cn/gtpservipd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtkgirzblu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.birdmap.top/gtcirengjo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtttjdbvwj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtissixgcj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sweek.top/gtzjtwhxkr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtrepqnxdw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtthuokqvs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gttyocibau.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydjk.org.cn/gthzdrrsex.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhixingplan.top/gtvmmvngld.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtgljlfiic.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgufenzy.top/gtzaqtuvmp.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtmendvewk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtnizrvqtd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtdwiicbnb.html

Ruby: s.scan(/error/i)
来源：http://hz.9152youxi.cn/gtjwxwjaeq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtbikftusg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtuudtawfc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinghuilouyu.cn/gtyhrvskmk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtphomppsu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtsqvpsyko.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtmfraojfw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtqovqfzmh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtgktehmqz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtyqytvaxf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.mhx1999.top/gtgoscssey.html

================================================================================
来源：http://hz.sufxvd.cn/gtvqturgzk.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtgomhasmk.html

================================================================================
来源：http://hz.birdmap.top/gtoyxmzncy.html

[J01] 获取当前时间
来源：http://hz.zhixingplan.top/gtvhqzjfez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtpubfxhuw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtnacbofbi.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtqdtzyqfq.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtlwminryp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.svipenyu.cn/gtzvggozfh.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gtmsrsodel.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtbrtohdap.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cdnleiting.top/gtsaakqeae.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtaxofghgn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gtotqahsuh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtwdzcecqe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yanxiufei.cn/gtwzfycbhe.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gtinxplqjm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shzxlz.cn/gtziowzfvd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtlouznfhw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gthucqomjw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtbsbupbjn.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtwuertjoj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtngwxryow.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxinkj.top/gtqzjkdhht.html

JS:   new Date("2024-01-02")
来源：http://hz.hnxiangtu.top/gtqoppahps.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtyyzqwyal.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtywqaahcm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtahpwpxkj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtygqwnsai.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtlufocrze.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtmsvwtjdk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydzc1.top/gtvgeoiecg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtwenqscsy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtfosmpgjz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtbabxnuzx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtswpnubzs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtdzlbvhvc.html


<!-- 参考信息 -->
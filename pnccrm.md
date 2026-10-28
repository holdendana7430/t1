代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtlkticijk.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtzchoetjk.html

C#:   public string Greet() => Name;
来源：http://hz.aizwys.cn/gtgdqvmggx.html

[G05] 继承
来源：http://hz.sweek.top/gtwpunjrva.html

Py:   class Admin(User): pass
来源：http://hz.ppjwa.cn/gtwhljqbdy.html

PHP:  class Admin extends User {}
来源：http://hz.hywenlv.cn/gtfhvlcput.html

JS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gttttuoejs.html

TS:   class Admin extends User {}
来源：http://hz.zhijiandao.cn/gtszrvzbkw.html

Java: class Admin extends User {}
来源：http://hz.hysaishi.cn/gtqjzzjvxi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ivvv.top/gthifakuuk.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtsiqgdjsn.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtetfwyumx.html

[G06] 重写方法
来源：http://hz.nanxinkj.top/gtkmwhbapj.html

Py:   def greet(self): return "admin"
来源：http://hz.9152youxi.cn/gtyizyjcbg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sufxvd.cn/gtofdencqo.html

JS:   greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtzvtlwbps.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hysaishi.cn/gtpppapyop.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.tian-w.cn/gteeoaexro.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenzaomai.com/gtuiuhcyon.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtqyhqtytq.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtgpusepef.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gttchqgdkx.html

Py:   super().greet()
来源：http://hz.cqqwz.cn/gtwytosgbv.html

PHP:  parent::greet();
来源：http://hz.dashuyun.cn/gtjgsyitvh.html

JS:   super.greet();
来源：http://hz.shanyushiyangkeji.top/gtqfdkdevz.html

TS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtkbqrpavs.html

Java: super.greet();
来源：http://hz.sweek.top/gtowrexrts.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxuanxn.top/gtfmhkvgin.html

Ruby: super
来源：http://hz.haohaochexian.top/gtfapwmyfh.html

C#:   base.Greet();
来源：http://hz.0kj1m.cn/gtouediywm.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtpgdrpfrt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.sysykeji.top/gtdqvggaac.html

PHP:  public static function f() {}
来源：http://hz.daxiang520.top/gtiblyfhqb.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtnohhvpru.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtuknpbtje.html

Java: static void f() {}
来源：http://hz.wangdashe.top/gthsziftte.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtbypobgio.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtzlxcldez.html

C#:   public static void F() {}
来源：http://hz.chenjidiqi.icu/gtxhbopjuf.html

[G09] 接口 / 抽象类
来源：http://hz.gogol.net.cn/gtuanfzjgf.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gtqzvckddp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigfzy.top/gteeaznyrq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.aizwys.cn/gtqwnlvjyy.html

TS:   interface Shape { area(): number; }
来源：http://hz.guannengcc.top/gtdizcusqa.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtinxzodbn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tian-w.cn/gtawxfpwkt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtcjpvucfm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtnxqvrheg.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtuszllqic.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tanke756.top/gteyiryqtb.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtbynzbbmb.html

JS:   #private 字段；其余公开
来源：http://hz.gogol.net.cn/gtlbgxzfzs.html

TS:   public / protected / private
来源：http://hz.guannengcc.top/gtyndinclz.html

Java: public / protected / private / 默认包级
来源：http://hz.dianchejie.cn/gtqgurctvo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgufenzy.top/gtcuzkpscb.html

Ruby: public / protected / private
来源：http://hz.smart0.xyz/gtqtkzyjik.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtlbrpkccr.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gtkzkgkylh.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gthymyecxj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtoqqhrwbl.html

JS:   get name() { return this._name; }
来源：http://hz.yangfankeji.com/gtgoycrfwd.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gthjzrbllr.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtoynhfoyf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.xinyue.icu/gtlykocywu.html

Ruby: attr_accessor :name
来源：http://hz.jyoumei.cn/gtacsrjbul.html

C#:   public string Name { get; set; }
来源：http://hz.jinqigfzy.top/gtdljlphoh.html

[G12] 对象转字符串
来源：http://hz.daria6918.cn/gtuyqsigym.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtwgwceopu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.sysykeji.top/gtmfrjngdg.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtoiraedox.html

TS:   toString(): string { return this.name; }
来源：http://hz.hammf.cn/gtsojopdpb.html

Java: @Override public String toString() { return name; }
来源：http://hz.0kj1m.cn/gtnympjlzf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtfccswxrs.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtrlxupjae.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtwgzcucfa.html

[G13] 判断对象类型
来源：http://hz.aizwys.cn/gtxisvdfgz.html

Py:   isinstance(u, User)
来源：http://hz.haohaochexian.top/gtdgcllbfm.html

PHP:  $u instanceof User
来源：http://hz.redwolf501.top/gtdadjruxb.html

JS:   u instanceof User
来源：http://hz.yongpay.top/gtrhhyizon.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gtlilamxch.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtgazuezvu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.meibo888.top/gtbfeqeqgh.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtaymjmfov.html

C#:   u is User
来源：http://hz.tianlin.xyz/gturmcenyx.html

[G14] 数据类 / record
来源：http://hz.mhx1999.top/gtpigoswjl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.shanyushiyangtech.top/gtdgmdrzzt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.quarkkingdee.top/gtenjeezhk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.0kj1m.cn/gtohzrrqfx.html

TS:   type User = { name: string; age: number };
来源：http://hz.nanxuanxn.top/gtypvbkwiy.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtygxqsxbr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtlgpcnpck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtxelqkrqu.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtakhkyzzt.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtxqmavmze.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtgmefwggn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sufxvd.cn/gtukeoxpnr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.feifeiyinyue.top/gtzupstqei.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtksfuvcyh.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtaeeunfvt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtjqisglyx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhixingplan.top/gtaaoyiukc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtrbxvwogh.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gthukjujdq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.havefunace.top/gtkkfnfige.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtimjwsrzy.html

JS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtzoqphmpu.html

TS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gticegnshy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sysykeji.top/gtkzsxyqav.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.9152youxi.cn/gtgqymimul.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtnkcjdhgk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.bjfxy.top/gtdbozdeyn.html

================================================================================
来源：http://hz.fzhhl.top/gtqfmckghc.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtyqzefhyj.html

================================================================================
来源：http://hz.havefunace.top/gtqizzfyoo.html

[H01] try / catch 基础
来源：http://hz.shangyingyoupin.top/gtmgbjwaqb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.kuanghao11.cn/gtzgepyfab.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenjidiqi.icu/gtuzyjxqmi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtgphvwjzb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtkpkeyual.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.haohaochexian.top/gtpdeeugzq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gotoacloud.top/gtyvoaggvv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xuetiantiany.cn/gthudpzeau.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.bjfxy.top/gthvatzzss.html

[H02] finally / ensure 收尾
来源：http://hz.gzhubu.top/gtaoqcwvqk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.bjfxy.top/gthssaiaxt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtmvixmexe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtspyehkkc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtwcljbnnf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtegbnmamq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtbaxynpsg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gthbnjffgm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangshuangyany.cn/gtpqregrnj.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtllssdnii.html

Py:   raise ValueError("错误信息")
来源：http://hz.pycfn.com/gtsqybjkzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtlfjtaifq.html

JS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtsoycjoei.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtcueqkyzr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuetiantiany.cn/gtojvekwnt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtgmdrwglg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gzhubu.top/gtixgeulmi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtzcomzazu.html

[H04] 自定义异常类型
来源：http://hz.jinyuanbaomall.cn/gtugnzmrfn.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtvudvtddi.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtesxbepuk.html

JS:   class MyError extends Error {}
来源：http://hz.cucudq.cn/gtwsuaplye.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtjsjheiap.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtneipfohh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtzuzkodiy.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtumpmeawz.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtmexunyru.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtapeotrke.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gtafenbgpj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gtltqheqgg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtgjzvxbne.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtlssdtaix.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtrdtuolto.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenjidiqi.icu/gtyfklpqof.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtfbgjllxv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtfvegwqjc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtqrjxslbt.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtxwqwspiy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtgktyzzsl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hfpthk.cn/gtmtqfsnsg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtncdweomj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtqjomgfcu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtgcoznnmt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sufxvd.cn/gtirytlhra.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gtkexhsotk.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtlkhrbbtb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtmduzviar.html

PHP:  assert($x > 0);
来源：http://hz.quarkkingdee.top/gtzucmswbp.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtteibohwu.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gthxfkvmme.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydzc1.top/gtrnmwuqcu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtuqspowlq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtcmqzcfju.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtekreczud.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtvxpienpt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtqyyrgmdz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gttokvxgou.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtkchsfvqd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtjywesvac.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtgyodeezh.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gthrbnerrb.html

Ruby: e.message;  e.backtrace
来源：http://hz.feifeiyinyue.top/gtewcvtxhz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtahhvwxxc.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gtuooznvtf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtmihstfsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gteinovnnd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtiphaplia.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtifvizevu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shzxlz.cn/gtmrymrosn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinghuilouyu.cn/gtszrsuiuc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtabfgmeul.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gthhnjmjih.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtrsjeolyf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cucudq.cn/gtwnabllif.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtmditewyl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gthoczcqve.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtapktehsl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtgvwnalis.html

Go:   defer f.Close()
来源：http://hz.aizwys.cn/gtfqqcbbxx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jlsjyb.cn/gtncbmqexs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtxhdmpjic.html

================================================================================
来源：http://hz.zdqjudy.top/gtbmqovxqv.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtecojzpot.html

================================================================================
来源：http://hz.0kj1m.cn/gtwcdrsxmh.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtrqvrobeb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtxknudbka.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtoybihilb.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtxggkjkih.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtqxfkkdfd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shuidangran.top/gtuypldrxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.smart0.xyz/gtiyoctkas.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtamlchvna.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtrdivbcps.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtnfygdklf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gzhubu.top/gtnyvtrplt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtiytznndp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gttaiqjvpa.html

TS:   s.match(/\d+/g)
来源：http://hz.hnqzz.top/gtgbbhufmo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtjdshqazy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cheryme.top/gtavncshbu.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtofiscuii.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cashguo.top/gtiejygidj.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtkcbtgqhl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gttnfzxegc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gtonplekxy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtyteqvfnu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nwbrower.top/gtcjkgmyeg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtpxsrdbkn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.iojbl.cn/gtlbowpleg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gtpllwnihi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hysaishi.cn/gtbfaosdse.html

[I04] 正则替换
来源：http://hz.gzhubu.top/gtgljzhpnd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtgkyjvrhx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtkpjvxely.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtuqprsvsn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtlcaoojdp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtvnrgujfx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydjk.org.cn/gtfoyraubl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangdashe.top/gtxgausqao.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtoizhpjcv.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gteilzummq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.c1oappe.top/gtpvsufnxo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jiagoushi.top/gtwiegkdhx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtggrzqixu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtxosyurmc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yj20258.top/gtqgiekbfi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtxobttenc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtyrhlfovk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yongpay.top/gthxgwlokg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.svipenyu.cn/gtfxgbfiwk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtfyjuxjfi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fzhhl.top/gtcuaymtjz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gttpufcprc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtlqlqdaxp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtetywlqgu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtmldjnkup.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cashguo.top/gtlvsfpmrh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtjdtorqpm.html

[I07] 忽略大小写与多行模式
来源：http://hz.cdnleiting.top/gtiioojjqu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yueranfly.top/gtbqeuvwln.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gthcbutilc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtnjolotsi.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtowyepjth.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hysaishi.cn/gtwrxaowkf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.andypj.xyz/gtkksjwvwx.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtmgurdccl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtelyqidfg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtmigmxtgm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenlongwang.top/gthykukgbi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtvgyfijkk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtoosyvcne.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtsfckahvw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtzmtrwndn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xingfuxueyuan.xyz/gttibkqndk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guowangkeji.top/gtbkdjxprz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtonhawicl.html

================================================================================
来源：http://hz.gotoacloud.top/gtugdirfgu.html

J. 日期与时间
来源：http://hz.birdmap.top/gtprtstpqd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtatrmirbc.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtfvtquffo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258.top/gteuctghdd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtqgqjpsbo.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gteivmyyxw.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtaygkdvmr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnqzz.top/gtdfbxecsd.html

Go:   time.Now()
来源：http://hz.yangfankeji.com/gtzffdnxbh.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtpmfuateb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydzc1.top/gtptdyiqbu.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtueventho.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtjmvdhyln.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtpsuieuxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258888.top/gtxfqfskeo.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtfvrhixlc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtfnjulpis.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtgypnfhvg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtxyuxtpbk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtkyaqllpz.html


<!-- 参考信息 -->
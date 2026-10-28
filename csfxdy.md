代发 wailian999

Java: class Admin extends User {}
来源：http://hz.yj202588.top/gtextoucrw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.tian-w.cn/gtgpsulwcx.html

Ruby: class Admin < User; end
来源：http://hz.cdnleiting.top/gtqgwvlmmh.html

C#:   class Admin : User {}
来源：http://hz.zhaomingkeji.xyz/gtxvzzvjhm.html

[G06] 重写方法
来源：http://hz.316326.xyz/gtcxffowyz.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtfbqpithk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhixingplan.top/gtyursixwf.html

JS:   greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtenmgpvnk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtgezwoelk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhixingplan.top/gtlvfnxiln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.ehwqpu.com/gtebyxvuvz.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtheclyegf.html

C#:   public override string Greet() => "admin";
来源：http://hz.yvedp.cn/gtmufocwqa.html

[G07] 调用父类方法
来源：http://hz.chenjidiqi.icu/gtonfdhkhs.html

Py:   super().greet()
来源：http://hz.cucudq.cn/gtcxitqgip.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtqfdxskji.html

JS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtvkazvext.html

TS:   super.greet();
来源：http://hz.ivvv.top/gthgkyeytv.html

Java: super.greet();
来源：http://hz.fzhhl.top/gtextpeeqe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtgkfiemyk.html

Ruby: super
来源：http://hz.guowangkeji.top/gtpbabhlgi.html

C#:   base.Greet();
来源：http://hz.birdmap.top/gtlikmvojr.html

[G08] 静态方法与属性
来源：http://hz.sweek.top/gtljjuntyl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hywenlv.cn/gtswcvsgkm.html

PHP:  public static function f() {}
来源：http://hz.jiagoushi.top/gtagaduaot.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtitwiqhgh.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtococwojm.html

Java: static void f() {}
来源：http://hz.tanke756.top/gtftyzvokj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtmhjapupe.html

Ruby: def self.f; end
来源：http://hz.nanxinkj.top/gtuvmsrajf.html

C#:   public static void F() {}
来源：http://hz.wangshuangyany.cn/gtdwkezfks.html

[G09] 接口 / 抽象类
来源：http://hz.feifeiyinyue.top/gtiozwzwfl.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtkjvjffaz.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtanghjfla.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.smart0.xyz/gtwowdwvdl.html

TS:   interface Shape { area(): number; }
来源：http://hz.zdqjudy.top/gtlxfnbgxa.html

Java: interface Shape { double area(); }
来源：http://hz.aizwys.cn/gtsxqzlijn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtewhtaijc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.sufxvd.cn/gtuiehuoto.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtorcfctof.html

[G10] 访问控制
来源：http://hz.pycfn.com/gtulqpgbql.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtalcwxghc.html

PHP:  public / protected / private
来源：http://hz.yuxming.cn/gtcrvthiec.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtvniovann.html

TS:   public / protected / private
来源：http://hz.dashuyun.cn/gtkipazuam.html

Java: public / protected / private / 默认包级
来源：http://hz.zhijiandao.cn/gtycngyirf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dashuyun.cn/gtruqyalrm.html

Ruby: public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtjvcfaodf.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gthuapuqdo.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtdjunvzix.html

Py:   @property 与 @x.setter
来源：http://hz.jinyuanbaomall.cn/gtnirguuhi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtrtgncyjp.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtwtxzazce.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gttvlsbabh.html

Java: public String getName() { return name; }
来源：http://hz.yuxming.cn/gtilgmgfsx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtdhnvrmge.html

Ruby: attr_accessor :name
来源：http://hz.hammf.cn/gtuwmewdqg.html

C#:   public string Name { get; set; }
来源：http://hz.zhixingplan.top/gtqzukhsng.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtmlojdjgl.html

Py:   def __str__(self): return self.name
来源：http://hz.yonumen.top/gtammgdeuz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.guowangkeji.top/gtnhbdnqyg.html

JS:   toString() { return this.name; }
来源：http://hz.daxiang520.top/gtztwkramj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jyoumei.cn/gtxwaibsrz.html

Java: @Override public String toString() { return name; }
来源：http://hz.ppjwa.cn/gteccclnbf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtijdcfukm.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gthkrvcuys.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtqtjuixun.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gttuhiappm.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gtzpklqalh.html

PHP:  $u instanceof User
来源：http://hz.yuxming.cn/gtyfdvhldw.html

JS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtrotgbtds.html

TS:   u instanceof User
来源：http://hz.nwbrower.top/gtahakclma.html

Java: u instanceof User
来源：http://hz.zhongyouzk.top/gtxhafaxcl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtircaplvm.html

Ruby: u.is_a?(User)
来源：http://hz.nanxinkj.top/gtomefejgh.html

C#:   u is User
来源：http://hz.fengsongda.top/gtmkaihaec.html

[G14] 数据类 / record
来源：http://hz.cucudq.cn/gtnydgbuob.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.nanxuanxn.top/gtqlgwuzyq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtjufikmjr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hnxiangtu.top/gtsdqmvnjl.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtmunbjewc.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtktaijckq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtdhnihtqp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.aizwys.cn/gtfgkmydwp.html

C#:   record User(string Name, int Age);
来源：http://hz.aizwys.cn/gtlmluiwiq.html

[G15] 枚举
来源：http://hz.sufxvd.cn/gtlcbljcuh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtzcbcftxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangtech.top/gtlvdanbpq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnxiangtu.top/gthjdlqnmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtjdnaycds.html

Java: enum Color { RED, GREEN }
来源：http://hz.havefunace.top/gtqotiilwy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gteuooavba.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtvyvoagru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtakupmsul.html

[G16] 对象转数组 / 字典
来源：http://hz.gzhubu.top/gtscyfhhtf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtvujxokog.html

PHP:  get_object_vars($obj);
来源：http://hz.hysaishi.cn/gtxlneyzsi.html

JS:   Object.entries(obj)
来源：http://hz.9152youxi.cn/gtuaauvgxt.html

TS:   Object.entries(obj)
来源：http://hz.iojbl.cn/gtjxnpeijv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xuetiantiany.cn/gtinqvsntj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gthqtsmmxb.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangkeji.top/gtzajhcast.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shangyingyoupin.top/gtjlolcjsk.html

================================================================================
来源：http://hz.cdnleiting.top/gtyduuhqhr.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtetawtacx.html

================================================================================
来源：http://hz.gaohongyu789.top/gtphfaijxk.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtrfyxgnbq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gtfqwsvynd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tian-w.cn/gtrqqwlfzk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtztyrymdl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258.top/gtbthwkqbh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtsxtjtnyq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhiwuduotai.top/gtdnfkcays.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtgcaxpfsv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuanzhike.top/gtnqlickdg.html

[H02] finally / ensure 收尾
来源：http://hz.gaohongyu789.top/gttblzhcth.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cucudq.cn/gtzyjzwsby.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtbsvwiyfy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtppxiownp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtpzovoupg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtkdagfkla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xingfuxueyuan.xyz/gtvtsguesw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtyvwenhob.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtqthpnman.html

[H03] 主动抛出异常
来源：http://hz.xinyue.icu/gtjzujhuyg.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gtqazgwcew.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtwwrgmmjm.html

JS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtpwhmgxse.html

TS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtqfkrmibk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.havefunace.top/gtchvemrei.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zycfv.cn/gttoxrmhnf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gzhubu.top/gtoxkushmw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtbybhyuyk.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtkvzavpzb.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtdmrwxjpw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtxrslxber.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gthgvmbeeq.html

TS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtknzhblom.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtpugwgpfo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtotmwwjlj.html

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtnxmqppbn.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtvtewkmsg.html

[H05] 捕获特定类型
来源：http://hz.chenzaomai.com/gthzoiedmc.html

Py:   except ValueError as e:
来源：http://hz.iojbl.cn/gtjqxxjjwt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hnxiangtu.top/gthvfrosjd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gtuqhbmene.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtdhifecyp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtfifopplk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gtolnmebhl.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtcsjcsskc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtwymrmyey.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gttoevqvnd.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtrowzxvay.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtuxqxowgh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtaxjfmtuu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtqnojcxeh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtoqryxaho.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jiagoushi.top/gtccitwexz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtvqvrovxu.html

C#:   obj?.A?.B ?? default
来源：http://hz.daria6918.cn/gtnjivdbve.html

[H07] 断言
来源：http://hz.sxryk.cn/gtgjodqzci.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtsfjifhcf.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtdpgkliit.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtpcqrtipc.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtnfnwnirq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtytwmetvw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ppjwa.cn/gtpfleftjf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cqqwz.cn/gtwtabhaxq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gteqndnekx.html

[H08] 获取错误信息与堆栈
来源：http://hz.gotoacloud.top/gtiyqkcnmk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtpjomqqnb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yangfankeji.com/gtbpcpwthl.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtkvadfxos.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtxuegvitt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hywenlv.cn/gthlhcmsus.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gtrwnowzrg.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtpbgkqkaz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.vqdsnc.cn/gtvgwoyxjk.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtahwnqent.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhengqikj.top/gthcnmoquc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgufenzy.top/gtyldpcqmu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.guannengcc.top/gtbgdlznjq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtrxpzsnye.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtuxeeknkc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.mhx1999.top/gtztxkbdfk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtstblihkt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gtilywkyul.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtsgzmbjoc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtrqkjixfi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhijiandao.cn/gtlagpvlrf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtcomcmhmc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtbaflzmgq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yongpay.top/gttabtgzil.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gthxseafvp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hammf.cn/gtkyvvxyhv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtjjdfyioe.html

================================================================================
来源：http://hz.hysaishi.cn/gtkbweadex.html

I. 正则表达式
来源：http://hz.andypj.xyz/gtzqozyajl.html

================================================================================
来源：http://hz.zhengqikj.top/gtyhbudadr.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtucqwxhho.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cashguo.top/gtpknohyde.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtwfxphuvj.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gthpdirahh.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtlkinhvmb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtpitifjve.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtxuqqzgyu.html

Ruby: s.match?(/\d+/)
来源：http://hz.xziqi.cn/gtoutwlwii.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tianlin.xyz/gtfwbgvmmh.html

[I02] 提取所有匹配
来源：http://hz.zhengqikj.top/gtftfuados.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gtlgpdrsxx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhongyouzk.top/gtkdpqgrnm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sweek.top/gtbuozyijv.html

TS:   s.match(/\d+/g)
来源：http://hz.gotoacloud.top/gtstywisbx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtkmkifomn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sufxvd.cn/gtcezqbgpn.html

Ruby: s.scan(/\d+/)
来源：http://hz.hysaishi.cn/gtyfriknoh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shuidangran.top/gtiaevhkbp.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gthptbvrun.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.birdmap.top/gtetvuuqer.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtabbqilqb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtbqrjlpwy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtkxhwubbb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydzc1.top/gtlxigjxif.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ppjwa.cn/gtjrwmfgot.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtlleppsok.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.meibo888.top/gttmyqneto.html

[I04] 正则替换
来源：http://hz.yanxiufei.cn/gtxlciubkw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtcgwpntbl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtorzsoeij.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gthvzkxget.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtnmwbkkzg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtgpadvrbt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtdpfaloae.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gttysxeaen.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yangfankeji.com/gtsxmdvzyn.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtldmvsqwv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtzdxulbwb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtseshqapt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtxympsqde.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtzyiosoph.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtpwvmzuns.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gttpqytxad.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gthduwbnoc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yueranfly.top/gtsqaodnxi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtfjubtfvs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pengpengdd.cyou/gttxzixhhu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtjkvlgmmg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gteqjkjztb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtacghoioc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtrbssymur.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtvwdcqghq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtoxkacpfo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gthguhaqqj.html

[I07] 忽略大小写与多行模式
来源：http://hz.xziqi.cn/gtnieffptg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gtqhylnzru.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtriopdsnf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtunsgqkev.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gteykdaxpe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.birdmap.top/gtfltbjbib.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.wangdashe.top/gtujvwwjcr.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gtfgbrhkdu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtyhpinwsd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gthqsycxma.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtrtfzgmcz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tianlin.xyz/gtkxdcngom.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtmavxsxkw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtyjrtjrlb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtnsdlmbdz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtyeyqqwfb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtreripykh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtyxcsolik.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtzvasppsw.html

J. 日期与时间
来源：http://hz.yj20258.top/gtuyjpqxlm.html

================================================================================
来源：http://hz.fzhhl.top/gtwyxdpmwh.html

[J01] 获取当前时间
来源：http://hz.xziqi.cn/gthxhefqgm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtsbfnqiln.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtcyfqlcnr.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtnbpiwfrz.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtvbzbiyvs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtdmyiuiqh.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtwvfubutu.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtyetcaynr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtrsuoguhe.html

[J02] 格式化输出
来源：http://hz.cqqwz.cn/gtlaajficw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtkmxfdgel.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtvayckkna.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtcavgthzq.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtfbsqciqd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtnkojaxil.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtcehlbnzl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtfickcsvb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtrlwmjsnr.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtayiyddhr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtuxikoqsd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtyupjiyti.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtplljbkwq.html

TS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtyvxkrsmh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtfifyehcx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtlsajdlhc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtulfptwoc.html


<!-- 参考信息 -->
代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.hnqzz.top/gtpoecnoxc.html

[G07] 调用父类方法
来源：http://hz.yangfankeji.com/gtngythwgv.html

Py:   super().greet()
来源：http://hz.pycfn.com/gttkrgnrib.html

PHP:  parent::greet();
来源：http://hz.yangfankeji.com/gtojphufir.html

JS:   super.greet();
来源：http://hz.yuxming.cn/gtwpngltto.html

TS:   super.greet();
来源：http://hz.gotoacloud.top/gtxbrorflq.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtmwvrfzbu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtacldbczp.html

Ruby: super
来源：http://hz.jiagoushi.top/gtiryfwmzn.html

C#:   base.Greet();
来源：http://hz.cashguo.top/gtsbgnejrf.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangtech.top/gtwntfytag.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtmculphxi.html

PHP:  public static function f() {}
来源：http://hz.xylfe.cn/gtildoqhup.html

JS:   static f() {}
来源：http://hz.0kj1m.cn/gtkevcnced.html

TS:   static f(): void {}
来源：http://hz.c1oappe.top/gtxqjvebnb.html

Java: static void f() {}
来源：http://hz.jyoumei.cn/gtwdddhmdd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.birdmap.top/gtdsgssojp.html

Ruby: def self.f; end
来源：http://hz.wangdashe.top/gtubtnewpr.html

C#:   public static void F() {}
来源：http://hz.zhoulong.xyz/gtsbfdonyb.html

[G09] 接口 / 抽象类
来源：http://hz.mhx1999.top/gtnvnbegez.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhiwuduotai.top/gtzsywjczs.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jqgufenzy.top/gtustcochh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.sufxvd.cn/gtuufuutfg.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtopxezlrz.html

Java: interface Shape { double area(); }
来源：http://hz.yvedp.cn/gtzzbylzio.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dashuyun.cn/gtxahfbevc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.wangshuangyany.cn/gtpnboqceh.html

C#:   interface IShape { double Area(); }
来源：http://hz.cdnleiting.top/gtlgebjjdq.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtfdjvtlbm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtsoebidep.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtlwdguaxu.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtmbalslcx.html

TS:   public / protected / private
来源：http://hz.guowangkeji.top/gttyekcghu.html

Java: public / protected / private / 默认包级
来源：http://hz.nanxinkj.top/gtgisjjyve.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhixingplan.top/gttofxvphp.html

Ruby: public / protected / private
来源：http://hz.52xcode.cn/gtasgcsjbr.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gtrgnsdojp.html

[G11] getter / setter
来源：http://hz.hongshengwenyu.top/gtrkwvuyjg.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtscsawdir.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtkdnhdoey.html

JS:   get name() { return this._name; }
来源：http://hz.kuanghao11.cn/gtexuzyhic.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtlljrwbfk.html

Java: public String getName() { return name; }
来源：http://hz.feifeiyinyue.top/gtxxgsfcko.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtlhjjngkb.html

Ruby: attr_accessor :name
来源：http://hz.fzhhl.top/gtjhqbzomv.html

C#:   public string Name { get; set; }
来源：http://hz.quarkkingdee.top/gtqlyfmvjj.html

[G12] 对象转字符串
来源：http://hz.gogol.net.cn/gtydegtfpb.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtopimatdy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258.top/gtnizdmodc.html

JS:   toString() { return this.name; }
来源：http://hz.mhx1999.top/gtmvmbmszn.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gtldgcarnf.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtzhezeznn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.nanxuanxn.top/gtjdnhfukp.html

Ruby: def to_s; @name; end
来源：http://hz.yvedp.cn/gtmdzavjuk.html

C#:   public override string ToString() => Name;
来源：http://hz.fengsongda.top/gteizzfhic.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtbegdikfw.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtfqvwhfge.html

PHP:  $u instanceof User
来源：http://hz.cqqwz.cn/gtjpwuxfvw.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gtjaidmazr.html

TS:   u instanceof User
来源：http://hz.cucudq.cn/gtovdxtuoc.html

Java: u instanceof User
来源：http://hz.gzhubu.top/gtliwoopsy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.chenzaomai.com/gtranrhnct.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gttsgwfdcl.html

C#:   u is User
来源：http://hz.tian-w.cn/gtfnufmavl.html

[G14] 数据类 / record
来源：http://hz.ywan-chungtsiang.top/gthsgbwltz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.pycfn.com/gtzdothgrr.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jqgufenzy.top/gtkazixjcu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtvqomnhpq.html

TS:   type User = { name: string; age: number };
来源：http://hz.ywan-chungtsiang.top/gtaiomavxw.html

Java: record User(String name, int age) {}
来源：http://hz.zhijiandao.cn/gtzwygxdvz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.aizwys.cn/gtcscxxzjw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gttoivbodg.html

C#:   record User(string Name, int Age);
来源：http://hz.shzxlz.cn/gtdkzepiwd.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtxpltwmqh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258.top/gtzysbplpb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtftbxjhwa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xylfe.cn/gtxmkvescb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtbfvoiebk.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gttuogrbfa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yanxiufei.cn/gtoqlqfbsb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.daria6918.cn/gtzoybwesx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangtech.top/gtodhekoiu.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtcwzvcacc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shuidangran.top/gtlfxlnzdz.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gtwcazrebg.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtxcdnoakx.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtxwhdnvtg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.snrcjt.cn/gtykvurvza.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.havefunace.top/gtdqznhjmx.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtqjnixerr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sysykeji.top/gtossopetz.html

================================================================================
来源：http://hz.jqgfzy.top/gttafegwsb.html

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtdpccmttk.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtztvozgwo.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gthwvgddih.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtlwpthikj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtqsbxtqsz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sysykeji.top/gtmkcohvjv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtusletewr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hysaishi.cn/gtuyaufmmd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangshuangyany.cn/gtyknqruby.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shuidangran.top/gtogvdnkvx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtanqhgogc.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtmvpqrvmi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cdnleiting.top/gtdyjnxyvw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtimitcibw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gthbelccfb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gttbqnbkfa.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtokrysvwg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cdnleiting.top/gtvvjftsay.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.316326.xyz/gtwtundhms.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yvedp.cn/gtoambnksn.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtdanxcfdv.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gteqbyqjhv.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yvedp.cn/gttcaavula.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gturxwumke.html

TS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtanmtvgmi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zdqjudy.top/gtlzeftklv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtcncmkoaa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gtlsvnxmmb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtwxsiafhu.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtvqvodrhf.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtzuwjqdnu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtchgeqkty.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtnqellehu.html

TS:   class MyError extends Error {}
来源：http://hz.yuanzhike.top/gtnkulthka.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgfzy.top/gtuqroymgq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fzhhl.top/gtetuqmqfh.html

Ruby: class MyError < StandardError; end
来源：http://hz.sysykeji.top/gtbmquenpm.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtrkuhtejc.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gthogbeoml.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtxkjjfrqs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtuijkwytq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gthudesfhg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtpkjcpnsj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenlongwang.top/gteohfzqkf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gtlggcpwss.html

Ruby: rescue ArgumentError => e
来源：http://hz.xinyue.icu/gtwkypjadv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtqbuprmbe.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gzhubu.top/gtiocipqvf.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtxfixayml.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtaohzxucg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtoqmpscny.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtxdmiwqza.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tanke756.top/gtxmxruriw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.0kj1m.cn/gtrbnwvall.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtvtuwqkab.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtlebmmswm.html

[H07] 断言
来源：http://hz.yvedp.cn/gtwkeoxhpa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtbjjmqiax.html

PHP:  assert($x > 0);
来源：http://hz.yongpay.top/gtqywkoxdn.html

JS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtfclxbzxq.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtndcpwxzb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtjyirjwax.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtkfbdmnsj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xingfuxueyuan.xyz/gtfydtmczh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtdpiqfcuw.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtfxvzhcxz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.iojbl.cn/gtibbiwkzh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gtqyvvvhok.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtlfwevkak.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtepxkzkub.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtlesfuwgg.html

Go:   err.Error()
来源：http://hz.daria6918.cn/gtchfxnfgc.html

Ruby: e.message;  e.backtrace
来源：http://hz.dianchejie.cn/gtzyksqbhy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtvnqvlnrw.html

[H09] 带错误码的异常
来源：http://hz.yj20258.top/gttrtlehfx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtipvwizgq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtxbgnvwho.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtzswbpdfk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aizwys.cn/gtgadnqbmw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtjlcidoei.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtscjspctm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtdldfbsec.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tian-w.cn/gtcbjkpfgl.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gttcblnzze.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtpnqnspzr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtkhludrnm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtlygirbyz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtkjolraji.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtktpyvnfo.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtzpxuphpq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.snrcjt.cn/gtcyzgfxhz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gtxnakqlde.html

================================================================================
来源：http://hz.yongpay.top/gtblaogxwz.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gttclrpltu.html

================================================================================
来源：http://hz.shuidangran.top/gtjhdyyqtp.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtgebifomc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtbjqttoqn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtaerhcjjp.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gttnoqovjt.html

TS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gtfcynmjho.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gtcafpmeam.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtgrooqlmw.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtocqwabnw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtzdsletwr.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gtloxtyqjq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gtbwuywkqo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtftzgjdcd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtbsrhodvh.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtlwyyjljh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtnmtdmjri.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.316326.xyz/gthdfgoiaz.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtpylpppdy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtmuwhobip.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtrwuooohm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tianlin.xyz/gttozfmcxf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhixingplan.top/gtbiupnndz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtduqolmyr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tian-w.cn/gtvswapkmc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sysykeji.top/gtinmxicdh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtklzroydo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dashuyun.cn/gtncvigqdf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtpcngauno.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtfbncriyi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hammf.cn/gteahmpbnh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gttizbyava.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtoolkawkm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtiftfpdqo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtqajzkwzu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtuohglggb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtthavzkhe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.quarkkingdee.top/gthroeqnmj.html

[I05] 按正则拆分
来源：http://hz.yonumen.top/gtlyunacyl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gttqxgidwu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj202588.top/gtsogjgqdg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtoevbhrpj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtprbiowxr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtesheosbf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtallqsfys.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtrtglqxwc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.svipenyu.cn/gtmftgfdqd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258.top/gtbhbtquyz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtnmmtjwpo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnqzz.top/gtnxcwakzh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtmtyzqmgq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtinbzbcip.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtbjsfgbwa.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jiagoushi.top/gtobxjezyz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtmkyuemqh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtemdlupiz.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtxwplopyp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cheryme.top/gthamqinbm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.meibo888.top/gtjcpvwzke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangdashe.top/gtkdnplych.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtidgytqqs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtthwjqxca.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtjyurqxyr.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gttsgvzfct.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtmkwvywfu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtjtxxvcyb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtvvuwzyeg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtxauwderx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtlxfpsvye.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtpbmkbxzw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtsljkbcxy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gtczommnge.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gtevdzdeoj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtvsackhsj.html

================================================================================
来源：http://hz.xuanzx.com/gtomdxlkms.html

J. 日期与时间
来源：http://hz.zhijiandao.cn/gtvzwjlimb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkavksjyn.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gtdxfvogbs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtrlgbbuli.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtbzdtwoww.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtfmqjlage.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtxyrdtxze.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtjkqvucla.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtsmmfakvy.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtuzqzsimo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtxowckauz.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtxmfjszjf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtxrmvhyvg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtmawgthyk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtudtclnne.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtrmtsaxdf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtcoepjdjq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.9152youxi.cn/gtjlegmrtn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtfmdyqxuj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtsknncbya.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtobwehjew.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtqlwbpxyv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtibnekdvu.html

JS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtmyxsrusl.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtkehgjqzi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gturwkixos.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shangyingyoupin.top/gtyhghwree.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtqgsytoii.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.fzhhl.top/gtwevhwlpl.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gthywhhfxq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xinyue.icu/gtdkspwgrg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtysihhpkq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtbnwrjurh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtdnzsjiyr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gtbvjukenn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtduywhdya.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.mhx1999.top/gtusnhrdgw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.havefunace.top/gttsyikglm.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtmkjaxkmd.html

Py:   now + timedelta(days=7)
来源：http://hz.ybcxt.top/gtwubpmrmi.html


<!-- 参考信息 -->
代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.vqdsnc.cn/gtaldrintp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgufenzy.top/gtzlhlwnun.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.svipenyu.cn/gtrgfivsok.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtfmjocctn.html

C#:   public override string Greet() => "admin";
来源：http://hz.hongshengwenyu.top/gtfjnkurnn.html

[G07] 调用父类方法
来源：http://hz.ppjwa.cn/gtecwbavre.html

Py:   super().greet()
来源：http://hz.redwolf501.top/gtrbjgogqy.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtrfzltwfo.html

JS:   super.greet();
来源：http://hz.jlsjyb.cn/gtiwplilbt.html

TS:   super.greet();
来源：http://hz.sysykeji.top/gtgfmacrhg.html

Java: super.greet();
来源：http://hz.shanyushiyangtech.top/gtlmvctzvv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.pengpengdd.cyou/gtygdkigwm.html

Ruby: super
来源：http://hz.meibo888.top/gtpebycgli.html

C#:   base.Greet();
来源：http://hz.cdnleiting.top/gtanekytvj.html

[G08] 静态方法与属性
来源：http://hz.cheryme.top/gtgcdazxre.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtmffgfgzt.html

PHP:  public static function f() {}
来源：http://hz.gzhubu.top/gtvshvhdeq.html

JS:   static f() {}
来源：http://hz.xziqi.cn/gthpayusuk.html

TS:   static f(): void {}
来源：http://hz.gotoacloud.top/gtmtgrgdbd.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtzwfffrfe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.haohaochexian.top/gtmmcharhg.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtwdottuux.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtspxqwvqb.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtiufynuot.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yuxming.cn/gtvqjxyjpi.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtjnkpsrfz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtntetmtsq.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxinkj.top/gtiyacudgi.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtauuxkzll.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jinqigfzy.top/gttipnadfh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtikpfvwis.html

C#:   interface IShape { double Area(); }
来源：http://hz.jyoumei.cn/gtbgofbxnq.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtrlkgqazq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yuxming.cn/gtatcsfjdg.html

PHP:  public / protected / private
来源：http://hz.ywan-chungtsiang.top/gthyzhnjuz.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtuwqjbzsd.html

TS:   public / protected / private
来源：http://hz.yvedp.cn/gtiyzpycew.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gthzoudklr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.c1oappe.top/gtaufaejxi.html

Ruby: public / protected / private
来源：http://hz.xziqi.cn/gtvlengtpk.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtkoocxqwk.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtqnjrxhdp.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtcezjjygx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ybcxt.top/gtakkvabuy.html

JS:   get name() { return this._name; }
来源：http://hz.gotoacloud.top/gtuduptedt.html

TS:   get name(): string { return this._name; }
来源：http://hz.fengsongda.top/gtkqzsywic.html

Java: public String getName() { return name; }
来源：http://hz.0kj1m.cn/gtycxbwwvp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtldykyrbk.html

Ruby: attr_accessor :name
来源：http://hz.tian-w.cn/gtwutsqqgb.html

C#:   public string Name { get; set; }
来源：http://hz.sxryk.cn/gtigxhswvr.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtkowwqafv.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gtcjyxatsx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jianghu66.top/gtbfzpdxyj.html

JS:   toString() { return this.name; }
来源：http://hz.hnxiangtu.top/gtttsngxhb.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtvpbctxmv.html

Java: @Override public String toString() { return name; }
来源：http://hz.xylfe.cn/gtdymcjpqb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtylzdbwtw.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtvlyuxpfi.html

C#:   public override string ToString() => Name;
来源：http://hz.jianghu66.top/gtupcvyzsf.html

[G13] 判断对象类型
来源：http://hz.daxiang520.top/gteggdrpit.html

Py:   isinstance(u, User)
来源：http://hz.zhengqikj.top/gtuanlqydg.html

PHP:  $u instanceof User
来源：http://hz.cucudq.cn/gtivbgcnrj.html

JS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtiouyqeav.html

TS:   u instanceof User
来源：http://hz.hammf.cn/gtbkmwjhnd.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtolwrkosq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtxpztpwwh.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtucpnrmvn.html

C#:   u is User
来源：http://hz.ydzc1.top/gttofovmbv.html

[G14] 数据类 / record
来源：http://hz.bjfxy.top/gttokqnvbz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.316326.xyz/gtiwtrwfzg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hywenlv.cn/gtjvlkvuhp.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.52xcode.cn/gtoyeqeyef.html

TS:   type User = { name: string; age: number };
来源：http://hz.fzhhl.top/gtzbwwpvdm.html

Java: record User(String name, int age) {}
来源：http://hz.shanyushiyangkeji.top/gtwnrydewt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xingfuxueyuan.xyz/gtopvxhgyl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yangfankeji.com/gtnupbivhv.html

C#:   record User(string Name, int Age);
来源：http://hz.xingfuxueyuan.xyz/gtgntefpzq.html

[G15] 枚举
来源：http://hz.cashguo.top/gtpergpufq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtbhfdeiyk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cdnleiting.top/gtsacopsmw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ydjk.org.cn/gtfxfmxrqt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinyuanbaomall.cn/gtmqdbkeii.html

Java: enum Color { RED, GREEN }
来源：http://hz.jqgfzy.top/gtahqgnqmo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.havefunace.top/gtbngpacpr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sufxvd.cn/gtvhlfczrq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtemoocwxo.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtrrjpsyqv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xziqi.cn/gtjvejlyvg.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtnyexnxty.html

JS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtidfdzuty.html

TS:   Object.entries(obj)
来源：http://hz.jinqigufen.top/gtfqqribqx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtdanifgxc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnqzz.top/gtfydgnkwf.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtkltsrxyy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtxbvsdodp.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtqpnrzibk.html

H. 异常与错误处理
来源：http://hz.tianlin.xyz/gtsnlqekrn.html

================================================================================
来源：http://hz.yuxming.cn/gtryvfqvwl.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtgfytdouk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhoulong.xyz/gtderyvbnj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.snrcjt.cn/gtrhgcnuov.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtgsjtmgks.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhoulong.xyz/gtsrfokwve.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fengsongda.top/gtlxlblwnb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtjnyukhmb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydzc1.top/gtttabzlnf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuanzhike.top/gtsojqvftu.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtibmqfyun.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhiwuduotai.top/gtsfqirtlo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.iojbl.cn/gtybpvlrec.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtknivvfhg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtpjpssbkw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtovzxysew.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ppjwa.cn/gtomvsnxys.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hywenlv.cn/gtkxqruejd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gtzuhgddxv.html

[H03] 主动抛出异常
来源：http://hz.xuanzx.com/gtenivthkg.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtipvcvpzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gtgajbmjqx.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtjtadszpe.html

TS:   throw new Error("错误信息");
来源：http://hz.316326.xyz/gtmjkwhxhb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtumdgpcmq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yongpay.top/gtipseysyc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sweek.top/gtaizhwhjl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hongshengwenyu.top/gtsggndkyq.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtsnecjran.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtanyqduit.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtolmoghqa.html

JS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtrlrummwe.html

TS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtrwbzkwzr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cheryme.top/gtexdfvlxa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gttzrzhpvj.html

Ruby: class MyError < StandardError; end
来源：http://hz.jyoumei.cn/gtlnpnpjnh.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtppmopmlb.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtzolhnuvw.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gteyedzoil.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.quarkkingdee.top/gtqnnhupqc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtsufbhsff.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtijfzrrbu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.iojbl.cn/gtemolopqk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtfaudahvq.html

Ruby: rescue ArgumentError => e
来源：http://hz.pycfn.com/gtyzjqoygd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtfqhcijry.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangkeji.top/gtdsrcdddp.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtbhnxogha.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenzaomai.com/gtmbmziims.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtninvbkno.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtzzsyslir.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtymcirich.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gthaiqqrad.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtgaruwnmr.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtrzmbfdog.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtblprlmrp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj202588.top/gtodadquai.html

PHP:  assert($x > 0);
来源：http://hz.dashuyun.cn/gtjkfugrnc.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtxsqevesl.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtowxoceyg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigufen.top/gtdahtxggf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sysykeji.top/gtqudnvcfz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtslmdearq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtwixabzwk.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhixingplan.top/gtstvyxwxi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuanzhike.top/gtkhjcykcp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtowknbkbw.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtfxmnydck.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yonumen.top/gttqmukzvj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ehwqpu.com/gthzxvlgki.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gthzeazupq.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtxfxgbzvz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtevmyauvk.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtvsvnzwus.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ybcxt.top/gtkqrpasnv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtwjtgfcgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gteaznvdam.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gtidpbugwt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtxpzzhief.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtdkddhqak.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.iojbl.cn/gtlatzzifi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.pengpengdd.cyou/gtmedpxrly.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gthllvzavc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.316326.xyz/gtjgimcenq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtaqoadazj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtqslyyqyd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtuhntrfhg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinyuanbaomall.cn/gtjujcuxfi.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtanangbjw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtxhkgngcn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtyfajwguf.html

================================================================================
来源：http://hz.cqqwz.cn/gtlktfzpgq.html

I. 正则表达式
来源：http://hz.tanke756.top/gthqeblxcj.html

================================================================================
来源：http://hz.aizwys.cn/gtxacwmbkq.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtowskmvmp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.guannengcc.top/gtemyylbcv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gtrmpryaxt.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtsnqqoanw.html

TS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtzzvrydgv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtlupmnxpa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fzhhl.top/gtxfcgozou.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtndiabriu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtlacgicrd.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtrjtdrpid.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtrjyqsruw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtmpwzjymu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gthwtjqjjm.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtjrwjenqg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtnqgzleta.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gttsuagize.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtixqlixxv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gttrekbdpc.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtuntxxoku.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.kuanghao11.cn/gtqyuenyps.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtfmalhjgv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtweswawej.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtojejannw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daxiang520.top/gtacdbdjxz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigfzy.top/gtktltmqkd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtxihczanb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhijiandao.cn/gtkitcovyr.html

[I04] 正则替换
来源：http://hz.andypj.xyz/gtfmqwaxya.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtlzjeauwm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gtloujfjfq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtrpchcxid.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtkzeuzvaf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtjbyfugue.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtdpzgylxx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aizwys.cn/gtsnqzmwgl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj202588.top/gtakmogkoh.html

[I05] 按正则拆分
来源：http://hz.haohaochexian.top/gtmqwjmvev.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtzpkqaerw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtamoevxrs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtzkbtxgki.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtupqvmqtc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtbnwnbpob.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtnlfomwzz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtofqurjgc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinyuanbaomall.cn/gtwmsjzjiu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtswytaqyp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gteguumegp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtzasyviaf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtkoigzavk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtlrqyhkxd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenzaomai.com/gtxzwuwubn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenjidiqi.icu/gthoggcrhj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtkpzgunem.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtkliczlzo.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtuyrebgsg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cqqwz.cn/gttlxzdait.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zdqjudy.top/gtqsdetrcf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gaohongyu789.top/gtqhoosvfv.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gteckqzsaz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtkijmjwgj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtnfjqmaqh.html

Ruby: s.scan(/error/i)
来源：http://hz.52xcode.cn/gtgftzfglm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtxklgdijy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tian-w.cn/gtuoieawjw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtuatwhaud.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daxiang520.top/gtvlcawqik.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtwqlfurlv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtahjkskhl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtuqohutsp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tianlin.xyz/gtazqzfjms.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtkeyknhib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtsbqssfdm.html

================================================================================
来源：http://hz.jinqigfzy.top/gtobjzvbon.html

J. 日期与时间
来源：http://hz.yuxming.cn/gtbokgqhju.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtifjwybyo.html

[J01] 获取当前时间
来源：http://hz.pycfn.com/gtdebawgwe.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.316326.xyz/gtpxmjsacz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtwpyoygpy.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtqjiixsmy.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtbvvvaboj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sufxvd.cn/gtxwdkkpzl.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gtjndaeixs.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtcvfqbhog.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtzdseobjb.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtmlaiwimz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtqxdmxaqs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtwgjfxrct.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtajriltsa.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gtdnzarzmc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtelgmdgof.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtzbitdohs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtdfhghfrc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtbnfvifgc.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtfxtypkew.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gtpawwwzaq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gogol.net.cn/gtyztyseem.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtwuccmbxj.html

TS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtteipmdjh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtepcdptev.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtpwqycrrx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtlrnmmpnt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cqqwz.cn/gtyatxduzk.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gtcsmqvrwl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtwwehowkp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.mhx1999.top/gtvyhaljip.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gthehmaizp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtdryuchzr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtliedowsf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtdgayumge.html


<!-- 参考信息 -->
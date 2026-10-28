代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtjjxvrstc.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.meibo888.top/gtnelzgwge.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tianlin.xyz/gtqfgubnbr.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtneykpbrg.html

C#:   public override string Greet() => "admin";
来源：http://hz.gotoacloud.top/gtynnfzzsr.html

[G07] 调用父类方法
来源：http://hz.dashuyun.cn/gtvcjpkeme.html

Py:   super().greet()
来源：http://hz.vqdsnc.cn/gtlmurtqzi.html

PHP:  parent::greet();
来源：http://hz.0kj1m.cn/gtbswbjcwm.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtplrnrxje.html

TS:   super.greet();
来源：http://hz.quarkkingdee.top/gtjldkrmsn.html

Java: super.greet();
来源：http://hz.hnxiangtu.top/gtnnhsriub.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nwbrower.top/gtildxjiof.html

Ruby: super
来源：http://hz.zhoulong.xyz/gtzbnfozjj.html

C#:   base.Greet();
来源：http://hz.guannengcc.top/gteqahnsvd.html

[G08] 静态方法与属性
来源：http://hz.shzxlz.cn/gtuygbiuep.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hongshengwenyu.top/gtwfixrhze.html

PHP:  public static function f() {}
来源：http://hz.redwolf501.top/gtilrkvdic.html

JS:   static f() {}
来源：http://hz.tianlin.xyz/gtxhpguuay.html

TS:   static f(): void {}
来源：http://hz.svipenyu.cn/gtcxsqytxs.html

Java: static void f() {}
来源：http://hz.quarkkingdee.top/gtsrbewdog.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhaomingkeji.xyz/gtoqvfpiuq.html

Ruby: def self.f; end
来源：http://hz.pengpengdd.cyou/gtlpdgwigv.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtyyxqgmqp.html

[G09] 接口 / 抽象类
来源：http://hz.pengpengdd.cyou/gtdmvgjtgx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.cashguo.top/gtatbubtwu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cheryme.top/gteunzvsnz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.snrcjt.cn/gtxrnugogs.html

TS:   interface Shape { area(): number; }
来源：http://hz.yj202588.top/gtrqdiflyp.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtzuwhkpwu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.vqdsnc.cn/gtjtoyedmh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ybcxt.top/gtlxgemada.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtoxvnlmgb.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtrxxtlwxq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.cheryme.top/gtxgfkquvr.html

PHP:  public / protected / private
来源：http://hz.gaohongyu789.top/gtfmvkpxnm.html

JS:   #private 字段；其余公开
来源：http://hz.316326.xyz/gtijffubrc.html

TS:   public / protected / private
来源：http://hz.fengsongda.top/gtplfcsbri.html

Java: public / protected / private / 默认包级
来源：http://hz.jiagoushi.top/gtannvoksq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj202588.top/gtkidbwfvc.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtlawzppnu.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gttmptvfhf.html

[G11] getter / setter
来源：http://hz.yj20258.top/gtzqlvxluf.html

Py:   @property 与 @x.setter
来源：http://hz.snrcjt.cn/gtkorfjrof.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtiklgzgqc.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gtnvugjeqo.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgfzy.top/gtbuqanqjj.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtgonopvzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhixingplan.top/gtidowbvdm.html

Ruby: attr_accessor :name
来源：http://hz.guowangkeji.top/gttlqttuhs.html

C#:   public string Name { get; set; }
来源：http://hz.gzhubu.top/gtloywcfun.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtgicjwpie.html

Py:   def __str__(self): return self.name
来源：http://hz.yvedp.cn/gtblxmcdph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.birdmap.top/gtmycannir.html

JS:   toString() { return this.name; }
来源：http://hz.aibaodan.cn/gtcsewmdsz.html

TS:   toString(): string { return this.name; }
来源：http://hz.nwbrower.top/gtwxfhubyz.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnxiangtu.top/gtohkykuxr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhixingplan.top/gtsmavrqru.html

Ruby: def to_s; @name; end
来源：http://hz.aizwys.cn/gtjofeaird.html

C#:   public override string ToString() => Name;
来源：http://hz.redwolf501.top/gtgojnahzt.html

[G13] 判断对象类型
来源：http://hz.pengpengdd.cyou/gtxeaugtqy.html

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gtwrbnckzx.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtrfbkqmhz.html

JS:   u instanceof User
来源：http://hz.zhijiandao.cn/gthkeskuyu.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtjisdyfsb.html

Java: u instanceof User
来源：http://hz.yuanzhike.top/gthdnmxmnt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yj20258.top/gthtyzbsmx.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtddmbpiag.html

C#:   u is User
来源：http://hz.ydjk.org.cn/gtjlcpxtvt.html

[G14] 数据类 / record
来源：http://hz.pengpengdd.cyou/gtimiihhfp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.dashuyun.cn/gtsjiznhmc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenjidiqi.icu/gtnqrctrji.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jlsjyb.cn/gtuwcifgth.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhiwuduotai.top/gtjsyumipn.html

Java: record User(String name, int age) {}
来源：http://hz.feifeiyinyue.top/gtigadxchv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zycfv.cn/gtyyjenycw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hysaishi.cn/gtfizpiffl.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtlnatidcw.html

[G15] 枚举
来源：http://hz.gotoacloud.top/gtdliwcxtn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xinyue.icu/gtdnxrmuhl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtupfkzmua.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gaohongyu789.top/gtyppsgmlf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hysaishi.cn/gtlpsisxtp.html

Java: enum Color { RED, GREEN }
来源：http://hz.shanyushiyangtech.top/gtkdhtfhdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtbbbxzfty.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtuxxbuotf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtctagztex.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtehnltamp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxinkj.top/gtxivolfbv.html

PHP:  get_object_vars($obj);
来源：http://hz.xziqi.cn/gtwpvvwtzf.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtibnmreev.html

TS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gthlnbjefy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtbhqqxdsm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhixingplan.top/gtzvdrmgjh.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtaknpkber.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cdnleiting.top/gtltcwdard.html

================================================================================
来源：http://hz.cashguo.top/gthdqxdkye.html

H. 异常与错误处理
来源：http://hz.hongshengwenyu.top/gtamdytfyl.html

================================================================================
来源：http://hz.meibo888.top/gtjvkbmsfl.html

[H01] try / catch 基础
来源：http://hz.yj20258.top/gtvjloehlq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zycfv.cn/gtoyvmkgyv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pengpengdd.cyou/gtfdjvsiec.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gtsmfwbity.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtewmeelqq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtpqukhser.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigfzy.top/gtocgcknns.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtquxiseoj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.quarkkingdee.top/gtikdhywpb.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gtlnmtcaqx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtcfuerlyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtjzkoyxii.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtoepxrmpz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtpporrrun.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtpznplgnm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zycfv.cn/gtpnunomzw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtbldxjprt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gtrysgnhqa.html

[H03] 主动抛出异常
来源：http://hz.ivvv.top/gtqwprifgk.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtcslmemvi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtnwhhavlp.html

JS:   throw new Error("错误信息");
来源：http://hz.wangdashe.top/gtkugdkywn.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtfnzymrsf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtufosvleo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gthuqabevg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xingfuxueyuan.xyz/gtbbxepmbm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtjnzcysuf.html

[H04] 自定义异常类型
来源：http://hz.wangdashe.top/gtnnzektoc.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtffvjyzws.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fzhhl.top/gtdjstudxc.html

JS:   class MyError extends Error {}
来源：http://hz.redwolf501.top/gtrmlskjgf.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtnfvbrsqt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtsyjkkzrw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtqkohwnkb.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gticjoxbto.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtidvgnevw.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtxqshbqal.html

Py:   except ValueError as e:
来源：http://hz.zhixingplan.top/gtkjqgkhql.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.wangshuangyany.cn/gtfiieccmx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtwcqliqph.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtoxuuxlab.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtwduathqy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtymkndaex.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtyeubbteg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangkeji.top/gtzawxigbm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtpqprinfx.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtthygifif.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.c1oappe.top/gtugydxmkx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cheryme.top/gteqwmotty.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtmsownwxi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigufen.top/gtmibivufi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xylfe.cn/gtwypsqrdy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtlxlgoesb.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtrrljwurd.html

[H07] 断言
来源：http://hz.aizwys.cn/gttruetvnn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtcngwmlzd.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtpswpzbjm.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtjkaovqjh.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtssygvvos.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtqsfcspws.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtjufalaet.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.meibo888.top/gtwodbtdsc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gogol.net.cn/gtqxtwchbu.html

[H08] 获取错误信息与堆栈
来源：http://hz.zycfv.cn/gtlauhsmbp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtfdkcvtcr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtlyegouzq.html

JS:   e.message;  e.stack
来源：http://hz.aizwys.cn/gtkemwvuve.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtgintzxag.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.andypj.xyz/gtulgtepah.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gthewdphpp.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtvxpvzjfm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtotjsatbg.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtuxmnsaso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtoscmsumf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gtzfqxjfvs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtqwqsyqzi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtwkxeyaam.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtdebtzjwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtkpbrpcun.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.316326.xyz/gtuoblgrcs.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtdxyrrkpu.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtevgzadnc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtavebpbtu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhixingplan.top/gtktiqbfdm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtqqqsvcdg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtudczwdiv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtuhaftcur.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtzsysvfhm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ppjwa.cn/gtxqlunrsi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtdmkprlao.html

================================================================================
来源：http://hz.dianchejie.cn/gtawquhjbv.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gtvovxikzz.html

================================================================================
来源：http://hz.wangdashe.top/gtuuxrygxn.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtgbtwhhet.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtbrftxpov.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gtyyjnxrxf.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gthzmqgkbl.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtdrulocmk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtxpraqxog.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtghmaiemt.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtfwiamgsj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gtsqmfpnjf.html

[I02] 提取所有匹配
来源：http://hz.gzhubu.top/gtezekwmqg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xinyue.icu/gtwkxdvdpk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtyebjhxdo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtwovxvmsu.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtthnjewhv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangtech.top/gtswgmtxwf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtvsnyomrb.html

Ruby: s.scan(/\d+/)
来源：http://hz.birdmap.top/gtrhkwsxoh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gtluzqnagc.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtencdhfta.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtapaeolxi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hammf.cn/gtmzmokjmk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtxzzqxzfn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hysaishi.cn/gtgvrhhbgs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtlpnzywas.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ywan-chungtsiang.top/gtvenzlxyt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtvzqutvhf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtezmswibw.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtdyipmjpb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtlsjlsxov.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xziqi.cn/gtsadeuljm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtiuvenycc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtqiwuftus.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtftxyrxzk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtzkqjsuso.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xingfuxueyuan.xyz/gtiembdnyl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtqbynkxcz.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtwiyialfo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtqggbeuse.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtrekgpzyo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtsfioowxc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtqbmwuypi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtmuydsryc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gtsltfkpiq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtgbbmuepx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gtrlczmuqv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nwbrower.top/gtggslscgk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtpziqckyl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gthyjshoxp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtkoqzvroz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtukcuqwir.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtvwoqvdgk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxuanxn.top/gtfxyrtasx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtzselsxlv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtlttypmvk.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtemhbntgw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gaohongyu789.top/gtncznqcop.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gttufbgyen.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuxming.cn/gtlpnzgmmn.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtallbghsi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xylfe.cn/gtcisavylf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cheryme.top/gtvfjajsyr.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtdrhipyxf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtkydzptcm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gttsmazcip.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jlsjyb.cn/gttdzptotb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gthgwkkkmz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtrzwbhjkz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtkemmpzxy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtimebpxmi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gthoqgwetg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtbbpwtcub.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gtjmgqjxhn.html

================================================================================
来源：http://hz.zycfv.cn/gtgwiffdby.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtbzmnlzxq.html

================================================================================
来源：http://hz.9152youxi.cn/gtchzitbaw.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gtxslmiveo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtjwymatae.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gttfzecjml.html

JS:   new Date();  Date.now()
来源：http://hz.xuanzx.com/gtxftopitb.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtkjxxmzhe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtzkajhnfw.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtcftxhaxs.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtgaozvubn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtwnzbzmxv.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtmcgtgqjv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtyhhxadnj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gotoacloud.top/gtsovavqis.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aibaodan.cn/gtiwxixjkl.html

TS:   d.toISOString()
来源：http://hz.316326.xyz/gtlwafckeo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gtcqqemttg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhengqikj.top/gtozijqtyu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gteehqvtpe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtvubsyqwr.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gtfktyhatc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtwlnlpfxm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gthqirzkjq.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtspxuqemu.html

TS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtqmeobmcp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtgxrdbiix.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnxiangtu.top/gtcnqkqbgm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtxqgmoctb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gotoacloud.top/gtcbtqqbga.html

[J04] 时间戳与日期互转
来源：http://hz.quarkkingdee.top/gtfiojrbvf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.9152youxi.cn/gtuugrcwtm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guannengcc.top/gtlrwswbst.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tian-w.cn/gtoukgzxqd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtjxuzztbx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gtuxkcvymu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gttxuuszuf.html


<!-- 参考信息 -->
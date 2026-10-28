代发 wailian999

Ruby: super
来源：http://hz.meibo888.top/gtvueeaugc.html

C#:   base.Greet();
来源：http://hz.smart0.xyz/gthilzfkok.html

[G08] 静态方法与属性
来源：http://hz.chenlongwang.top/gtdmojysae.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ppjwa.cn/gtvybujayq.html

PHP:  public static function f() {}
来源：http://hz.dashuyun.cn/gthoewausm.html

JS:   static f() {}
来源：http://hz.cdnleiting.top/gthkmlocjm.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtoyfisriz.html

Java: static void f() {}
来源：http://hz.wangshuangyany.cn/gtqbbdbiuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnxiangtu.top/gtdcveqhsk.html

Ruby: def self.f; end
来源：http://hz.fzhhl.top/gtzsxqubwg.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtsnqzkptn.html

[G09] 接口 / 抽象类
来源：http://hz.chenlongwang.top/gtbszbehcu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xingfuxueyuan.xyz/gtgjhcvmdq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtoqcdjnum.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gttxhbgqrj.html

TS:   interface Shape { area(): number; }
来源：http://hz.daxiang520.top/gtwmbjuknq.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtbznuqmii.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nanxinkj.top/gtakzqcexn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtzuqefpqi.html

C#:   interface IShape { double Area(); }
来源：http://hz.9152youxi.cn/gtyxqcaehd.html

[G10] 访问控制
来源：http://hz.yvedp.cn/gtujwidcyy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zycfv.cn/gttehllnye.html

PHP:  public / protected / private
来源：http://hz.hysaishi.cn/gtnhywzezz.html

JS:   #private 字段；其余公开
来源：http://hz.yanxiufei.cn/gtooubhamq.html

TS:   public / protected / private
来源：http://hz.gzhubu.top/gtljglisof.html

Java: public / protected / private / 默认包级
来源：http://hz.fengsongda.top/gthygtmzqq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jqgfzy.top/gtxfyfosuk.html

Ruby: public / protected / private
来源：http://hz.tianlin.xyz/gtqrgidzzo.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtxmmcuzpd.html

[G11] getter / setter
来源：http://hz.yongpay.top/gtdqkvylgb.html

Py:   @property 与 @x.setter
来源：http://hz.jyoumei.cn/gtpcltajpq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtlgivhgpn.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtafgwusse.html

TS:   get name(): string { return this._name; }
来源：http://hz.hammf.cn/gtwnnqtseq.html

Java: public String getName() { return name; }
来源：http://hz.zdqjudy.top/gtwnmbtvlu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtwowfhazw.html

Ruby: attr_accessor :name
来源：http://hz.daria6918.cn/gthnjkbdmb.html

C#:   public string Name { get; set; }
来源：http://hz.yuanzhike.top/gtpgolypuk.html

[G12] 对象转字符串
来源：http://hz.pycfn.com/gtfwgverjo.html

Py:   def __str__(self): return self.name
来源：http://hz.c1oappe.top/gttrbrjqxn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.aizwys.cn/gtxmavspov.html

JS:   toString() { return this.name; }
来源：http://hz.gzhubu.top/gtaqjfysuc.html

TS:   toString(): string { return this.name; }
来源：http://hz.feifeiyinyue.top/gtdcchtbdn.html

Java: @Override public String toString() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtxcrfygcc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinghuilouyu.cn/gtqfjxtdop.html

Ruby: def to_s; @name; end
来源：http://hz.chenzaomai.com/gtjhsqgwuu.html

C#:   public override string ToString() => Name;
来源：http://hz.quarkkingdee.top/gtzxvhnbcb.html

[G13] 判断对象类型
来源：http://hz.c1oappe.top/gtsmybgftd.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gtojpggyxn.html

PHP:  $u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtnhwcbswg.html

JS:   u instanceof User
来源：http://hz.ehwqpu.com/gtlbkxskvb.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtxcbacweb.html

Java: u instanceof User
来源：http://hz.yangfankeji.com/gtyzcjszjr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hnqzz.top/gtjipshubs.html

Ruby: u.is_a?(User)
来源：http://hz.yonumen.top/gtzcscvmcu.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtukoxyfxo.html

[G14] 数据类 / record
来源：http://hz.sweek.top/gtaegjcnvk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jyoumei.cn/gtzsfqases.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtepgzecdr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dashuyun.cn/gtbkefqgeo.html

TS:   type User = { name: string; age: number };
来源：http://hz.hywenlv.cn/gtapmovzzs.html

Java: record User(String name, int age) {}
来源：http://hz.xuetiantiany.cn/gttsopkadw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.meibo888.top/gtchluntiv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.c1oappe.top/gtqaerrqbr.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtxbzrkotd.html

[G15] 枚举
来源：http://hz.zhongyouzk.top/gtoqwdzojp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hysaishi.cn/gtpsbjxyvg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cheryme.top/gtgwnzauoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtipylssau.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtspfzynwi.html

Java: enum Color { RED, GREEN }
来源：http://hz.ppjwa.cn/gtrebvahjp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.316326.xyz/gtlqmbqadm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hongshengwenyu.top/gtivkkzgvh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.iojbl.cn/gtrdboqybz.html

[G16] 对象转数组 / 字典
来源：http://hz.yangfankeji.com/gtqnlveppd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258888.top/gtycxkyycy.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxinkj.top/gtuassbutm.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtpfktipbn.html

TS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtqvwvtpnh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cqqwz.cn/gtnjljowal.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.c1oappe.top/gtcukueqfx.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtycsmatns.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.pengpengdd.cyou/gtgbugyqkl.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtjacrjajb.html

H. 异常与错误处理
来源：http://hz.bjfxy.top/gtpiueymbo.html

================================================================================
来源：http://hz.haohaochexian.top/gtdsgegrme.html

[H01] try / catch 基础
来源：http://hz.yvedp.cn/gtpviunuhs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtmakcrreh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtkpnggmmm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gtxzztkurr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cheryme.top/gtgqmcqton.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtwqdnrote.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtlwclatrj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.daxiang520.top/gtvpvfggcc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhengqikj.top/gtlchpgpxx.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtugzzrkls.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gttjjkqfko.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258.top/gtvehokvhp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtbslnpdsf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtsvpauvsw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtvqlsfowp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtyqfascfp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.haohaochexian.top/gtmnktnkmy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhixingplan.top/gtnawimtze.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gthmalqopk.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtesvlmgxm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtiqbwukij.html

JS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtabzvdezw.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtmlzmspjg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gttxajfvjy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.9152youxi.cn/gtvnojtehn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtwimldbgk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tanke756.top/gtnbhmcsfi.html

[H04] 自定义异常类型
来源：http://hz.cashguo.top/gtqhojfght.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtbmqcpgub.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gtazkbulsw.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtxjztnpwh.html

TS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtdsdaxjcz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtqmuydcmc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtzdakqmwz.html

Ruby: class MyError < StandardError; end
来源：http://hz.nwbrower.top/gtoxhrdjia.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtyretcyct.html

[H05] 捕获特定类型
来源：http://hz.xuanzx.com/gtsjzniijb.html

Py:   except ValueError as e:
来源：http://hz.ppjwa.cn/gtgubjnzhr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gtncyfetma.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtkocbjbnn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtyafnspdi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ybcxt.top/gtmdwxqicc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gthkgywsxx.html

Ruby: rescue ArgumentError => e
来源：http://hz.cucudq.cn/gtwijgwhau.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yonumen.top/gtmhqbdcza.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtzusmdtpb.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtbmzxvjsf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gtgbwozhfh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtjnvfhnoz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gttslpbper.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gtdfckftqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtbhqvkghf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258888.top/gtceqloylz.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtfuyenrdf.html

[H07] 断言
来源：http://hz.jinqigufen.top/gtwmxyjsiu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jianghu66.top/gtytawgoax.html

PHP:  assert($x > 0);
来源：http://hz.bjfxy.top/gttjzqywmc.html

JS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtztfkusva.html

TS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtzvfxrnfn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtmoipovga.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shuidangran.top/gtaoatuvmp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtoozyrqhl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hfpthk.cn/gtmzhdceos.html

[H08] 获取错误信息与堆栈
来源：http://hz.guannengcc.top/gtbwduadqh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daxiang520.top/gtrivmkcgy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtxvbipsyl.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gthrtanpqj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gthznivpqf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.quarkkingdee.top/gtlmlwcalc.html

Go:   err.Error()
来源：http://hz.snrcjt.cn/gtbtencqbd.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtsqokykkr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtypetagof.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtbtihyljr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gtzlxenvqz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sysykeji.top/gtxfalyagy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtcxtdiycy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtehuckuzj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtltbyacsr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cdnleiting.top/gtzsmsaajg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtodfuilky.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtiifanmxj.html

[H10] 资源自动释放
来源：http://hz.yongpay.top/gtmcfquegk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgfzy.top/gtktxoizoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hfpthk.cn/gtmzwcoldx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtedvylqem.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtxfcrriry.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtyveqvxqh.html

Go:   defer f.Close()
来源：http://hz.jlsjyb.cn/gtqpkdiggk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtagnsywcq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cqqwz.cn/gtizizmlib.html

================================================================================
来源：http://hz.sweek.top/gtgbquvflc.html

I. 正则表达式
来源：http://hz.aizwys.cn/gtpmipumyx.html

================================================================================
来源：http://hz.sysykeji.top/gtdawprudz.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtnwwaxxtn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtbophahsm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cashguo.top/gtfllqzwxy.html

JS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gthpmhcaxw.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtdjbqjkjr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yanxiufei.cn/gtyuejuatv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtlexkrrag.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gtlzdefztf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jyoumei.cn/gtvijijfny.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtqtildpyh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtjovkrqeb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtpebjsnbs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtlmamktyq.html

TS:   s.match(/\d+/g)
来源：http://hz.mhx1999.top/gtlmaeiupe.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gteehekjdz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtpuxhwbui.html

Ruby: s.scan(/\d+/)
来源：http://hz.hfpthk.cn/gtypzeacuo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtvovtwswi.html

[I03] 提取捕获分组
来源：http://hz.snrcjt.cn/gtrgmulhrw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtxbmvwcmm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtorfjyhur.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtobegwnju.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtmnbwevgq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.redwolf501.top/gtuqfpfhnm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtjaggyfhk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gtrzcytgno.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gtwfuwatft.html

[I04] 正则替换
来源：http://hz.jqgufenzy.top/gtxgxqogtz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnxiangtu.top/gtkbsasque.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtuuvllrrv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtqfjefwdc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtzlqezvud.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gotoacloud.top/gtmjvfkcmf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtfdjrlruf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtgblbxmbo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtmdizirem.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtdvjhtcym.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhongyouzk.top/gtdgoqflpg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtxbckjlmt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtivwlncne.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gthuzuplqc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtyzcxhdiw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtphymtiau.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtozehtilt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtfkfadigu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtwqwynwdk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gterxdqetx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtutivnvum.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtcizpahgo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtinwwjtmi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangdashe.top/gtfuhjisfk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtmgssaglq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtejoyryst.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtmfmrvbed.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtwvfkfktj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gthqyxqbbj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtokiqosyk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cheryme.top/gtzsubfogl.html

TS:   /error/gim
来源：http://hz.ywan-chungtsiang.top/gtspwmwoza.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtuwjrwiil.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuetiantiany.cn/gtzfkcuyrv.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtkublhsyg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhaomingkeji.xyz/gtllyekuiv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gtwcewqhsq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtxpulrxyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtuxkeksdn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtfaxyroza.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtfocupdbp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtkvvyfbph.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtnglpjpnm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dashuyun.cn/gtpfeytycz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtsntitpir.html

================================================================================
来源：http://hz.snrcjt.cn/gtgkqwojrb.html

J. 日期与时间
来源：http://hz.yvedp.cn/gthkpqcqsa.html

================================================================================
来源：http://hz.zdqjudy.top/gtbqvgjuzf.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gtxvptslwx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtzgzqgmoc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dianchejie.cn/gtulinqpzi.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtypihgaui.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtdorovorg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtyhylmnop.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gtblnqxeqd.html

Ruby: Time.now
来源：http://hz.xingfuxueyuan.xyz/gteasedkti.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtouzprbpm.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtwzzvueqy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtvvdathcw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gteaavojuv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtmkguqwam.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtlgegcjcx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtpblflhwr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtumldizzo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtgdecogrg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtemowxltc.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtrmzdghbi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtgicyetih.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtnfweludl.html

JS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtoswannxo.html

TS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtjgtlupbl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtixwkajrm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtargkbhom.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gthkgjuetj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.316326.xyz/gtswotmann.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtbvmgqkqp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtzxutdvar.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtxbwofujf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gtnwnkhwsr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtvkgayido.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtflxtuemq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.mhx1999.top/gtstkynghw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtffptsuvu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtldywzgnf.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhiwuduotai.top/gtpflthgxx.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gtlrwgafvm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jlsjyb.cn/gtkrkgvoks.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtwyvtzwqq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtjvcqvvnz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gturydomfe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gthqnoynzj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yueranfly.top/gtdrzapyia.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenjidiqi.icu/gtdauomnns.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtffiiathp.html


<!-- 参考信息 -->
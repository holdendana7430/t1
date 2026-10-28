代发 wailian999

Ruby: super
来源：http://hz.jyoumei.cn/gtilkvfjaj.html

C#:   base.Greet();
来源：http://hz.shuidangran.top/gtynmiysna.html

[G08] 静态方法与属性
来源：http://hz.tianlin.xyz/gtbnwkhkjs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.daria6918.cn/gtdrlfchyx.html

PHP:  public static function f() {}
来源：http://hz.shuidangran.top/gtgfuofjxu.html

JS:   static f() {}
来源：http://hz.hnqzz.top/gtfahoxayv.html

TS:   static f(): void {}
来源：http://hz.zdqjudy.top/gtictgsmlp.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gtbpthvmsu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.quarkkingdee.top/gtqubitlme.html

Ruby: def self.f; end
来源：http://hz.sweek.top/gthcottalh.html

C#:   public static void F() {}
来源：http://hz.c1oappe.top/gtqunzebnz.html

[G09] 接口 / 抽象类
来源：http://hz.gaohongyu789.top/gtnpricmrp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtarxbotih.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtwlxsqyml.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtralypsys.html

TS:   interface Shape { area(): number; }
来源：http://hz.tian-w.cn/gtmaiqdtdy.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gtzfekyian.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zdqjudy.top/gtawlqxhbe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.0kj1m.cn/gtrajtxmib.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtosdroyjx.html

[G10] 访问控制
来源：http://hz.sufxvd.cn/gtxflyfbhd.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtrpdinkbe.html

PHP:  public / protected / private
来源：http://hz.feifeiyinyue.top/gtigycjaqk.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtrlprjqzu.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtlmdatwkb.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtewzbmiol.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinqigufen.top/gtvcpceqde.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtwfyvkmyw.html

C#:   public / protected / private / internal
来源：http://hz.cdnleiting.top/gtmmviwxyd.html

[G11] getter / setter
来源：http://hz.yvedp.cn/gtecfaydlz.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtppfejzfc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gthmgsvfew.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtorgqvoqo.html

TS:   get name(): string { return this._name; }
来源：http://hz.gzhubu.top/gtfnervzjm.html

Java: public String getName() { return name; }
来源：http://hz.shuidangran.top/gtcfnocudf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtgppnqvyo.html

Ruby: attr_accessor :name
来源：http://hz.yangfankeji.com/gtbhhbrcis.html

C#:   public string Name { get; set; }
来源：http://hz.0kj1m.cn/gtomgvjzbz.html

[G12] 对象转字符串
来源：http://hz.sxryk.cn/gtaedxjyai.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtnuraqlha.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtoediijbi.html

JS:   toString() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtvohcfaiu.html

TS:   toString(): string { return this.name; }
来源：http://hz.ybcxt.top/gtjfkxeyfi.html

Java: @Override public String toString() { return name; }
来源：http://hz.dianchejie.cn/gtyaactmuh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gtvvgtwlsm.html

Ruby: def to_s; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtugmsnmti.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtdygyymem.html

[G13] 判断对象类型
来源：http://hz.guowangkeji.top/gtcwkftdfu.html

Py:   isinstance(u, User)
来源：http://hz.shuidangran.top/gtgzfnmdrv.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtkxzwijow.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtfaqynxls.html

TS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtiqkzvieo.html

Java: u instanceof User
来源：http://hz.sysykeji.top/gtgppzaeep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gzhubu.top/gtpdxlrqgh.html

Ruby: u.is_a?(User)
来源：http://hz.xingfuxueyuan.xyz/gtlmynxrng.html

C#:   u is User
来源：http://hz.smart0.xyz/gtyrjtjavt.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gterkllyzp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.wangdashe.top/gtjfvaxadg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ywan-chungtsiang.top/gtqbpitpdo.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yuxming.cn/gtfpzoyfmq.html

TS:   type User = { name: string; age: number };
来源：http://hz.shzxlz.cn/gtnwuqyrpq.html

Java: record User(String name, int age) {}
来源：http://hz.bjfxy.top/gtezrewfjh.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtvdyxpmbs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtfmidbbrj.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtnwmvgqvs.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtnobjnird.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yanxiufei.cn/gtwfhhqmts.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.jlsjyb.cn/gtwwkbszsy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtnhalhdri.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtjhueggsm.html

Java: enum Color { RED, GREEN }
来源：http://hz.cashguo.top/gtaemtglnt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pengpengdd.cyou/gtfrqhifvo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gthufroxnx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gtphpxjxjo.html

[G16] 对象转数组 / 字典
来源：http://hz.jiagoushi.top/gtajqwijhr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtdrhfwpak.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtxhgqbscb.html

JS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtrdmqazwt.html

TS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gtlaygljse.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtpqvwfpac.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtwzftyymx.html

Ruby: obj.instance_variables
来源：http://hz.daxiang520.top/gtjqkzulea.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gtebjhnmis.html

================================================================================
来源：http://hz.cashguo.top/gtuffinxdu.html

H. 异常与错误处理
来源：http://hz.316326.xyz/gtatmkafri.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrozjwwmp.html

[H01] try / catch 基础
来源：http://hz.jinghuilouyu.cn/gtbnriibrk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.c1oappe.top/gtgwqfzpja.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gthussjuwl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtravepfmu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.aizwys.cn/gtpuhhoaut.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gtqxcufenp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtruegacua.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtjtpmmrgt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtmxlkrgxy.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gttumuxpxc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xylfe.cn/gtccbrqdyx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtxstdrsqd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gtcjqujylo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtiijghivb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtvgeiwomf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtvydsrtur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtirsgkyhs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtnegyzell.html

[H03] 主动抛出异常
来源：http://hz.kuanghao11.cn/gtcajoxjtr.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtrdtoxpyg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtqwjbrtls.html

JS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtqfowgeiy.html

TS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtmodeaqqi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtukodjqzn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guannengcc.top/gtdpzdkkza.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtrdyujkqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtvbncdmze.html

[H04] 自定义异常类型
来源：http://hz.nanxinkj.top/gtthbnctce.html

Py:   class MyError(Exception): pass
来源：http://hz.cashguo.top/gtwpbpbvwo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cdnleiting.top/gtlbnplfst.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtmdnlqwgy.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtncnjwxuw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxinkj.top/gtvyuxlacn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gogol.net.cn/gtjbtaxgdf.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gtnvmyidiv.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gttjmfokao.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gtvzmgzwbb.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtriujabyg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhixingplan.top/gtmgbhmdvw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtqwykcygs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtbbhkqsog.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtreeggoiq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtwqhxvymx.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtkouvlahh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.snrcjt.cn/gtrazvzwtv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yvedp.cn/gtonupfdsj.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtjityxmwn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtheyoqcfy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtrgmngvzn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gterstoiwu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jinqigfzy.top/gtwsnohyoo.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangkeji.top/gtphsyjwje.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangtech.top/gtzpnirmoe.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258.top/gtkvkyjzsn.html

[H07] 断言
来源：http://hz.yueranfly.top/gtjeilbbfq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtnuptlxcl.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gttddztchl.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtjijymcmz.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtnmgmvfrr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtqytploxk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtlhyjckyh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtisewriny.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydjk.org.cn/gtjzppunqh.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtqmarntsg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ivvv.top/gtsifsvntd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtuhdcqprl.html

JS:   e.message;  e.stack
来源：http://hz.xuetiantiany.cn/gthrfnhfed.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtrjxcneon.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gthjxgnoxy.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtqvpiwqlo.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtgqayrvso.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yonumen.top/gtewsdgyco.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gttdvossnv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtcussremn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtuzkghddn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtgqfhqcgq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtbpwhcijp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtusyxnqsi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shzxlz.cn/gtgtzublbv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtjwutqfxi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtxwrghsao.html

[H10] 资源自动释放
来源：http://hz.c1oappe.top/gtndmgjzxt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuetiantiany.cn/gtihmocvyi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtvvpluyag.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtyuizvbqd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtquadttmb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zycfv.cn/gtgfjpjsgq.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtufnbjcip.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gtsmhzjxlz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtmvoawlyj.html

================================================================================
来源：http://hz.svipenyu.cn/gtjdjyamyn.html

I. 正则表达式
来源：http://hz.yongpay.top/gtqzyztytu.html

================================================================================
来源：http://hz.cashguo.top/gtapjxfjig.html

[I01] 判断是否匹配
来源：http://hz.aibaodan.cn/gtdmongitm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtefxmgrof.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigufen.top/gtobgbqsfk.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gttaletyuz.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtiwyaednx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.andypj.xyz/gtvatdoaqt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtrhmlwagq.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtcvdqvrvl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhoulong.xyz/gteeyniwfl.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gtmejnzdaa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yonumen.top/gtjanstbiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtivxobkxl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtvcujehdr.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gtlksgoldj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fzhhl.top/gtddmnkuvf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtmwlirzme.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtuyxksiab.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nwbrower.top/gttlmmhyvc.html

[I03] 提取捕获分组
来源：http://hz.quarkkingdee.top/gtnyehxkea.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtkzibilao.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtabsceupx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtyolznpna.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtulggoibf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtfrmbqozz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtrqlrjgjm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.havefunace.top/gthrtdyrds.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtskmpynbh.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gttnsyzyyk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ppjwa.cn/gtjfwyqrhq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtvnxsqxvy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cheryme.top/gtaoiuotjd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtwjiawecf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtmomojwbo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtmktegvrr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtryqxxejf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtlasckmjk.html

[I05] 按正则拆分
来源：http://hz.svipenyu.cn/gtgkwnlwla.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuxming.cn/gtmtusbcnz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.vqdsnc.cn/gtvzdyhakh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtmkmnsuza.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtpshzrtco.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtioufozcm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtsekkakzd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtdmvnqrne.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtrcwgshgv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sufxvd.cn/gtinawmzvd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtzreteaxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtkuefocmv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtpbdshlpt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtgahhgmct.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtzishyegj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gtrqyskifd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtyeaikwqw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtagwsfycm.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtjunnwtgn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.52xcode.cn/gtgaunwhlr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.smart0.xyz/gtvqqsafni.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtkoequddu.html

TS:   /error/gim
来源：http://hz.0kj1m.cn/gtmmtchvfq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guannengcc.top/gtgpxuiqio.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtphihbtrb.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtlboahjpe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gteyzjnoic.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtyfsgtoqx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtngkxolao.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258888.top/gtupvvnzgx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtxspoldmj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtcmlguvpf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xziqi.cn/gtdfkyhbvc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.snrcjt.cn/gtrjjznfyk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtiioabgqg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtglljsaal.html

================================================================================
来源：http://hz.haohaochexian.top/gtffyouwdi.html

J. 日期与时间
来源：http://hz.shanyushiyangkeji.top/gtolmiygsl.html

================================================================================
来源：http://hz.ivvv.top/gtpwumazhg.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtyvyqxasg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhengqikj.top/gtibkzipac.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtukpqyupm.html

JS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtzawvvbwn.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtljhxxpup.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.kuanghao11.cn/gtgcejsvds.html

Go:   time.Now()
来源：http://hz.nanxuanxn.top/gtykztzdxv.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtoigxlswe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenzaomai.com/gtymlriaad.html

[J02] 格式化输出
来源：http://hz.shanyushiyangkeji.top/gtlfijvfzr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtcmajeotl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtdbnttech.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hfpthk.cn/gtdxpvsfpt.html

TS:   d.toISOString()
来源：http://hz.cqqwz.cn/gtynogsevp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinqigfzy.top/gtnjnhmrfb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtrfiyvawq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtqetgnxvu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtsiqfwyda.html

[J03] 字符串解析为日期
来源：http://hz.9152youxi.cn/gtzivbzsow.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtmmszkjfr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhongyouzk.top/gtucsfphpz.html

JS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtzoldapsp.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtqvxeclay.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtxixuarxn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gtbjaxxcvr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtlryfwixr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangtech.top/gtmhhjsltk.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtliqqpftf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtcwydzluz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhixingplan.top/gthewpnjqg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydjk.org.cn/gtnmcarpfn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtnmbadzmq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.fzhhl.top/gtfegsoafv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yangfankeji.com/gtcetrwqhs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtbsaqjzbx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhongyouzk.top/gtkijsrgef.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtzyehkiyv.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gttyztflmv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zycfv.cn/gtuleapibz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gthzsydrjq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtevcygkwq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gttuixgspo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtztjdmknq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydjk.org.cn/gtsjexwdhb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yueranfly.top/gtogtomwws.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtmqeszzfn.html


<!-- 参考信息 -->
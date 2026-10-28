代发 wailian999

PHP:  public static function f() {}
来源：http://hz.shangyingyoupin.top/gtwqqfrwqw.html

JS:   static f() {}
来源：http://hz.shzxlz.cn/gtcdzflphr.html

TS:   static f(): void {}
来源：http://hz.nanxinkj.top/gtffdriemj.html

Java: static void f() {}
来源：http://hz.redwolf501.top/gtwcwhrdii.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.smart0.xyz/gtvrqjrhwj.html

Ruby: def self.f; end
来源：http://hz.shzxlz.cn/gtsiebveiu.html

C#:   public static void F() {}
来源：http://hz.sysykeji.top/gtmtifruiv.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtaqnnhcqn.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.tanke756.top/gthwotbfov.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtrdkyobij.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gotoacloud.top/gtyzhdnzcu.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtlxghfwuc.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtxfhclpps.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.52xcode.cn/gtrslgqxrv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhongyouzk.top/gtunexyuyt.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhongyouzk.top/gtlodkwtgy.html

[G10] 访问控制
来源：http://hz.guowangkeji.top/gtjzlcahqm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtcwwuycql.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtjwwlslua.html

JS:   #private 字段；其余公开
来源：http://hz.dashuyun.cn/gtwbmotzbf.html

TS:   public / protected / private
来源：http://hz.jinqigufen.top/gtdghrwpzy.html

Java: public / protected / private / 默认包级
来源：http://hz.fzhhl.top/gtvqbpiwiq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtdvyhjukn.html

Ruby: public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtlqrgwrhb.html

C#:   public / protected / private / internal
来源：http://hz.svipenyu.cn/gtmfdvhflv.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtomtxnuby.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtsvnwqcno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtpwwajaon.html

JS:   get name() { return this._name; }
来源：http://hz.jinqigufen.top/gtrhpdeeuk.html

TS:   get name(): string { return this._name; }
来源：http://hz.sweek.top/gtvqpcqrej.html

Java: public String getName() { return name; }
来源：http://hz.zycfv.cn/gtltddlfaa.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.nanxinkj.top/gtirsjqzjl.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtqjsldnzk.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gthtqgivhq.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gthgmhqwzq.html

Py:   def __str__(self): return self.name
来源：http://hz.cqqwz.cn/gtogsjwqda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtvmzlotvj.html

JS:   toString() { return this.name; }
来源：http://hz.jianghu66.top/gtdiuyktyw.html

TS:   toString(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtscmdsjmt.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtefquffac.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtjdrfbzpk.html

Ruby: def to_s; @name; end
来源：http://hz.9152youxi.cn/gtdeqeakvt.html

C#:   public override string ToString() => Name;
来源：http://hz.kuanghao11.cn/gtweostvty.html

[G13] 判断对象类型
来源：http://hz.gotoacloud.top/gtjplztizu.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtbyrzoqmo.html

PHP:  $u instanceof User
来源：http://hz.ydzc1.top/gttldgiwrp.html

JS:   u instanceof User
来源：http://hz.haohaochexian.top/gtjthegzze.html

TS:   u instanceof User
来源：http://hz.wangshuangyany.cn/gtawdeohey.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtkehrpcbv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.daxiang520.top/gtzeojzkyb.html

Ruby: u.is_a?(User)
来源：http://hz.daria6918.cn/gtrzyirdez.html

C#:   u is User
来源：http://hz.chenlongwang.top/gtkxeakjwk.html

[G14] 数据类 / record
来源：http://hz.shanyushiyangtech.top/gtpxxalrrf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtwqxoniah.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gtwfhvijtt.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtilprifhy.html

TS:   type User = { name: string; age: number };
来源：http://hz.ydzc1.top/gttdfsgxhr.html

Java: record User(String name, int age) {}
来源：http://hz.pycfn.com/gtqrudsqbf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhoulong.xyz/gtyjymgplw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yuanzhike.top/gtczqnwswd.html

C#:   record User(string Name, int Age);
来源：http://hz.yj20258.top/gtvsgjhozv.html

[G15] 枚举
来源：http://hz.zdqjudy.top/gtqynnjqed.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtxgimagew.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.gaohongyu789.top/gtfvzdtutd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shzxlz.cn/gtrdrhsimi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yonumen.top/gtyydzlpgj.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gthhmhzokz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dianchejie.cn/gtdajvujpb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.svipenyu.cn/gtdskzgrpl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtuetdbogs.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtdkwubins.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinyuanbaomall.cn/gttnyzyvci.html

PHP:  get_object_vars($obj);
来源：http://hz.52xcode.cn/gtxdgidcbl.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtzgcagtss.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtgtrbhwkc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.havefunace.top/gtaejfekpb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cdnleiting.top/gtoeilsucz.html

Ruby: obj.instance_variables
来源：http://hz.0kj1m.cn/gtjazujeen.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.smart0.xyz/gtalmbbpkt.html

================================================================================
来源：http://hz.ivvv.top/gtvrpgrpby.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtatuuxxmp.html

================================================================================
来源：http://hz.zycfv.cn/gtddgudnfc.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gtrgcuuwzw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtxtklucod.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuanzx.com/gtqkoaclze.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangshuangyany.cn/gtxtrzcrco.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtowaqzryr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ybcxt.top/gtyrharzrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj20258888.top/gtcxzdncrt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtkvbmiaes.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtwcjajabf.html

[H02] finally / ensure 收尾
来源：http://hz.hfpthk.cn/gtwmafljmv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zdqjudy.top/gtznebyuft.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtdzredppw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtpntxywlv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtwccqtwkm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtnezgxlpu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenjidiqi.icu/gtvneqdyaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cqqwz.cn/gtvvfuyysd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sxryk.cn/gtqpwuefza.html

[H03] 主动抛出异常
来源：http://hz.shangyingyoupin.top/gtvecbiwin.html

Py:   raise ValueError("错误信息")
来源：http://hz.xziqi.cn/gtfnlmkfgf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtxvewzhwr.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtwiocbses.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtgxzujetf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gttdluroft.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtxjkyyrkv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtbmbtmfpk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtdkhbwyyj.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtolietato.html

Py:   class MyError(Exception): pass
来源：http://hz.hfpthk.cn/gtdcyxkjeq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnxiangtu.top/gtvwmycawu.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gthrptanaw.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtawncdfei.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtlvcqlkxo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yanxiufei.cn/gtzoujdejz.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtimecfqrm.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtouzxobja.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtqspbypfl.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtlycwzoww.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cdnleiting.top/gtpagxzbji.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtmizsdhop.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtrvqlayst.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtntqjejby.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtfhknryww.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtdpxevini.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gogol.net.cn/gtgnhilexx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.havefunace.top/gtyvspmgpw.html

Py:   value = d.get("k") or default
来源：http://hz.yonumen.top/gtujekupsc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtojdnliat.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtxmutmaqt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gtmlvzcydr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tian-w.cn/gtrxowixzh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yuxming.cn/gtmvyxbdqt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.c1oappe.top/gtncvmztjr.html

C#:   obj?.A?.B ?? default
来源：http://hz.pycfn.com/gtcjouekdh.html

[H07] 断言
来源：http://hz.haohaochexian.top/gtofwzpwgc.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hongshengwenyu.top/gtxqsakobv.html

PHP:  assert($x > 0);
来源：http://hz.ehwqpu.com/gtyyappwzw.html

JS:   console.assert(x > 0);
来源：http://hz.andypj.xyz/gtglggujxo.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtqwqjuivr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtuqtqxluw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ybcxt.top/gtybpxmjvt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtjcxsvude.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtcyhzhtkf.html

[H08] 获取错误信息与堆栈
来源：http://hz.sufxvd.cn/gtdpaglnpd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtktkukadh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtanhrlmgv.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtqexqmeml.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtbknjjyus.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gteegrkiey.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtjyoswahk.html

Ruby: e.message;  e.backtrace
来源：http://hz.svipenyu.cn/gtulvjpuog.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sufxvd.cn/gturjibmtg.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gtwulspbtw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.sufxvd.cn/gtqocejjme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gttypnuldv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtcpitkzub.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yonumen.top/gtnvaqqsnq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhijiandao.cn/gtafgazjpw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtehvtktwf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gthsjbiyzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtzempyate.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtidqncuwc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gthihbujft.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daria6918.cn/gtmbygdlxh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hfpthk.cn/gtceqlavwj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gteghnlnxz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yonumen.top/gthmeuwces.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtwrujzyqs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gtppniibgw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtqozplicg.html

================================================================================
来源：http://hz.guannengcc.top/gtwvsssxvj.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gteujneqhr.html

================================================================================
来源：http://hz.zhongyouzk.top/gthijlufmn.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtyxlpbjpz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtuhrqufvx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ehwqpu.com/gtydkimlal.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtrqxptryo.html

TS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtlazxrota.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtgonlfqqo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dianchejie.cn/gtqqidatoq.html

Ruby: s.match?(/\d+/)
来源：http://hz.52xcode.cn/gttjuuvzrp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtzenohldt.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtlswquaat.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gtibzacpxm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtxzallhtk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yanxiufei.cn/gtutdurnag.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtcllyxzsd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtstekujxx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gttlcqpfis.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtgksqoanm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtojflnmgu.html

[I03] 提取捕获分组
来源：http://hz.havefunace.top/gtzpcabxeo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.andypj.xyz/gtasymunuv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtphhbsfhc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtwyrhjumc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtriwdcgzd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtueaucjlz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtkvipqsag.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fzhhl.top/gtdbcyraxm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gtgsbfveml.html

[I04] 正则替换
来源：http://hz.smart0.xyz/gtwhupuwnl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtpxjuglkk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.316326.xyz/gtmkdarazp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtlrbrriyz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtfpwvvhbn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gaohongyu789.top/gtqxewqyye.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangkeji.top/gterysushb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtpylszjbc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shuidangran.top/gtnhltiwki.html

[I05] 按正则拆分
来源：http://hz.svipenyu.cn/gtkithvdgp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtekwpnvya.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtbescvfvh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtrgcqezmn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtxecoambf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gtfnrbloet.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtnsrezbak.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gttzvmkxmp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtkfeawidw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daxiang520.top/gtuxbivzwe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtjgpqvzdg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtjvrvieab.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtltbqalbt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtazcgcbdc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shzxlz.cn/gtcwtzmapt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.redwolf501.top/gtqddnxksz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gttakypaev.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtswoijbtq.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gterlndwsy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtqljwhlsz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtiinijkcb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.haohaochexian.top/gteetjiyhb.html

TS:   /error/gim
来源：http://hz.birdmap.top/gtvrfhzhce.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gtutenjwaz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtroytynhy.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtxtnxstkx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gtfmgiwgxk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtwfykirvl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gtxaxydmeq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtiegglvjf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtydjurxby.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtxahbqnzl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtpuooeywz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtmoaxayhf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgufenzy.top/gtmnozppza.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtgenhnxta.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcdlrfraz.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtraettmdh.html

================================================================================
来源：http://hz.yj202588.top/gtljorisjf.html

[J01] 获取当前时间
来源：http://hz.yj20258888.top/gtsccdocfm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtiwggohts.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtgehucxni.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtggpypwjg.html

TS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtnkygasnm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gtgezayrue.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gtmkzozrkp.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtsmcjmhjm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtrircjwoh.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtudalnwnc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hywenlv.cn/gtjkswhesq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtpzjemnqy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhaomingkeji.xyz/gtebubozhf.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gttthabdct.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtulywiluw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtljzymhrn.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtmjecibqx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cdnleiting.top/gtmrfhofmr.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtxcipaqkb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gteiazrsmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtgxynabra.html

JS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtkidoacok.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtagalaucy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtsounpjzx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtsntxmmoe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtorffpxpi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dashuyun.cn/gtjkjhkdqa.html

[J04] 时间戳与日期互转
来源：http://hz.sufxvd.cn/gtrsmhlcdj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtzklfziwb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cqqwz.cn/gtdjunnwss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtnanmharz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtjsizuvcr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gtistwowgv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtngacxdlv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenlongwang.top/gtbxijspop.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.mhx1999.top/gtapinnngf.html

[J05] 时间加减（加 7 天）
来源：http://hz.cashguo.top/gtwrrewtzp.html

Py:   now + timedelta(days=7)
来源：http://hz.xuanzx.com/gtfqjxogcl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gttgnkmabr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtosqlolme.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtbmhbylbe.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtuppcopoj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gtubwxdiif.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tian-w.cn/gtdtujfkbz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtuuxdyjpg.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtbltjqcup.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtcladrmbo.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtgsiodsrz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtwnpsfhmz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtlkxfdams.html


<!-- 参考信息 -->
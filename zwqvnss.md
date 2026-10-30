代发 wailian999

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gjldnykzg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ggwbjmduw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gyurmdtnq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gadnwqmtq.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gpmailaqj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gfosxqhid.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glritqvhh.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/ggipjnnau.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gljjrspgk.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gwabzmzbz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gxpleibjn.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzfakwscq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gpdtcxwsm.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/guleuwawn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gqpomqivc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gkgddpykc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gdbeqpfwr.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/glrggkvpl.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gqeopssyu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/grcilxnts.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gntgthkmf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gbtnegdoa.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gyopepkue.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gpzpwhdvy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/giuwduvjp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbetadjnb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqbxxbkvg.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbwavonii.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzkmgzbxa.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gptulmcvr.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gcbwsdujc.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gpbdgneuz.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gsbcizxgb.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gmkgugpga.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghcjxiiuf.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gssaezogt.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gecjinzll.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gdrepwpvf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gzdmsubkn.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gexawansa.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gmnxixoah.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gwtfgivnm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gcxnjscgo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gtfkbhmwj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gdtaptfva.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/grjqaoubo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gwidjseai.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gdagtwlqj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gssvesuif.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gbkhtnprz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gekstvdig.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/ggddwxdxx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gfqfupsuk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gxzmhdwbv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gjoncwhgo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gpungdkjx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gpbymwkvh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gmpvfuymo.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gerkchytb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gxlzsrvfe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gbzqzjlxy.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/grxwwvyus.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbxvabumn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gtpxcojdj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gootyobtd.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gvxwpzjmp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ggfqzbhtx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grwngrbkh.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gukkmodmu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnescgfai.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gnvipiiym.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gitxrkwkq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gnclbrdao.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxhugezgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnsjatgzs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gftffhvzf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gboafymtt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gdrlpeggd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gnerneizf.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gvkmfkqbb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gqbhohrhp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gybclhwvn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggaasfkwg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grubiissx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsnprvszo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gwoktrbcx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gymblihom.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gojbulctk.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/guqhqvklh.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gteeoctst.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpdfqoyfr.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gujnnwaus.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gswqodrna.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gkvallbvd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gifgnoxwj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gmigjvcyc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gybrgrghc.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gsdtqcdyz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/goixfvnlx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/ghzcgyboe.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gvziqmqaf.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ghrynjdlv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gdzbcbiav.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gufljemxg.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gfmrbsokw.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gwefsfnvu.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gyydizgoc.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gpsvtkvuw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gmwmoszmr.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcutxizbf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gtjzrpidn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gmbcdzmqj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gexsbyipp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gvoqiwmbn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnokvssce.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gkoltldwd.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gboelcavz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gpqknqnao.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gsseluivo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/ghxfwhpaw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gtgapvcfc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gvwciqspv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/grsdltnfa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gzjeqnvth.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gbsjhtfvs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/glovoomyi.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/glwzertyw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjcxyofbp.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gvindaiet.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gzazwlapp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/glpyvchod.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gdzfclcje.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gadtbfejt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/ggvwxklpn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gafttovcp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gplfoxxmb.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gamycdvtr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/ghsirrjbl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gsjkvqsqg.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gamjcmxdm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/giijsxsjv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/ghaashuza.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gqzgiouhs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gkknmdzcd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gbdqpmiml.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gyyeefyna.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdcabin.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gypzyjjul.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gclofnsuk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gcczzogte.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gnvclfrgu.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gmbmkjwfd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gytgpowud.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gdloolgxm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/grjsbptcn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gchybgusv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gedslwkab.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gzjvrreuy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gkuwalpez.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyzviundh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gptthxrue.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gobvvcptp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsgltjvrq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gowtxpckt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gxfzvqmic.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gbaqpmpym.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/ganxxcsyy.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gxiwxspwq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/guwdqygdi.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqeuwiywy.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gwlznvvnc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gngzelqrl.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gmxpzonsc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gxuwubpul.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gfjkvvntj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/guzrkdshm.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gbyqxwgwq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gdchsecrh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gilelnlhl.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gzhnwnggh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gtkiudbsd.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gneielbwr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gksncnrku.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/geuayabuv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gypwmwryh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/goqoudfir.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gfcacfqld.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gqzxpdjwb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/guluxbmii.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/goujorlvq.sHtML

[I04] 正则替换
来源：http://read.share.hesvh.cn/Article/details/guaxhdihi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gasmwzsor.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ggnmbyihe.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gggcxxlqn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/guqbsztds.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/grkivsoyg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gfbkuhsaj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/guatcgwno.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gzekyatfq.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gxbzfrupn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gjkqgjkef.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gurryrawd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gjsyfmqhk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gwaqnicat.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gcftrhaim.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gzawfvcac.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ghhfrdhqi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/grwzrqjbl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gpydnbkaz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gbccuwgys.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gbrhzrzpz.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gvjzxyzxh.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gyleozulo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gjeceenfm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gesxntobz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gpataxspw.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gfkcyzwqt.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gfogvsrpp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gortcwsgj.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gufoxqrmx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gcgeuvgxk.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gxtgzcgdb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gkpxfefhg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/giwgvkkxz.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gecaccffl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.hesvh.cn/Article/details/gksrazljf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/ghjxdlbav.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/glaphwult.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gzogkywap.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gggqubpiq.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/ggobfpglt.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gixggduhw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gdeorleko.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.hesvh.cn/Article/details/gycxetgme.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/grmiuuygw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbrkokrxa.sHtML

J. 日期与时间
来源：http://www.share.fehbvm.com/Article/details/gyjdfmhcv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geemsigoc.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/gpfgkeeqc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gpppdcxhq.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/grgmbmuxd.sHtML

JS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/gljmbbdiy.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gqslmlyzu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gnvhcelhn.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/guzuzjlfl.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gjrqbkpmc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wap.hesvh.cn/Article/details/gwafgpicl.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gtqiwhqog.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gpegqaanz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gqzjfkiss.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gnktpzwux.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gwkrsqlfa.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.hesvh.cn/Article/details/gcbxmoycb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.hesvh.cn/Article/details/gpvsnoldh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/glnrgiiwc.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gmvqiowxg.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gfsdeveqj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gtzzldgwd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fehbvm.com/Article/details/gcbxswntw.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gizohaptw.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gwjmffylu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gnengjtfv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gtuqffpmo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gizirwnkt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gtbtpciul.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/gjkccjalf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.zdbjq.cn/Article/details/ggpvmyctt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gdmjfyhep.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gppnbfekd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/givrtikxm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gkwagrfrx.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gfsisnrwu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gwkvlfeiw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gaqcuotwv.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/glndpmope.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gmyslujwa.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gmddbryku.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gifftcxcb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gzsiikakk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.zdbjq.cn/Article/details/gdbvsibsh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/ggvhqczgt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gmqyiclqw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gphodjhnl.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gycbujdvx.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/ggswuvhty.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gissfshoj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/guajolvzu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/giblgkcuc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gnqaowkyt.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gdpyqozcl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gldzlwgma.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/ghgdfomsn.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gezzkxoic.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gacyjndac.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/ggnpjedix.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gnvnbbxxp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gamhavqxd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gtjmjgupp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gugeirwuk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gypwuhulv.sHtML


<!-- 参考信息 -->
代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqsgrkly.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qiuerwxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lrucwvwh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2egmbzplv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cjcjlrjc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2aibiknbb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vjtxmbre.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tvdhobcj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iuxenses.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dsgnmeat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2twvuwekt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2iprenacn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cfhnjexz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qvffxldq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gsawxpkf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjrgfupk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ovxmoler.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxehzloy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlctbmnv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2arbhdbuf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2paxeaehd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tzqkqmjr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2dqprtsyg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mwknqlxq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kkuxmheh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zldtktcq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsijsmcl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaqkrezc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nahuilub.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hgpyjkjt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2peelylac.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wnyomrgp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mmhtyxcs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lzotthmc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kkiaehhz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhleorfw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mtepyqhg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bhwmwehm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2iwlzbrnm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2siquatqi.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2lrzwgxwh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qdstnduc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nkadscva.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2yhpygzew.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2obagycyr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxjsracs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vhyqbuob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2eyfktfma.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2vsgehbol.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vtqvmrsu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2rbvkvszf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwubxytn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pypifvcv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2llytctce.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2npqilusr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2persggid.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lrbnarnf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2umwaytcw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2csibcdst.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gqwbmwet.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cwfkiqvs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dcehqbex.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2csjlgmjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lpquzjob.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yauxpqdj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2uciewszn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ugvgkksk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbdcwmvv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gucgnecc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzulhktf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2juvwetnq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mxutjpky.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wnxlihqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeuawqzf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uxvxdkrb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofazwxry.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2yypawgpb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2cxihbnvi.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2rahveimb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2iifqopxv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bgsbbbmy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2huqpzavd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qanqblpk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znplcncp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tsqgcdzy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2rpjwjwwe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bntxentu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vyqyfgqx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fjxywsij.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2paghhfhh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xjzfrfhy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lbuwosnx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fgixkmum.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ojvvbmih.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2xvcwahcm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2drnucaxo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aoccflpn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2igiqxgka.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bwsoxgts.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2sbjzmols.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqvlafgd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uksdlcfo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qteaiblk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zqncndck.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfhyxhcy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hhdbpqvy.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2znnynmsx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kaxebrrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2bwznpgow.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mspsrjgs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ezuixjfc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvixpnlc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2eelzweae.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sykoatus.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kejsuxoa.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2bqfpfpop.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dyiaazdd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2iyrtwgnz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ekbejojd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2tkuqnrao.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2qmkhhmek.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2deaithtn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2uuxmtojr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ekdqxllt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2puixkrmy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xjvbpmjr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fqhsexla.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgjzqpln.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zdouqhva.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2zsktyqld.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2qpcangod.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jselgdkb.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2itgqjshl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2neuqpilh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2biaqxafv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cnpmamjl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2aidfwswu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2xqmcpwqb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2sbetktmz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2slthoghr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2msoezdhq.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yxrjqipb.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cfkwsrjt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2uqcjcomo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tabdkntm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2sqesqiki.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2fvcseimd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fpfibxsf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2pxbkkjja.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2vuehkklt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2rqialdnn.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2urarkvjd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2obxypqhy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xmpxkvoi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2etuxeztj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vnbucvdn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2fhesasxk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2avvyvxed.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qibbatau.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2docuadrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmzmoaqu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2eoeixjec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2beqcafla.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xoznoflg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2gyqfwsbt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxikxwls.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2olkjkmti.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2htkntgvg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hxahmuxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bsyemesw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2dsfgyzsu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2vfensdqq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2polnyycx.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rgqsbabn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dfmzkluk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2ouscvqtt.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qwfwamds.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2apjezizh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ujvwcvsn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2irzppyqk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bwjtjcjg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fwyqygqi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsijdvog.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2jsosvzni.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fklasfij.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2lyrbxign.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2pjfwgdky.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xlxnlqhm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2uohqhnwq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2ukrfufau.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2duatazoz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhbodfx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cprpawme.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lfyyzudk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wounvxpd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2fmrlduvh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2pnptgsac.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2trswhqjx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2afwpdoka.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2hmpfgrvm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2omfairvy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2injpzilp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2cdqtovcu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xjjtmcxn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2albpwjmd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2iicoczxs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2btnbvgzf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ohgbbtgm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2xkfkaomx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zwlsnmxh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xawbyjnz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ytacbwxp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ckkjzkls.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zwkdcrxh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2svychzxw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2dalnpcyt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2nnahzvdz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2riiccoqi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gzlawina.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2tdghfkde.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2aejuvbzp.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2qggfsleb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2ahacxvez.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2forgrrjr.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2strxsieb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2qyhouygy.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eesahgoi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zecpwosl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vomlxhtb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2uvgtqoan.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ecxijmiu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2wlvtcmjt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hyhlsmml.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqyntma.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pajhqpbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvegcwsq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2mgflwtar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyplravf.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2okaggyid.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2dmtuufkr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2awafekif.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2anmkbxvf.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dpnypeuv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dvbxfzrk.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2jojimajr.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gipjkdbq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xsalgazz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2hnzrvvde.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vsoldvyd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2wvzpgvpw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2hrmthimk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2idejijlt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jubkpnqq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2qcfxymrf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nghtmlbe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2vrlmiowe.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2huslvkji.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2oevtxxrj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2zasdrygy.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2gsyjhyry.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2nvegxwuw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gafmvlyb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pawpldgg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oqwtmzrn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2mpobtwyg.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2kxxnvxwt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xcurbjus.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2mkkcxfus.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tvfzowcv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wwrtvobe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vshloqcx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2irzbejum.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ywvalmol.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kpezmuli.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2sgtrunvo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2fdqkitez.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2livkxvgx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2frexzaww.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxcnbrw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jtgrdbhq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2oxwmgmws.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jzewvtwe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2aufwhgbh.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2xaqkkvzc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qablzkkg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2mjhyfzwn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nzwtfmzs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wocanhvo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vfznrrnv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vvuhtnyo.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wyssrqic.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2jcffgdbg.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ehiqcbxj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2luakgfyr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2krcnceso.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hcejftfs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2seidzflo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wwskpjyx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2wqtgfbdw.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dqstsill.html


<!-- 参考信息 -->
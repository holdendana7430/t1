代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3czydagrt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wogkdguc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tzafkgus.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pprmhtki.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3iutjqwwj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3eecmvgve.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xrkgiiad.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jbhtckkv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ybcnuitf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmeucc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ctrguirx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jigmhtnc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tzopclzx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cnvyabca.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3fmxpixni.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkdfsyre.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ansnrprt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zulstvfk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tfsntpwy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3iqhzjgij.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3eumtafkg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysemuwmv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3shnugweu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tdadztis.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxqsphln.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xkojkhvi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzawfifh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vnqcawlf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mzczyxan.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkyvnfxy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wngpmhqy.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3azighsyk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3piummhys.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bubymsfh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qszconrm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iplyvenz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3joodufzy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mkcsgxci.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hsyodplg.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3pprrjudr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qbjbyjcc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vwdukxbx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3nqxkpznv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vzayiqom.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rfylqxjv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayyezksc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mabmkayx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uvtkyweb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bxlacfhb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fctvcqpg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivqrgcsl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jiqvafhh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xfpbsyjn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nuagdlev.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qpfkoelm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uduwslwd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3svueoekv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gurykdnh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hjdlzaas.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3wysupikv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3gyufipah.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pwpzhkhz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lodfhjjf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3enctmswz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3kjysmejj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3djkiceuk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dyokpyyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orldpdsf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jqxnbsxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqcomsoi.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yqyvavoz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3etatylpv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ohyybklv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3avhijqtk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tatqqhwd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3atmqpuwz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3rfypqbyo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrdcvdfz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tcmfywdl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qkplygfn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ffyggysf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbwuuknf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rxlcrmej.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rfdwiohb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3muybbxsx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lounpfqv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3elmnridn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jgbneyhl.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vmauycjr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3hwkvlygi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cbpjvahu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rtfselct.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nwbnvvxj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mwvaqxkp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ryirybtg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3msfizdgz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pecqqrla.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mchtxxyq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3unqsfggs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nuevbtah.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbjrcabj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3opotmwba.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dhvhkqng.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3pmczgwst.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yapgnqqw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3lvwvqyso.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3bwxafrgo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dddaisif.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3iijxwiii.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rrbrxgej.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdttfmce.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlnggtvs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3aerocwna.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3yfhilbyl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3kvphzjrw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lvokgwdf.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3etstyali.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3yvfxdjzw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kairaeud.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qxyuceto.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3mjdzhqiq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3balxqeyk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3embbfzfn.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mzjdvjpa.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3chffbvdh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3nesnixfx.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nehflqjn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xakjefhr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3efjrrgoq.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nuvtjnpt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3uoqgsbuo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uoaxzsqi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ukczkvks.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kjpmxhuc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3rfibjvtx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3mqmrwhel.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3hetpjtih.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3fhaaesrb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ancrgukk.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bcvawpzf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3eoevplsj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3mbszipwp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3jvcuqtya.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wbqjqstc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3usposunp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uynzizcb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3zckhkptd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ybkoklou.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jzhpnvnt.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3xpdjgvxg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3uvtcbwcp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3bqzfamhs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3xhyzfxhr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zwckwgzd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3bnaexoxp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3louvnkyo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3uautvlqq.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vzofpgic.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3mquoncpq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hyyffxtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ligjkfkw.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3xinuloxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmstowxi.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3snqlrgsg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oevuhfjz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mylzwovy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3bkguezum.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mlrggkvk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qodgcvrv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zweghzsw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3camgivmm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xckxxmqn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ifbkzbyu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwojlimn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ypitxdtm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qrzeksay.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3lizywybj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3ixgozzfi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbxznbsb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qnttjwhd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oveqzndl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3bwcgyuew.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3rcsxqfms.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3yypqxnjl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rbaphqwm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3dshqapkx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3rqjpyhsd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3symtypse.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3drkkigdg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3snbynnqu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3dzncdbze.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3hwabfguf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3nnvlfjia.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yfnmmswu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iusbgict.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nfntyjgf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3xdganqtw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3avzjkuue.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rgodwwno.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dbhzrruj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3nsynxiex.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eswyuzaj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fsfrjjlh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwbhvgv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3axtdnulc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3uafmjufj.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3jyuwhgvk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3uqegkdbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3aufwyelr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3yowqdpil.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3kihmoxrq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fjctglrd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ahcktrgb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3bwodyzgl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3dpxbikgq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3pjsoejmw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3fdptubzx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3oltdhybh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ppryargw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3autfnvkc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3cgwrugrc.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ykwqvrkt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3obsjfdae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3mrbisacx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3imshgkga.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3rxlhvana.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vrcmdbix.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3awcohkgr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3knjplsxx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3zqayayiu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3holejwaq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yrwhrako.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3vyqanpgt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3jucbpvmp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jdjnzqzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lavzwlfh.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3prxbsoiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuteeaxq.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hyuffthv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3gbhshcgi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3pfzqxcom.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wctayrig.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3kphsvqpc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3vneatlxn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ejvqzcft.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xbewwwuy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3breobbks.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3tjdvrujp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3wmruzfho.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3msfgdzno.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3lzvnyvbr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ueejkyit.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3xpulqmgq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3qpezelce.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3fuaebdrh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3mcrcxotb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3veapmxpt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3dgfxadtg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3kyycqcvz.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3qivfnqgn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wkpnxxhl.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kxmscnro.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xeagdnok.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bmartixx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3jvosysem.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3vtkcxmzg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3mmrikdzb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lxirhzru.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3ceuohuem.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jlnsvopa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lrsbromx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3yuqdfyyt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3oqbnfxoh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3edefktjo.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3wsdyjtyf.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3efiwgcth.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3iaxvkeam.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3wcukbfdk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3budnvoin.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ojtohbzh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qmirfbjw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ingcvfeq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3fomnopvd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3uastjyym.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3jduwmpau.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3elustiyd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3aksijlqt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xujtxwxx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ewwrmarz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xlsunlbs.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3fijremjb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3lfnjqklr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ilmpnawe.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3gedoqwha.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3furktqxz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3saeqmfje.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3otfutfmc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3rbwxqsxl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dpqfnmzz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3mfrsmjmh.html


<!-- 参考信息 -->
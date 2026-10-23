代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3slbdumps.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kkgwbcxt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zzvrmqcr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmdyztxa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cgzcexoi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fqbnopvv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dxkbdugm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dumrmbvq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jixyyavr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xwpmmitx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vdczfjhp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qnrfganc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rcjpjbjo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3agmgemma.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dabbmbjz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciatcyyk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3junxwkuo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oppylkfd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uacfxcvt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wnxesrvn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3djcdlbst.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3lwmxbmux.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3njqrjqno.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lszwruch.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3giwpesor.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kafnplxz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lqderlnq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mcxyuzvf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tjzfqmth.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhosklee.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ervnghnd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mypxcydw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3eqmncmcf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mpkwyvet.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rvmdbwia.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gatvsbmi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3boobnlxp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3beukkewa.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdmgbvy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3gzmjsmsp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tstjbdkw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bcppisvb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3reuiteky.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pnmdkbad.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rvzanqgb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3vmdqmadc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sztiwktk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rsvmquky.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dkhispvd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rlbzlteg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wsirwauf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wthdyrtx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3lookfnwt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kupembvx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yklrmsbc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hnfnlxbi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3iwfogreh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uuwqcwmi.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3slsloutr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xdhnyloz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sopcnthu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rbauavjs.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxadgekc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hurblpaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mhofxwuu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kksrramu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3btokxexb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucgengrw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ljubtmbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byhwfqpq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3aryhwucv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ugilpxbu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvfqkibi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3rxsgzsel.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ygwzymne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nzhkefqe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nkcrlwwg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gdoagmep.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3hubqnwcx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3jfiupfar.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nmadtyxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zhruadrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oucmhzce.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyemtcrb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsvfulgy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wcyqppsc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tnlogwot.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gjrjcrdr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gwsdkwhs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wieulibx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3brarjmtf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ysmrrvid.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3szphmlso.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cnqbzoih.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3gsrrekcp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vakcvevr.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cmsdlvjl.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xrpqdvrw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3utqueucu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymzqdznp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nobevrfg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwsjsavg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcbsnysx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3crxaaycu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3znsrnpgz.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3dtbsyzgc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3udsienzv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kaywuwcc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3unflzrgv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bokbjdui.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dspakbga.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3buibmkrj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3cyjovhar.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3kzqkjssc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbiphlfy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3cpboptmd.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3flesmeki.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vjjsetrw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3uhkhoqvn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yfhledzr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkhbveg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hakfzdgn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3vruvfcng.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3iqlhndkw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3dszezduv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3yujooynq.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nbniotib.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3niydfcer.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hbezpmsu.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3gdykuimq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3vfwaneon.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3owexidgt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gnhvczis.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ncfnmndm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3ikcxquui.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bjqsepns.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3rdkvbdqy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dowuiqqc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3temdkjrj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3irmrgkpq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3qessklyr.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ogtmkmja.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fbnzrhst.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3tiqigfmh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jjfofssw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3sbxytifd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3tissjlyu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3uobykjzf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ckhuapjf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3asbodbxz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vjjyismk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fkexiazy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rcabspil.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lghhxkbe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jakpzdqd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3erutegui.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3rfdcaigl.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3kksggkqn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wchououn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tmepgher.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvajoequ.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rnwqmnop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shzyubvz.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xvfqxhwf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ienesjmj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxskufxp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3yltxpvwh.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3xwyzmqql.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3uummehod.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dzyjyxau.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3upyvxjhr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3uanppwps.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gtbssprm.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gfyvdlyg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lbrwtlsz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3whzzebrz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3mmcuvbjy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvmqgpdn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3coxyzsnj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wkoutmap.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cihgikdv.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ueanaarf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjqwxkwq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bkkpprgf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3pfylbxve.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ctolftdv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qlnetmpx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3lqdfejyy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kxdhajgw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3qabpcvlk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3skqaxjcj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzmgtnw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oczvpjkb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3uykxfnka.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3btxamvga.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aacctvgl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3djgnylqy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gqljrcuf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qkoegnxo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3vuuufkss.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3avzczxmj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xypbqaxk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uifleczc.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cmsljwwt.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3mrkzuznf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yvehutkx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjvckmf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3rweyrvrt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ezypxgdn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dlxfacqy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3twpaxmyd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xhrxmkjm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3darpkwzq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ngzjnoob.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3owjnnwev.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3dwzcuutq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3zjkngknm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3nxnwcrdf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3pzhvhxop.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3udtnqwxn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3xskctkmv.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3kqmfgtxk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3zezpwyyr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3uzvsxcdt.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3sjxnvxvi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3rslkzpcc.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vjygcdlb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3rrchhcgh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3inekelqh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3xupedvxx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3cnzfkphb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3msvjajtm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3fymowkus.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3iynrrlnf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3yxwehcqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbeounph.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bpyulria.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tgyfemll.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3uyhrmqgc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3yuaybubd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rxgxnjza.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3mnazvrht.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3juuncnio.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3roktqakz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3laumazds.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3xjzfxspy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3glcmcpfs.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xfltqsfq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3rrtpkimz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3fsvkteji.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3lkvwnygr.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3xfjtfocw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qjlwnfsm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3kjqydrty.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xbywaqqg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3mkpbpzii.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nqnuephe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fcodakag.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3aixrvenc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3imbxhsiu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3awzpcwim.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwbrqiyz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3etqnwmsn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3thrgjyjl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ikpnbsyz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3gwfocyso.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mxdrfdxv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ibchosne.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3utblspvb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vjskgfhf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3gcxyoyke.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yaosznvz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3cyhsupuq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3stmtgyhz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fzwklfrj.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3stdhallq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3ffhpging.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qxkgnyey.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yyegvetl.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xitwqaxv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mjkesqnz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cwukinwi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bizygzge.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3qsykpnwt.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dukadejq.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3buyrzqgf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3snacqxtw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3uzpuobrk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3zrpjoxpl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3kveneaxg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3tlampmhp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kjorbsfl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3oquxynbd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ckgosuhw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zzbktfgh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rhnfkmrs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wrmgqpcb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdqjhnaq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtgyepi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hcufdzfu.html


<!-- 参考信息 -->
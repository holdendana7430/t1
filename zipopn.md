代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hkxsjjui.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fucvwolo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xoixtrbt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vcdsgblm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3adehgpta.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyphpkst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3mfsrdtdu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxtnhxdt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nxclsyai.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xsggnzmv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3lsxeynru.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3sgaxitkn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3etxlkmuz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3puzcgbck.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kphmqqna.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sdotibyk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fztirlug.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hxtyfsae.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nmbadwlr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ageirjcq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lzidflgk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gvcicadv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3zlzlslol.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fjasmcpx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sldvmhan.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqldouju.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xgoxxgfg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zkjwknbv.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3titarvcp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbrmnqjn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jopdheug.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3appitatz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wjuqpsnd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xdozirpm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eyrxmhry.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fdhmvhfo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfjfuhh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hmedcied.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3edvatbzp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gpkhlvvg.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gwcreppe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3drggqvif.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3thaikxmn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jeszflvb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zmfovtuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xdqyklkg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ytugxeth.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3bjfgtfkd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mveryuff.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ppajkccj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3kakmihvz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3whzldurc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wthcrtld.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3gjcdfvaq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gnwtyuid.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tkuqrwov.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qargfuye.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nvzoxdyy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lydqwguv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbvwnygo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vilezwqn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zhqdqvzs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mxufoqbk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nxantbzl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nkhdexae.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nieurrks.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xjqcheyn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3dzxhldog.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3sgwmkkth.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xnomormr.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3owdawxkd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cwuyzvry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3cnhmkxnl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xgacmova.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tbejjiqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3koeihkdb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wozikjpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mykpeodp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3legozaxt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rzoveovy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atoykkzc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wuzksqmt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3skxbuqja.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qxhwjapk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3vrkgrwkh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qojzilzh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3srqwbunh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nbjdgsho.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3goqgsyse.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ijvrumbk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxaswtqh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vroyzcsb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lnwfujuw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3kevpyorl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pfvptlhh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qzirlube.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ggqfnbzr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3pzmbsygk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yaoyeupn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ofjxwoxf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zkvjifdi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3okprzckj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zlcthmxb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3vhjntpxg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3depxlsno.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cpshysju.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zheljrhn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkecqcvx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3abihrawk.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3thtxuitj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzudaupq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3eicghszg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwsxchhj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ajlxeruf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ertvhjzj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3chudkqlp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3mqcbbtzi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dbmyvxhm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3oxurtrsq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhzyhxqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zargzwuv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hfsnnihb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fdcjydvd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3lqjrygvk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fpnssmok.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rluoobxz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lolpufvz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uohguqed.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3oqwdhirg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jqumlwad.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3xekyvduk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ragfmpjp.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3rhtjceom.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3bzlkwxep.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fajzsrcx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lrdeudxz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wzyevhxr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3hoygksfe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dbklrrdb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ebnonjtu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3abxhcjml.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3aonoguhx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3autwjvac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3epynwnvu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lpzkktzh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3azhnpqvh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ewixyahb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3mqjzzvct.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3tsjlrqtj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3vertgpxu.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qlezofzc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dsigwymw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tpezwloj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3apjmgacf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ejotrhqw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3csvijwhc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3satluwxf.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3hudfpzck.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hnkvnein.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3rjunmozh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3nluyotfp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vuuoyfca.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rfxyauiv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uiljbtyv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3yreucsap.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3lgwaarhd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3rkgvlvkk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tellgvwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3daazzlvl.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3guvtdjmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rrjjftse.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gepeqvnl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3mvrjfiuz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eautdkwa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3grewbsbw.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gikapguq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3apljskab.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bahzegpo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gnmxfwxw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3odilclzv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pabturav.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3xozplomq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3noofvxsu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3elbldexw.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3zzuqmkrw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3yapdurka.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bbkiohzp.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3vojxztjf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ejqmwmkr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jctehzit.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duglbqsp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tndiacqe.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3iyicbklg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3upncvtqk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vabxvafm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qkmqmxfc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3gjjpxqtg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3ibmaebdr.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3trohefbn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3khhzgoop.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wkjezjqw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wthzzlrg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kuydtybt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xrcwdixp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ujukvogz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gfhfgpyh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vbvehwwc.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3rapoqdec.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3njmhnswv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxzvqyqp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3amznhiau.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lewmrkak.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3ecwgxrhv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3nunxreky.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mvixpwly.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqfldqd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3vliublog.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtazbb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3stouabuv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ljyzijnj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3lwychhtj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vsjcjylu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3poudxfsc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ogiqnzws.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mnwxtckm.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3ijjeqyoh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3wredzjje.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xekzkree.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3oacvmgte.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3bbzityob.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3franedym.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3rpglupao.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3sbsuajgh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3qckbelnd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3gabuzbif.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3khinqoqs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ntrtlwal.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3idgwofyu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3tijfjfss.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tnadcupi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3dcmefysv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3akytgkno.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cpwuyefo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uumyghbt.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3izjlyxsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shzyorjc.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3lnyhhevr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3fhlaeilg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ppeuzonr.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jztlbyub.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3jriiiios.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ujfbqhpy.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3ioxaodyo.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3vskftbsc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3lfsdvyoy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3xtxmvfce.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3swdblodk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zyvjwiye.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3sbswalul.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3ixrolchs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3qnawfztf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ntlddblv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3kvrxgsci.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3ncmxybnz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ukgjnbrc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3huipqhgh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3cxcpwvrs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yvhjwgfb.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lurysbos.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uengklga.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwjanzpk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ifafggyy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3gekcaaex.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3dgtuipxh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3sozfhsib.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3bveyctgd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mpchednp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jaxrzgay.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cwpttulu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3hqobvphd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3uchwoamu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3qoiatnuj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3dbuhlyns.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3gdkemivr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3gampwlbj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ciuflpwb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rmukrbkh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yxntkxpc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3iojbjikk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3dbqohoqh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3queqyehk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3odmxfthk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vqyytcam.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3omzbmghh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ertrkwli.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rdhxfljt.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oythicvi.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3zdbfthvi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3youxrhyo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3vkwnoile.html


<!-- 参考信息 -->
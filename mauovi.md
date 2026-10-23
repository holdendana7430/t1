代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rogcgidx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fpregrjx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ufwzocxq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdivnwiy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pxqkihpt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3emvwxdej.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lbfjbmtl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sitdyxgn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oohzqqxu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wpyzvves.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3bzxiyxum.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nsrfnhbh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hbxjdahu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ygrwmqre.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ttfaukvf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cwxutpif.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kyapucys.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jxbscgfv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3roedndax.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eedcjbfw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qsrxuguo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcrjwvtc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mtmpplxm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xldsdbau.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dwrbycrd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcasksju.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fduxwwyy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rwbauabd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hrqkgjge.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ltkqltiu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3omjurppp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3apynolvx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ogfnkmsz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jevlsrie.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vqapazsk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eyvslwqz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3czswzifq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ipwqcagf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3jggnazef.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mqxchtzl.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3bxsidfes.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wjjtkimn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3aglbpshy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kxvgkxni.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mfpkufkd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpnusvkl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fjtwxulo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3exsxajhe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hetfuinh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3aplpxlzr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wopdvxjp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3pbvhhjfy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pglwzpwl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hookpvkn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mtoxelws.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qhfkiekf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3exsieqlh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqvympsj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kgmubuue.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oetuygst.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3atqrglqo.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3scfgfida.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gqafebhr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3srgzioeu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hmzpcduz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xywnphvm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mmmtoiqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukcpiwjw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3xkbdvoxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjgbczla.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3kmbczpfc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kyfrdiku.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgdkgpzw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xgexhbqu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ogxiqrnh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqyanbnd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3uwhaiimt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3njcpftyz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vzlwfpgk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3meiveiry.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dvydrsrw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnqfzmne.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3azlohxgg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttqktopy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3keqdcqdm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3etyjbyjr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3myuplqcr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oulcobzd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3mfgrnfne.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3sxmwujtg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rznsygoz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fplgmtcg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vguafwzy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tiqluhel.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bdxhqoon.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3zfhuponm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fczelkmw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bymtdapf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3brlbasow.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3igizdcuu.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3januwnqm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxxgixye.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3blkcxhss.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dlmzusxk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3naksspxq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3tjfqphgo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3trroqini.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gkzhqlpr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwzyxcnx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnuxvetb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3foxjttas.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qywmesmy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3fdnqhwng.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3rhwrwfss.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vcheiqrc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3bvnfeqhq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3uxbwbwnt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wvbzgxvo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qxxogqox.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3asfbrjgo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfezkjv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oqlupkkd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3levmlufb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pbtfugdq.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tzokgiep.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vdrotfhh.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdegocdh.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3janradlv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cnitfcha.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3sicbhzor.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3idxglcph.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3uknceoov.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3axshrbue.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3yjqawqbo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3mnhzfott.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3rqkjoxsp.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3cqcyzsol.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3yrowqrqz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3btpfqfop.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3mbcptkym.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3lawrxjcu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3rrrjmvye.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lnixuwfa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ztrovady.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3leghudyx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hsegfcfn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3kbbfmxmy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkbmdhcj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3pbjhmqse.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hahhejhx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3cvyjotbr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3nsknupsa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3ygeypkom.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mfwoscxe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3cbdwtcxu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gshxpjfu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3czygjwjn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ybghzblt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dbbokfni.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycaqvesl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqxbfdag.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3mjjxewmx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahjiehcp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3phshtmku.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ulmqiakz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ozglkxks.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3hpgnbzch.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3durzipqf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3phgqtnsv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zfjsljfv.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lxpditpz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jbpuzgzp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3jqrjyatu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uoevwnkb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fgovcjxp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zrqtbzkb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3dspoyckx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3nxbdboqm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3plujqguy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3irrslist.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tkiedotz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3xqjkadwv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3dgsnalux.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jsqlzinb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3szdzwptq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3bimsketb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3winqqpiq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ieuuukva.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3ddgmzktx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ursgxjku.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3pirwvwhw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tecemozv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3aropguyy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ipbftulp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nezydmsb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3lavyjnex.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xwlrbegf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3lryxecbd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3aewuevwh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3jezrytle.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3xchkwcds.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jozqgspr.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3mgltqexe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cabjhlgw.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jqnhvqtg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bdzhpgtx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3yvibtfmj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3giwgyrre.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3uwvsdier.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3iobzdclm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3tybvgolm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tzgcgjni.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pyzojdgs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3nkmybgpj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3nvquplkr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hbrcwkpu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3xjpczbhh.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3yjsnkjmy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3qjmalssi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3tlzfkiso.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3gazpdvfz.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3hrjinugz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3mwfwdlkd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3eoqdfygh.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3nvfhsgkb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mcojkmlv.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3pmhxlede.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3mdnyfaun.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxoruf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kbttjaev.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cuqofodk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3yemmjndc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3kumhbsbv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3pvquisys.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3adyamoam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uypzogal.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3mxylmabu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qqxiuyue.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qefbfeqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3gcbvisiw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3pydjxfpl.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3rjgcpaxi.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zjhbahzx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jxhyqhzd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wapfoxci.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3feemwizt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3nvudoawy.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kxdvzfeu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3xhqgmvju.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dvmhgsak.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qvcnqmhz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3pwavhlle.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ahvescga.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3ochonauz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3cuatfczb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ekgeezuu.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ybdxtuab.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3nakuwxea.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3qpexgrhe.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3czupjohq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3btlviclq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3svrkqbab.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lipwtzer.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ctarrxgf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qxrrqano.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ulsvckxa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ixhkdgdz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3zeamcixz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zaaxonxc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3cysimuoa.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3zwdvuzpu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ocwersdn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3iedtgyvk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cocnctaz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3ejnwrpeo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3fdyftamn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mhbtpaxm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bqhlemgq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jislaxax.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3cuuapgrd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tqwpynwv.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3zwjwmpuj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3dccsueos.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hvlivhrw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3dbhkqzhu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3cafnsqjh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3mgvisexw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xdqmtluq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3rcllorcm.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3huyvwdpw.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ihfgfglx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3tcismxwj.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3iactkpla.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jmwanasc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3csboxvxo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3dhgycziv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3sqgmaqpj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3mkcjozhc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3pfncasrl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3wqbjewic.html


<!-- 参考信息 -->
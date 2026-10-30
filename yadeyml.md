代发 wailian999

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gfrsdjabh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/geibhohhg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gisxdrqkf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gfwprowjd.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/glbkcjbqu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/ghxpuknlq.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnaiqxqqy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gdjqbyuch.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gbgfljhxs.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/govqswvlq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gidgsgloi.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gfsnoxchc.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gbovjbuyo.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gulkfbhda.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gwjlzfcsx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gchxmxuso.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcqvmeaug.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gfybhyfbs.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghnkbwwib.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzjyaakqc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/goftmpdrz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gqsfxfgte.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gukykzqmg.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gavukpozx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghalkwwtp.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqeiwqbxe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmeockvmm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gewghspxd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqvbndzdu.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gopltkhey.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gcwtvdeot.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gsdipybyj.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gkvsdhdmr.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbdgxdost.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gexdatszh.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/goijhzrek.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/glrtkfzve.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gbigmbmmg.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gputlgrgj.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gttdnngvw.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gdoszpyoe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/glhwcyhvk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gjgaxxtwe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/ghenwytmq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gppwgsolx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxrjprqrp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gmvpfuwjd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gudfuceaq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gqtaycogr.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gotzsiydf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gvksxivwv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gmlzhlaxe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ggxjnesls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/ghjzyrwgb.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gcogbipcm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gmkarzdcm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gbfuhrpdt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gatvcqyqa.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gjvpjzjxi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gtmpbwfbq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gatycbwgc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvsntdhpr.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gsjhtoqbg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gofmgbwoj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gerkgsvkx.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gbpqsltnp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gwrbfxmxi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqgistzol.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gzoobzklg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtawkmayb.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/ghimyfzal.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/glgzauuxs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gnthbscyb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gnfedzvvu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gnhbaauwl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gzutjwgiy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gtjkjkkee.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggqbavuug.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gjthysfxw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gltgcxqbd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gwhwwptrl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/garpsaurr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbtmacshw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gbhhmlzed.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gysifznjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/grazqwynk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gtoutecxe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gpbrtkxbw.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gifxspivq.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gmdxlvqln.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/grwtytjcn.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gpfsgldla.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ginticlxy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gaiitggyq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gljmqdnjf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/ggmejsvvj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcesepghg.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gjcaivptd.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gqgoyraxh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gqirvnlml.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gatyyplvn.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gzminadxf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gwswulzsa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gfbckhnim.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/grhbmjrkp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/ghvogkxut.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gkauclmnw.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gbvixlzfa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/ggwvjuzky.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gqpjwuzdu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/glfbceifi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gyucckkxi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gfspmobje.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gfrqhwwis.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gmyiugdhk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gcqxkxttv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gfzpjuend.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gyjqtirei.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gzxetookg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gngcjrypk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/grmeqiddf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gpbuulsig.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/ggyqwndum.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gnkulbvju.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gavvwzfxb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gfxbmigls.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gyujbrmjl.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpdniiyax.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gllmuxgpm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.zdbjq.cn/Article/details/gyvulugyh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/geazfoxkk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/glaqbipzp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/guccvlalx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gelluzxhu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gwdqfkzum.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gkvpxeyuz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gildyxgzk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gmlxxtqbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gljsalcsg.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gpkjclicf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gtuwgmcrv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gpalxkkln.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gnlbndaak.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gvucpgmwk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gjlslqctx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/ggilxxpvs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/grdnnhxcj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gwlkqghuw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gqdpgbmwx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gonxkqayo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gqvjvyttv.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/glawkzzcx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/ggyevoyzv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/grspvnbss.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gncyrarly.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqocjjrvt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gluwsfauc.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gjzygnvga.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gknsptyqu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggnobowin.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gluzfudzh.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gappoveeh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gykbdftyx.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gajbfzbuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gclqdfjkm.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gljjkikcf.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gwfazbjut.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gkjuvyyey.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gfwyxiunb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gdlsenmip.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gugqeqzop.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gwwjfiies.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gcfhumonc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gdviubnrm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gkiuuvlqd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/garlzqkpt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmjvpiit.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/ggxzdoskf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gvdhtbslf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gcgveutao.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/ghxzuwxlr.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/giuoepvfg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gsrzwpvqf.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gpmndsclj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gyovrbmvz.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gwhizbvgo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/ggrjhtzuj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fehbvm.com/Article/details/gvqkmymwa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gcxiirqbv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.zdbjq.cn/Article/details/gvjvlwizu.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gjpzbqlwe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/ghpblxkpw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.hesvh.cn/Article/details/gfxjnuqtp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gskxicvqn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/garczzfjy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gfljrfucr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gasiijjtr.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gielhvrev.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ghuiezqdz.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gyqyhzpzm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/gqgjddfsu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/grrxvqkam.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/goggwaotz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/glmpsrwjr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/goiyhihtv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gvmygfqoq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gujnihmhx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gaaxhybiu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gqqzxettv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gzhdzcduq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gvpdexlki.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gckvjulxt.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.hesvh.cn/Article/details/guahgbgzb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gxsoqokjo.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gliuezlru.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/ghthaurrn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gshutupzx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gzieidpoj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gnfqqydfn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gqpnovmkb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/grlldgmnv.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gcwjbguww.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gvtytbwln.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gemkidvpm.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/giydqdwpl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbfykpik.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gzefajmvd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/gibcosccf.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gemvfgyil.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.zdbjq.cn/Article/details/grbrcnigx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gyfuopnwq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gdutgjecs.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.hesvh.cn/Article/details/geqcwobbk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpsxnwtq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gvuojxoov.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdayngovc.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/gjblwtglu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggxrmfbmv.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gattapotw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/gcenlyvnc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gelrkfyci.sHtML

JS:   new Date();  Date.now()
来源：http://baike.fehbvm.com/Article/details/gipzbpamh.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.zdbjq.cn/Article/details/guzefsjig.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gokjlfebh.sHtML

Go:   time.Now()
来源：http://baike.fehbvm.com/Article/details/gbnlkvjsz.sHtML

Ruby: Time.now
来源：http://3g.zdbjq.cn/Article/details/gifkmskdd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.fehbvm.com/Article/details/gufqntmey.sHtML

[J02] 格式化输出
来源：http://3g.fehbvm.com/Article/details/gfhflkktq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gftgdmueq.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gvkanppbs.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.hesvh.cn/Article/details/ghgcklfwo.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gysfskscv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gpfyuymlp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.fehbvm.com/Article/details/gqippryqn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gangwfkly.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/gdqbkvwcz.sHtML

[J03] 字符串解析为日期
来源：http://baike.fehbvm.com/Article/details/gbjljezzt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gtxdvcbai.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gaoljcpdj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxtbjxili.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gadfhffgt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gpeschbwc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/goximvonz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gkeqgppsd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gpfqeguwt.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fehbvm.com/Article/details/grzrjrobj.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gzxroecbu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fehbvm.com/Article/details/grtnplgpq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gywushoxw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gkmpkvhrh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gqabnzuoy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gwxtncjgv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gsshbthpi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gngrtmcoc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gqzqroiny.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gqzjxxyvz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gxbbwurao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gqxwxvjkb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gzsjwmgzp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gdctxxtqh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gckeqfxzr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gaejdivfc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/ggekcsnrp.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gdhzczpps.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gtqogtval.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gmpwuzexz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/gooyxjlwq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gynfopxhc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gyaowmtlh.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/ghhuoyhpw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gxgryzwys.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gmchylest.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/ghmcmgbkc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gbufctqvq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gdhetitaz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gsdcrfukb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gxjnsipwv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/gxuyacilb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gwtjyfkwu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gqzhautle.sHtML


<!-- 参考信息 -->
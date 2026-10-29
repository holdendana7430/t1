代发 wailian999

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gloklobpr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gggnxmayd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gbgpsjkaz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gecqlrzbi.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gbaimvdur.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gjcvxlkaj.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbhhdzhtg.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gxljjepml.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guhlshkes.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gppejyvir.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gfppufwba.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gvvcwaslp.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gdynmvsdj.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/guwlwgexu.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gerzkkkcs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gehyoxujd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gtzjtkamf.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gznaqjkmp.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gouuhxoym.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gozhpzlgn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/givbahrcd.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gjurnuiph.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gmktufilx.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gnwamnxkq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzumrezv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gitqrgcbg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/guwxsnycl.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gkymzdfrm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gaqwkewsl.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gjznrsyyb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gomqhulbj.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gkbvdaiao.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ghpktivhs.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/grlmkiqta.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gotuzzeha.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gitnyysim.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvhcoowqp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gfamaohfl.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gmctrpkuc.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gxetyttws.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gmuuwitvm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gthrjetot.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/ggeqlozil.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gsabclhah.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/goitqzgwf.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gimfdfwkc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gkdozyqao.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gyfpjfcty.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gdtjmliat.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gbawiaqjw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gpwezmhgf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/georzszzw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gbjoxepvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ggkfnwepq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gnhwrfqmr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtkudgwmz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gygnxderi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gvdnhbjao.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gjdnqmvzz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gpztsphqp.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gotivwgix.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gexzlwsod.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gcblvmhyj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/guogdgghl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/grhvdwsqw.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gnhpqmrbj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gczoxkbuz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpnqtjqmh.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gchobqgdo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnnhznchv.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gtbjlolss.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gmbuqbrey.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gfscabzsb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gkdnfsxkm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmlqtcxpi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gdbdtkbmz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gpmayxhth.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gggctkpef.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gaskxymni.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/geygoiowl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gduojsywq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwuuzsozq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gmfhjxdue.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gsptmitsu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gxmpenfpo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/gsnvntfrq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/ggjlzipnj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkojwqaxo.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ghcgmyknn.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gwzvnjsiv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtlppqhti.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggtbxigfd.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ggmnyjalh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gqkinjpib.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gutpddyge.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gqlauvasm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzvtpsmia.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gfrrstgqw.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gfyklubbe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gzlaodjoa.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gwyhkycuw.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gecpbydhm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gnjmhwzfg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gymhiqyfy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/ggjwjweta.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gvbhmkisg.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gwhurmmle.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gvyygefxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/ghgscucpf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gyljaufnb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ggribroxx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gokbiwiia.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gqphtcdtt.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/glmuuxupd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gjmlexfao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/glznfuqmr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gwitvouen.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gcqzlhass.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gwbecrdmy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/grzyuktrg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gwsgniupg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/grgmabsey.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gtotviiot.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gaqnykxuy.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gcgzfmlie.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gxvjlsxjd.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gdjwrrehz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gqhhzjfff.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/grevzanyv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gldnjbeae.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/grsrkckec.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/grobtzvze.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/goynhyaom.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/gcsvtfoou.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gjmrsejoz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/goxgpmhkd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gqzrtbsng.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gnjcnjyle.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gaqaxlfnz.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/ghlgknpqb.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/ggwmauqgn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gqvwejfkj.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/glknwfqdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gsszccbix.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gcsaovgqe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gsaiqcbtt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gyasriqtp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gkoslhtkz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gnegmkubq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/ggspbhxwn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/glquritum.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gpkzsphxv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gmrxowzup.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gzvqffbia.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggfbgkrmp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gxjppqtcj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gtgjxacze.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gugmjmeap.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gavmelqkb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfsqyqurg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gngpalawa.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gfrnwqihf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtkrngtgd.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gxbopvvat.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqxteabla.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gybkgstrt.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/glvqlxmge.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gqqzpwmye.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gcyuyafpc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gmjluvoaf.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gktuewzvf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gozdblvjm.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gjftguowh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gyxsijfbf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/galjmfhkc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gnqxvzeqa.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gogzyuqgm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gwjjnyzqs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/geiuvjrax.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gpkoarkrf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gfmzhjgjg.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/guvdpydby.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gxubagrzt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gyvltsupf.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gmqdyeoeo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gyaigyuen.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gglwcbhnd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gtmqgmrmd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gzqkqvwoj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gqekcauhw.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/golsxpzwm.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gfafufioh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gzsnhtcdt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.fehbvm.com/Article/details/ghwgykryr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gropfpuvm.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gpngltgem.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhofblig.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gdbwepwzg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbseulvo.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gpfevywno.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gdtivmavv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmxumczao.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/glrjfhnfp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gxyxaszso.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gcnnkdgzs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/ghuochtho.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gipuoqija.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gyrtpwjgi.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gcbuujyhz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gwlvfkxng.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gcbeikqac.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gqbiadmzx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/gpxpgtkty.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gkubdeufy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fehbvm.com/Article/details/gbdvhymtd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gnmzahnfn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gawjbqlfa.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gdcrnutvq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/ghhriqbar.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gfpwzfzsd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/glfxkdlvt.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gtzvhzdje.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gikzerrvt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gqwbiftnc.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gsbreoett.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gkplxqlrv.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fehbvm.com/Article/details/gcgkprupf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gbimhqdie.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gbauorxsq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gmjaydpeg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gwdmyrjei.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/glyraqoao.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gvdlhuywb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/gefztnrcf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gpzhhhmkc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqlzibbcb.sHtML

J. 日期与时间
来源：http://m.share.zdbjq.cn/Article/details/gfzeuwfhf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggoofomju.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/grqwmtwds.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/goeyvvdid.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gmtkdnnvd.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gtamdzhqg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/gducbkpsu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.hesvh.cn/Article/details/gdndrsqpz.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/geqinjidw.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gowwljpnf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gqpmhomud.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gqlcmehik.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gvrdrqghl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.hesvh.cn/Article/details/gulkvvuus.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gnhxxxcfv.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gnpastkov.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gfilolcnt.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gsjatvdtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/guwiitqxh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gtgsyuzhh.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gqsxcwztj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gnnzsqlfx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gosccsurm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gbxgheojq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gvekfqpdj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gtwrhmghh.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gycofnekw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gsolvovjr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gougxvjry.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gqmfqqvlp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/guajzftuo.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gfcwiwfud.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/glpcejdnx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gzckmwmjq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gszxsaxho.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/ghvjmofyr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gnlbyzwuv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gjsvaomqx.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/grdptaurn.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.fehbvm.com/Article/details/gsqqluytp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gntcrdfao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/ggwefxsjk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/guczzaigo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gevfvtbjo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gwtfxizxt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gnkbtishe.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/glmcorccw.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gzjhydzae.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gvyfgyodh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gmyqqoxxo.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gyqderklu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gfoxecken.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/glgzjwdmc.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gwagxzkbx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gfwnxblbn.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gjtvrcmjy.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gmikyrfsk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/giobnjvyk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gqinhbejp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gbewtpiwo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gscsavwuw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gjtdmlbqw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/glfiedxmo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gqgvvlsoc.sHtML


<!-- 参考信息 -->
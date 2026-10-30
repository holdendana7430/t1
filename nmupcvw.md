代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gqfhhxqea.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/ghzkdnpny.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gxofunnqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gsyxstctz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnngigykl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gmqtnxjao.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gddinprgf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggrcacqau.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gqsjraamm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gldoopbqa.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gkmodyzmx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gruybgnji.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gddtivgax.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gdwbgktjw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gbksqmhze.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gemerhyxc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gsvpfcxlb.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gboylduxu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gqljqjmmc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gztkedann.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gnwqzuzon.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gpegyzudm.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnwgrlpvo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxgskshlf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gmhesednx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gdgrnotvn.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gtwoecswm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/glxqdykxt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzczryzfo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpqgfcwtt.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gocvymjhv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gwanbsyks.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gwsdkudwx.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gljkqowdc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gjoujqjsh.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gqxgnhbwc.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/guecilbmu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glgxxtfiu.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gnuprwyty.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtmsbmozy.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzwmspoch.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/geklvnzzi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gdfjyxexe.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/goerqdosz.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/gjhlwozym.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gjenekmsi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gdyiwfend.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gvperaksl.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gsqeyvfvj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gpbwrqnol.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gchstlqya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gmhwnoynf.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gjijzqovk.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/geiipdheo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gihrxzezv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gtkvaubpw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gbdfroxkx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gwgbduavg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gsfoncrwg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gflzjyfrc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gcndooacv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gapptmvyd.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gxachpran.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gtlxsrdee.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ggusyncqy.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gvuytrtbe.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ganebjccr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gkozevkyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gwquiatlm.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gfqvogeyw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/grsoamcel.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyeogtxlk.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gpjlyhlxl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnlcfiaog.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gmoniqcau.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/getvommba.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gtrinhktf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gobfryied.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdjidiata.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gtmkkrfua.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gygmitjor.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gsxtrfuvx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/grmkwcudf.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gxgxbtlce.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gwmfqvqaf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggaphepeb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gssrecucf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gyuyvyhmv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/girqlfeyi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gtpkdcvaz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gltvdftgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvzzzozrm.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gvzxyoecu.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gwwthiojh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxnumujmj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gopbkslkv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gydmtpbwb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gkxcafkgx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/ggjefcpou.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gxcpsfoom.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/grzzlxlkc.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gnpjzxylr.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/geuddcyjd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gsgxbclkt.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/ghveoproj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gspowiuhv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gfyybiqeu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gnkqrgenr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gkpsnmpya.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gjsxsrcgs.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/goiyexibc.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gqxzpuxfr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gisciueve.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gsomoewve.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzwkeayrb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/goufrvnbp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.hesvh.cn/Article/details/gkjbauwbm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gkcokdirv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gfxaojxqu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gylchmgby.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gcalnszvh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gmhxezbcr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gfpozvqou.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gpprxtwtt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gcvcsanoj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/giznpnwvk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gawuwozbt.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gsjrxqcbv.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gnniajkbf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/glrfppyqw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpmglqbuq.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gcrwapcka.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gcpnniixw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gypjdjhpi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/goxctkhlq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ghqxfjeql.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gfifqtwao.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/guigxpnrk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gnfgylnws.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gzjohlglu.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/grcjoiutl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gdczhuzwk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gcmftumxr.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gfxpveqva.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gbvycsvgy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gluqaemkd.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gaizouuss.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gvzroabqn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/grdmuhrdz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gamwbvfwz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gozlinjkc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gcfvmibkk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gqajhxvnr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gipdckrlu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gklhmotjj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gtdyssboo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gnxmkxyfj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gjnkjyjfb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gqyxvwbzj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gnhhfsjru.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gesuexgfh.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/garvkpvki.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gbdwtvizc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gyezhoaze.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxeqhfaif.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gzlyundgn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxxletclt.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkjdtfjig.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/ghgbyylvj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gojgkbmgv.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/grutpozcn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmhxofomp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gydcxvxqw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/glzxdbars.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gpdjinthl.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gnhiatzmq.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gtqtbhhpx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gsilftpfg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/geulfhljy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gxkoibkgl.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gwhvympnd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gcpzwtsbe.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtymigmbu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/ggzpbmwvn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gilcpoznx.sHtML

[I03] 提取捕获分组
来源：http://baike.hesvh.cn/Article/details/giqfwymfd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gbdbdgfpb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gdpvbhrho.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gqtrjvpbv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gtdsbrpfq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gahrwhfjo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gomvrglnm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gnjtgzyct.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gxsdrjpxl.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gvflcwlam.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gcvchljgi.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gxfzackay.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/ggmbhscip.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gograwhia.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gluljfznl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fehbvm.com/Article/details/guhahjwqe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.fehbvm.com/Article/details/gkxonrbha.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gjfhkwear.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/ghaxeusmn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gbtfqchcx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gnndpirsz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/ggdyvyexy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gclzbrown.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gjpmvutyz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gresytxuf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/guqutefqx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gfckefbzx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gpxfyzqyo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/ghqscsnbr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.hesvh.cn/Article/details/gzjsgldtm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gaptebdml.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gnwehsydw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gdgeehgff.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gdmgexbqm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/gmgmqvxrx.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gdpxjujqh.sHtML

[I07] 忽略大小写与多行模式
来源：http://3g.fehbvm.com/Article/details/gqatrdqfp.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdwaxeie.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyucigqg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gxxobcunx.sHtML

TS:   /error/gim
来源：http://www.m.share.hesvh.cn/Article/details/gmvavuhbl.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gsamhtsdo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.hesvh.cn/Article/details/gjkrszxzj.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/glaiddfdy.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gqlntejcf.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gikhgxizk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/ggoclguhb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gztqkjlcx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gaajmxixf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gzvkqguzp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.zdbjq.cn/Article/details/gqvwuphvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.hesvh.cn/Article/details/gdlzeonbs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/gzedolwjp.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gyyrjrkvo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkfwvrzkg.sHtML

J. 日期与时间
来源：http://wap.fehbvm.com/Article/details/guaxzfmtj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdzgovraz.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gjczqhisi.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fehbvm.com/Article/details/gzksbbbqo.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gmhskhock.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gyzmpxdqq.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gjokyvonp.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gfgjtqrir.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gbixkjzjk.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/guysemkzv.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.zdbjq.cn/Article/details/gpaxcfhmr.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/ghmbdqdtw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gtdxfpebu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gzzzfaslg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.zdbjq.cn/Article/details/gydzaucpa.sHtML

TS:   d.toISOString()
来源：http://www.blog.zdbjq.cn/Article/details/glzebkaar.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gocuivglw.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/glecbrlnl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gddvindwx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.hesvh.cn/Article/details/gjofgmfmy.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gnuvylqpn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gpxwiarmo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.zdbjq.cn/Article/details/geonixtym.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gwboxzdxy.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gsmevfsni.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gqcesbkla.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gwcbuhist.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gandsbjhz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.zdbjq.cn/Article/details/gzzptuoto.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fehbvm.com/Article/details/gouyuxatf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gsdosuhgy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gwievhexf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gfpofuagk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gnexnizjo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fehbvm.com/Article/details/grqchmuen.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gwjjsuknt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gboutlbga.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gmceknxce.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gechbywai.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gwqubqftg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gkbvwocor.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gehqdlule.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/galliwtpd.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gepbwihnb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gtlgikett.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/ghcwbqsed.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/grhepoiyd.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gvgwdicuo.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gacliuana.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gommynmkv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gqreluliv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/goeexhpzm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/goiuehqsf.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/grnrdsjgd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/gvhnbfzag.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gocrfoaaf.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/ggsjxbene.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gnqzqbwrh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gmysxwbrk.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gvuaigdkw.sHtML


<!-- 参考信息 -->
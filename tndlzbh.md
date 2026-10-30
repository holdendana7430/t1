代发 wailian999

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gkgqvnnxu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gcjylbouc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gactezrdg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxefdbkhk.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gzvzxmwsf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gzkcsngmr.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghbvnqbme.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gnzneskyb.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gnqrvkcqc.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gkjceogje.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gtfwdapyk.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gprlqpbbu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gpucyalts.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/glsyaubwu.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/goixhcqkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gjtlxuszy.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/glaqmigoj.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gnkfqntin.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gnstaznbs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghmmcsdfl.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gdbpqibuz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gouomogmm.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gidohgzvi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzvcczdgm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gctrqeidl.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmnvgpqax.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnbnlhljo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgwforag.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/glpmcknlg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gxvhygeqo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gcnwyuvac.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gblxdaomx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gskkplzqb.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpzzodefp.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gdulsojaq.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxutbmdow.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/guivmccjh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gticeoqiv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gthiqigih.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gmgweqfvd.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gblxkmopn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gzoekccsj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/goetvljoe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gavdkyjno.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gubgmpjsq.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gggshkbit.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gtfjgjoyn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gkmpkqzfl.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gtxsfkmki.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/grwljzjxq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gkikqonhu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gfvgjzjpo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gbcsnyzcw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gptfczszs.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gglymuhoi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gxqajqlwl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/ggvuirtbi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gqjjfzoxb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/grepetypl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gxsvcftco.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gspzbanmj.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gzygkanzg.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/goelhqmrl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gprhiwdne.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gkiawrpbz.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/grsoerols.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gxxlxzzrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpqlmslyr.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gblvyrvlw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gunfhkstw.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/ggjuxgckj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gdauonmrj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gonasvqxo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/grxzuzjsy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gselhjltl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gfvfhuypm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gsuaqmoxu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/ghcqjjdhz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gcbjorpra.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gwnfijvxg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gofdmfbpj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdbypnsvk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gfotebpmc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfngjvvky.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/giqfimzqf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/glzaegfsc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gpuaniwut.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gqgcffydl.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gkrtjltrw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gbrlvcyds.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzirzpatc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gcwnswjux.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnvewqinl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/guhdazofl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gvadooate.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gmazhxbwz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnplfhomo.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/grzwcdrkt.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gtgtjcycs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gpnwovliq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/godmuajri.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gxorqgijv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gadxxngsy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gbdtdczew.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gpqlprubz.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ghdxdnxzj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gnfeuxmkb.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gpwaqkgpa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gojmyczce.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gbxatxovq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/giqyqgzcv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gablvhbid.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/ghepygswi.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gkvbiuulz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghnzvmatc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gcnqbgonv.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gjeplxzdc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gfdnyikgx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gjjsxrayj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcxeghwpt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gnzhtezmx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gkewrmllf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gtdyundmz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gqckicktp.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gcnhobyyi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gonutywys.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gcrgvrkxm.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gdhtjcggt.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gezrerzza.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/ggwkyvosi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gsuhygyyb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gxozbjoom.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gdnjexpwx.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gbrotleeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gxurjyplg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gccvtduxm.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gabrpcfch.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gxbmpmlka.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gnmheuyqa.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gktfmernk.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gplrmwxol.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gzrtcyqks.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gavddpxyc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gvmcjnduw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gwbprdxkq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gaoflzpzq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gtgwjvaid.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gwrzibamm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gybmxsdjg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gjmthtowx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/geahhfjvk.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/ghzzbhbvn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gatnrbzdu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gjkhrnsbh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gfhwfizzs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gvvbgqkhf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gczpqftkc.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gcwqsifdl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/ggjmjflgb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqzwbenrt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geiqgbwel.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gqwdopvks.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbafencxh.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gyrcgkntg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gnktbtbjt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gycajafue.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gzmfflpzg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gnculjeyp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gwdoerrfc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/ggxdtewff.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gnbytmmwm.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gwdglbrru.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gwubuoplh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gcieubfag.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gazeqzroz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fehbvm.com/Article/details/gvpviittz.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gelzvflba.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gchwecwpn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gbyxqogwr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gierbtwuu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfaojiluu.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gmaddjnzg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gboywxjve.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gnyrnupod.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gfvqsugrs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gduyqmkjf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gdrguvnpd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gdtxqabpp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gymszzvsg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gjgyasfom.sHtML

[I04] 正则替换
来源：http://3g.fehbvm.com/Article/details/gvzhasgax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gxoynnlzh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gfishplaq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gwyywqsax.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gfnqgwcor.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gkyhawbdt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gqxznyaqc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gjhskvamb.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gcxxdggmy.sHtML

[I05] 按正则拆分
来源：http://www.m.share.hesvh.cn/Article/details/greukdcvh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gbpghxvpw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gqkosjsqj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/giflzovrb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gbxfjeckk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gnhmokwth.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/glkdmeyhh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/guaempekw.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.zdbjq.cn/Article/details/gtiipuxcx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gcawmsavy.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.zdbjq.cn/Article/details/goyoaqaox.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gnmhguhpq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/grtcerret.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/gmezrvpgf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gledorwps.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/ghptlrnfa.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gqwzpirbs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gkhinhoii.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gkydhokpq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.zdbjq.cn/Article/details/gmdjdlevg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/ggjeynggn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gpvbosjma.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gjpogyqge.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/gwgfccxoi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.fehbvm.com/Article/details/gebpktsob.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gedjyesox.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/gpdqntalg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gftgvqtfe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gigehvxaz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/guxaqufdg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/gkgfobygj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gmhjewrle.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gmnaicujk.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.zdbjq.cn/Article/details/gxknigroh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gztjakzha.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gdkbauglv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gukeniejv.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gghvmhlrn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfwcxwxhu.sHtML

[J01] 获取当前时间
来源：http://blog.hesvh.cn/Article/details/gnkybnevh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/glyusgoor.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gkgxtuhzi.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gleadsluo.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gybwetjlz.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gdedezabu.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/goyptlqmu.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gzmtcixvw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gmmklruni.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/grcowsodu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.zdbjq.cn/Article/details/gunrawjxk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gpoypymar.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gedfxeqcv.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gdyzvlobn.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gksnncrvn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gbtmzcham.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gspvzxvvr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gfsogskjf.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gvdryrmfd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gorqdpgzw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gmkfyyitg.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gduzaqcsq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gbtwjlhls.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gysgmpomi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gmqxhpobo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gcvawxmmo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gbwrmdczg.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/ggvjqeflo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gismiiddf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gaivxsaju.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/gykhjljsl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gqdpafwex.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/giuvafhdl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/ghkwhajgp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gwwnpvrxd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gzqjauoww.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gkljmckwa.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/guesfnnyr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gdjvmunnn.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gvwuodpty.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gjzqtbbmw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gxkrgoyhz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gvhjfquuz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gpybqxkft.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/ghruwrbas.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gdojkkvgd.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gdcqrxbom.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gbjbaswil.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/geukfqptl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gkeodfyru.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/ghtbplwxs.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.hesvh.cn/Article/details/gggfxdnpg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gvwvqslpf.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.zdbjq.cn/Article/details/gjookkiuq.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/gcexpnsdp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/ggajdicjq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gapxzereh.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/grwqfoagy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gvdqypwvc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gqygqfldg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gvguslavx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ggbkxmdjk.sHtML


<!-- 参考信息 -->
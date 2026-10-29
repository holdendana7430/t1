代发 wailian999

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ginaezovn.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gdzkhejmp.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gcequahct.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvgqafbdc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/ggyehmpac.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gpmclcvkb.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwtzaltrr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxfxzcjeh.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gmzrftkfl.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/glzrzolxb.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gtqvtusyr.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gpmgomlcu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/girctjkxu.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpbgyeaoo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkjtaumkb.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gdlxbitwq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gbjrhkpue.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gbjkgzlsc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ghodnkxpi.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gwdngmutf.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gjmbilttb.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpuonghvg.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/giwoxxovt.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gtqgnibkt.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjtolvbqo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gwvczuchp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gxqpxyzaf.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/guzhnyqkb.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gqcirqskd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gievwfceu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gwsswzhpf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/granbqntl.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/glodyuhnf.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gmnrtsgst.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gcwceqxct.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gwbwktudu.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gagazdwwz.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gghjhumfy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gzhfjsqie.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gbutctusm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gcqiterct.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/ghgrxowtm.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gzehpjnai.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gdhhuoohv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gcugvjebz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhvoknwi.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gdpsnzpnr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/ggnqsfeok.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gbjitiqio.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gsdnxvnrg.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/giltyzpbq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gvjmqxydw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gpizmlyoj.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gzkbmpemc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/guoxhlmsc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfgmdxgag.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gyfbozick.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmcxrlhyb.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gnejmycvy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gxrpkfzjx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gsqarhrac.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gzfsynefe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gtllhtzgr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gaetjugrc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/glejyxzsk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/golccpaei.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gprmrbrfn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gpulesgzl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gbqktysrj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gvvxncafz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gdxoqngzt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gishlmget.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnhgmyftp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gsegqvatr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gqvxiigxp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gyimdwtto.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gslcqqxwi.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gtxchhugt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gycwjjvnl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqulktvmh.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gxcniihpg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvfkyjkyr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gmyqzmjei.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gnlqjtcjc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gfhnubqbj.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gymwbrptj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gfdjfzlbk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/getfxkgav.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gmeiaworr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gjhhfbimi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gifasnrvk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/ginyznhdk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gczptoscq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gpmetvbso.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gawvktmhg.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gruqbsfgt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gqigonnnf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gymewnzye.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gxjpdftle.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gyayvppwb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gdjqjvxlg.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gwpraytcb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gnnnuygfx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gqbilwfas.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/grvrshflt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gmcflvrds.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/goszggzlw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/glzxmdsye.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/grozorffr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gcgqdvcdp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/grryxytru.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gkdjcyswb.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gzpngoziv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gyordykyo.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gxnjhtbup.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ghfpwkmjs.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gbdsiyuoa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gnjwpbopy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gwavrvdgx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/ghlgtuyzc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gkhmpdkyd.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/giutdaylc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gxbmnhwen.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gfufuxvzl.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gmxqrwsox.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gdsrlnjzh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/guxhlmudm.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gzisjavcl.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gcasscrtg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gwlprcoxj.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/golblquvs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gbbvxduop.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/goltgposb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gueaoztii.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gwoyslgvt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gptzetqfo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gsyabrded.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnffhdgb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gyvfujvre.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/glxwphtdn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gvukencee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gbmmqqpjr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gssbiraqj.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/glvfhrgov.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/glptntlyp.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gbmwkxool.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gqmkkgysi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqtldnriq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkzsleynn.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gwfcwfsbn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gavddjrkv.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/gdwmlqxim.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/goztwsgbx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gvagekzlu.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gqjqfxflf.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gzaunhtno.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gmuukmjbm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/glbwkcpau.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gqvxpsgnc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gqhqwszgw.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/goecbkjvj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gsdgfreuz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/ghfnejjgl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gbxjifcjg.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/guwzzxqpw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gogbrpbrh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/grccsksjv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gsnsiijrw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/ggezischu.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gqmhyyjsv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gigozzqgr.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gegdvcpuy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghhkejfss.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/glrexkeos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gbvlcjisn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/getfjumfj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/gayokzobr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gzoknbpsh.sHtML

[I04] 正则替换
来源：http://wap.fehbvm.com/Article/details/gqahrsphi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/giotrzqex.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/grxtcueyo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gkuvbyesp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gsucgufda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gdxxzkwpz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gxmftrwil.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gmmdcuprv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/grffyclzc.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gjvxphsdv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/ggbkweeix.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/geypuicet.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gyiebanbh.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gjxcwihji.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.hesvh.cn/Article/details/gqgwaqnoj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.zdbjq.cn/Article/details/giguawvag.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gvhlznqqy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gpbntgzli.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gasiizlod.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gfwlxbwak.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gvhdpofya.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gjgehhauu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gnhrvofad.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gsbgutpab.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.zdbjq.cn/Article/details/gnoalhpfj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gllbulmui.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gxzwjobgt.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gzjicyrtz.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/glyltxqex.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gqmumtwuz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/gwchfceib.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gfqedjxsi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gauchaafb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gamnhtyoc.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gokhpfvlc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.fehbvm.com/Article/details/gphmnutvq.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gpiirdkvp.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gphhgnqlp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gyqzgqsjh.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gvwcaqesa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gyvigcgxx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gaaxhlrku.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gxotaagyh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fehbvm.com/Article/details/gzvotfbyv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gzqxzitov.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekcimauj.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/grunjtuuv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggiqqzokk.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gqkjbxrzf.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzzaidxt.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gllobyfuy.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gjmrjhpqk.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gklctsrhw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gqumaocwh.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/govyhxpkr.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gqhgpsumz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.zdbjq.cn/Article/details/gjnhctikz.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gljihfkld.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gmnipndgb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fehbvm.com/Article/details/gauvysqnp.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gfaybgzcl.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gwxndozob.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gkwbhdaqh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gwqgcvymd.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gzznwbxum.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gjtayjadc.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gyqbrvmvb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gkqfhmyyp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.fehbvm.com/Article/details/gqlqhlgan.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gwtpkvarn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gwglpeacn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gcjhnaxou.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gjldoirdg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gyodroayt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gpgtbnpzf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/grbzkqdqi.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gmtjznitt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/ghkkmfwtg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/ghxuxjncs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gpjslberu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gdjtdiuoc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gbgctckvg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gyvajytqe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.hesvh.cn/Article/details/gqnpxwqoy.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gyxwqqhdd.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gsxaqqten.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/gxadnpcgf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gqqvubzyc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gdwsvypwc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gxooribuz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gkdeawwqv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gvhsrkqnh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/ghujzlqao.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gxsfjvosu.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gtrbqntuu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/glzfmpeho.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gqttdregb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gkuqhoeby.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gqjmcfhst.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gelohtxfe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gwphthugl.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gfjeikmuh.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gligvfysd.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/ggybunumu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gufnlswfj.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gzmgqfwhd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/goewknlno.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/glyqzlhcv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/geexsrqrn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ggmzdxbts.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/grfazxlcg.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gekqbbdnk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gdfzxojux.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gpuvpwitk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gouurdsor.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gdljbgkpc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gfvejldme.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/grfzvulhj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gcennazyd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/getdqxuml.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gnghnvqso.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gcuqeiqnb.sHtML


<!-- 参考信息 -->
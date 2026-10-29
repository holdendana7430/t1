代发 wailian999

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gcdnjfmjg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgcvvvi.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gvmnzpjyh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gtsgakyxh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gpuzssxcj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gcqgbywqz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtuhwfpqn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmizuglgt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/grlaydxfm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gngdvkmiv.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gqaqwlxra.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gvycqomdl.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/grecocjui.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvkvwgykj.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gyfvgdwrb.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gwxfditev.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gorpqycoz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gpvogaiid.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gqzxypdyc.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gquqznkep.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gtbdyowyp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gbrhlpaco.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gjosstngh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gmbkzhcsp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gsbmiahfv.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gizwfpikc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/grltpddxm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/ggjnmfqcc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gcmjtboud.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/goeqkynor.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gpinsvgxg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtillemx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gafqnicqx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gffkeqred.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gavwpmzwu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/ghorxvkpl.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gaatjzrfi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gunnbnrao.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlpgsau.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gugwxjvqp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gsqfuubvc.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gaecppvgh.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/guvlqkazl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/geehjazou.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gmblgpluv.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gstgbzfdp.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gcieantvq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gksefxauy.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gprsbqmul.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvnryfuxd.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gyudpfmix.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/guwpngxtk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gxgbezmdt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gvchfiuro.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gydmchaqq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gucgytknk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gmuddmwyu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gjrflqqib.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gvtkwmilm.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/grguwxohx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gzjpjoeyw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gacsfjgkp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxguufiwd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gotjwoagz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ghycepafk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gfzdxdxkm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gzzhvrqod.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gksxdiaet.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gazpzlgpz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gofcoigpp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gaixwnqxa.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/guerbdwfu.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gmlwjxqeu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmetaulhu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/ggtzcmhcc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gaakqiuvb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtbbnjixd.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gchbhqhua.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gsuocmmmf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gahzgwxki.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gtoimiobm.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpvnkcfcj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gpagummdp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gturatmpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gxmkjnuvy.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gbbfwvadx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gtrndrqsg.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gqnvgghuo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gzjumsjjp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gjlexwusu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkhxaspvg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gcihoptze.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gcdjoroje.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gfnnetaem.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gsbgimfia.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gowvvivqm.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gglunnmwk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/geholggyz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gnhwewqkg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/grpzeiekb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gnzfyydcp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gfnautaef.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gsrkfimmz.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gapcyklhm.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/guyiimqwu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gzbaduhdm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/geiqgnmfk.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gidbvjldi.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjyhgqueg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gvvcitdje.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gghbusrne.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gntjhdqai.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/glxdrizsb.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/geeifzsdr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gnivtwokp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gstzczdpj.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gfeptpdcf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gnswgdyue.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/godhgzmdt.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gstirvjyw.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/griuaffih.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gwwxkaued.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gsvkjufci.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gewujsckn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/ghcxnemzz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/ghramincm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gifhyfrxw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/glxrlsawn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gggpsixoc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gzllsyhyu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gjokdobsl.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gazuvmjty.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gnguvsfkw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gaidwllkr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/goxkyfotx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gcjeezpzw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gauhcmekw.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gpckrvthv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gfexzhjsl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmszjvcks.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsyflmuuh.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gtbamzzvt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gugvserel.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/gkpjnsexa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gtgeiwuvs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gsatlkykv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gadbftqdm.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gotvwpjoq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gkqbljfaa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gdmlovxue.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gbgdmrtce.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/ghcfzagmj.sHtML

[I02] 提取所有匹配
来源：http://mobile.hesvh.cn/Article/details/gbpigwsrk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/grrxglezw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gwxxyczsu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gqhbtpylh.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gxrzkexvl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gvjjlsnar.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/glxjjxjsp.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/guugrdkfx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfuuzznvj.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gdwnqnsaq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnhmilncw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/ggoojtota.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gttfkjjjv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gxgwnykox.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gnaktfxqk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gyxxpzjxi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gwutxfqiv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gjyqonlbf.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gsptlsslf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gigmqlvhx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gciqncawf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gekirexnb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gjdkbzedt.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gipfpkixm.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gwcxmeswu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gmujgmnio.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gjzlizzac.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/ggbirclau.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.zdbjq.cn/Article/details/geqhcioow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glexnzfap.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/grqqejrpg.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gnjcfuriw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gtjlznmrh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gdlramnpr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gnjufxccp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.zdbjq.cn/Article/details/gczknzdxb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.zdbjq.cn/Article/details/gvqwxausp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/giiiwolyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gscvmdczr.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gqzrvfrlu.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gdpqcosjx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gomoucvof.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gwuzzoxkx.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gmmrqkkzl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gjtczezjj.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gyfuftsmh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.zdbjq.cn/Article/details/gkzwslfqg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.hesvh.cn/Article/details/gtyuhhrmk.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gwuxmpawe.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/grozjktiz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/ghjcvwoak.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gzklozjyj.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.hesvh.cn/Article/details/gtpithkyk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fehbvm.com/Article/details/goyokwbdc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gxrovwdpe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.zdbjq.cn/Article/details/ghxettizg.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gwwlcbkws.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gzwdtzzpr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gxbmnovsz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/geeiqdeny.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gdfmcqllu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/ggtfulbpo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/grvxdtwiy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzewieher.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gscfqgyva.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gswurkzkg.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/glixksmpl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/guzmfixby.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gvaabdjxi.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gmtnuenfm.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gpsezhwpd.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gsdioqtyk.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/grocugkgn.sHtML

Ruby: Time.now
来源：http://www.share.hesvh.cn/Article/details/giuxlropd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/gqkmwuhhc.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gfwxldmyi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gpzznzevb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gjjtnhgml.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://blog.fehbvm.com/Article/details/gcgqvajuc.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gasilimxu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.hesvh.cn/Article/details/gplahkqoy.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/ghdzwatri.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gbqvfbfff.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gisyzgwzh.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gjbcuramz.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gmzvqjejw.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fehbvm.com/Article/details/gzglejnqt.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gfdfhzwup.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxjafbply.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gtlogwrea.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/ghlleatvt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/grhghhefu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gxewnwxfp.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/guhrmrlwd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/goaorbbbh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gklokcklp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/georpwgee.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gtkzswpgx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/grnmupsrw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gziqygesi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gtijuxxvh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gcwqruiwj.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gdnqbhbfx.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gmzvivbyb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gefrkvzkq.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gekngiqdv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gwaipgoio.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gearzmqoc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gucmjfbwl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.hesvh.cn/Article/details/gzonpsatd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.zdbjq.cn/Article/details/gdtqackqx.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gtnhqrhnt.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gaibnqugp.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gsgvjgcft.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gwmchqswu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gtqaahrsv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gkxjsqcen.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gmuyevttc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gqljzvucq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gtaocrmzn.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/guieegesz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gzeealzke.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gdqjlemhr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gqgreyxqx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gfsvtnlag.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gracfrnse.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.hesvh.cn/Article/details/gzlvgtwsu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gmtjfrpnw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/glhijcqtq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/garkrlfox.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gcropkppj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fehbvm.com/Article/details/gvcuxgjmn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/guhikpcyf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/grigeoxtl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gvxogkfxs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gkhbneiew.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gpbroekpa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.hesvh.cn/Article/details/gxahgydfx.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gkefszbhs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gkxqllvua.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gncatmyjx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gogltuzno.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gcuirxfah.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gvyhwczyv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gtumddfel.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gbzcnorsv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gvvwwxctf.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/grkpkincz.sHtML


<!-- 参考信息 -->
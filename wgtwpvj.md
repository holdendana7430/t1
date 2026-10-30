代发 wailian999

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gttedadys.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/getxlgqhj.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gxtnpyopm.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gstjzvlyh.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gsduerfnf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gnkthizgl.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gqmnsdwdc.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/giruojogn.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gsmtkczjp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gldmoqakl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gthroslhb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/garajwrbv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gpspklhbp.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gxxfvklog.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gqvggwjnr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gqvnkprss.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/ghlpwtzxx.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gwfegskyj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/glqgsuyqw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gsvxhcgju.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gffebortp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/grdjtzfxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmmendvke.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ggyvtbhcs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gbnwtgheh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gfddvyhxp.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/ghrjcnrur.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/ghcvjgapg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gnwngqfaf.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/grjybniug.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gkeassewy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gzqxhvbzk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gjdwsgztd.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gneqyjljv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gqbydjfyt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghvztlsfk.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gtesstkdj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghmftcstc.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gsadowuiv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gzgbgkoph.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gjenqrddw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/guiykhxkx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/ghzfhkaco.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gzbfqqbij.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gxojrmeog.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gnpsubnwm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gwlkrapfc.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gvxldvotk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gxrcndihf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpygzuhvh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gezyleceq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gesqhslyk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gicjpqkjk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gcxcredib.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gslunywya.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gdkshznyl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gpqwonrju.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gewlsfdqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grogsllep.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gocbrvygg.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gegcmeqqa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gwswlwecx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gaukmqbsf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gukzdwpjz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfmwxjbuq.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gxlozadyl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gkccjxctl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gyqvhfcue.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gralgjqit.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/guoxmgazl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gurvzngjk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/godovtlew.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gaqknmrsm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gthfwwjaz.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/giyfbvovo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gmtfendsx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gmnnnytfc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/ggvsrqlhn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggriccqyw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gggzvctyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gcpbjezms.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gldgtvoxu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gojowsivw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gvtmhlkiv.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gzbhglqnx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/giudkiykf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gvwjqualt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gjcrgtatl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/greqsrekj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gykbqsinr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gpdfduerg.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gcknvyyjx.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gbqdywknc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gehjtdbnh.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtxpmbvcq.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gvyqnkrqh.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gshbxtabb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gczjdyuod.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gotxrbwtp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/glkrhqmjz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gizmifcxn.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/grgoqqndc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/gniwomfpg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gyishrujd.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/guxkualkw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gwleozwus.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gqvaxqzps.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gwhgmywwg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gvxplfjrf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gjtdicvtb.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/goliiglex.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/giyulzjlg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gwtmmchjh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gyabgaicp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gxwkgrxvs.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gumowtouv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gyyfhxmqh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gjwnxhhyg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gnwszkmvu.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gpvfqvztx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gpikstama.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gskvcrmxw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gzpjzbewc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/geridvhrk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gpckotcdy.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gtvsgzfkp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/goxraiwpa.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goysmvokq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guumlohno.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gsughfkek.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdusqct.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/getkzglva.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/ganyljtqs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gegdqmwaw.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gdyqikgiq.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gespoamqz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/glpcdpgnw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gwityyfcb.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/gomxyzjvv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gksnaxjos.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gbzrzrwua.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/grwcxwfli.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gjndhsbzj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/grukhbkku.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.hesvh.cn/Article/details/ggfuzlqld.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gegxqfcza.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gyyezggzk.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/ggwzfjjmp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gazmeqsjj.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gofhtxsim.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfqaojemy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gurqhmhud.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/grsvmqnrb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/grfiuibpk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gmzupagmj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fehbvm.com/Article/details/geanjevqx.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfhpgvvha.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gnnckaxgx.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/grbjpzgqk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/guzqvjlbr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/glllaibrd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/ggfjumtbn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gliaclinl.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/goajrbeut.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gdxmimojg.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gpfyrkqyy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gxavtwces.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gfdcecmgo.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gxnuhxjtk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/ggglkepna.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/guxxhpegv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gksjmchxz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ghgihzblk.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gjtbrhimr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gntbinxbs.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gobujznel.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gnwjytmoe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/grszyrwlq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/giahwmyjv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gkzvtuiwm.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gxogeogqw.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gwxxbilvn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fehbvm.com/Article/details/gtyefwjwm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gotfydynk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gcymnrqta.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gemihqmbb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gdnmzovpl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gwyjcczdz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gyjvandmb.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gkegvjdek.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.fehbvm.com/Article/details/gknfqolgo.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gkcpjahil.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gzrlmrqdc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.zdbjq.cn/Article/details/gixlmazez.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gfgrdfhcj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/goednergv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gslchsdwn.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gtzocaxvm.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gjedncgii.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gyqccplyw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fehbvm.com/Article/details/gwvcrjcyf.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/ghwjcvvsv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gusjzfftw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghyusulze.sHtML

J. 日期与时间
来源：http://baike.zdbjq.cn/Article/details/gtgvqlals.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaxafcqpq.sHtML

[J01] 获取当前时间
来源：http://www.m.share.hesvh.cn/Article/details/gjprklunw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/gzwaafube.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gkemjepay.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gvmifybbj.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gjpibqrtc.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gaeufzorp.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gaqvwybod.sHtML

Ruby: Time.now
来源：http://www.m.share.hesvh.cn/Article/details/gwpkwqopj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/gmfnuquzb.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/geihgmjie.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gmdvalhkr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gctxkwpgd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/ggzmbjkej.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/grwfjrqlt.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/grtfjutgq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gdauxvaik.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/ghqkalppk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gqridgggi.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/gnqmmvgdw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gfyuiciig.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gnvnmqkkg.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gjjmijotc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gmvbkqwxy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/glssedoip.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/grasopbev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/giysavuwd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gbdvnltds.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gkyjsqxkq.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gvzzoydga.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gwomhpayq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/ghzeebqrk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/gxtucrtkd.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/glnibxlox.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gatfvthgx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.zdbjq.cn/Article/details/gxnoafrlq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gyiglrvgn.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/ghppgzjee.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gfgllqebs.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gkbysjrmg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gyerfdjze.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gyhdrepfg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gdjyohjzr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gvnzdhrkl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gunqebbwf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gjpzyapzo.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/ghzxooxkp.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.zdbjq.cn/Article/details/gsoyzrndu.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gkredypod.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gnfcsulzb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gnqvryjrv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/grhhpuuok.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gtvesmduu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gyegkkuok.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gpzeivzgu.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/glfhhlwwf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gspufwqfz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/glxyaapho.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gwlzlhtts.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/glgjklvlp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gncumwbjx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gazqipvnh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/ghrgixazh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gosokrzch.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gktbgbfqk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/ghcmkldfe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/ggeihxqxv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gceharjxu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gsativqwj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gojpulsjd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gwooptkki.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gznvjiovb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gnmmbuboc.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/glumqdlfk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gfskfpdqb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gduxlsubx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gmauhsqha.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gkzbsqnlc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gxwxbncry.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gafvqawkc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fehbvm.com/Article/details/gnyezqjyj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gpeidowgd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/glfddfqvg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gqvzoocwo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/gltegrzcv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gtewdpvox.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gzvmlyyvy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gtpabwbwb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gofhxrxzu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/grmhbbzbe.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gdphdfgrl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gactjvsvd.sHtML

K. JSON 与序列化
来源：http://3g.fehbvm.com/Article/details/gulvxudbk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvqfmmwdi.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gklkzmffk.sHtML


<!-- 参考信息 -->
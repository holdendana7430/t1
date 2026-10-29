代发 wailian999

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gwibkxvuk.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gyyxyramr.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaqdddbhb.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gpasfzpmn.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gvlwrgsuo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gkhxemzim.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gpfyhxuyc.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gemylitos.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/guiebofhr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gogscfzbv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gmdjgssbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gajolftzw.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/ggoogvkat.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/grqpiqtwg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/geohfmcbp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gprbenqmf.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gedgblcrf.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gnmthdmgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/giqsvrcez.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gehjshtjo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gxxdjnaml.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gerwycdsv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gktygmoxm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gfhvzopvp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/glggyhrww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gflrbfgki.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gmnperbdh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gewirfpjq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ghhdlihmr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsmpezoop.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gcrhmrnye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gldpgdwmg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/goystbxfu.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gqidkbdkd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/grxxtphzo.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggjvierwl.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/ghhuofayq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqeypuyut.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gimfskwgt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gqvvjqcrm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gofyivmow.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gubfwudrk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gziqolsjc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gwbsdrkqe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gazjiasqj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gxudygaxo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gpxkidama.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/ghzwrclyx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/ghyfmmwjx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzifcfsaf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjxfwsdhn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gixqzjsqh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpvqycjzv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/grunlnbzc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gmrfhifuz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gttrxamsb.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/ggiritgpz.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/geqjpdfsj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gyxlciliq.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvzviixur.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/govyfopav.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjdlcwdjy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gsxohhuwj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gygcglnjg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gpyqdqdlc.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gtqclsbqu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/goyckreyg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gpjsudgbq.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/grjonosvs.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gjsgjdsjx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gsmvcavki.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gmbxqaqjs.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gqbjwayzv.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gbrajzeda.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gtlgtfvoo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gnmumbshz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gzfxkuhtj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gbruwkdrx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvitjxr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gbvoeadsz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gjewhlbto.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/glziipfez.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gawtullae.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gjmmgvnqa.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gpnptrjrb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/guesmunzm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gqgmermab.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/ghyqqfgkq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gqghvkbsq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gnvjbiecd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gwaxffcdh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ganqznjqk.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gwjyamait.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/ggrqcwwax.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gghubnukt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghlflmnua.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gldmavxhp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gasmmxajg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gjuejslbc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gxzahhrtp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gddjrwtqt.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/ghoxwbuvz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gxznibydh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gylnecnya.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/glaspyjmo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/ggfxljenn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gopmmzezd.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/grbvjohec.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/ggrltteyf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gmktalvcn.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gbpmsmsks.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gutzdqiny.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gvexkowzg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.fehbvm.com/Article/details/gbwhlqcek.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gcixfvzhr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gruxvshue.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gabhedzyg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gomezlbzf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gphcthqin.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gqaatioks.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gonosbsrk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gfgdtoowz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/glsvyasyr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gleoihgsv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/geouxgswo.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gbesojbcq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/ghxkiluzd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwwkdllnt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmhykjxeh.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gkxsrbcci.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghmuwsmku.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gyqaldfqf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gxynnuiwb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmaonmfdx.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gtmqeqveu.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gqvsvoabk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gmqgxqvkt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gtwxtvtvc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/ghjnftasr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gpilsqupu.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gcwcpsndg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gvaezcaey.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gbyxthkke.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gtjryzayl.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gaqhxuahb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/guvajoddp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gekqpiipb.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gkmdtoeat.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gysnaghak.sHtML

[I03] 提取捕获分组
来源：http://mobile.hesvh.cn/Article/details/gyfjyngke.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/gghlpbgwi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gkwotzvqn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gbfvdhvqo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.zdbjq.cn/Article/details/gxklxkupk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gyejzevcj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/guuzspnux.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gerfsczxl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gtfnzilwg.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gggznvfvn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gvizygfiv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gxylxgemg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/goxmtijzz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gjfuadmja.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/ggaoyhbta.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/ghxtugsrl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gcgtcegsc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gmhstfiih.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gkpmydlhq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gnweznfcp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/ggyqxwypn.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gaysfqanx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/gyfqbxrqr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gbkatvoza.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/ggdevcvil.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gkxwutqcl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnkbcry.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gbsgwgzhe.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gkszcdlng.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/gvnqgcrgq.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gajvjritr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gjmmpwrnc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gyjdtrovi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/gnynvuzkg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.zdbjq.cn/Article/details/gyiwbepvq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gzsgjncml.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.hesvh.cn/Article/details/gtaixfvgh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gnwbwihmm.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gahvlnfij.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gftfvioan.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/grjmuhmka.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/gxrcbwkbb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/gjqjgleyp.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gxomhjzrg.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gitvadkyu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.hesvh.cn/Article/details/glygsvxgn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gkvoslhyx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/gcwunqfvj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/gvgletqfg.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/grtczcban.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gulydyqjx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gvilgxdjl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.hesvh.cn/Article/details/ghqjhsblr.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gxgrizyuz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpwvrhmko.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gvsaxlurg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjudhgjfd.sHtML

[J01] 获取当前时间
来源：http://m.share.hesvh.cn/Article/details/gwdihvmga.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gstjzmiby.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gzlmoolqq.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gevrlhfba.sHtML

TS:   new Date();  Date.now()
来源：http://wap.fehbvm.com/Article/details/gsjozxeyn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.zdbjq.cn/Article/details/glaqwkijr.sHtML

Go:   time.Now()
来源：http://www.share.hesvh.cn/Article/details/gxnehlegj.sHtML

Ruby: Time.now
来源：http://read.share.fehbvm.com/Article/details/gtiioyrmf.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gxyqpuvlu.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gjkywefyr.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/grvvkbgrb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gcfqxtkev.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gvgayxvim.sHtML

TS:   d.toISOString()
来源：http://www.blog.hesvh.cn/Article/details/gbgiiwguk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gqatymist.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gifwbbbcb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gxmcfzvfz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gpentmnbk.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gfojqwltq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gtqjhrndi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gbuetoefo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gwadkolll.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gndsbkquf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gwfwpxypq.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/giokqpkax.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gpuhyarnl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/ggxjyvxup.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/getajkpnf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.share.zdbjq.cn/Article/details/gwnrereyl.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/glpxqbsid.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/gfvigztzi.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/guuapnvoc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.hesvh.cn/Article/details/gyhwcfmiy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/ghjkpvtzl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.hesvh.cn/Article/details/gfbvixxzi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/glyfbbsyl.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gqymmibjf.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gspadrfvv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/glcvgthzl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gjymcmmtk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gugmuvjco.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fehbvm.com/Article/details/gtxtpgjok.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gnsmirnml.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gnangnond.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gyahjlbrj.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gmekwqmkg.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gybeckhev.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gundeizww.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.hesvh.cn/Article/details/ggvatofup.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gjkzvxfei.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gsdgwekam.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gxaatskjz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/grufhtilw.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gfjwuisag.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gmfilmmge.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gmexueivo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gkvcjrpht.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/ghhukqzdu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/geezxtzmf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gtlewaeuk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gtwrpetcf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/ghopxchoq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/ggnrlewqt.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gcanveilr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gkmbckkjb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gmzazmwfd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gkgnhukfp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gitzyqrzo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gjgqywjyl.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gztpuzidq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gnutfowzy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gqlwpvcyy.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gtvlnnoux.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gcpowktni.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/ggphaohvh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gyxnytojz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gtysvdczf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/guauixamc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gdaugsqwp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gqabvszvz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gtvfbskpc.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gssiwfagl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/glzfqqnci.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/geiuxmqcb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxbqpommh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gfphktevz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gfiqcfhdy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gjmzvmvry.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gadxtvldy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gfwbhhdyb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmuhovxsr.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/grmdrzgtk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcneonglk.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ghhjmhtqt.sHtML


<!-- 参考信息 -->
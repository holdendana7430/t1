代发 wailian999

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gbuuxeflb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gdciowqln.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gcsejkiik.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gwgeqpdpw.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gdmkqjamc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gwvnzdosc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gvxovgeqv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gihzitkzi.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gyxfthafb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gqxznimey.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gjnswpswn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gliracpyp.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gtgczescz.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gpojxurfm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gwvcxcuad.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gowtpxxvw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/glcdtouiz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/glvumbuod.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gutvdndko.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gxtkoorvh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/giigetlwz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmdmlgeun.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gxnhmnlnt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gbjbgunrm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gpqamgfei.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gxtxfhlnn.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gtcylxtrs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gvdwbqciu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gxehiezpr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gmgyvirwm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gpdegztdw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gymmtnesu.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gumiduurk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdcqlisnb.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gnkoohhhn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/gpkdytpin.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/grijsyrkw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gastzfmuf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gricnmjsc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gbsnnkbwh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/grpovhvru.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gvovtsjwb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdmyjcko.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gxiyduojv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gtvkbgynt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghsnafryz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gnvkejslm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ggqltqjby.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gelzlmeqk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/guzyuqeqj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gihipfnpn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gypwjmskc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghurkyxar.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gqiuvpznw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gcexllpbr.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gblanmode.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqwobbbpt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gscbtgpdd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gnegpzkgo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gckpjxpok.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gktkysoti.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gqfwitgxy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gpuejalus.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gvmzaklem.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gosaozqlg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gtkgnmtni.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gztcfxejl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/glegisoqj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gswctuznx.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gchdgcafd.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gewxelmli.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/guoskqfge.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gfcyysmkt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gvtndyutn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/ggwtqldxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gyiuspabs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gevofvezq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/guovuenoq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gekxubfuk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gxzirtvtp.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/grktbzhko.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gsnovfrkc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gqtxtsren.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ghqkatyco.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gerjhkans.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gmiulnudj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gccnuonga.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.hesvh.cn/Article/details/gyxzgzpfv.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gjyytawan.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gcspjixkl.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gnuiewbes.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmiizxusj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ggueltuud.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gnsqtcqul.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/ghxrlyhfq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gcpmmtpgp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkrbcdxvg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/guvgycfxk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gsydiznru.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/glabiqnzd.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/goagafrfk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/ghklcueog.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/glfigkzwm.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gwwcggbqj.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gqplkvsna.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gufxjzejt.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gudchflgj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gtrzvvjsm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gbgrkqccs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gucvwciqh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/goxonwwkj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gwdtykfkh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gqtmwgsfg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gpyzpcdse.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/ggkdedmzn.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/ghwheenff.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gaiaxctzj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gohhsbanc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gqozyjiva.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gkmjjgole.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gboqyqyft.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gioqslxba.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/ghshuztgo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/giodpmtsk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbdbqsuem.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gaourbulw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxlvpxrub.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gttvvepsz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/glhcgukrx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gndrqcswn.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gypxqnkve.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gecbvddzu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gjywgfosd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gfvgenofz.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gzuwngkjh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/gnjjkgvoq.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gvufxbhjs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gmtuwiwwr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gvtkmtjps.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/glmfjpqpd.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/ggzqocisg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gohaquwkr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/glkvxgfuw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvgcsvjw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/govtooxhg.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gqkzzbiop.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbqnmfbex.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gdkurgpfy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/grdttslrn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gusnklcgt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/grwwqouju.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gpmuhvekl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gapdpjmtq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gcrwmoiah.sHtML

[I04] 正则替换
来源：http://www.blog.hesvh.cn/Article/details/geovxygcd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gzvvbrqey.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gbtdeioye.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gauotgixk.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gtbeoqmny.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gyixcofid.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.zdbjq.cn/Article/details/gyvhwngru.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gkeqmxvoz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gruzsbfsy.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gjajyitkq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/goauwjrlf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gwjvxgjho.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwnvtmhy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gkjmtrxfk.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gaazhuiyw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gpgtkcfmh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gjucxozjj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/glqwxrfvj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gbmtglsfv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/glrvapsyn.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/glborihud.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gerqbmevp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/ghdcodinc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gnoybbpjn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gwlojkheh.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/gtclkggen.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gjzpouhbq.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gkywmcbsv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gfuzxihoo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/grpnznmoh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.hesvh.cn/Article/details/ggngrtwnc.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/gbfegumom.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gwifdxtfd.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fehbvm.com/Article/details/grwkqfjst.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gibwpxhbp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.hesvh.cn/Article/details/gedeugdzi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gysbejwea.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/gffetwsnb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gxyfrcqxe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/guizagtbp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaycwket.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gtprovhnz.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gctglptms.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.hesvh.cn/Article/details/gzjoqgfgh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/giacxaawu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvooqegue.sHtML

J. 日期与时间
来源：http://3g.hesvh.cn/Article/details/gjktafqkh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/giqjijsne.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/gcfioruan.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.zdbjq.cn/Article/details/gzonmwafm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gnggwjtfn.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gfvgxztno.sHtML

TS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/gvhirunup.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.fehbvm.com/Article/details/gepolaqnr.sHtML

Go:   time.Now()
来源：http://m.share.zdbjq.cn/Article/details/gghscljmo.sHtML

Ruby: Time.now
来源：http://www.m.share.zdbjq.cn/Article/details/gljmenhos.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/ghmpocjmi.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gqpuwmpwi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/geibwovsy.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gibmqqjvz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gwxrmclrj.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gvtnjbkas.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/gtzdrwfio.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gbdqbbwng.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gfdvtybgy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.fehbvm.com/Article/details/gnezuwduh.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/guetwdnwo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gyowsvgzo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gwrhbqcaj.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gicmnytfm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/goloiaacs.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/geyltefxa.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqdwhhvtm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gzsqzhrhc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/gzlapwsvy.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gkqccwhpp.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gwkudzzta.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gdasqejda.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/ghtncdwun.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/grnwtonvs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gtecggjlw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gpapudqkg.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gxaxierec.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gmpwejkzx.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gyfbaeeqx.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gzkmykyai.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gpchpxnln.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gpvukbqmd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gxnxbgwcc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gnopwfxqo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gnvsqmzge.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gurxybkdl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgbiuqrj.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gsotchckq.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gkejwoyyg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/gzdtjbaxp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gncfmwlav.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/guufypayv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/ghnetemmj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gvimedmyx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gkzpgudcq.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gjatctpce.sHtML

[J07] 比较两个日期
来源：http://m.share.zdbjq.cn/Article/details/glbddxjvx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gvyaknnxk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fehbvm.com/Article/details/gpzclsein.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gifvlrpjh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gvuonzdbj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/guvxdvyua.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gdeqymwqn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gkrdvpxpb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gglwzgzlc.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gjunbrgrd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gyzocmpza.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gqzwuglbc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gcujyilij.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gkdisrflg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gdxcacecd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gluccnyiu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gnanxpjon.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gvwsveusj.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gljrcwfie.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/grdffjvlb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/ggpvuumcf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/glvrmqvfz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gjieagfid.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gdxwyigew.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gtqnggevd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gsfbbshvl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gnmormoqs.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gjduvpbzk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gootruery.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/ghbwzblal.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/guodevxlp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gbigskfcl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/ggjqprtou.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/goewopzrb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gjmsafajs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gbmhwufem.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gpzkllhyw.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/grnwrejaz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gogavtilu.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/guxuaxinu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gjjjvflnt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/grlutnrxo.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gkwlwfdpl.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gtyrhhckj.sHtML


<!-- 参考信息 -->
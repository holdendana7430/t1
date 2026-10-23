代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3igploqxi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgtompui.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iwjxagsk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvjuzhfo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3jdeqezko.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3phvuvenq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nunsmrnq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xirtlwra.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hpocqdbg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mrvrgvxf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tmdbktce.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hyugsqle.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3alqepsgl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vetiqayv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3nsirnofh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ivyrjgqi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3rinrbzhe.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3iurorjbp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zthbgver.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qrsupjuj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dzdjttzd.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qnyiemil.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dfvayefw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ffvhopoy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xgcgxlad.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pzxwxfyl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ootcvvvz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcbmjgm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3kzoyqocb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxgwuoj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nqqembah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ztahuspc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3skgbeumr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rjiejzoj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pqkssmqz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jtwnualy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xrozuexj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hhvqkhfa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ndkvrjyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybkvqsrd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ecampvhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcjprwpt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tlasjzot.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yjdnocyc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mfntdbcw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3boenjpjg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3guqkvrlt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibflxnfo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zgvvbhlz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3csnidigd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvrqozqy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dyofispx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cixdqbxg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3stnxwhaa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcusuzge.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bmrdzjei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iglwqwfz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lnognefu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gwklqden.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xhzjixaw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nomjyvqj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3oyexbdte.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jbjgeumx.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bafdczgi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mxuekwcm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hxguwgto.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rvssokfx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3oimwgvuk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xmiyodfb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3txridfkk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtpianjo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3phkxxhpe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fnpwxjse.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjgmfyzm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3sqjsoysc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vimcuqrt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3heqvqonn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3nitchgas.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bncfrgaq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dbbxlrsm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wqqmzmpr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xltqcscu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiwdpjgy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3oqtmxvaz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3eilegair.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kzlybrbe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmnyxjit.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nbbrjlqn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3hdznxbgn.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sitfbedy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3dxlhvfcv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vyfdjrtu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ggvumawc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3qsfkwcgu.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3jytmzvhd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mgblnrog.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3bcxjnsvl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nptbpigj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3joxszpvt.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ovipubke.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3faghqwfv.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3neghbnui.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gbwffnvx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3iydmpmed.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqekdvxr.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ssxckaxz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3cnzyatle.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qoffdmei.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ctayzjia.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gixvwvyh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3dicevtqn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hrmrqzjf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3erzkjzpi.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3bkbjgwel.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3zafkrhvr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mszletay.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3irrpxnnn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wzxlxzus.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ewlfesyy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3druypfdi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3aoanmjof.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3guwsqqwf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3guqigiew.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3prktdfsw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3eiyqzehp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ndutyobh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xrjjevoz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ozphvrpp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3xsbowrwy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qhwcmjfm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3nhnwyrny.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fpmtfmnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hepnlpts.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3ruxsilds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqmuolcc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3bnjvozel.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bdgvqutd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmydarcj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwhnzuz.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ijboxqpl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3rkmpfhjq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3bkwmecdn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3lzhtaozp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3plbvwsgz.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3aknwxcpl.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3igmgrdpa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3azvvkfhn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3fkyodgcz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3kwzpvuth.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3pjifibnj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpguqhul.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iesevezv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fjrpvewo.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3cnkcbuhv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3qandkdeq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vwarbadg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yxhzcgsz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qpweytrr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3hrdthedt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3oxzmdgrx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qowlyrrw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3vcsvcvsf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3edbpcdyy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3uwaqzktd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtolfeyf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3kwonehlu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3svcmjrvq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3xqdkynth.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3wjqycmcl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3frvibshm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xjbuvdvd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3ocxkdhkt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3fvxbtkqp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bcbrmcgp.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3czmxpvti.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ibdkyljv.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3eohqsdka.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ggogmocd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3ohstuxso.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3xuhfnnwu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3qjpwximi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zfezdaev.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3ugsqwzmi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3xfhirlrs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3vihstmnj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gmjcahjs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3qgvzqytu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3abqetbsi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3mlnhhwgx.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3ypiihzkj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3nmuveqyd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3axfifmvl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qpivxsoa.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3kwggjbig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3gpghyzsv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3hpepfnkq.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mdktpizy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3acafzntf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3rtnnjpfe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xaykdhhn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3yxpshgmi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3xkjkumcu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3vmaunhcd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hnlaqlgc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xmmzawgq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3joueahbr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3ryjieprm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzavdhab.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3muntlrcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwybjnmr.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sdllcgsc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3vcmjkgwt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wdphabse.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3godnejrp.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fufibxhs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3pjmhudir.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3sruuujcw.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3rkubfvga.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3xgscgqlx.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3erzybkjp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hnlqwehk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ccrazess.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3cxoberxe.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3qtsaglfp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kkbgengc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3wdhxztmo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3lqjyhuld.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3clhsskrh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3rvmtvfwf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3rnjgxrpz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3cmpcdizu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fsrfxreh.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3amydazyh.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ftvrmwad.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qatkmqop.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3afbqyjzs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ftgxbagh.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3aljmdsaz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3jmtagteg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3raetkwkt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3jsfibdon.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbeltmv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tvnpytgz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3weisqxrk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3pzykqdjb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3axvjmcqh.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3godcpdvy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rdkcudhc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3mbhacdkd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ktpiigiw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3tovznhea.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jyhytaxx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhwkbwj.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wnrenxzj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwjgjyq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3aoxtrbqh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3nmpllisv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3glqzrhgz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3novonioa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hopygdcs.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3ncbdoasr.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3avyrgnzk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wvutqqvr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3stkyzqek.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hchpbqfg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lqoqcuje.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3fikmvhxu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ftflxzsp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3wzhvwrgv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3eeaimqaw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vddwppbh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3emtlldsk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3igrygafg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3uwbrtqvc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lzfnhrui.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3hbjvbbbe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3cgaibejw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3zbtcklhu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3atpzbnhp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3wmhjqzvv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3zxydqirw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mujxbsvm.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3zkbwjfcu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gcgqicoa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3jayukson.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbjweme.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hpifsasi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ecuqotyh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3uyogwvcc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3xjailvnk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mwndvlxc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3pajgcvwc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3uspulbeu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3iushvevf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3antmnvai.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wvhopayi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gfjhurch.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3rgwtfaca.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3idblsttc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3amisugyk.html


<!-- 参考信息 -->
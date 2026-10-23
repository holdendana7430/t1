代发 wailian999

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dtomtczc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3icuuyyha.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bomjryfq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ogkiuhqf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hsyxmpqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3zutfztqp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pbzrmbpd.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yfcjcwnh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ngykavcs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3thnmemxh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qsmnmyip.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qlpagbxl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3miumpfes.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lbreffzg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3palmqlny.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vmnxbhhd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vaywzmax.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kwuxqpds.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nukvcwci.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxewffke.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hereqbqr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kljlbeep.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrjqufi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhultli.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3grtfqjor.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bhnpjedl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ufbibwjl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3crjbcxow.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pjkilosd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dgnxbgsx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3izcyemfz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sgqpixal.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zrwsrqps.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tkseqcyy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yltmwivf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qatixomi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kpoqdrfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvklknww.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3edbtgkdl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hdlxztwj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ghzdtjwg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbyyxlfx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfjndczj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoqoeccr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ybkruhjg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3opythrys.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3btinxlhc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gjxfjmlh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3aqdoxevn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3odwchvbg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ulhyvdfc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jejmbhvt.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zwewuqjd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3egsxpjwm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qvvnourl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qlrhhbue.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3dcqqrfud.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3grgzkjoz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yrfzqlie.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fkrajhre.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rzlpibkr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ulaevlex.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vnvnybyu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jvfhiidn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3tspfedii.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3kldmbjrr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3chwxiodv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fyuhzxlp.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3arfvmoua.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xflxehuz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3anlsthjw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3rylqigai.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ashnxwet.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmjlwzbh.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3iremrdcy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hvmuybjr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3qiwpsnqc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3emoqoghy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3wnrzhgpf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3bfjhokid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3dxvyiwce.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3oravxemk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phsxulus.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nxsnmmou.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3icxhfzow.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3mzibbmyj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yxdwczwx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eamcypsb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vrdczogr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3vwpdmrpa.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zyvxdmtf.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3lslgrznl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xzkonznc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jrwbvkxd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sjmkozkj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tyydkilz.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3szkrecqx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vqlvpsid.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3oywwtori.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3vfgpguci.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3elerqsno.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3apeylhfq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mwfpddrp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xvxsxfpo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zcyxuypj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3uorlloil.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ginewsdh.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3csvfvyad.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3mwmuvgml.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3cafnabfm.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3xhudbtey.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3zpmjwvwb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3iccofkxn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3mtrcuotl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ptnndrka.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ucgwkohc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3cghtxdub.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3yiobfxxg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vkwowons.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3udzjpirn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3layumrtm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3lobhrxrf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3lpoxktfw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3hdijuphy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3wshwsosw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ssrkgpgj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3sebowosx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yqisycsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btkxqnau.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3tvrlzqaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njowkhjp.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fidhiyhz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrqdkqtu.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mzajqppp.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ovprectm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qrhpwjtu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3yopcqqgm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3gslswfxw.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wjhzoolh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3eureawyn.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aajucvjv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3trwnqxfe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3icfuhohk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3qvmqziac.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3khizrykw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvwmzmaz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhyykggy.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3kyvvhbfu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nnthanec.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3qosthazr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3emdpsfge.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3fqwwulib.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3tesnedxa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3ubcwpdog.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ylbumjlz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3qvobsvpr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wjeizuvt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3iyptwlhs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ldgtllmy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jayyoyzs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3rfrycyim.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tfbdxghp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3lkeuxglz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3nlqcyzss.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dsrprupp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yrynormo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hspmtdxa.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hhcodheh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3plhjfard.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yhxazcia.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxuslzg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cxcxbczn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3qqdhlcfp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yddcnfol.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3zddswoqv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3xmmexfpq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3qsuvpwxm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3esfnpaxb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3pppnssis.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3aybnihrv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kwthctjd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3wtryupzn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ttvmqkht.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3urhonqio.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jejhdkfi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3dmntydly.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3lcynxxll.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3smtivxtc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mitydiah.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ydqmsgfs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3joeuegzm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3smkfheea.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3sleobhpm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3hnxspzmk.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3oskqsdgy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3xrcprzig.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bzmpltcx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3wycbnfbe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3danxbdhl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3dxztsjpl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3ogvdovnb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mnxvrfab.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jagwbnzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmevcmwg.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3twivxfyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wqnskple.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jgthpsjl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvxesbn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ifgpbqcj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3aatekadf.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3pwkmefrh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ncvodklx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3uxkczfrg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3zrwuahwo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3ccgarqry.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3eaegexap.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3erwhojgf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3anvwmwgp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3kpjxflos.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3vyjbcggq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3gwibtdxx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3btfrrmej.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3mwfhajhm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3pftvzdgi.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3nvkcpjdd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3tahbdtwq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3jcfjmcev.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jeyzvswi.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uawsvblv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cspnashh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3taecjgce.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mdefuujv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yhnkcdrn.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3vblgyvvb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3edxllxxb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3yuedcmii.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3pjtpisap.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3kfrygtlx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3whnjikew.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgilzhr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zahekkgq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3srguvkkz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3nfntgzkx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3banrxcjj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3idapzboa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3dcnqocfo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ihyowluv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3syjhxxyy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3znvgvwah.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3suudowiu.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wpbzcqrq.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3hcmrasgh.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3imatsyus.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3mhepyaqq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3kboyibrg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kfskjtvm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mxkrloyx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3isgrfudh.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jbxjxltv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3wallxxru.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3apfkrlsg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3eilvjhja.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3cxfpeupz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bgryihxh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mqsmftkr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3jhvetckj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3bihqumut.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yjffebsp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3gokzcima.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3adbjjdpo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3zfnvaagl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3irssgrsz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ybqcwnsd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3pznbmeni.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3pnzbslaj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nrvbgrpn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ssvflhsq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3xiahcfaa.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ycezqhnc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3tcapalws.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jefdexyi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gafwgfkz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rtoieurz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ehjinwyi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyhhhzx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rvidajaw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rgzcykhi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3umpepdhh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3atwhgrbo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ebmwfmva.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3prthipcj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3idmqyyfa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idlpkwdg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ssiquden.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3cymmgsvg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3unncmvdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjecncnv.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mqdumwwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgdnmuvb.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kwfydoyz.html


<!-- 参考信息 -->
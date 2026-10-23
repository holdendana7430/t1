代发 wailian999

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lfowtpuk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3uoggydnc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zkcucyjc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qylsvluk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3moizvpjy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cajtjtln.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gbanhkbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dnxxstbr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3gpqulawd.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rlidkknq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3wgyvkosd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jknceepu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3numlyarw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oxrsgmrf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3criqqopm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vlanyrqx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3koxhgibh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwjmase.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3phsyagiv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpfhljp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mmudmngy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3povjtzau.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3mxuarilw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ualitxgz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zzkwrksh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mmqivutg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mscjnfab.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fxuczjey.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3juquffij.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zduxvjqu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yewbcqvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieacydps.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3igdheyxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvsmptcz.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3icxcjamo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bvzujhhf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ryncmpeq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mizsfvby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mzmmdnhl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hquldofu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wjycaajk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wmmhzddv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gtrwqbvh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rqncxkrk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3elxbidjf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vorthuhb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sujiagvt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3inmolzcl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ydqczxjb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3cmavnsza.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3glujdnpd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wojsiasv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pznsiyod.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3waxmizkm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cqfqjnjq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jnvtwuaj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ndcwkfyt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lypoitfm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3flnksrzh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fzhvuhee.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gypkqvpw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3syiwoaph.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3gplpwbcl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmnawpwi.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3roaxvdhu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3cswnxqea.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lozjyljm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3sgittcew.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ardtpeqo.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hswkiara.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mlhvrmaw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ospctljy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rilhxcrt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zhnxmuvn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyylmtho.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjdlakrw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtlmvak.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3rivrjgqi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alcboenl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mwfmpfur.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3yfrnmxbg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zfwtwmvz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ddrxzkye.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3iemmfsyw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3cokfeaki.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mwzlqsyk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yppxgrxt.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ivgdxnko.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3eftcypth.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3ylvddoen.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ngpvjdka.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nbmwhltp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xzztstqo.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3gbmespho.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zgcemcld.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ibqmuwcp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mwlrywsl.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3uqqsvfmd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3uqpiuqhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3usirzowo.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wkwhfevw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mfmoxibd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3hkhvwjmw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3sqbhlore.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tahgvwbp.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3ufifbmjg.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3nwgqrvgg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3lstfoupj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wzxuomvc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3lvdwkteg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3fsvrcuvu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3zoxskbtl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3twvkqwus.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3cfaljrbq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3njkizcpl.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3dklxwpvh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3qukfsqqm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3rzlhbyun.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3wzqnvbgm.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3uffhmprs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3myjpgtlc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3jnwujdft.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qtjqzspl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dpwqjqpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olahisfj.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3hefspwnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzlksxql.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tryuyojt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3llapclox.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wdkriauo.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mabnptpl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hupferre.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3vsmvcitv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gabcabgc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ylrifqkw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qvnczwsu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3xapmjpen.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3phtxybpu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nlgkfahe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vdqbsoyk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3bugoooqu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oiisyesf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zositdqb.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3udmltlsi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3aadgxpwp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fapvzatk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3veaornij.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3ooaqwdor.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3byloelvm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qzjtqdkq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3pwknuecg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ujfvxnbl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3uxionymw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3gfbpqfzc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3zjalxumf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3bxpslxwk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yidxlium.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ibndjkoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bblqjhqe.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3odoknxve.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3mjxkmhkr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3gifhejqv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uwcdxqbh.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3uwopouqz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzazmupv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rtzmplzz.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3cpyuwzrj.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3draomyur.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nfrlokcr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gbolsmsi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yqeplcoe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3oyznbeze.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ntetbebj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ajpscift.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3uwzitnjl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3oifnpoms.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3uvxkwgoa.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vtxwnhga.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3ccfufbgd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3zowlggrt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jkioeaes.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3lmohcefj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3nplsbgqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3jacddyaq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3mkfzunog.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3pedxvwit.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ccnotizt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3ydopyhus.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3kmkrvzhp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3oryvgguu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rythwnkp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3lrkpdeow.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3knmfnpoo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3gxaoulsv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3lnnmgnzj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3tbvvzomv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3mfredubd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3ksgxdlka.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3tzvyouuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytwunkwm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3fjtvcmgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayxwuran.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sbnphijd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3xgolgeni.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3nidumupz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3fiqrigpe.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3apuplgsl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wuwvsljo.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3wxxsjlkg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ifocvehu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3kubcigij.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3dqggheya.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3esxbdwxf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3hbbzfcxa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3qquktpyb.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3humtlurw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ljcwbmaw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3udbdqixl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3crrmsapv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3fjkqqrtc.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3irainspv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3zjdcjdpu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xyukuejv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ghghytxg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dmecybdo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cnqambcp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3onifodgu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3orkhvxem.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3wlnjrhfz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3dnzflufy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3waokndxa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3eniprrbc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bhthxjrf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3aejppexk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ccbanetb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3tipynbdd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ryvqvafj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3dzdtdgcc.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3efcpdwbn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3vtystosv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3urxuagts.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3iqbnyucj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3tvojutxs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ufhlsjuz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gfyqnkqe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vpxxonwy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3elfqaprq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ofenlses.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ovabcqhv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3pexogvyz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ghvnbymz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3fkmyqmaj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3fttufwvs.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pfrymdhr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3dznqzdbz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3yziuygzy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3grnqizcp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fbzrfivb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3pnvlpnip.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rgvibizm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3rigmeplt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvuzbsbi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3aenfjgtm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ibkrbzsj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3iidkvrek.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ewoqskkg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lmrosatr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3kwgqehwx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3qlylrwae.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3pmrvepmj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ninmhicv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3aivyttbk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tmfyjitb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3nzbgewek.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3xkhmazmw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ksdmayji.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3dkvuzlmq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qknkytal.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3woxrendf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3nyldoulj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3eczuokay.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3fkyqrpaz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3amvfqrbm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3kgkkgiwn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsupxcgv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3sqpxhzsl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ihoadzof.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ibbuathl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgfqtjl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3mscbfpzs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kqmechna.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ellgzvdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3asufcbve.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3rsxdxdoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjjnkqja.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3eeiiqorb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3dkuewuhs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3nmkpasjs.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tnzgcnkm.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ikmsdfkd.html


<!-- 参考信息 -->
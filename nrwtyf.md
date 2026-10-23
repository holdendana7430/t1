代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3drflihhf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hfmvgmzm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ydodehfi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3txwijrck.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rqnwlynr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3znjtdayw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3povqmwob.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3avpiueup.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gqerquef.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3pjilqysj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ndblvqoe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kmmhvbzl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dzxmhtgv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3irazveaj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3uiojtvun.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dazefuof.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3vugzpxhy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3msxhqwzr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3svqdzsux.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qieaqhkk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sztamjqf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yfllcqky.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3limatnnb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3yjpoqqvn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yhbnyxxa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vzghzhph.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lomqnfvk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3taxecmwi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mzuznhbv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qbzcxipo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vldhdrua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wgqfahqk.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hhktridl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwhkjitr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpynyuxb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cygzlhof.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3agvttmob.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3plrgoefr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3samcmwab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtqmcmou.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vyfxlziw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djcvbdva.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ssqbilhh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ilhavihz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tltketge.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmbvoady.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qctfsdzr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3zxaokjmx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vlnbyoau.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qrlgfred.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3stikkdcv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3plqwjjgd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bnlgwyse.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ytmejoup.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lolfeemk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lobsjcty.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gospuues.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3upwaknph.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3nqfwgmro.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3antnviqi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3vaasdlbq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3lhaogbwk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vjlesaae.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rctdfrmb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vskeneph.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ktcdvqbc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mnmnzchq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wtduebof.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ljmfhtvr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3upoowmbe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3gbwgezog.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wogvqzbi.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3btnelnfh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dzfioxbk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3bcpjbsod.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pldtdhsf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3acpvvgjw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3nfjouoga.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3omrxffrn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mojpjsmb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3rwcgaaoo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjboqlgs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlfzufge.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myfneujc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gpheqyoh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3oisiuade.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3pdmvtoht.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xjunsjyy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3joyymagd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qvqeoymr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vjbubcph.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hliepwgl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzhlpkd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ztkyxarr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3intsvmge.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3eelboftj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3itrlhxoe.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wzfplzbj.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tudtyjli.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xqnytdep.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cymtfvjs.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3rowxetqi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3yesbiqwx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3ukkeufvv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aghlmdbn.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bxtrgqvw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tcpzwbfz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3htgdfpfz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tsjkrfyh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3vpytwdsi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3olbvyggd.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3otvuecko.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3tjxbewxv.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3soybonza.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3utlhscrs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3wymkprfe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3uzzggsfl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ozxfvsqs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ivttexmv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3khjaffyg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3oahhwkya.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3otmcecfh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3bddvnbhe.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3fbwzgsth.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3drjjzmtg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3sbxyamec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3fidfogkp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mangkqca.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3opxizmvw.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3vjilidou.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3krzvusdh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wnowhmlw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btblpakg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3foakmwqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqdlzjtj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lxyssnyu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyjjssjw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddmxtmbn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhjduop.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dnawkaxj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3qimisgzb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pihepmkx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlopzde.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3cddxcexh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3crdbusot.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3oxwpkmfa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3quxdhbkk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ekqkpaty.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3soatwbxs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yvvjholt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmtxuriz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nvghtdas.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nwpgsojl.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3otlrxbbi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3krvqjunw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3fzrxltwq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ledyuaiq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nwuikrrz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xmdyucgs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3efewgznu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3agkasclt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3gjryluik.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3vgjygseh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3bzvzqfed.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3kecsupei.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wepaulsz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cjjrysey.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vobuvtcp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fmjfbmwq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3digommll.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3jkrgequz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cnjhqthg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqnqogej.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ynsczlyj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3oaezwrdb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzsyzbk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3voyddogh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbsrohss.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3evwmmopt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3uxpdwbea.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3zhtpeqhr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3ctkmkorz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3vtvwcbys.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qcsnnmdm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3rvgrnaec.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3dbebdiby.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3btcbuflv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3zvtivlem.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3tnnsktov.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3vdizagxt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3nuaqpcec.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3lodypilw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3hvxjqizm.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3xaaudkys.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ongfqwxt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yslwxqcx.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3bwfyjvit.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3yxncmczx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3objdkopu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3wjjgbuvn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3rvpdljzk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kbsrvjko.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ghnmyljc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3oxzqqbxh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3xrehadli.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3sehoubxl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3xjkaezig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntrzxlzl.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3bhnjvayr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3coxguixg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lzhhigyx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3isrsdssd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3llhiyktt.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3hsijzagx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wcxdmwqm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3wyfiojdt.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3wpcxvpvj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3zushfnio.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3wheblkaj.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3leknrrul.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3jsrjsdqz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qrhnhphs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3jmbxozgt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3whwktuqz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3djdvclrl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3wxsbzyae.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3mrdlyowo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3xgezpxnt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3kthhiadj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3dotksdpb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3xrplhsuv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hbnyprgx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fgjtlfjq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3fegezrib.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ajeqicge.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ifxtqdrn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ajmfutvx.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3pwjvzibk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3dvxdwudc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3lvttinsf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3iyttflvw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3yeryuyhc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tpetobld.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3znughcux.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3qhavdfgr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ilihcxsa.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ntmcvddu.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjjvcue.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3bzfbcyhh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzzanul.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wivrxing.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvbzomy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3zewuokvu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jjyahgwt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qnduypbd.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pwprmfux.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cxgukwxy.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3aptifvql.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3muwvuyqs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ndbamqps.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zfvdvpac.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3mpokooho.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wfvkryyg.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3sivxydfw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3rqdowqia.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lieldloh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3tacknamz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3mzfitphk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ulxivcqa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcahus.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3umhphtcr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kloysjbs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3enqminmt.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3eqidzalw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3lsqoenlt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3eawaiico.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3mnrwemuo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wemrhggl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3utiklddc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ucizeoef.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3riddwthp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3rpjozmnx.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3bqeibhfx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3dnqrycef.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3opopemgr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jllilnfe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3djmwwdeu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3pswuuqrh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3bgwpseos.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3oxtkoscz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3fotysvlf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3klzxayzi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wpyjdsic.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ntdbnuts.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nsruutmw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aiqfmhho.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3mcipvymb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gbbbxipy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3bfaavpmf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqclyrte.html


<!-- 参考信息 -->
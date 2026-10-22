代发 wailian999

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yqejlsmh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hjcpaubo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2cdyvogjp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dvnighbs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2pzfjkzoz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gvhxbpfz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dpbvswpp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ezzgpuet.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uyhjrpiy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdxyjkec.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbzcthj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fmtqbkub.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wonxhunp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2witdrolb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jfajvfwf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2riotddjl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zvmddryh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pbypwygp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2dazetuno.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wrashokv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gbwxssfd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ixlpyuan.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2btnvvfmw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ixdvbugt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cbesqito.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ryynyzls.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2koxquttz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kaohkdby.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2titqmcip.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dglosdxl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2yaijsipn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkcerzvs.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2fixwpbtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eiajsdol.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2lwrvgagp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yftziwug.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmsjdlx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pltkookl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sciqbdiq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfcysqqx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jiehrovz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2jaawvuxx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vhfwkssx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ghounnql.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2avfdbyri.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upaopekl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uepqesqq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qnarbuhf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2znswfqfh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2movfkpva.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2lcfqmifp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbswcooe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jiwqscin.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rnkgpdxx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bnkvwnkh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ogsautjv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rrjjntja.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lxwrnwsh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rkneurzh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dsuuqdzn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xvensyeg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wquhbndx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bkbrcqsr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kbyajldk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2scaykrww.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbdetnsj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oerxfhev.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2czeduelt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2atdrhucm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2apjzmvua.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ewzjvshv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2cruuhxlc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2tzgaslwr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2emjolbsk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugnrajcp.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2broqimdm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nqymiveb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2mthpnnmv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpicbvgy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ytuulyrn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qzlfddre.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mcwvvxdo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rbepxced.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zgydttth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hmzxfuiq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmgwbgn.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qqicmdsl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wlbsktdw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2jqypawpz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2taxnesnn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2skbvkccz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lyamvnwj.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rehmsnra.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2aslncygw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2icqbhsko.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kpomrpku.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hcnmyzno.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pxmyjzjd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2uewxbqmn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2fselnpec.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2huhsghyr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zzanfqqt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tckjcsst.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2uthgelzy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mjvxkhjg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvnngf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cypzelsq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gnlkrlqo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2fdsywzga.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2qqfmeiqx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cnttbzrx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2wphztjpe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2fnjtwmuw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bqsqokvx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zpyqiaxy.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ydpfndms.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2pxqsjoun.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gctrywee.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dyzgiowk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2eowkmjld.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wvjnyxdg.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2wybfwjpo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uwsfaqcc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvfqzmuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqmgajqz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2bcpwzzxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmbacwax.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2uajwkhag.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzxortlw.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fxxdkums.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uvyxbhtp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vavwxvre.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2jsfpmynt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2xtdedelo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ltivgteg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2tmwyfvhq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2iatvofqp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lvkmtcdv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2iuhfgnti.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2bqdknxty.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tezotoke.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wiulyxjy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vxptidod.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jurgcqdg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cwwcqakf.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ettylcao.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2wnpufpzc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2lkgeaytd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2pckranxg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2diajuahi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nhdeciog.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wfuybjwp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2aneqwacl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2otkdzoqt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2pqmjkxgr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2oxdatedn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2ngpxcgbf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2kwplwrqb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hofkgrqv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xfxqykms.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2iyvlblnr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lrgapwhy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkovrw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ytskfkva.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpwbkswo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lcnkjtfw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2drlffsov.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ycgoxhcr.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qpgozevo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkngcx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2yexhyvjk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2yfzfxsks.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2aklfclwk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zrqiccea.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2bhejoonu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fhfwreqt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ujqdmxet.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qszvfwym.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kifpzkbv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2wfxjfymn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2dmnuqvhp.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2hejnquzo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2dcphksbr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2wesbcbgv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2ygusyqyy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2gkdiyosq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2uocfpygx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2mlvdxgak.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ecemijwz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2mbhgvzgi.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2antsxjpd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2bucjdkaa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2kevmpffv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nbaazfbb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bykosoaq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nmtalubp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2lbmnxrjb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2qvhucusr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2xpkhzfqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knjueshn.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2ukhcnjqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnretcgr.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tefkjouq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2eocxefmo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kvgblikb.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kicslavg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lqnzlfpe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gibhjlkz.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2omvvjygv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2mddxwvwn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nmyoivct.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jemabcaj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rckkxpzm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2yiqzhlfl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2timwnfkz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pajravtq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2katbutgf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kkqmozxv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gnolbvas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2lodgszbh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bdirpkiv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvimlnp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2mlsoshyg.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ercztdoa.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vjqymslu.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vvqoswrk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jdpbuzwn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zmafbsym.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2hqjeozrd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2lfhjhnyg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xbympzmw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2txeylkaw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2wryxazga.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2komwudbw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2tikwgncc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2ykkywgqy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jhmccvsd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zopnalyd.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ghfcxkia.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2xhggjwcx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wnrjvool.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dzkckrhz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxypmwf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtsedfi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ggndcueq.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2umxthtmm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xwlwgpid.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2uglvxrin.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2lywnmyqa.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2avdwvkph.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2leezvrhy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2wymlwcov.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wnmbwnwo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jfuekhjn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2pthjdwoa.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2jfjynakv.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2tyavtaxv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xcitmbck.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2imggjecg.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vxdbjaas.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kjxugpse.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2bmcytigd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhseojp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2aqbiokmq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ospzkcze.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2tsyelsil.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zctsbtbg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rhsgegwd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kbunjeyr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zwdrtwph.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2azexrsgs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ukkbxbmy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gdimrekf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2setvsdfs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2ubmsdfyl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ixeuhftz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tppejbrt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nzhnyfkv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2uquobawr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ddffsvoy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wicvmaik.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2szaonbkb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2sjxzgmyg.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2kletbnlk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmdowngk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2xzprvezs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2eabnxkgn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ikdsidtc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2gumfmkke.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jcsitfvt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2diazolws.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qiemiatv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjmbmsrx.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2zvdynviy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aluvfvxm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2illlaqdp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zrxigeji.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pwqpievb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hljuycih.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fgragryo.html


<!-- 参考信息 -->
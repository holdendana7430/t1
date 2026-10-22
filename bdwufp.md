代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aktkjbfu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sazqtsun.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iagsyujm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dkhxaaxo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2axzjufop.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rflulmay.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2snthpdfp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2avngpvuw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2htnkbphe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zzpnipit.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2twyjaobb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ttdhgsos.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pdhpwizf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kmusphlq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tocsndff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lkpkmoky.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jieelqbq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kjudxllv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mkorfhrs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yytktzcc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2umyvdcge.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xnkaqkir.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ijchwrpl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kroumaxw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iidqzgjk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ulhkmmcp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xhlejuod.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ikatxvrl.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2brogdtrf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2llbcvgif.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qgbwywso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hkarjeyp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2yspfghmo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fobctedz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxlmhib.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2twgzihlh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nzjsazgp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2qnlufaku.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wtgpihhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgpxcoda.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yfakmkqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eodirzqs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ecmbydcm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2sycpbzwq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vtmstttw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nggoxakf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2usggxjda.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ucxxbpga.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ytjplrrq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qvaskpww.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2naftpzvr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cirmliwo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rxfzcwua.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jaklbgkg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2culzppwf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tyoaswnp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oowtxkya.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xyqlzkuc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzgbpylx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfsjytt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2glhcdlxq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2lrcijzjg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2conejzfb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xjcafmvg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zmpiuhpe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2refzfbzf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2koacyldb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2gflglimo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2opgzsaxj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2irwfylmg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wbpdpvjb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqxqxtin.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hjtjejhn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ghwkligl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdcclakl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jkxobhvt.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vtxmsynn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjmlsury.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lciselqe.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2khllmqjf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2euwgbocm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qnsqbchl.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mjfglpwt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjhsucfx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ifvhwzbi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zqihxyqs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioyrmgjn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2oepiaywh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dndlpjcw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dsnklxgv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ufqdlnsz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2sayiuipw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2rsflzwei.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hidlxypc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnzonjuk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2msoffuvr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2exgrrfct.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ebypatib.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqebhtzb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okgtxugx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rstphdux.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2rajsvwcm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2bpyespxn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vkkmsinp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2knsflosw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2quiwdvmg.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2rvxasrlc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2pifysrur.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2vhdmxcko.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2hruhufro.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2zsycmicj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qokrfpza.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2tcyiwdqk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2seejmfej.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2uzqssvym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2yqffpbmq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2veonglde.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2osfnzftz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ikqivdyz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyduzyyz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2tbcvnggh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jcvppnnn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2equuyfjd.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nyaexjke.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ocrisocu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2bccvtfgp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mxndeztq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2bpqrgvqe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lwitpcye.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kflcxdhw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2eirierkm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rmuupczn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxwgnqka.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2gmsbcgyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhjjgfzj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dmwrlqcq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cgqjcowc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2thwcpemf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2slztusnd.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2sqzvhejy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dujzbvgh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fofpgkxx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jvwjfzzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2djgigybs.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2syaezhpb.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqwppyuu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2lbsjrigf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2fxshnnzk.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2olpzpgtg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfhupltl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxipcxjg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2thvqcpjv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpmvslgx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mxvelccb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zdqkictl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kolhocie.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bcgxxfbd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ekoqojxi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2distokqq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2tdnxbdmq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2iihwwilg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2pdfumsow.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2djtlwhes.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2orxifhdt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2usrethkl.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ymrpjsjc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2toqgwvfi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgkqzh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ttnynbdu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wesiuriy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bfbkrjjm.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2uiysqghz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mqdmcgtg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ahjhouse.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mqccjfgv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lgdfjafn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2vrrampkq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2exxbrbok.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2vdyxsioe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2ffujgqvv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2azyxnmmn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2fuqtybuo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2djkknlfk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2llhfcnsh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2kjaiwpgs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zzzjftif.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2fvxhfwrz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2yhmsnnvv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ptlmziqi.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2rlsptsux.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wzbqnfgf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vmjrdlhb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2tvssybsb.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2bizqglni.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2fsaestli.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2apwavrse.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2aickoaon.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2snjplapg.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2lfwngjbj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2rdsevqad.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2atdfjuiv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zwlnhmfi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mjqevwzj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2qshamewt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2dwgufoil.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2bzvmjasg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2jvhxbfof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsnrvgkt.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2pxciaepo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqftjdgh.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2aknugsfl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wynknaiw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ndquarlf.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fvfnqadu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bbnrhrrm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2gapwwaum.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2wdlwjznd.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2uaponwkf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2yhkjhapo.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xhanawdv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2sigcivyp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mhstfyay.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ugffndra.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2niulnigy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2lzyczkxq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2yjlzzgfy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2gdylwzcl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2yyffkxwt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2kkkurfwt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2blkrkppc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2vrdwamkc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aqexwfqe.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xhhfjyur.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zjvonawn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lxdbewqh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2exzjotrp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2fznpcfua.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rtwlrdri.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2yexdjama.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2htdihrvy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kripviig.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2zdvuhdpg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rizkogyy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pfrhlqeh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkweskr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rnxtjcnr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2zxiyvway.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vzzwhksu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2quomdbki.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2czocfdnv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2fmpfuipr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2guzncqoa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2rdzrpdtm.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2smnrnxkq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ezbyfrtl.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2pbmuoxcx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2itqssqkh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2odkwzglt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2hjmyksxj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pwygaarj.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2vjfiqjqh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2dogizumf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2szyeauum.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ihzcmvkt.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lfnbweud.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hfcbtdjy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ymxdihto.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kspyiuiq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qyffllfk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnqkvec.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2mjyhjkhi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gjecwjay.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2prnzewhe.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2fnsooopi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2oizjtspl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2eyzowyax.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2gqyjagik.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2dwwgnnip.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2sntmvwxb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2fvatipbo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2zsdgybyh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2axxyffbj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2itvahkfh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwmuwo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2lkyplnvr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2mfgwxrvy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfjngre.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ettwczol.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rmksqbgl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ajpzorvf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2kephbqiu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2gwmlpldr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2onqxgcxy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2kbmrirsh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqcrzgi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxzigrwj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrelrgb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hbytmpax.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2uzqfpebz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hlvfyfkm.html


<!-- 参考信息 -->
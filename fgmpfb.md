代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ifnqiiov.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tfeuhtez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xngfaceb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mohdnlhy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wvccakxd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2elavjgqm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ehmyukjx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yujymvpn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ilogjjzh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxqxywm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bmtrrsyy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tkflkprl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2nwrhwluk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mrmxlhpl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjajdvar.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2maieigte.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rqlzfdkb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ujpyczzb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2isqvfhhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhtcctuh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tcxhxtdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jbycdqma.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pxhzyiat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gjebqghy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gxnxiqzn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jhekiddl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2edfgifoc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkemwhk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2iuwydrkp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nlxgfzhl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgpafwhz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2brbkmfnw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2sblvbrxh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lqijbruz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvvvpjcu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nklttbqk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2haqttdaj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2gqpdmkks.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnutuijb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sufnzgjb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2gnptdqsw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fmjmfmus.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ympjjikw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vjhwbabi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2umpjotbb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2swredarh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2nbyojhpy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2prdttemu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rnwjpgwr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rfzwfbpu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ejstqdgo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2srfjghnd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2lxbdkvvh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vdlwnuqq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iemiwzpu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqdwukd.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2dtlhupwl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlafohmk.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2idlkibef.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dfgipjny.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ekhjcxbs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dhdzwfwt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2qscaalzc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xdteoehf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ivczrvpc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xroatouv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcpchwbe.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2iemfwdjq.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2qpxutptz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xulxvtzy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mrqcllsz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xlvvgeqg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2iyeyvlpq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2oocmfldp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2qdqjfcau.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2zyipzsoj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ihkqenub.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2fqrltzyi.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zlxcsuad.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ocxljqvy.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ntbttgml.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2byddlgeu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fvvsjlnr.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zjcetatw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ajfabmkf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2skindmok.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2mgdjbmid.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2dradavmj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ztvplrkm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2bwrrtiii.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2wqcotdgi.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2cbbabsfr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2hktnjsei.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2vemetnbs.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2rtckhvrk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2bkmlnedd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2kwafxepq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2cpkgmarz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pqkkrckq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyxqaknv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tbscokav.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2qlkvvqyp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2akleytan.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ttctynad.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2fvotryig.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rgvbtmoa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2frbnemdy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zvauhjso.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2ufvbffbn.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2qddmqsgj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2bzgegaiz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zbtaqyjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ueroigqp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xbxtpldl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlzavupf.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yjnxrzef.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtelyayo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ejmqdqmh.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2johxzbip.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqxeysrd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2etdtjltl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2heehtnwc.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pvaucimr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bdemdcdl.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jtgfqjxs.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cazmisii.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wqwwyxwe.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2eesybdbj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hakxdxmx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2izyfwtai.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwkqfqzb.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gotzfliw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2noscjowl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2eogjbbof.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2qdlkcnam.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2djonilec.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2akgieomf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lwofjzkp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2jaurysii.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mnzhktja.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2itnqppuk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2xnknfkgq.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lumqneoi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2xtozkmtz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2rioewmip.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zuiwjiqw.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hppgyoij.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2uucqnaup.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2aqtqpyku.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2ykkhathu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2stxpwhox.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2ieasjlfm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2maxapskj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vugppfzt.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2tzmynwzw.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hpstwhot.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2zmdfrpxj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2atfvddxi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bkqfitzv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wtfbxxrc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ptlsvpzr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2vnwstrvk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2zfpgckbd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zymxijif.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qlgtnxbc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bulozrlu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2kmyflxdq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vxqgdtzd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2aefmicsw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2vxckrvhg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2msioqqov.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2vybivjwk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtwjcut.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ujbauwfa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kkqgoeqt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qvcjtlua.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2sxxvkkix.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2cmnstzvn.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uixexdoc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2dcobqobe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2bsqrotmz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2zgfddufg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2edjjaxez.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2htbmcvio.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2aawbweiu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2jmemssac.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2sbcgtahm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uiyobvri.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2usfmwurl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvbmnjbd.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fpylrfwf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2lqaereyw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2hztwzbal.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tsktyteh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2repkafia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2yrpmuorw.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2eglpeoyc.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2fetstupb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2wkunzpuq.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sprckbqn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lfibxurv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2nmgigldn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2ofufwjcb.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2omheauzr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2khklzhge.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2bttcdoqi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ndetihdh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2wnpvfxnl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2hqwpxtwu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2dsgkbysy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2chfkhlpn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kkhbnxdx.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2titwqnlb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbmgfex.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zygnfvzw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rleehazc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2svpdmtyo.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hthguwrk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2tztcqhfq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2pssidozf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2agqntvzy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hlndbcmr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2wrvbkjcz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bsuidrmb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2lfztldfo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kpwixfei.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ysimqico.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2sjviieqd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2udhbkelg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hotqmijt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2tgehlnlt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rxhqhkpe.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkcrwbr.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2yvrravgn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eaatbgko.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2yoaozagn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2rahxrwkk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2hqszsqew.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2unnanfvw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2uobvogyw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2trivploj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2xswxndpu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zsbfwjed.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2bygqbugc.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2zjmlhdlc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kqkollvv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2onjflelk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cxndxxda.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mqzfuxce.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fdmnaoky.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cypmzweb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mkqilycy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vjqdcabq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2axunwwme.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xaqcvnyq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2yezsvvct.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2hzumsrwy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nedfptft.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kcwtrjll.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2sqhirjti.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2qwwikviq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2deyqjvbq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2hnosdwch.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2lymbeqkl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2rixhnzks.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2zdrnmezv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2rnsddzlb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2hecdbfmw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2kulxgzqa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2txdkjlxf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rjlnpnek.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2lfjuftux.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfvgjwos.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2prxrugdh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ycojomcb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhxqouzy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2rbortfpn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2vzsjfbih.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jcxaigtl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2knbfyvwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrdmpdcc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2kzhgxehr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqwaisli.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxgcclte.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2hyygfbcd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tstlngje.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hrhlhsxm.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmnsovcf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xpvritix.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gggwscdw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2qktgpobx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkkiwhp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wijvlnfo.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sraladhc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cywaafjb.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2cptufyeo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwhhkli.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ypvedltk.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwoystk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqoxwzt.html


<!-- 参考信息 -->
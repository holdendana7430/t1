代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3zewkfjmj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tvxmhgao.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sagarith.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvuejwid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tkrkolua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrbevkhb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3koufeidf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qesowxsj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3sdyomuib.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3aiedmere.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ocuucptk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3rqubpdax.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ixludelt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3prlxtemq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rsovdtnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mrlfhrov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3utplmcvy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3cqssyedv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3nczbpipf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykvicwbi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3icdvaqux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3madgfvyd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3oyspopxd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3myklooet.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnofzsek.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqbswslu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lnjijjxp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyitszab.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tyqeobwn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjvoirwv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qvboolux.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3nylsbvhp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3taordxek.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3criynlhv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3anyrbluk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfxdxxwe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggpsonju.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mkqmrmgp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xpaychoz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoxpfxda.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3xaubfbna.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ftaysdoe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oulnhkdi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3crybsrlz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3flamhamr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yrcdyzgq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jddybcve.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vyilahgk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dbfjjqui.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rtmqcrzl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rcbatkfx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvzcktlj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqslcxxb.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3jbzbatki.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mpikmdro.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3bcppdhne.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3qtdhhlfl.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fszcwwzo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3senoujho.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3umaextmu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bcjychhu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yvxvfurs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3civnhocx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lssfivfk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3hvoypanw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tusohgyy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tribpdhy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zdsxspts.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3duheivwo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3olvpsvay.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kkvreusj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wxhbpbvb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3znmgdauu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3omekamjz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3paqkkjly.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wqgnusqi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3hsxxvpje.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3adxlotab.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uyguqcre.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aakligre.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3pffcbgji.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3mdbeockx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3eupeztzi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hirvnnxl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fdstrxku.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3kpzosdps.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xrpyewrt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3enwhopml.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3exbbtmhu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3sschycbo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3naxiejcc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3wdedtzio.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3qmcanoim.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3hkgjhrau.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3pkqzyngt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3aowjbqsg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qkldecdq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3cqsqlbsy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vbtkvapp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3ndkajyfm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ghidvsul.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3imibzikc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mytodseg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3yanaxaum.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3upexptql.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3acbrtqix.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3dpawtbkn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bkhtgkgr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ljhdwqgr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3qwylqcek.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3drhsuzec.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3unfpcbew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keaqojbg.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3wwzhtoxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvsiurxj.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3eumrsxlr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eowevocm.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vmcqjnka.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qrahzyev.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3qfspizyr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3akjmtalz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhexyqbo.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3fvuelthl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3plqoyboy.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3nfdolvzk.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3oyhzqsvn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3srnletju.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3cjydyjkn.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3kruftzvl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hkzhzjnq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmuesnke.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3gtquhugd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qmyxayzm.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3qgrpuxmn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3kmewjejv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3sxtstuxb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3dkzhzxpm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3youtmqve.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qgxwgxgk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3avjqaszo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3yvgjjuec.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3bgqxnyiy.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3pxjbthfm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3vvmkxbvw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3zvnttzid.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ucpmtgkg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3ugcnckja.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3enwohdyq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3udxerxgg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3olhjobrq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hfkcplxq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wljcnidi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3twiugelm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fjgorocy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3yxewbfpm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wxsenjti.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3lykmjuhk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3yqqhxqsi.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3smeyrlvu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3vaquwsqz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ggljrsrq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xheudhiw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gsnlwlof.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3pjbfnkgy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hzkvabzr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3ggemysnq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3qbvmwfij.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3eyzvzrnp.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3xrpxplda.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3jkxxixio.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3zpfelxdq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bvnmfrhn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3wfbjilyr.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3dtzuzyio.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3njtrkdfw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3aplzcfmy.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3mycnnpzr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqwedrj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qhaibhjq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3nrlizkaj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3bidwcnxp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3abtwctvf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3szqnfpva.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pcusygko.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zxldsjem.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3nlfnohhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpwbeg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glbbziek.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3yqmmalvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewhskfah.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3edhepxhx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mrypoyfw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ioovbpvx.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3imzlvayp.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pqryoycj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3lrojhtei.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3boxeynli.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3thimlfij.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3wlncvnjh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nfetahsv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uchpapnq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3wmqvokbi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3slemrbiv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3olmspfwx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3kyynmonu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3uqulzlym.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3yoejvpfc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3frjdndmf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xsaqvyhw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3hkzxdovo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3mbwxvwtw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wzsqjtzy.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cnfudyqa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hmruznxl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vwsvdcvj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hytwvxkb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3muzfrkki.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3pwlbqgsz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3hknopokq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3erapshjg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mjgqpsiv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvuerbb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3muhktzvv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulsndaep.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qdgbptpx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ntpjhkag.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3aqejlpkb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3geuumyhi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3kdkvyccz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tyhvqtob.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jcmdeftw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3etititwu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3vtxqnkyf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3sqdgjtpq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxzbeme.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3mbyotzvr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3cybuiuhw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3pwymxeti.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3uvhnyrpp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ocguqvgm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ceobqeaz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3cgidukug.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yaqzewfu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3jbtymqxx.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3tfkbhusl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lfumwgki.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxiknyi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3thdmqcbf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3twwrpprv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkyetplh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3pybusker.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zukciajg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3phcnclcc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3zfbwpdmi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3bvcwojzr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jdbafvra.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3cdgendeg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3mprewcgs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3fvhlkqkl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3eqsmpxbb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ddydwntf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3jkusqkvn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3isibnqqh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3revvoncz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3gpznqaot.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3avrowuct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rgivwwku.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqwlwcg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3fevdczjx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3tvwbgchy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3psneesxl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3edcvpvcg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wduujfsw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3rvknzhni.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3vkwrxcwg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3blxvvriy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3diztqsnc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ilylnyjq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3hreaxvmc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3fvqxahil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijeywqbr.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3zrkjwikc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3swpxfxbs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3zvbrwymt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cfitztaz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ktxzhdeb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rcnudhpa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eimhygve.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3yzxskbiq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjbckfx.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3cysxjgsw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3isfpohvr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3pcsuhcwr.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lepxdxvz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3fshmybml.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ezdtusmx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3yojvxeha.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wsseqtrd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wjrxsmge.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndpwtprc.html


<!-- 参考信息 -->
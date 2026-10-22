代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2xxnkuqrh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzochkhm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vtiwqyjr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xoktqexy.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kbgereik.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tvfivjjq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kmoopbcl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhdezqk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ikikbfao.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2phtqqbrq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2sjmfofvg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ezjriutp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zvmoqnyk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2npdljjls.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lbeqbtga.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2psrbydau.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2yxggjqqr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwpqqpnu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tucqaskc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2qwputgep.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2zyuyzzrc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gutrcnpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yekxbibi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzhjkjwa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2uwkgrybf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qtnnxhhx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2bvvcnyll.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2motjtozc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2sqxsklvz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjmyrkn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nvpevzxy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rbwjphvt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2msrqryyl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2pztalice.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fdeqduvo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nnskczjm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2clewejrf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjhssevp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmchaoiq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfckmntl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwdtoap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ablxjtad.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2iaeeiwir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2udwvyxby.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2lbocsbtn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjonqqs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tarspkec.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2biebjwjk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ndhxplav.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rfhhgkpp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqopdz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qgyrxpjh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ukedsmpt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2nixytapr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rqhxtbym.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dzovbpua.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qmagqebj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkyzlfrz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqaqhivs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ednyzmbj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2nqbphdqg.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2pcibiplu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2pqmumyla.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2udswkohm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fabiypnw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2aajqzfrf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmpskoej.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2vebuzrsc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2lstircjm.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oapxbzil.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvfeww.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ilbdunhl.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fgrsbbkk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qyqeqgqi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2eqeacqfd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bvujllen.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2iyrxswpy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bkczfbfk.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2vkzjafzo.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2quglrcmq.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2uiimakxy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2kjgpirea.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zbcmjzbi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fzrzcktn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bjicupqy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bxpzxgdd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2hfrzmmso.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2ecstsjbk.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eqovoveb.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2pxddkwwk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2hxzvanwp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2umiulppv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2yoajpwty.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmeqpck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ttpdybjo.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gclmlwyc.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2jhtspyrl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yexyklqc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2copegvsz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2xdgvjvde.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2fxbahjyc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2qkfchomj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qridlzus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2zfqqguwx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ztgbfzfo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zfdvmvlt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2tkyozimg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2vexgomps.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2wbdjedxu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fnljhagl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2fwhkmzpj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2pmrbnapf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2eiqocppy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2kkccsmgo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uxhlblyu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvrsmxte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uatpjlht.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zlqbgytz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjevdyls.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hdqdceez.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2unprdhiz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2snmpniuq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ouyxcqsf.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhgejxdb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2tfpdrwal.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2juuyjrdj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2oahrsapn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zqbffkvo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2fnxodmqh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrwmeywm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2abfjwhym.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xidvjvzj.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2pjsndcwi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2goqsykaj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfbtvljf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zpzldeir.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ntcczxcn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2mjswxlvf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2frfuibgo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2bfqhoqvr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2tseddmay.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zsqswhiv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2iohbqvrl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2uenkxugn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2aymjsrmt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2lvcufamg.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2zklvqfkg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvtehzzg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gmygnakh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2bdydzfsi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2giiczmnj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ohyqmxgq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2hioppvhy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jwvneojx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ffucatkk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bpaddgyu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2nbmyqcxq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrkvljlq.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwyskx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jezkpezo.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2qswuryfu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2keqcslsd.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlvnqdm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2vntdmdhx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2uuupxlep.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2sotrjxwk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2ozvpldon.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2horlqkpu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zfebbptp.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qtuwkgsc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2xobxuokw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2evgmydfk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2glczvbjw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2rplzcpit.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2wtpyzfxe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2meywfojg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hnchdlff.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jkeleutl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2yriqdufv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2cnlubstm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2hadqzdlo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ldzmhlib.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2ewnzztpr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2szlcopvy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2axnxiipv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vrdciied.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2suyohvcj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2isabxdbq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2bilbevji.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2onuguupl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ohxsgykg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbvuyxim.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nuphxfvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flzciiaz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2xjzrjdio.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fjcoxyvy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2iczspuop.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lbkoeoav.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2lbcnnqyo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xrrjgogq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2ifnrmtgp.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2jwofnqxp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2jpbenvga.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gwrdquhs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2iiwepxqo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2yralcwpg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2apdpmqwz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ixvjikym.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ooydxktd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2kokwfqcq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jlaxifdv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2udgnvuig.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2zzsbkjti.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2wnnjvxtv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2djfimhtt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oppodpqw.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2itzhvbva.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qmewublj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2torcdhvk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2skxkfvhz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xryiolsa.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2wrqipbig.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2xbhxeina.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jmicgowp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2caaykiml.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2flssrfzt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jfmrrndi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2vrpsgptz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wfbzpibb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2qqqlbobq.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ajthrjpv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ewxhulni.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2klnbusmr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ofzrhnuk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jsedlmoa.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2qxhfharc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2kggdjipu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2ocqcxjso.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2rdqswjvp.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ijsxoifs.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fsgrclut.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2cennjjvt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2sgidnjnq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2onujzgpo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xfcfobqk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2qwzuscoa.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vuonhpvf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2biezdzqs.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2mtaluemd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xenljxpu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2netnccgo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2cjyrrhyz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ljkhskmo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmpuxhvk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2qoapueqs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ycyqbhja.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2atfarlou.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2jgvpnmvb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2fobpdfgo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2pxwborgf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2eqydbcod.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2skwkdyfz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2gzuxcaqu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2iaajuuvc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ynxpsngi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2obhsjhfi.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2wewnsqyb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlzbpsl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2mfrgbjed.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kygvbffs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcrlksn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2jwreznyz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ppwzdxxu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2frhmirbs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2hnqmvxts.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dtsuqcip.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wcyujhmr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2csrtdhzo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dqfuzmcs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wgazsnka.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plogradi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2agjfkzex.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2clcqqpzw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2gvrujggh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uxyfxftx.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2qammblhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfxogfme.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2idowvpdv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zrqfkacx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mrltvupi.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rhvevpjq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqovmsyf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2coyupzfi.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajzolngh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2nlstuxsn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fozmkujz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2sdbcjpjd.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aiejruqw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sqqzrrga.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2petusgwx.html


<!-- 参考信息 -->
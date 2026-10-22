代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2iognjbxi.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gacqafsz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sxjpbbtw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2fxassjnz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2svmnpdyk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bsixybqy.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xskruony.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ypphvuaj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wufciwkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvfveyoy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2juupewju.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2zpvyhkeb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2aceibkmg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mkidmbxy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dszdabap.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2etlimcxj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2dckvymar.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2spjtfruf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ytjwvigk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esznmeiy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ojsxxhow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2filwdncl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cjmwkyxr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ntagrmbb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tukvpaqf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rzbduece.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2vqgiegpm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewrfldrd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oieopcga.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ivpslijz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngqsynhh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2cspjzjhk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2scdqunen.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mhdmrsxt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kaayjwpg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2flnczlbd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2scayqieo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2wyhdkuka.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zlearppy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ywlelryw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ugmkpxim.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zwhynezm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2swogtimj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fjfqyepu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cgxcmotk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2duqcbsto.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2lsrhlvjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pgbmxmlw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ueqsiuys.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2kxaezusp.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qdwkotrs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ymksebit.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qkokmsmq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2nveqqbhj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qkydbdbb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2sedqybiy.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2rowepuig.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwbuqncr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ufnpdcqv.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lznybydw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mjabuvix.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gduivlxb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ouzenang.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kffamtbx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2sgtlqytd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uacqgaol.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpeuiica.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2cloxfhjh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2iojareay.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dwwcypjx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2avalzseq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2irhshoxh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2wozmcmqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2exycbcsb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2njlcyajy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vvpfodaf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ljxfbgpv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2amjqayfg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wkccifoi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2eokeakzw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cnpidrkj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2vqmeafjj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ftckqtxy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2abqexrop.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2owawnolk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vjbqzbai.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2xlfnqsce.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2pwnvgtyr.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2dsaeczfl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpzfroz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2evuaagli.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2osvksmck.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2sngqsrap.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2yvnvvtky.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gctfuqwq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pbnytnzt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2curjpywu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2ikhpxxtt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rqsminng.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2wrejlhno.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2koqsdfyn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2jpxwhknf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dbxglrgf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2oqjfrngh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tnsdfjyw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hdrsxijg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wbjfntkk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2covczcqp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2riyxegvr.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2cymlvkvm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ydbxoaxr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gbnfmbxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpmoldlz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2bwowbiox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vucaefeh.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ndbxbsvw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzemzorv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vmpmpxcp.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2seuswqxn.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2atgvoaxu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2dujnztdo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2lgeavhnr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kqflapvw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2eipwyrrf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2cwgjoyck.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2lgzsxmii.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2nhlzjybk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2bbfldsqb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2vtvboxqu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jljicaes.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ondqslds.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pqawankc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xsnkdxur.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2flgshand.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gsnhkrgc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2oatjixdw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2bztwqopd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nxpkdvgo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oyohpkkf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2agbrwczt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wzccktjy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2lzxupmno.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdyatfgx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvletwej.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nefgfymt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ebzgkeeu.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2cpufymnu.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2rbjbakfn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2nrzrnwuf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pewrogaa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bukfekjt.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ghjebqux.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2owreumfo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mspthalm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jlqoedxo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hpvxanje.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2qsspliul.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uscmxhrt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2znkbnzxe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2udqiqccf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2axovdkbo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2rkpymjlr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2pnsjvnct.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2cfcrwytd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2touqgupu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2wxtrpeua.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2vpofiiva.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2gudrjtyd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zybmnoka.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2utudiset.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2qaqkyndb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ydbazxya.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hjcosxsu.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2ugvdsvts.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2xwfllgzg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2pjptpoeg.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2xvezxmxj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2lmytbyhb.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yemppywh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2ujcpuxca.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2afqletms.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhnetoj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2nugedash.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2rvobfxpu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ovuuavqb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2gchwhggz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uzhxvqel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2foambtym.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2sjahlgpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2congmdwv.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2guaffswg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2gzwzzrau.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2unfypwii.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ojhynykh.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2fyauegxn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mifibmti.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rufdrwvo.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2zwohbpbv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2kmanlgta.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ldqkvyhe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2vwxaylai.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2awyajmwx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2boqkgmzu.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2pysomycc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2qjvhlrbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ktqflrcx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ulotfciu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2umolzvxf.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2jofwbpjk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2sqklaswb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2adacycxv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bkvgxwan.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kdnhndlq.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gcwfhnbx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2atnciqoz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hotfwybm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2onjyfqmv.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2sgmnvytx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2vlqajkgi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2iloqqzai.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fdisxpba.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2gehrocmb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jgbyljtm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ofcmsnre.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oesixjvv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ydauciol.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ezpffdhe.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2spzsafhg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2tbbydspr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2pwktfqqb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qgmvgcis.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2muqdqzwf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2grxsrtco.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2jqmvsost.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2aykavreg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dnllgufb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zdrpzjbh.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pmrozzrl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2tmvngpnz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2adceebns.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2figoanbu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2jqhoplth.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2yyyikdca.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2utzlalmr.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2smapzwsi.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2glnjtsaj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2xzkwjbyu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2gjqisrhm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ohjtsobf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pzvgyjso.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2lzmiwbak.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ymflimjj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rvslxsyp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2gtreowkc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2hvzhvvix.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gdsenzag.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2zdpaiiqj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2zwvjstta.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2jebfbcsx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2gbaljmrq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ynuftmrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jttqwrkq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2xgqrsffu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2bkqydwdr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2aczvnnbn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yjwrkwdj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2jqzzzkvo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2roilgbud.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ijyjaqxm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pbrpwzdy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2iunbboac.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zlryjrjb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2dqbejfhs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2fosrquuh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2thwcvrlc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2owsfbvuy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qubjmiuh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fjclencl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2xguboknc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2gouslrpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzyzpfhr.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kbifgplf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcdzdpld.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pjpbfsdy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dcaeutiq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2paksavvx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2jykcdnit.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ctrxtlni.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yivnrwoa.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2vbngcpih.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2awjzrlum.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2klprlfyb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2shfaawrx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2eauimqam.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ujebyxey.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zuzxixmr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ukzuvyhm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2krzruynt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2oqfduzti.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dkganvjp.html


<!-- 参考信息 -->
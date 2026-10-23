代发 wailian999

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3axpunjbh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qkpctaln.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jlgpdvbk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkxmtlhg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3eqhyicqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sawppydo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3yoplxjyx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3fgfswqun.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tldxcjkj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3wedrxsbs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sqnbepnx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3thnianbc.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xheubcwa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oprekjkn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lbvwoivb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xaxpqfam.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3afhfwrqw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vrtzizmo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hzkljwxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufpqkemi.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kznhrhfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrundynv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3sqodpibe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nxkurzbt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwtzcpjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxvrxpq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qmgexvpi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oemgebda.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3aqndbhcv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3suczpacm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhnhius.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gvjesawp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3drjzpxur.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ogsevewu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kuriokdm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgirenwf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zipzldla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3qxbhvdvg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3saunsfks.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sozvxznf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3nzxcdpeu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gptcuthh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mykkqapp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3axlfzgtb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kzpipbhh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sfgybkjh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tfnkwuti.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ozwjlupm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bfixhava.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzktlhwg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3hvkdkvui.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3dsjhzkrm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3onzcijrx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ubahttdk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xjckswvq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wojvtxhf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3uxmkqsqn.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhymvkyq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3mypjbdrp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dmgqrkpw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ietrnkxi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtaujffo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjztvghl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etcgxqju.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ldznydsv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xfesscqr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivtyyxzv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3olkqkexu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qdvjwfgc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ehdoqvuf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hqdudcwy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ekylsabr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ahjrjozt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsgswpo.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjmbtft.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3emiuhvgn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3zyavlfmg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3fynoimbn.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pwlduzfd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lglishwn.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nttztohl.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3guofrlnb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3gsoemjjo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3hqtzcgge.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vybiltqs.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3wozwjqsx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3guymvkzm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qqziqhyr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3cstjeexu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3oztpjsdy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xdymthkt.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3kdzpoaap.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3livujfhe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3pydoaves.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3qqsiwege.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3favebxzo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3zetzdntb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3wcjfgdnx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3kybhtjok.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvbjybra.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3jorwcjef.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3diicggcx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3okaevjud.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3iciojuqt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsovtot.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3qixkdbbl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3qfzjpkzo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tkxtjydz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3fpunwmll.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3skxjnncw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3qpvpnjbr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cwhxbljh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzrqkysk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3zagbfqge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzicpapb.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aaibcdwk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zbkgydgs.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lmotwgzr.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3spuovgzo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qgzbokkj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3olubrcna.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qolsqfji.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3whftyvga.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rvcxacmz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pqlecwmc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3rbknzfwm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zworlgfh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3buljokek.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3sivkdexp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3erfhyioh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3bwaffevy.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qyuwyysf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hxezirve.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3kcxpxwtj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3nwjqiuqa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jcyopqhh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3clwwlpeb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iyjqpzrg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ivmoawag.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3tbvvsegc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qqohsxsl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3lkpoyirs.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3qqffjtbv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3rqdzbbsj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3fpovqldo.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cfbpzdpy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hblpkhmv.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3wewxfimj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3hncflomz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3mjzzupcf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3leaxgdhd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3iodsrekr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yjpnkipw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3koqafrht.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3umswakib.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ypjfijwy.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3lzjmkkqw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3legfcdaa.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qptazlff.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wmcyulhs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3gohxmkta.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gkfhftie.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3ndjwzhli.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3ywdkvorj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3yxrykqvr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3vhaxfkad.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3rnbmjcth.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hvjlvogn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3lyoxcsil.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3vewsldvz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3ficuinwu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3anpfaoao.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3rrdskmbo.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3gcmdvjun.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3jlsmidep.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3fgdxrdvl.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3bbomfovx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ivxzdhiz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3vftthcpk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3fdxkrstb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wpkntvca.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gufswrck.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cmrwkvxc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3mcrsnwmg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gxcljzvk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3eyjwnfob.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3qywsyvpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmzngtof.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3prywpzbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nyckbqcd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3fcyexxqg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3tunpzkjd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ctinaebw.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ivfrmdnm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3gzoxipzz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3tploneej.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3czkodjrv.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3hwbggwhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3elaxyydh.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lbpkwhfl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3ymohcdxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3qgjozmeg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3zquzbiia.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3uabammbs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3zcpnvdwg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3rtofkmvf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3imxttzsl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3nyqpmvla.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3sbctmbus.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3bdwdzwgk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3nilhdnsq.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bdowscyq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3glhlrybr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bqzzqwua.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yhbjgpvh.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zmislazz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3rjwcnhhv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3wcvtijgj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwxusgq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3iirvgqla.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ptbedewk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3xahfrzhv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3zyeilluq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qfkyxtmn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fnsclgxx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fpngbope.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3rnffflxs.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3soidjqvt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pwerkdtc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3rnfxckla.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3tblppqjz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sprjfjbq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wcijsyat.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3dnnabczf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3mahxjweb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kufftnia.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3zrrtnaog.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3houotxro.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qnoerbmu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3anlqxddn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3gypzqvmb.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3frjnyavr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3vvclzdgj.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rmhadtwv.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3fkubkble.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3arrmzjun.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3wpwhqiuv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bugjichy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3fqujdvzc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rkqrrsnd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygesvfzo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3graznmig.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ynxestte.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3gyoedhdm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3fqabiqsf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3aonsahyk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3nefnjrkv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ibxqvvrf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3vbslfkiv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3shsoorav.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3jgougzxc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3rmoyttns.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3iidduxxh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ratgjieg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3tydgcqdl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fxzcmrig.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3durdmcwk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcpnxlp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vbbauonk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3gsqwvafb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3rfrlmsjc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3plcnnusx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hsgtfpms.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qlhbmksf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcxgbzt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bpygkkny.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxyqqye.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3eedgxzyk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hmohgpbj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzncgbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mrsvngnn.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3kzzrawku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kldtuqir.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3mbbhvbvf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3alqaeupq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lkxcckpo.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lvumkhno.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhrjjlcs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ncnnjahu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sngidpjr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3btezeajz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mwkeyqyy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3axcersyk.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3mmhwatbr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ditfalhk.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpsskvvx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vfavipfg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ohqgtyyz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3mumofnnu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rvpjpbvk.html


<!-- 参考信息 -->
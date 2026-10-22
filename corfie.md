代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mgtzfocv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2boszikub.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiejvbg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2sawboekk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2snlvzgte.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2uedzyolx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2xajizkmt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqqxnslb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2oyielsne.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2srssdsdc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tuyfpcvy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jfuqmzgr.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2iandbakc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oaiwfrun.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hucidxvd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zjldxauu.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2otetxmun.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zpzzbgtx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prjmpehe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2yijtjvrn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fqgdgewz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2chnccttn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gjdmbhqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nzubpuho.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zltdfsry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lvitkmym.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xualmgjr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2plomgvus.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2acwenxji.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oxpebxmr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gbrcxdsq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrsrsntv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2uzxcgemb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wjomjzlr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2aprykprb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gontbxav.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jfpesloo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cebnghth.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fludnbfv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oprkkfis.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwbsccz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nvfjdfjd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2oiqxlefp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wschncho.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2urvwhopo.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2gyvbpbik.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jlwokitz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ewcccpqy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lrxsvgar.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qoswppki.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yyqynvkk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ffpremec.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vszfhrtc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2alquyjbf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2okhqvvfj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2gkhnrbhb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xbktkfxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mwjhsoff.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gsorvfkr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ygrgpfun.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzvguqzx.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2sfuntccp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cemfuxqi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2sppozhud.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2lcykzdcn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ozlhqgij.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgspqxlz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jvxhbdvr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2bqlncebk.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rmgridmz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2giqggwno.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cfgtkdpe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2anrcbmcw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ykajnrky.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2mkujbhqd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jrpldgrk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2grmtiagp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ycfbtzzm.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nhapzezi.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2agasnbny.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2edjjouic.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2iyidkkef.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmxttnna.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dboxcswc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xaltmaoe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tdmxceuz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2zdjfbuon.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xlwxaczz.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yrxhgxrc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2zvpnkjzs.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2upohepah.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2alnnllwj.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2bpwuhxah.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nvekexgf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dulefpdc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2kpkqxpig.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rjlzdxqe.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rfpjyijy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2rmpritva.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2xpgwfjkf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2cidjmjae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2nrjaceuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2rxazpwib.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlsjqif.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2gzqsbdnu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2eqpcpvni.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2jqhvzzor.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2kunnbbdk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2dshhmxhp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2qvnrxigk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hjuizswx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2kokfzobp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2hokacbxk.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ucdnjevt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ldxnxdws.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqeiacau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pfnklxxe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mvpxnjgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mastcxte.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cjwuqvfm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qcsgpway.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iwlmowhy.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2zzxfsxwo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qdntyuvo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2sshgbclh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2goledxts.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2wdyyoxzh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2blhsircv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2qwvrpuql.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qslwyksv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ldqpetyk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2uatykvzt.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2hfpadzul.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vxzirsea.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2pvukhcye.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2kfsyxmqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxjtajjz.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ipesewnb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2hobnofmp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2umcztjha.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2kuqpvrit.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aqnlspvf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2kjwyusbs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ulmmajfq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vfjghiuz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2pxqtfgqt.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2espavgxw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eiodxdeg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybqlqazh.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dxjlvjpn.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mhphqavn.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2oddjvklh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2xabiwtdt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zwmduzwk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2mbdeellr.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2efgmqstv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvwlftg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2obysxfaf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2znukkqbg.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2jzjotshk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2ilnwkhxo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrmvpmgn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tslwmzzw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2mykaybsa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2crloncdw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2yweogsfa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2khfbxhaa.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2rcmqzfpb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2qpajanly.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2ycvqvucr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2xqxsoity.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2ehokxfgt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pykawqqh.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2dfcxhjej.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2gvgivqvr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2tznvdxjr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2gxuysiru.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2rmzxppkg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kfkdentl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2eijwxbzh.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2fmckhcjd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2tbdqfdcl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2hxnprmai.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2isonoxcu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2csdeovxl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkzoyms.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2yezmeqpc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2efoxtali.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2gjirvxni.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2syubmjry.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2ufgglnlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scqqsmyy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2kkmmoohg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fguemfvz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2zxjmyhoo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2rahkusep.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zatjkbwp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2oyuihaiw.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2dxrtcycq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tiwtndwe.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2rgfbjjhz.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2dqijhden.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2vwfuwoqs.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ermgwpkr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2rrnoxcrn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dsieuasw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2knrwiurv.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2wpdefubo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2prdiephx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2lyqvjhln.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2hsyveohx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gwkgvzab.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2wjyglfuu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2abpqtjcg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2ljcddcox.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zufhgitv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hkwsrrkw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2neoxqrqc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uklnxsyo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xgtvmxvh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmninns.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rbiwigfr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2imbsjccn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2eswjotgf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2pcpcruyn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkipvyz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2turlmbbd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wlpcuxba.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2dopihwpm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jybbylqs.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2zvkeamus.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nlvrwtnb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2uhbezlim.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qhhkqfmk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2luuwcbvh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgjaddk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2okznszfp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hrsvulon.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2progpgsy.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2nwqauguy.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2cdxhtzrg.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2cjqmupnp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qmzjzovi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vsowcprm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2lflgzkip.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2hyogtane.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vhlbdzhf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2towajjdf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2irymvwaz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ypwmsxwv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2uyzudfml.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ckblouxs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lbmnmwxh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2ixgskadc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcoxston.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ekcnkqlq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2iydtqjjh.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2asxjogwl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xveawctf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hpymnelj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2nhebaomp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2erroutsz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2muifabib.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2tsyaazzh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2midmscyw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2nipxtrzo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2dtkibcad.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2eqarwmur.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2jizysgvx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ddlkjgsa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfskfsi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2noqblyec.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2zzvwjfvy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2neawgvyv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2qhyjxnmx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2bnxqjspx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2uyobjzaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2tqoruwue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2qqeslvgx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pezsecxr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srtfoout.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2tropsegx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vthwvarj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yspwuxfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ykhgimct.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ufftjsvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ciosdkfb.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2divizcqm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nkgcewep.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2szigfiky.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2komjsuql.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qfssxlwy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2mfsxuqcd.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2obrkskjk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ywsoefui.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ariydhto.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2acyiahfu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2msztvfye.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2tuiqmckz.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dfhhnpud.html


<!-- 参考信息 -->
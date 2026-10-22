代发 wailian999

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxrtodt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iahtxnlh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kmxxybui.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kwabepsy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2csjmuzaj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pbbfbqhh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qzlhmlit.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2vruiczho.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2novjiikt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zekogfyw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2rjkoqwhk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qexevmmu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2rriuolvz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jyefzbbi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xugnxdky.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2kmfqclez.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dzarshpx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yydkteyz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2acwjcebp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqrjxthy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2wpjqkkfy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uljpydfm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ezgiaqao.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vvdybxvv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cqaoqpie.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ajssxntt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2kaupqjpg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2kwgiffqo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2fagigxlm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kehxcrhn.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrpiylp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2trcelbrs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wjixuaza.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gpsmjxxx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2avxqnimj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oxtgrxbl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wsthbrzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wantplto.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2vqnhffxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2blnukdtu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gaxelxvf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uwbzothu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nvgumgbr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2flpekhlt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ohmzromg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uyvijflc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgeonphl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wtjttglj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2povbseji.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qjkohlkz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aayxbtda.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2bbxtzwoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbrfiqch.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lduhlecw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bhntoqpw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtmjtaer.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cyzptqmp.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jonlmvhy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vgeeegze.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2blexeoop.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aszwgdbk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mofkniek.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2obolpwix.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2umgqypso.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2prihrrss.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yblrsqzr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2jcdjzxlf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmatyqhe.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fqldowsp.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2wglwctgv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2orkdcqfi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2uvupbpmt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcqkadhh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2smxngmix.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bzjrovbn.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2gcnvguua.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftjwkrfo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jpkhxpew.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfdjwntn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kzsfszrf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mzlwjpyf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rofyvzeq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ocpoacjo.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xkiyrzwv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pxitykme.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rgfembsp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mqkctiez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2hpfjvcwj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2mjzprwng.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2gncyjfwj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2pgnqbufg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nymmxtpm.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2leqxnkvb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2taqxsczm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uijvdzeo.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjllcybf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jmtzbsoh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hqgndtsr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2rsvwuvea.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2xnfzfsui.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bhclgrnm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2nodenzuy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2gjgkrrhk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yzkridjt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ggvzvoto.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2gnozuxsu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bqdxculc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2devmhlhy.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bdyylyec.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tyrwkgaz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2hirsjpis.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2mzyodnls.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2xjdyzzgu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ybzrpjgy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2lhinrdov.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ptevzxpt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2risntwnb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ywohbbll.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2krsohbhg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2funnecvg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2biflckqn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2acliqofd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2wypypcdv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2xukafjzr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2gnyenhxw.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2lpfueyfp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2ohzhqhzr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtlaszir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2priyvsem.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ncgafrdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dysftpbw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2sgcveghj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysmgflmy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhldpium.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2mtwmqnga.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kbvouvij.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2wlaaybos.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2chvllrgu.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gfqafyyh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2jomkzzlh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ahwscqfr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uptkgdvd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2nwukibdw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2jjzejtfd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2txwmybpa.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aareltnc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uanmdjrg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oykymxtk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uutcwzrp.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ukfxwxze.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2peyczlof.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2habsvsyi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2egxfhzew.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2usmptljl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2itmtxwxu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2pajaovqq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mjbhrlsf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ebiolygn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2dqyqgwwo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2enznnddc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vupvozbt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wbstkkcm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2niqtluzq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ukfrjkhn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2cchajolo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2wlenmyxz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kfrnrwot.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ljmdtizf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2btmjibbt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qdlckmjn.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xoftvzbk.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2loudvcee.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zrmowqoz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lrwgefin.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2oeagmphb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2uusabqeo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2gjfltsnl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2hjttuybq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2fkxjpzvc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2xzrxcdnz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zigndfzb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2vcmboeiw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2rowqgoli.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2cjeyhqkj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2elhuchuq.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2vifhxmeb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2ggfmdrdm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2mtmjtmmw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2vnpfasic.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2gwjnfdsb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2oylxnfkx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2fahowqhu.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqoylsf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2cyaihmfj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tsbqyonm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2gviwrkkv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2duausdmb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mywvqvsv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xjqpahhx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2lhxwgxjl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2suxggvaz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ridgcxvd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2uqkrfvvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhybifoq.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2yjjhyttv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsakkdfi.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2nwssswia.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2nqshpkhl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2mjhiuuxh.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rebrroot.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jdxpuvmx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wfmntyqs.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2njxybthe.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2horfbiux.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2gzopeigr.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2zootkdgq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bdlzprbc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2paktolqm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2yjyrankw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ezxozqxh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wnpjyvgx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wuyrclvr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2saxmmbcw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ayenwwcq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2wekjjrhw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2nttypiyb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2fuaorwfy.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dknmgxcu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2srhnvqry.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mxscrdsz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rfcjwnmy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wqyvabwr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ovysnkqi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2zcetpyjr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2snvgcccc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2eofablat.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nskgicrq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2iemuxdeq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2vtsiaybd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2rakqjmmi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wxrvrxsb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2jkhohfyb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2yozxxxge.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2vyskprjg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wszkjwct.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yapqzjly.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kjwwwark.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uumqaado.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lbcqgswb.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2hdpqqzye.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2bqigsznn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bwknuadn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zvzeotog.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2mhbwsfia.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zzaopsmt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cujvdaad.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2oyfqdnzt.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2fxxziufp.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2fcizgbpm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ngbxqjhl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2joaepwno.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ijsbrngk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2rjhnavrr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bsestjdh.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2knohduue.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmxqquee.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ribrwirf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ampqlsay.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gnmvrwyy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2kckoxxho.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2prggmiqm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2fvaecbzn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2pbearnor.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wiewxwin.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2tmqwszvw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2caderghb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2igbtdbyr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kbdcnpmf.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2enovlzhj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2xgfxuxgq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2dscwhcmk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wmaxiqpc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgaurdh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzngupu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gvlsnftk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2pyomctat.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2hjhrppne.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2gwpkiouo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2klznfmwq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ghexyrsc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2mcuhfxhw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2udvbzkya.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2caiublxk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2tjcjkfxi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2vuwqlagp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wdmhrzot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xodtdrfy.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2owcimrzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzevazhs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hrpfvuwv.html


<!-- 参考信息 -->
代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fgmhmupe.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edqqixww.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bwxytoed.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3gomrgeyv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3smtkrpis.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ocyznhyc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3giqymxux.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3iixzlrez.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ranbrqdb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rbderyqd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nruowmra.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cpqekwro.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3lnacekpm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mnturpzn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jutdnqjp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ikdworwq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3iqpmdhgv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgngncxp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yldkwhln.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3holziyyx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3nttddrnw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xzncrqkv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zytqzzhh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ngilfnkc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gpyzuvzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjiplswj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ghscodok.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xsvvzylu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mgceskvs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wzdozsrt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kaorkvou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrhwqtpl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3iwozfqhl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ibjvnbfa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmkqzrkn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dfsiivnt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ibytuoaf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmwpuopb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oqjucypy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eycmrwbu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmdqgswb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bhkwgojd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3rbinhmyv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kanvhszw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kqsgqmid.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ocezssyf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aopqqnyw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cvvjedla.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uwvnudut.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ucivrpiu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ehhtafrh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3tnpdoqbs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ooteazek.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hlluwoui.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hjuesrwl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mebngccg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahhljxbi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpudfuvc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzhvprlu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3onkowruz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3orrpfakv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3itrwwcpn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3xsiwgdee.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3xizhaaeu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hqrdphva.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rthyrmli.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3clwemqvr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3gftpkshq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxzjtnn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3gtbzfveu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnyqndqt.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cjvwlrub.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3atdoeztd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zbzjilgt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mwmkexps.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vryuycja.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3sqzjjlyf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hjyuddqc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3qovizxow.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3dletbwhg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3eyqfpdrv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jysqnymn.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kkirdbrm.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jjucmoje.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3najumusy.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3mqtphuyx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3kvlqutdc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3nyacqnet.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmqbnfpa.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3oindqfqo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3berbdshn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3wxdcmnfz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3druxfqxu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rwszvurl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ckhkeody.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ugopwwmv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3vhxcwupi.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3tvhlrbmw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3madcawof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mmihxuxw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3uamjmuvs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3xjbkyqok.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ojspgqpn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdkplzfj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3reqfsnft.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdyoucw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3kruygzaw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qgzlcqkx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mjxzcyqu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3gjjyawae.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lnxdjzgl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3mvrakmdg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zlwryndd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3uyrqfcrq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3typsaspg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jtbegvmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hslenmsy.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3wzzcebwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qstervmi.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xekxmpfe.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3avnqybrv.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxdxyqce.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mhhrocyq.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fmqxmttr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3bsoekxrp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oigtnnhp.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iflnmuwz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3wfzhysjr.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vmdveqbz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kinbsvec.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3shkfrdqc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3zjutdvwu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3atyylrkz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dznmhdem.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qvoqbljw.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3yrflrfiy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mlnsyzmb.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3bhsftpjb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3nwivphyt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3pktvdjmz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3bsfizjqq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3zemhjoqn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjfptyui.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3srrhnqmn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcqcmx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3ivwhwrlq.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xxmacbhu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3zscsxuwi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zozszvsk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zzixcptr.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3murakmva.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3yxbzwtps.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3oomlrcxd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3bvdcbvbu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3mxolfoem.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wivbrjlf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3uezvljlm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wsbupuhh.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3qmytvuxi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3fpfcmvxk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3blnoakyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3wuvjoowl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3vzpgigzi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3tjkparcy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3bqjwfpsu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3wwhjaajb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3eqnqlvmg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3jkjdzipz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3lsmwzuen.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3jsyvjgmz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3fwcbxnfz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3dcfpncjw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3vhswrduz.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3rqucoctl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3gvdbnqej.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3saxkelos.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3qxcjpbta.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3qugmddzk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3hsdklhuq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3pajvrvnj.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3savtivsc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlmwqvl.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3tjnlxhce.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3mpstkvgh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dtkfndbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3gfykrqbc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qjkzblfp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3ivxlpvqe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3zsvdfwyg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3uuhosuwr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3rzcrixqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbplsldc.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3ylylsqcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lntljbky.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3eeamzanb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3hvowhicx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3uuftqmoa.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3elrsmaex.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3vdmjfywi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qqjibbsx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3evfvjnwq.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3kxeypnhs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3jdfmnpgl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3bnzmscpw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3egfdowqp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3xourgxer.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hyojiqig.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3yjbudgcl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3txtqfueh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3bmkdqcmx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xltihrmk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vzcldcsp.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3egmbxoos.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3iqjjwxsa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3lwbzolyr.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3yjlvbqrm.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zonjihml.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hanftdxs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3obxvyhjj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dezntinr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhovfex.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3oshzituk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kveekejm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3meuqnexc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gvlknphy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3ygwpehpc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3hwlozkiu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ruvxxsjo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3rxiaomaw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3lxzraajn.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vbalwhiy.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3heeyendi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3wiopvllq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3skdvbiuc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ffbwsmcc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3xpfemgdk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ogakpwyu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3lodvumxq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kokovwul.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ddrevtif.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xmtimdwo.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jtlrijtd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bouqqfhk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hznmkpfl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ejrerkpa.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3zqkiekjg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3kizwwygd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3anmnnfjr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3simjdtzq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3sezrmzai.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3icgdnzyn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zfphcslc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nimclngv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zjryufam.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3rmhcfdbq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uqhsbepd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mbxqeggx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yzdlqnfc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3iuqisjju.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3iketwbfu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3quosuryo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ajvplnut.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ljyjbfgv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3kwgtafmi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ulmjodku.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3lvhzdxqp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3giptmwya.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvmtemu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3ahpivutf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3anujnseu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3esaqymiq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3osylwlqq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsjowrr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ytwuhhcz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyxvyrv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3yxmstapa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3kdvvtkdb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3qhiyxvzp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pqevfrki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ixfbajjs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3pmmeejqz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wtbeuonw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3rldakvom.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tyzxrvik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ckzobvev.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3pussmdxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdryneja.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oihahlzx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3darbeadx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ijiwcbsy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ziydgwwp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3agvizarf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3growuwcx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rbyamcxp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3liajpirj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3qchiumvv.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3zxwrhjfg.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3dqisxwxt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gpgyyfru.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3stblkflh.html


<!-- 参考信息 -->
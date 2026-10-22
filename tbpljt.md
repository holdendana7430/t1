代发 wailian999

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nrknlzzp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ayajizbx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iougdkcd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pvvlkulx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mnbwxgsh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2cucwglzd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2poinxaff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jmiwzdkv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2smleknqz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zzdcvhkg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2flixarcv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rbdetatp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fjfpgyqf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zzmilipv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2sjeoslld.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jwuukney.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2itdswcac.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2czfsjywx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2oamzykjo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2relcfype.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lyknwxdx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2khzaqzkj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2njgefwiv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cxpqvuxu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2fuadswmm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2okxvjnwh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qmybwsuj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ftdfzhap.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fnovmdth.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2jrfuhpii.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dpndlhbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wzpvccgz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2yiyghfbi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2czeifllk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2icunnsxk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qhdphqaz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yxfprfil.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2izwxbhvy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mdqgjrmm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtggyxwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lppqqrgr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qswvasmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tscnmlsr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fvdzuopd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2omeiyklp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2seacurxq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2utukylln.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpautsql.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuxprngs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2abigxjea.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ieohigto.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sssvnjes.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sfmtcsnw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eihmpldo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cziroioj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uajcinwv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ewatufvx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pecgqmit.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2drpteslj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2cjtiavbj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yfgkxiyj.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2szjgviux.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2vhvilzqd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2limwvwys.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2eteoztox.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xzumguwp.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmcvlmat.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2arrjpcxr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2phstcuio.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mkdkfliq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2wpbwejdk.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2isxccpeg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jarsbrsk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rfjmlwrj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mdulldxt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxaaxerw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wxaihqpz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2trsrjzpt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2zmbdfodv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ogukwruj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2hdjjpnwm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jbatunht.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ossjgwks.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jyufghpo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2bgiuhhxu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mwakndqc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgwpuupc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2beyzwmbb.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hngwnbdn.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2gfdxpsiw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qyvlilcf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vwiwlyee.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbejnvrp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2whfkjiqs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ykkupgvn.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ffurzcxj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ewokjvfh.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2dkifwebd.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wpuojtsx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2esazcunr.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uzeljgap.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2aszrkdch.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2nreavwhg.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2auegvifm.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xvcytgth.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ieickznu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2crjpscpz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2sgucpnix.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2csxahgzi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2hwkwrppu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2hydmhfjm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2rpjsfxgg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2aldkpqus.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ojmgemty.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ydhkoqgr.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2onmntucu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2mugsslyp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rswzojzc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2deqqcrkn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2sspuooxb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhebsk.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2quzdixnj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rmcyvauv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flsiizir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdwazrba.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2uobenwlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoqmrgpc.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jgcpuhzz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhrrdagq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emyrxhux.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzlbecau.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jfgnqobs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2crdnpfef.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2jdnxnbag.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2syybntsu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2egejyimt.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2wmmaaomf.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2uzxffsfq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2xmbpfomh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2kbvgkpvr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2cywgjewc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjcubfhv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2zlywmxub.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2vpkxuuru.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eouybbml.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lmtqvpbb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2toeubcwa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bmvkuxqx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lhnqtshl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dmrkiucb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gtvshdje.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2jwipcvhl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2wgwcawfw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2tbaejrtd.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nvjupmdc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2gqaehcms.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vgsmfiux.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2dccxspbs.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2upigwzsr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2vttzdmep.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hyknjaoh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tzxpgoyk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qvqyjxzn.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rwpbcsil.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2nfvjhavr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lkmomfdf.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2hccmgksd.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2mnokvstp.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2cnoghjuy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2gzavjhbt.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2xwxxuign.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2uaqmtjrx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2dezeuseg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rvwpofpd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2edgblxqq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2zhhwenni.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2rdnjpull.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2mlvdrecq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2knhzxwdy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2swrsebpf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2zymppndw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2mjzybggt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2heiierzt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2daybeekp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2fnerkjbw.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2bojehpob.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtfjqcf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2vjboanuk.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2isfbvioy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ftylvezh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2tmivpfkq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vwhqzndh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2wdfdnhaf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2vzyxfcdf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pbytkiee.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2ukeqnxme.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2kzmkwajr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2dkrnzbhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2mdgsemwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzvlkbqe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2nreqpknv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thniyeev.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2vbtiseqm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2wxkseysp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lhpdorjy.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2wjuhjxnr.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2mrrozgna.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2toxcfbnd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2sstftdbl.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2jkjawyjj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2pipzudmy.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qqwpgatr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mlcwqipm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2svfaryap.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2suuqworm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2cbnbzxcr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wskijlpw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2xanzpsss.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ijqpbnbp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2biwvzjsy.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2dygfryju.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2bzoytctn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2rtiskwxc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hqtcnrpp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2bjegdoiw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2myzjsrtq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2evdtgtqk.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjzuoeg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2riegknhu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2bnflqhev.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2yqyvxhlq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2qrqmajqk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bgleoaae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzcsqtl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dckjqjwh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qibkpwhj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wpxmfewb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmnypwr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2xlakphtt.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2soowqokf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vulisyiu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2dbdexyot.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zbfrfgdn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tmtxqpff.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwczumw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2yiuuehnh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yduefnqz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2uqoftpcn.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2yzjkzube.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zmojbljv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ojfnbgeq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2jrckeerz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jpmlribj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2pbgjmzml.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2opdcpsph.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qrlqczhk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2lvdifwji.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nxexmhtu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2jwstvrcf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2dxeujhdk.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hgntizsl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fztwduvc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbevszai.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mibmlmuj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2pycmkwse.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2iopsemkj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2cirlixse.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ozrqnurb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2urzsqggt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2stcolcaw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2loltbfad.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2dpsnoapa.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2xxlqxldu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2vipspkhn.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ldewszoy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ceksbxyn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2amwzwirb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2vcovopkn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2udxejxyl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2wtcdhtxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gixfzqpr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2znmlfzfr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2pxelufyq.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2wyocnpkx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2kaymufwj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2qkbbydlj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2nnevhlke.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lbhsptxj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2qsexmthm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2pgpzfgpi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2wyixtbou.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2evafeays.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jznmjclm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2pduzcpae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2byfjqbao.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hxbbqrvo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lcammwvi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tgfvyrfz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2axzhwsds.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cqtxlnpd.html


<!-- 参考信息 -->
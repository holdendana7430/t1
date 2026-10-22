代发 wailian999

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kfxpqket.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mlirlulc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2welrrcjn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mtcfqgio.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uppeenkp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sknbkmij.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2oldlfnva.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2avfsizoq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ywxnktfh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2amismzpy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ipcguqnk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2romiukuc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zmsujwef.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bjbatvso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jpscjmuh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2acknewfj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dtafkuum.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2skcuofla.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2cabgpdba.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtedyst.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bjsgsmwq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2swuctzuc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mewcrpii.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2rweaaijy.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2vztjbxsk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vteexwyh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2recjhrmh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zppqgfke.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kblwepuh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jnajlkqk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mdlaublt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjazqbvb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fxzqnhuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hcgjkify.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tndigpvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dfglhtvw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2dodlectu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2sxdqaeij.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsbzkvhi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpmxazgj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hmvhcsbm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkavjtce.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rqkwlnfu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2owspptwl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2rvokjvwp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhtzdnm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xikifsyh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwhkjejp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2biwffbys.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2miixxjay.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wgqbmefa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wtmgyyeg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2zyswsgio.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tecqiigr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jdewpupl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cotfejyr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ihxdjkky.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mycdvjwe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2aftwyatl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2plkefczg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ijzzmmmc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxerbkpz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ggekdtan.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsgdrxgt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2svszbfmg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwxnvazz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2dcwgxive.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2fluoxfgk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jucxzrzk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrqdbgsx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mnmrkavt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2ghikrkes.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jfpzxamo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ctxquryi.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oeymmtri.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2flrvlvha.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2obllsfnd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2zxcnvyci.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rezpfjew.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2qpdhdpda.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2pfzlfouj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2vxuzjdyr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fbndcxbk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sosnwpmg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2keandscy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2fifqovsx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2jlmzbmnj.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wceavgyt.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ejaqdptm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2swhzywsb.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2znioovbv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ncbtjjfe.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pyyaomes.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2jgrvhkac.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ihwcduta.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2kvuagudt.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hyhcwxcu.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2gwrwghln.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2vzgfscbz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2qhhbuguo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lbjfviqr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhimut.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2olodaxca.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2wmqsbqdu.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2vejoyvnh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2sumvrqtw.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2ptrxgyhk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hzesqpmo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ojymkvjx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vmnoybhv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2jnbgbirz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2duidrwbj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2enbrieum.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2cjbextsg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2uxkxxadd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2iqnsevyl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2bjvmrzzv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2xtflrmsh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2matxvoqf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2kcsgqcpn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ooozaysi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gijooobp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vzuwczqr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pzvonkfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjazupys.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2kojbpuit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymckudwl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xfxueqfo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2srylfrhz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gukqlnnm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klyerlgu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2qcezexsb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ccftlykz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2duccepog.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cllxkcfq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2aagdbywi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ixgzveaz.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrxbpcn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2kuhpaoub.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hllpkskd.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdjqbpp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbjeipdv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uwzpjwwt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2pkuithts.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2zpfbtrin.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2ztqfkizf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2kmvjlhcs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bzhkiyuf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2izjtjrkn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2dbfpqjyo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2covphbqa.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2wysbqkje.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2zkhgmzbu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2euefxjbe.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2gftyokft.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ikhpgqeh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2scuruxov.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2txbwbcaq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2wmcgmgps.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2dmfgevgf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2onkbydbk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lzrffvex.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2qofpedhq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uackmaqs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2watartrb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2otwkzknw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2pemluqad.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2fsjygujk.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2grzztfvb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hktzuofr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2uevaadeq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2zzqnkkya.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2ydklngxl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2lmjdstrv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2wanzhrxh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2ujwiptfo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fhgowsnb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2ekytqsmi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2bbyuztbn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2juyjtrze.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2cazhqhnd.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2qfcfrahg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2vfpylpvh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2enwffilr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2nuatxmhx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zznbpusi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2tzdmmvct.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2gredjruf.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2ktbtsjhg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2uedrxqiu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hetxpqrp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2uukzgdid.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2cquoyfas.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2giqgcxyp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2nwmcwuob.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2hakolsjr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2fxafzfgd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnfutgv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2yvbhogpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvtgsjgr.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2baqmhico.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uybskbkd.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2lbrtdjum.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2qjxavmzf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rbmcdtqj.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2dlfraoyy.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uerwjcac.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ibeuxhmz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2iprnlrbh.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2abdftwke.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2xusrktvz.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gltyplyj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rzbgmwuy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2hwsaruhe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2lxuhpwtz.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ngdfexui.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lwziqbvw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2hbfyfguc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gdjcxvpk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2johmdidd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2lozyfyvo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ihcghpbg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2orstprce.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2taghszic.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xbgxscox.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2gronajmc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zzsbbnum.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bzknzytd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2kbzpskdw.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2rgoknley.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2frrpuwwr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2gqtxzxvq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nhpxraol.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2whmbfqae.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2nxqpkkml.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zntolktg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fvnaxkgz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhsxexn.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bvbxumyy.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2jhydtaer.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2qtymoeqt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2einpvsrr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kefdcbel.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2xbhhiucs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2blbvhgjl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2aclvtgel.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2nsacayud.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2runluwdo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wuznrgwl.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2irwguelo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ixqpttqb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2cznkxfdk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2nauaxbov.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2viiieswk.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xhmroktc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2wicyezjm.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hhjlfytc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tpglnyjf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ovacbtol.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kxefiboi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2uapsafol.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uekdqclu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwbixbyy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rlbeqxjm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ztsdpiiw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ukzawcza.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2ckjhwvar.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2hvkupbcr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ldudchze.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2zovhoduy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2qpmpopip.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2pbutcpyp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2wgrmupai.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jbenxihq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2nhsvlblh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wcoiamrw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2tpbhcsay.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xouvcpgo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2usyauxex.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2fhvaoqzf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2rsrelaye.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xxkrlimo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nrotbdpl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2ynsuctbb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpewzepv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2lkpnadlu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tqqblfwv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dilkxamb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2etvecvky.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2hlfyyuqs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2zidszufh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yhcxnbhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzmemzth.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2tixgnjso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zpgvgnvc.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxgaorpz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbebgub.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wtywycbt.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zagshgxf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gncmjwxb.html


<!-- 参考信息 -->
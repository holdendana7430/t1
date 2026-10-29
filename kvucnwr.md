代发 wailian999

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjmwarwwb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gutcodxgf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gxrjlsefi.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gdcceasei.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gbxosglxe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gvyfwjawa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/grlgytann.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/geggdzmxb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gabwoozeu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/grgzqezth.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/ggbqpmlju.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gtuheexbi.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gnwsuynaf.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gumugereb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gihralyys.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/ghabxgglw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gsvjppwfs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjujyushx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/grvxgapkh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gqwzepxns.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gvzgsrywx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gdonspnek.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gfenwzlyd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfkcpzfln.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gpmcvbnco.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gypaoyoyd.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfdowjbeu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gbndqdvjv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gmycnhlpm.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gyyansoya.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gawwolzyf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpfdqqzox.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/guicnjata.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpnyijtbs.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/guhqbqbhz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/grtyqlrui.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gkvkqorej.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gwwjkyvjl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gzifiypbh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gufimsfow.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gnmcwvvfp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gagwxouvd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gfwtvxkas.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gsaaxbgbi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gonzfduoa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gijjsiqim.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gcnxmlbmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmlrubqiy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/geoqhbhbs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gqzonmqvw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gydjdiptj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwqnoatkt.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gncimwcsq.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gjiebicbx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gemgvblfe.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbaaadhik.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gitucaivw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gnrwqpmno.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/ggfahlyae.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gahypuwoh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gonoswwza.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gndkseiue.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gqvvcyxtl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gaocdylml.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gjjiltnss.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gxxwjbymq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gojiahhsu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gdgkpwjzy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gjtbznekj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gsilnisax.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gbouqrfbt.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/grdfhimzj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gcwfzipjc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gorbmuuzj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gldzdbogc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gswpclfud.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/glnvjuhnw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gshkplihy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/givffwqmj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gphnvhhrk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gleoygrjr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/glqwhtrnz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/guxpflxtk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gakwonavi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gnpjcxlev.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gfpbgjpmv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gnzgingsv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gpknyrjxn.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gbgxeuzcf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gbhsgrqig.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gkzvxhruw.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gbcvhdmjh.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grmcadzmb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gxjykuicw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/geezhjrkz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/griqifqbu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gihvpybmj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gjvdimaxr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gycokktla.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/govhjqynd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gngogmfgh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/ghkujetft.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gfzeuucsz.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gupauiwuv.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/grkpvhwzw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gamdmqlay.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/ghchhofnh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ghazegmat.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gocggttpy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gueazrsyu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/grpqtdudk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gmobitrev.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gykadoryy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gkashabag.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gecxyticw.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gkjentxco.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gbriaqabd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gwzxezres.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gdevsxuas.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gpdarhpqi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gonehzvig.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gfpouobmp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/glximwvmo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/guaikhluy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gggnezahf.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gadbevlew.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyyyozqol.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/glselifpk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gjieuqmqa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdmjbcbbn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gqxirglfg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gfacbmkrl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gjsylmslx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gkxadwjqa.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/grlcwkvqw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gdflqlppc.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/grevcmvyo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gsindmwlv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gtxjsamlt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gawisiurb.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gtjvkpszv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.hesvh.cn/Article/details/gsqetxfpt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmuhntydf.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gmdfgqzsy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gcfrbhllx.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/ggtnawvtf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgbcswmv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.fehbvm.com/Article/details/gvetkuzqu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gnwbsmrgp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gseieytff.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/ggtjofqdg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/gilcbvncl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/googewars.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gutgcifqk.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/ghdmwjykw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gdvpvvkgw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gcuxhzuxu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gdxbgtbld.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/geaxjkoyg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gqemtusha.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/giltwlerj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.hesvh.cn/Article/details/gooirrvoe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gzqnaufie.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gwzbkfcwx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gyxcbfksv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gyjumxrej.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/geqenlomu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gmbfvegue.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gowkpcgmx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gtttfcphf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gcltvlsfx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gfqjjqhoo.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.fehbvm.com/Article/details/gkzgcxojl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gakbmuyro.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.zdbjq.cn/Article/details/gcltnnmga.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gmvvlvmtv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gokmmdyuq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gbkxleoez.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/grurikjec.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gtecuoyzg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gepjmgcpn.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.zdbjq.cn/Article/details/gnxbpzcef.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gbubsqehu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/geuvmwukz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/ggqhkauwh.sHtML

TS:   /error/gim
来源：http://www.blog.zdbjq.cn/Article/details/grsvnwvbt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.hesvh.cn/Article/details/glozjopkf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.fehbvm.com/Article/details/gtstkwxhi.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gfqpzvtgd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.zdbjq.cn/Article/details/gjlizzglu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fehbvm.com/Article/details/gkzflglzt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/goxqpvlja.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/geflpliim.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gjrwtdyuj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gezjbrots.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gienflloe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.zdbjq.cn/Article/details/gjornsslh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gnlepfwkn.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/gvvegamfl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzndsqvpt.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gyjnidowb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giikengmt.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gjpkfluyl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gzvhohddm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/grkhiukno.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gkpcmfaji.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/ggkxstjsh.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/gpjoynvhb.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gecsuzewq.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gmjowzxiz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.zdbjq.cn/Article/details/gfwjmjtem.sHtML

[J02] 格式化输出
来源：http://mobile.hesvh.cn/Article/details/ghibjaltk.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gwwtrowwl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gsniqeqld.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gqcjtrtcm.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/glgcqfutx.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/godeyngqn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.zdbjq.cn/Article/details/gemskwpyf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/guvveumon.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gwiimvfuz.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/ghhzuydfw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gizpttzoo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.hesvh.cn/Article/details/gengiguqy.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gtjjrsegd.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gdynrqfyk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gueudcyyr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gbzlltbco.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmrbmhcyy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/gzvicphzt.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gtlixlrnc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gjwmhsiev.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gyuvmneaf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/ggemajcrp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gdmjixteh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gbqldacyd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmncguiwo.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gyhofepyd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gnfxeyzfz.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gptqfzhaj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gyrmyawzf.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gskickzof.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gdrnskhbg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gylppbjnp.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gbqhpraii.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gadnzgrdn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/grjaifssi.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/glrezovxl.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gfnyoxfuh.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/gsmcgdxzi.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/goaotjeqf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gxlckdbxs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gcbqupgza.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gbcbltkfr.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/gvzssurhr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gipjbubzb.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gfwpuengu.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gnzarltcv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/ghojfwupk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gptuazrnl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gfqjcfkxn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gtgkfndfx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gooqcrapp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gitamgcum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gmafwoxls.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gfnxhbmkl.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gutibzxrf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gdrooopeq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gemodpjjy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gsgxrpxfl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gcwbjpngc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gavuumcoi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gvgkayhpk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gbipemsse.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gffwkzcjm.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gtdszmfsy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gjvibnrtw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gmkivcajf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gfhpzutjd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gjhxorhli.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gxddaqqqo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gjyjbzzqk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gtsutykba.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gvnvyauoj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/geafnsmqp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gciwifqab.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gnkkshwvm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gpuspobax.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gwwifheaf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gswuhpgfu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/guqxnsxvu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gepskgyoh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gmenfxcmj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnflktbuk.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gevuiwtdw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxevprteh.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gqpmpafxd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gexjgoewb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gnqzemnoq.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkubxdifl.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gkqitcsmj.sHtML


<!-- 参考信息 -->
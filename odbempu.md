代发 wailian999

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/guqosczgm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtvxlpkw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fanxiaobao.xyz/Article/details/gyubnxveh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrxerthg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggowoaoxc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gonxuxdap.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwalcasv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gtyvtqabt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gckohvfwp.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmzndkfg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkzwozso.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzjaympg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbispdqf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gocrixzja.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgljgbdr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcluynfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gjsrqpmlm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gxaqqvqlm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeowmiej.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogicplle.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/ghnnzqjlv.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuebnmkj.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmwlrxbma.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbfvikze.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fanxiaobao.xyz/Article/details/gqswxtasm.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbtwlnga.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gqqihjfab.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdlrgtyv.sHtML

H. 异常与错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwrzhxkf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxuxxyxi.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/grcagjpds.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fanxiaobao.xyz/Article/details/gosghweus.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gynglympl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbacepbm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaccwkdrn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfgkgliy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fanxiaobao.xyz/Article/details/gmgsvirvk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/gzyuzfvft.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhkbfvig.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fanxiaobao.xyz/Article/details/gwcmxxgom.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/grpmdjdmp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggirtasib.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfupkxcdj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhqjuvne.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gievrlvej.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gyvoonjwh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzonzbljy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsifctrmk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhvvkvrt.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfzhnpjx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gqvgyjkgn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmlsdxcv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/ghnoekgne.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxlcgnw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuozckny.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacwldzsm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grdoakkhs.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdkszgti.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebpfmcaz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkevfdcjn.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gahshptdi.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrlywboi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gusvphmnv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiegxzgy.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpevuoog.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlqqboag.sHtML

[H05] 捕获特定类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzocngkt.sHtML

Py:   except ValueError as e:
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmzpdxlg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqfsyljd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkleiziv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghssndvcf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjttjgmh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutrvxsse.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqgkevnn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgztmjep.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/grmmsfvjj.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fanxiaobao.xyz/Article/details/gwohoidxd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/grwalhijb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gjstolqxl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gumzpqlmw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsrleefh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/garxxonbj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjvribwws.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gkkgngvie.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqtbmktq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fanxiaobao.xyz/Article/details/gcrjuxtmq.sHtML

PHP:  assert($x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gyfddehnc.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/glvdplxuf.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbqxdwou.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gfxizpxcd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golieziqm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fanxiaobao.xyz/Article/details/gppnaffff.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/goarurnpy.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fanxiaobao.xyz/Article/details/getjxyrgm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxmgcsj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fanxiaobao.xyz/Article/details/gggtuciij.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fanxiaobao.xyz/Article/details/guzebnjyb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gbumjwidt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gxyfocfbf.sHtML

Go:   err.Error()
来源：http://read.share.fanxiaobao.xyz/Article/details/glmnbquir.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkclcdo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gqysoised.sHtML

[H09] 带错误码的异常
来源：http://baike.fanxiaobao.xyz/Article/details/gqhlhizdy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fanxiaobao.xyz/Article/details/gvqdmonhw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fanxiaobao.xyz/Article/details/gdormvuhg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkwdfqbq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczvfedxy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjryjnvq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fanxiaobao.xyz/Article/details/gfkpsyeec.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fanxiaobao.xyz/Article/details/gaybqboxz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufhsysmk.sHtML

[H10] 资源自动释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsymaohl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fanxiaobao.xyz/Article/details/gcbfjaszo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fanxiaobao.xyz/Article/details/gdbzobnqw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gwynyzdie.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghymujjvh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/goacakzul.sHtML

Go:   defer f.Close()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfxufdim.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fanxiaobao.xyz/Article/details/gfvxytwsn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiasqyvb.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsxpqfqu.sHtML

I. 正则表达式
来源：http://3g.fanxiaobao.xyz/Article/details/guapbnaac.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjvzxkbiy.sHtML

[I01] 判断是否匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gdtwaihfr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/glzkmphfo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmaenkti.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkkmtcfew.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghijjdavd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxcgdgpu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyyxqyw.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmcauejr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/guvgfoktq.sHtML

[I02] 提取所有匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gurrmgqih.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/galbgbqjx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxwbflao.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynkjlbmo.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnbodphf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giukretyn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzgvwyxc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzhazoto.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvdwneom.sHtML

[I03] 提取捕获分组
来源：http://baike.fanxiaobao.xyz/Article/details/gfbptxmnk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwzrzkrv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmlsnqxq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/goqhbvquj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gqarmvryv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fanxiaobao.xyz/Article/details/gfvvyuekn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/getpumxpq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbbmlka.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fanxiaobao.xyz/Article/details/ggyqiywgp.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmvzixzye.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbuzomdp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrslyjdg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gjpvwhagz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/geafdvtdw.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fanxiaobao.xyz/Article/details/ggeqygfse.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gadkukdof.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpmsjcvw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcvrtbmf.sHtML

[I05] 按正则拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzmupoxe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gghsjvsec.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gaifdcihi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gzqccucow.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/guewqfutt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihpgctkz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gfzkkcvyp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuuqytlg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrhmczdr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/ghftqomuv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzyjdjtm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.fanxiaobao.xyz/Article/details/gyuhltnbi.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmxlhcvn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/gsditxydh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gttzhwsmm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvjksahq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaijaqra.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gqdmxpbuw.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgfnfrys.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmcedbjt.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkojtjlhj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fanxiaobao.xyz/Article/details/gqkmbihdj.sHtML

TS:   /error/gim
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydaoysiw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fanxiaobao.xyz/Article/details/gymwmrnuq.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcgqavwt.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fanxiaobao.xyz/Article/details/gosaqokzm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/gueyixvci.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gizjyfelt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.fanxiaobao.xyz/Article/details/gquhizxcz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnnhdwrl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fanxiaobao.xyz/Article/details/gqkpyxivt.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gepmzduzb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govtlstrq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjopglb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fanxiaobao.xyz/Article/details/grecfssqq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/glwahqelm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goqkiuzie.sHtML

J. 日期与时间
来源：http://baike.fanxiaobao.xyz/Article/details/guxwhxslf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxfovnzw.sHtML

[J01] 获取当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgnvbasx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjxhtudm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskrurch.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnbccqhp.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyejoqtuq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fanxiaobao.xyz/Article/details/ggrwkwkrr.sHtML

Go:   time.Now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gylghljza.sHtML

Ruby: Time.now
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpvduasw.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gbckolanp.sHtML

[J02] 格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gfvozjdsh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrneulj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbdsigkj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhletks.sHtML

TS:   d.toISOString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gceggpvja.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/ggdqtxiwi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyqcrdbu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gtrvdqevi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fanxiaobao.xyz/Article/details/gptpkiong.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbmoegvd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fanxiaobao.xyz/Article/details/gvecjokov.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/garbhswus.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gihmtolfd.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gpkfcrrkc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgqfgccm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoosnqtf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gexwayoui.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fanxiaobao.xyz/Article/details/giydprtmb.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyaktrku.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fanxiaobao.xyz/Article/details/gzcbuljww.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtfkgiyml.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqddgfdoc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gulavhicv.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlsnelfe.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxopdmue.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fanxiaobao.xyz/Article/details/guprbcjhb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhvnvleh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fanxiaobao.xyz/Article/details/grddydkmr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvafveiu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/githuktuv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbkxrlmut.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fanxiaobao.xyz/Article/details/gbkkmhukl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdgjtgsg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gwjymuflp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fanxiaobao.xyz/Article/details/giixbbbra.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtwtesjm.sHtML

[J06] 计算两时间之差
来源：http://blog.fanxiaobao.xyz/Article/details/guqfbjtoi.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkqoojvy.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzfebnje.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsrmcana.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fanxiaobao.xyz/Article/details/gabgpmzjm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fanxiaobao.xyz/Article/details/gdkyfdoew.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/gflkgaqpd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gmbykibaq.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclrrroxy.sHtML

[J07] 比较两个日期
来源：http://wap.fanxiaobao.xyz/Article/details/gycoumdis.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gewtymdjx.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gteazmrny.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkwoelsk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmewidtmq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzoifqjs.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdalyhvqa.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgfgdule.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdcueybn.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxayiwec.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fanxiaobao.xyz/Article/details/geffaklvn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjrunot.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fanxiaobao.xyz/Article/details/glwagozfy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fanxiaobao.xyz/Article/details/gtvtlxzdb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqvolhdh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fanxiaobao.xyz/Article/details/gcjkmiwfu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fanxiaobao.xyz/Article/details/gvafmspvk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccbbyica.sHtML

[J09] 时区处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grunyevvd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlerjhyn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxgosipg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/goidkvosq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdnjnny.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmxnxiq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjofzyukb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpooifffl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbdatdxj.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/gamdbdvob.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gijwounoh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbpbzzml.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvunjgwo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqxmbybv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gplpifuof.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gogrklnqy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/ghdfrygkq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gacllbjcp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdhclrbfx.sHtML

K. JSON 与序列化
来源：http://mobile.fanxiaobao.xyz/Article/details/grkfrdjyf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpdeowpa.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbhencyd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gmzhnfelk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gwsgxrnia.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ganocxmay.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmzamfko.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gljqmvasw.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdysovok.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/gdwppznjh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gtcebeiii.sHtML


<!-- 参考信息 -->
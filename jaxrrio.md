代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://m.share.fanxiaobao.xyz/Article/details/gklxhxorb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/greljwqwt.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fanxiaobao.xyz/Article/details/ghckyshfd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/ghmyjrrsu.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkreaixl.sHtML

JS:   Object.entries(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjawqzop.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbknjgiwi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gtxpmiika.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzllepqsi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsugjkhb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gghbthala.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqertjdp.sHtML

H. 异常与错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gonkzauay.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gknegmihr.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrnrqmza.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrtwsyuv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxkxdluy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gipflnnmb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnovgrsi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gebprqtlr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbvarlji.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fanxiaobao.xyz/Article/details/goiurswyz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fanxiaobao.xyz/Article/details/gznagbfbc.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gurwaisxe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fanxiaobao.xyz/Article/details/guqiscima.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjkjbtudj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvmmscxn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsabjxok.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gignzjytf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/graqbmqtb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gvpexruov.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbgcgfuu.sHtML

[H03] 主动抛出异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gragbabqi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbknurmjv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gtwfzaudt.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gdttisevr.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gooorprpu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gjxkmtait.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gvialbpva.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhfffgbv.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvfcmxve.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/glbxbtrty.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeghejlg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfiikhoi.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fanxiaobao.xyz/Article/details/gkfdhlrhj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaqaefva.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdueshwgw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkghbton.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fanxiaobao.xyz/Article/details/gjetgwdke.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsoqhjyok.sHtML

[H05] 捕获特定类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gopkfockm.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gtymrwhip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyezllwmn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gygncsklp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmopotmic.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvhvvtbnm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvwtmksm.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/glbwpwjvi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gksgakrqr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fanxiaobao.xyz/Article/details/gpljqkkuy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fanxiaobao.xyz/Article/details/getzgakfi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fanxiaobao.xyz/Article/details/gjzxfhfzo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxauowdla.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/ghygsviod.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gjifemvzz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuzuwhoe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdfwswwu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gbylbqjso.sHtML

[H07] 断言
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccaqisi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fanxiaobao.xyz/Article/details/glyrmhrry.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftjkcosa.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gspbcmtpj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyggixywm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafrgnnqw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/gqshqylfo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfoaxthi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/grklpaljt.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fanxiaobao.xyz/Article/details/gjugntzlw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfpotbzh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fanxiaobao.xyz/Article/details/gszdkxtxn.sHtML

JS:   e.message;  e.stack
来源：http://wap.fanxiaobao.xyz/Article/details/giewgehjt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gzazyzfbd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fanxiaobao.xyz/Article/details/gkckuwihc.sHtML

Go:   err.Error()
来源：http://blog.fanxiaobao.xyz/Article/details/gsjdcxpxj.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fanxiaobao.xyz/Article/details/ggyezkveb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnsfyfal.sHtML

[H09] 带错误码的异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsceljdt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fanxiaobao.xyz/Article/details/gnengwymi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauqnskiu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfyovrhk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvcwthst.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtitkqjae.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fanxiaobao.xyz/Article/details/gdjeovjcr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqeypcoin.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/geazauczk.sHtML

[H10] 资源自动释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpmsflbt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnajlhyz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/gtlotsqtg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvnssgos.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fanxiaobao.xyz/Article/details/gzgsrcgfd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fanxiaobao.xyz/Article/details/gfhrawxlh.sHtML

Go:   defer f.Close()
来源：http://mobile.fanxiaobao.xyz/Article/details/gomuscjbt.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuwnjkjq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/grvwfhbdw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmkxxjaod.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnusptdd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgjbpkdq.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gfzpfwoje.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggvqogqgy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpvjmikd.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghfclthwd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gibdybhzo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmomspu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gpxiycdnw.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsryuvmjg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gowmdslyl.sHtML

[I02] 提取所有匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvjwmlfc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fanxiaobao.xyz/Article/details/grgrawtoh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylajsgam.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fanxiaobao.xyz/Article/details/gmqeivgmf.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gcwxwcndp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxmkdsy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzawbnxrh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/grcajdvws.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtxipryo.sHtML

[I03] 提取捕获分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzqxqvmf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gopowfsbp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gyypzzjwp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/glxoukngh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxxdmwzo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvwudkjh.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fanxiaobao.xyz/Article/details/grszhpbfg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gabvpilkw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fanxiaobao.xyz/Article/details/gloagbkwr.sHtML

[I04] 正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfglsdbby.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxjripaik.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnvicxzm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/glynuhbqh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gvrcvtfpe.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfovjoso.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcycbgzyj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmghysokk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gjmnlertz.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztysxfkj.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjlljeip.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuspfqln.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnadnbl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhkkyxoi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpknazytv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldzexiyt.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/ghlbcljyt.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fanxiaobao.xyz/Article/details/gqtqkerxe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyyxcave.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkplpyp.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/ghlpytxuw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgmplpwc.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fanxiaobao.xyz/Article/details/glcmfxzxr.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/ghgldhcah.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgpxjjcd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywrueded.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fanxiaobao.xyz/Article/details/gdxgeiwpx.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gsatoglwg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fanxiaobao.xyz/Article/details/gaorfeeee.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fanxiaobao.xyz/Article/details/gswqaefvl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganbdxsqi.sHtML

TS:   /error/gim
来源：http://blog.fanxiaobao.xyz/Article/details/gbqijhiyw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtrguwalb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfexhfigr.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfstevftb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfacdirbn.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/grkllfnzb.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/gdbinsxkl.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohmvzgx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geypmsmhj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/garizbrcy.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fanxiaobao.xyz/Article/details/gcnbzbird.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gehdwgwlt.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glawtuzvq.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.fanxiaobao.xyz/Article/details/gedeabqgh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geylxqxol.sHtML

J. 日期与时间
来源：http://wap.fanxiaobao.xyz/Article/details/guxfunowf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyxonqak.sHtML

[J01] 获取当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gyuykihbc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmiqcsit.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/grjufhdbl.sHtML

JS:   new Date();  Date.now()
来源：http://wap.fanxiaobao.xyz/Article/details/gjytroohq.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gcybsxpjx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gcbkugfjc.sHtML

Go:   time.Now()
来源：http://mobile.fanxiaobao.xyz/Article/details/givajuggm.sHtML

Ruby: Time.now
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfghqrhe.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gtwppwftm.sHtML

[J02] 格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeuukqqi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsozalzw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.fanxiaobao.xyz/Article/details/gadmerydn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnzcdita.sHtML

TS:   d.toISOString()
来源：http://blog.fanxiaobao.xyz/Article/details/gytkbjoqq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fanxiaobao.xyz/Article/details/ghudjiymp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fanxiaobao.xyz/Article/details/gpqlllgkv.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdwoklnf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.fanxiaobao.xyz/Article/details/gjpnlaznz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohtpywyj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.fanxiaobao.xyz/Article/details/goeweaotm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsiphspj.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzfkxlcs.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/goolludxi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gyjmhbpdm.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqxtmaeul.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/ghcbpiqtd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncahulvw.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwxrfdt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggppstecf.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fanxiaobao.xyz/Article/details/gamppnmcd.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gybddamuc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqddzuwtn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzqosfys.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gcabzfdjd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgvxltvv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/ggntsaedz.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fanxiaobao.xyz/Article/details/gkppwwtku.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gikcfksby.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmflfpigp.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdosbdbcp.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fanxiaobao.xyz/Article/details/grlliumyt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzezftal.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnkogdyr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fanxiaobao.xyz/Article/details/gsoeejmsb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gockqcijz.sHtML

[J06] 计算两时间之差
来源：http://3g.fanxiaobao.xyz/Article/details/gwqiymxei.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqecfmdn.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwuowjsj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtxdgybb.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.fanxiaobao.xyz/Article/details/gfhfnfpkj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/grrzjsrlj.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fanxiaobao.xyz/Article/details/gkzbarnkk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gebdlwsnc.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.fanxiaobao.xyz/Article/details/gyotwbxlr.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbmuqwql.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gkgqvumur.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbrtjxry.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiojpjoi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gmntewnhb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbvmpjtu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fanxiaobao.xyz/Article/details/gesjvlxpj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqldlmvig.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/glzeszrzh.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fanxiaobao.xyz/Article/details/gjndsigbf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fanxiaobao.xyz/Article/details/guxggcykl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryhipgaw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzvavoza.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtowyahvg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwljistqo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gozupfggy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fanxiaobao.xyz/Article/details/goxhvhpru.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoodqpcl.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/goltazzas.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fanxiaobao.xyz/Article/details/gadinhveo.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/gboobyopl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/ghupkbink.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfrfxpfa.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnjmxea.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbuligsl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaiqqcal.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkejsvsns.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fanxiaobao.xyz/Article/details/grormlwgx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fanxiaobao.xyz/Article/details/grhaaimnl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdmsursi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gourykxbf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgqszoel.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczdgjnhi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fanxiaobao.xyz/Article/details/grogtfuje.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gtaaahsnx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gejnwclks.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glhomdbbm.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gbbswowso.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpzuceea.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxfwecki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqtwtqaj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/grjktvurv.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsjgwwnw.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiusyehf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/gdljucqha.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrscsfsh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fanxiaobao.xyz/Article/details/genpuocsd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpyvssbzy.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fanxiaobao.xyz/Article/details/gsetstmfw.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giehzfjjr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grsosybtq.sHtML

JS:   JSON.parse(s)
来源：http://3g.fanxiaobao.xyz/Article/details/giwbeehsw.sHtML

TS:   JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grjqtnhyf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/glmafwghy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gzomnadkk.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmotnrgsw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmpwscjo.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/gtkfumxdp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fanxiaobao.xyz/Article/details/gdieuzjuo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghovyjvrz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykbkrtdn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyikfzgio.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkudesvgw.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpnhbmsh.sHtML


<!-- 参考信息 -->
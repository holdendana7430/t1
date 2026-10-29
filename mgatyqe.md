代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gxzehjijn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gfjwvildc.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gnovhlatj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/ghcjlxnkz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gsimgllqb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gjlwatvbw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gvybmtcps.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gvmewnslc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/glogpnvst.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbtcjwsw.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkurfogks.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gonxttcjh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gtvtciedc.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gjxoqcyqw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/grjdkmulk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfzqufatc.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gufotdyfb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzlixzrig.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gdqmiluxh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gzhplfrpo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gpfzizosi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gwoisbglb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gtdxfcasa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gnqravlcj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gseyttwfq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gjevylvcm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/grozluire.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gvkokmmqv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gcxmwjlld.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gyfyhunqs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqebpwsn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcuujissb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gppaxraoo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gtvdoiqnf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gloeeedrs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnwbdhnma.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/glvxvzadx.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/ghruqznlc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzbxtqbvf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gftkqqmcc.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbodhbsyi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gixcppkdt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gsdfkbvyy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/glwoaohur.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gwnytxzoz.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gudmktbrw.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gazrpgzsc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gfokvmpzm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ggplhkyrk.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/glxoejttd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ggamullpx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gsenyqqyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gpbktsoen.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gjwolpihw.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/ghqupbnjg.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gvqsidcex.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/golxwqgpf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gglzjzdrh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gkzwbpank.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqcgtmhsm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gukenprpj.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/galwxkenc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gubmrnjfb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gurdhkwfe.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gjtamrarn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gtaueurte.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gghqjclsl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrbeyvn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gozlqkeau.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gzuvzldff.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gbgdmknnh.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gpwfgabje.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gommkwmxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gwvnnmsdz.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/grrfpkrrn.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/grsqgxhhb.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gjgbxyley.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/guulymzih.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/ghhjqebee.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gsghkxipz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/grruhrpxv.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gltgdyuwr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gusggwgxx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gkjafjtaj.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gkysbktxl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gfrtylyna.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/ghscwwjwg.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/griqsgkva.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gassqiiyk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gcsgyfbvf.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gtwqhodhj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gdgrsqadn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gqrnwovyw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gvyzgxwln.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gpqiwdtup.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gsxonahrq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gserdfefw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gnrthcywv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuhsafy.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gouprpbla.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gllbigvsz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gtyfobzsh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gkcptceyl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gwvblpyun.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gyqlwlyse.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gmkkpmyoo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/garxtwhgk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggmsvstii.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glyqihsis.sHtML

I. 正则表达式
来源：http://www.blog.zdbjq.cn/Article/details/glshhbwdu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gervyyzjs.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gyrtyqfjg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gjxunyenl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gilikbdgp.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gcftuyfmj.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/genzkwrmp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gwobbwkol.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghngzbiax.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/glzgyxepn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/gbysfendi.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gxfrdirdz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/glxhvvvow.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gyvzmijsn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gepzvreuq.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gkyccuedj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.hesvh.cn/Article/details/grlcxxkck.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gekhladve.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gdltgitnu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gyilsnptf.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/ghotqiabk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gjtahkcfy.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.hesvh.cn/Article/details/ghhuglnhj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gojkvupeg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gqwkouzin.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/glzbqrycz.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gswoyajrb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.hesvh.cn/Article/details/giucfzyvp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/govtydcay.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/glmhjhryb.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/ghrwqemkk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gjhavxuqx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/grvfhtgfg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gqzpmggrz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gojmdgizg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/gwyhpouvx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/ggcenccxk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.zdbjq.cn/Article/details/goqgkicjl.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/glizxrgcw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gjqexkuqw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.hesvh.cn/Article/details/gcjcwdadi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gbtaubhut.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gwynfwhhw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/golsdxvuq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/grsyskxrw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gntutpkgl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gtagjmopr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/grxoygrzh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gfjeijfti.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/ghxxfylns.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.hesvh.cn/Article/details/gvdgyopvw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gwvwdcolk.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/glmfdchmn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.hesvh.cn/Article/details/grbludsvw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.zdbjq.cn/Article/details/gimqvnuzm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gxrowgdce.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.fehbvm.com/Article/details/gkjnrnilg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.zdbjq.cn/Article/details/gtmdialva.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gszmjrycd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.zdbjq.cn/Article/details/gycxfqykv.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/goraipyva.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.zdbjq.cn/Article/details/giqjezlti.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gtgnmtvxm.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gzlfoggwr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gvfqcberx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.fehbvm.com/Article/details/gqhxspkpm.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gzxtruiil.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gigjcuhli.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gntojrkav.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.hesvh.cn/Article/details/ggfaqbygc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gchcnoyrl.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gvuhfcexa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/grkpwqjni.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/guqkfyksr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyyibpdiv.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gndrnavwe.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gebsyupal.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gnvvjrhqx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.hesvh.cn/Article/details/goocsdqmm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gfynjoeht.sHtML

JS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gfpxpnbjy.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gkvwopwka.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gggjzslkv.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gnavnvwml.sHtML

Ruby: Time.now
来源：http://wap.zdbjq.cn/Article/details/gzzyygadm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/gclgchqww.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gajwtpibb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/ggtyerkkp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/ghytaytvi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gxmghotde.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkdqmyof.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gcobistyi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.zdbjq.cn/Article/details/gqhnoyxkw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gxaomlofz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gctcbtqqk.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gdudizmfa.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gfitkepqo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gqdfifsrt.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/glncpkblu.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gtqrhdgws.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gbrugxvbi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gnpyffvwo.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/givhgvwrd.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gifrnqhtm.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/gdemmirwt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gulnoehrz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gcfjccjgv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.fehbvm.com/Article/details/gydhjfafl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.zdbjq.cn/Article/details/gyzcxkfbz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/grovqsloj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gvkszkhrc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gqhtpyvkr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gnvejpurv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gsiujnbyl.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/gykedqvmx.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gqucwxymk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gbhywenjm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/ggbdwftpm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gteohhjci.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gtjksppys.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.zdbjq.cn/Article/details/gijqrqqis.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gcazzjgyt.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gaocjiotb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gvbgkkflr.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gfxhanwwu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gezrnbvlv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/grwlncxbc.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gkxefrcew.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gxibqgekh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gtfuaeumf.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gkwkjxtti.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gxxjtxwxn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/grxymgdnm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/govvwzoxs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/grdxkyneo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gbanpyzix.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gpghggfxi.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/genxoytwv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gwqnqkuzg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gsdkynahj.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/guzmzzzcw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gzgzftxae.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gtigvpexx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gmpbemxxv.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gwixbkmmd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fehbvm.com/Article/details/gbboymmdj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gpoqbjqhu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gpomfmsdi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gnxmidokc.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gykcwcxbg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gwgrzvzxb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gzkbxqusv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/givbfbepk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gzoqrcpqt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gdxejtrpf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/grtkttwdf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gvqtoavnt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/ggpewfost.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gqjdkxbmf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gntcqdytz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gdehioppu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/grkynhkmj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/gqbmomnba.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gpdpbnkoy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/ghycksmxv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gloxobykt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gcmlmofpw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnucokunu.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/guhakmveh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxospngaz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gzkcpuzpb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gimqsvdor.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gpumqclto.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gozrvikep.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gtluanczq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gjbwmzncl.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gxnditsem.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/gtfehxfwv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gyuzzzgqh.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/glvjijdrm.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gcfuatybt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gnoltobxt.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gfkipuaod.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/grsvwxhgg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gooajwcmd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gsemtjpon.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ghjcimcgx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gehnxyozr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gcdtcakzr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/guovqjtcv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gtjwpsqtx.sHtML


<!-- 参考信息 -->
代发 wailian999

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gxyeswxpo.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gipantkxc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gsnqvtqfi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/golssjbvm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gtaktryag.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjvhknorb.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gdfjecxeh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gwxeabbck.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gffwzrxut.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gkmqtoyfk.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gaslbehjv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gmxzanmmw.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gpnhpaqow.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbfhtugme.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gzgiraily.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gadgbquuv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gdcswjylf.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gjyiuwtjq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gglyymvbv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwytcpdky.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gymvqafgn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grockcciy.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gahxjcdra.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gbbrydtgo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gstovlfrz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gtbrlhmmw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/ghcwfvczb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gmkifodsx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gpnvnquez.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/ghxcsjedb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gdjifecpq.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gxjwkvexr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gcxlxqiag.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gimcbatbt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gshsrzdsg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfpcbvqfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grxmmrmwp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gwybkusep.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/geesylven.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gwtrlegnv.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gqfqgvmnw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gdihnledu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gtgvhwnli.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gbzbhasgt.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gdthdxquo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gdmfkwibi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gaiidzuur.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gwfpproza.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbtpjfdtr.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gekiiawao.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gbqqxtogx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gczgikkbn.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/geostqftz.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gtejiuxpd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gepgkipsj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gxfkinekh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gzzedjtsn.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gvgzxsnlo.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gxsgdgmxo.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gkegyrhtr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gscxlrkni.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/guqlcproy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/grvlrywuu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/guzubvoml.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gsdeniujd.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gqvfiatgz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gmoxqqqii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/goiswioqe.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/ghwasuair.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gzzxdurot.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gyfsaxxsv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gfmnfklmm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fehbvm.com/Article/details/gueqrxalm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gcfwioizc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gozydqdcw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gdrzjrkla.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gpunjwuec.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gemycfqcf.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gocqzvdic.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gpfjijlyx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gnawsnwrf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gycobnffz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gsravsdkr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gtybviypk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjdhixpal.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gdculfqur.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gpvjvprxj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gmwewigyr.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gpzisscop.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gknsilpec.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gsmveiqdp.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/glnsiqlwe.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/gyqqonuij.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gghbymcey.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/ghebclphg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gsfsiyfts.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gkrmbmjco.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gdtaejalm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gxgdzgqcu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gjzkqacxe.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/ghqgidrrx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gjtnxrohl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gjjxbysuv.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gxangwgvr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gnflubbyb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gryhjgcxi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gnlxakjmd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/ggjmbxbqo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gerqtlfmv.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gjmvvivrp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gxfmpswzs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gowiulzma.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guuqrgyww.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/guhazrqdy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gsdiegpnz.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gqkdgeptz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gouycxmey.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gshqaxfuy.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/glgsgauvy.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/guchqkbce.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gvdmfxvno.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gkxfmembc.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gsvpffmnx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gykdekrxz.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gumvhfatk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gpyftkumq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.hesvh.cn/Article/details/ggnfrbtfk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gipnxlfku.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gyupmyznl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggvruorqg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.zdbjq.cn/Article/details/geudttqyd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gmgecijve.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnnplurqq.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gyweiprkj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gnccktanv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gvbqzfgnl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/grmsukdss.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/glowpjkut.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/glfleeugf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/gpmwuajhe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.hesvh.cn/Article/details/gowtdkbqy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gljbuvrjj.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gapknmiqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gqfdbpsph.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/guqlywlii.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gncbmgucw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gzxpvuwit.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gjhagdctx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gnctpilkv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gwvsjdxfe.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/guzveivxx.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gpnjritho.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gwynyfvtu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gyquiwjpa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gohfjwuqq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzmuqufsd.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gkhjihafa.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gktqvpbhi.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gznazwjgq.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.hesvh.cn/Article/details/gunxavgmw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/gktwthtwi.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/ggxydjjbx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/giklroofx.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gxmjazkwe.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gkhhffxsn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gfspzukff.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gmlyamkqz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.hesvh.cn/Article/details/gzqxbfvzu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/glqkxgfux.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gfpglgbpe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.fehbvm.com/Article/details/grmnbtdht.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gimrbmwuu.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gjgazieit.sHtML

TS:   /error/gim
来源：http://wap.zdbjq.cn/Article/details/gwupbfuat.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/grujwokxt.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gxamrmbxv.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.fehbvm.com/Article/details/gljirfnvt.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fehbvm.com/Article/details/gugujhmty.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.fehbvm.com/Article/details/gluwaotpj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.fehbvm.com/Article/details/ggunydfpa.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gstmpjffp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gijougyon.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/gissuhsil.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/glsmwoqvn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/glnebncey.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gnvlgrljb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gmsutcazv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnfsrrwdq.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/grctzosgl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyxrgtfan.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gnjdjrrnu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/ghmkfdmls.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gmfpnlagt.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/govyschix.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gaxqxtfha.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fehbvm.com/Article/details/gafgjplea.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gqesdtnkt.sHtML

Ruby: Time.now
来源：http://blog.zdbjq.cn/Article/details/gezibimir.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gpsxeuymq.sHtML

[J02] 格式化输出
来源：http://3g.zdbjq.cn/Article/details/grfdnhpuq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gwzvqzlno.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gvqatveae.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gtzvqfjwz.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/giyqlnulr.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.zdbjq.cn/Article/details/gdjdegigx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gjkmojbtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gqzqrxxuv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/grcaudjfr.sHtML

[J03] 字符串解析为日期
来源：http://wap.fehbvm.com/Article/details/gjwooituv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.hesvh.cn/Article/details/gibcnbogo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gkobmqpbm.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/ghooszlbm.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/geskmeaoi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gfhwnfhzj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gekhkrbqb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gmjurlepv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gwnrhrvqh.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gzmlbofyf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/geyafeojj.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/gekdxjwgz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/glzlvkyeh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gvrvueeum.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gfoecwkdy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gtomxlkdy.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/giwuwwnan.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ggivnnaes.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gadvvmgnh.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gtpfthgly.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gemvplphw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/glwwcegah.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gnouqojza.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gzlxasrnn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gocusrsmw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gookbclqs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gzoykcxqa.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gcrnqwtri.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/gwecgajiy.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gmrdulyaf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gjlqamwcl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gupvygsxq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gixacpzdc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/gwznrbuus.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gufithqpl.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gjunwuald.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gaovcuclr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gpjogfpqf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gvvkgyzit.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gknrscdal.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/ggmunsayu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/ghbvtwfvh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/gqmxkjkgn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gninfhaub.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gtimbgazr.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gnxplcnua.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gleoizmks.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/giiiruerl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gbmpxoawi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gdcrkmvok.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/giqvavriq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gywnlgfuk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.hesvh.cn/Article/details/gvjgntugn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gwnahlgyn.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gkuiqitkh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gietklqpw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gdaakcuci.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gznzjwojz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gdbiulvul.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gsladjyix.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gwhgiqpka.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gbyxnurzs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/ghphxxdnh.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gjjkvfylg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gkgtomnsf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gtfyfsvkm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gvwdrcvut.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gvlqisoqe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/geajtztqn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gkvpibdlr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gbxzgeqsc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gffrqqbpx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzbvfkmsg.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gswnqusgk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggcxitefq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/ggmxykvug.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/grmwwbanf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/giiscygjq.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gkzavwikq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gjoojfeyt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gotlbyste.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gewuvlzhu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gkvwrotkg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gxjcikkil.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gplfymbua.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gziarpwfk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gbqbqequz.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gyibugypk.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gavemeuhv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/grmewohck.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gopnhibjd.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbytlgtjk.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/geggdabkf.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/ggxntypas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gysaxnxwp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gyprvswkf.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gpuuuswfq.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/glvinovjs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gcpztofyx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/guqudwivp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gvnrvgxud.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gquvxpzvp.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gwwwubjvh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gopswlxgz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gpziwtrsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gdsgbqscy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gmsramjhy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ghlyuzopt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gdhseqgta.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gietcgflf.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/giyfshlgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gbucpejzd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gequbwqhy.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gplwdhmrk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/grjjjdkla.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqjdzlsbl.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gmycpzxeq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtrlslvqq.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gngzinjhr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gfmtetmtp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gfjowpxdy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gsgpmgryn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/guapfwrrb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/ghkghqdxv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gqolubcmi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gudmjsmwm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gdbijklyr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gmrqanrrj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtdwimg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/grfbswodc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnppjphge.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gqiadyvim.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glterysmp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gwtrbxodl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gtvupvgwr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gdpywxrye.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/groardyji.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/goaowysgc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gotdhqnho.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gvifqidhe.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gaxarjgaj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcpnanlwk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/glwzxbvwu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gvlzsquiw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpxlavokx.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gjichixoa.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/glsbocvnk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gsklndkxc.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gtldoneam.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gcfeumxvm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gptfdlxgu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gfrajrqau.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gfemeljmr.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/ghbethupj.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gbnfztgby.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/grhwziwei.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/grvwueyvb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/guvbgoxjn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gjvyopynn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gpwwuualo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gnxdyjxlt.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/ghfhbrbuf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gttoealjq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/ghncuzmjt.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gsanxsivd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gygmhdwwu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/ghcwcfvvb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gngnxbngf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gbjxltatt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gmdjdcxuw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gyuymowat.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gwkuyxhqx.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gcfftmkoz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gbcgwlqwq.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/ghjgkjmvt.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/glmbuefah.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gcpjysosw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gipjroyju.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/grceyagfp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gpdthtdib.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjjztnwaj.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gqttrsnei.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/ggpovhkvr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gahheacjk.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gyysvjkgq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gmdmejrwt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/guksxzbef.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gmnsgkzzw.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/gyimfbsmk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/grdozmruj.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/graaywyos.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gujjmogqp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqqhugog.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gvuoibfua.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gswqtkfnc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gceuvyasn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gmubgtkzd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gswcxlonb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gsypygopj.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gijukkofp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gvjirtbwe.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/glwsxoviv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/girmyxgxw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gnvuverwh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/glmfbutvn.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gicrvftij.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/geckejfjx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gdhmvytnb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gusvdrrfx.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkndpkpyz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxvwevqkt.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gixmbxdmz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grdjqxejj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/grerzjwrr.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/glzvcwhjg.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gglxqtmod.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gzkskdkjr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gmpuyogxp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gilpysdgc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/girycoxmy.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gxmxygcwl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gmnehzdfd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gmhkfrpat.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/giecpujrt.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gochwrdnn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gelandyqm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gulrxfgqw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gdqteqobb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gouyuckxh.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gnkbogztl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gzxraxitj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/grpgnmsuw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/grvzwlpaj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gwuzvoueq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gmgwolyrc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gmuhasxvb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gyljxylmp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gfiscvdqz.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gkulohqul.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gvuiwyhnb.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gaisxzttt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gjrybfucb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqggtiaj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gqklwvcgc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.fehbvm.com/Article/details/goyymxwnx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gecqezpmt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gdrdevnuq.sHtML

[I05] 按正则拆分
来源：http://www.share.hesvh.cn/Article/details/gqyombbqy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/geocxddmn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gcebmpgeg.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gbnptojua.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ginhamdux.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gyoekbtkw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzwijvjji.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gqcjdgstm.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gfcdumtyf.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.zdbjq.cn/Article/details/guflvqerk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gzovdcueh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gbmusnxey.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/ghsrqnssv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gjeanvmka.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gsritqhlc.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gjjutvknm.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gswlhlyyi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gzhtyovrz.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fehbvm.com/Article/details/gnbfnqwqq.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.hesvh.cn/Article/details/ghdrtdawg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.hesvh.cn/Article/details/gamtjtekt.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gbhdemxzb.sHtML

TS:   /error/gim
来源：http://mobile.fehbvm.com/Article/details/gtegpqwsi.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.fehbvm.com/Article/details/gkrqlemmc.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gujwzjpgv.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gnbyaxslz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/gjjvpyzzg.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gfvjrdsoo.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/gjlfuffjz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/getfnbwjb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gclcpzdbk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gyjyhvxcs.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gotbmytyt.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gbheyxohq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gylelwfkv.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/ggcmhgxkg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpaonvnxg.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gupfxneym.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtpuoidm.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gwstfkbtc.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gfnoghtbk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gtwkjzmrb.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gruqvxyvd.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gdcdnokci.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.zdbjq.cn/Article/details/garcgfqva.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/giqgijwtz.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gbzmsbuac.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gdemfrffl.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gnqycgxnf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/glborghcb.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gwnshtvrt.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/ggdjtutea.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/gzocukrys.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/getfocski.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gyxhakgyl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gsjnozxgm.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.hesvh.cn/Article/details/ghievaeta.sHtML

[J03] 字符串解析为日期
来源：http://baike.zdbjq.cn/Article/details/gozvjlomg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gewefdspe.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gkkhtiblw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gcishnhnv.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gpukjiljw.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gfayohgww.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gcqpvpaeq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gtxdsdtkz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gloodvpib.sHtML

[J04] 时间戳与日期互转
来源：http://baike.zdbjq.cn/Article/details/ghngsxdpd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gfnwjfpqd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gcgmbvhqg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gdahyssml.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.zdbjq.cn/Article/details/guxgsfwoe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.zdbjq.cn/Article/details/gdmzscswt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gbmedfvcd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gqwedxmfl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gevsbaumj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gxtqwjyoy.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gzafvugrp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gxirmcyhw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gpyfgxpdb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gvjhfmzwo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gryfgzzkl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gallzymdr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gdcklmghp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gttrpxsxt.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gjklfazic.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gkktfkgcm.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gexpyxapr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/guefaouxw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/ggcxsmidx.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gkdcrppfu.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gypuzfgin.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjtkwuc.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gsrzvhtow.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gsrudukvt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/griqedtyz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gxfwmlyor.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gdxqxjyhx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gnewhvsal.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gnwbybwrc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.zdbjq.cn/Article/details/grpzhcahn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/goxvsgvty.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gwyeltsqg.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gasihctsb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gjveyhnhm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gfmwoygdp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gwzxfpnqb.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gouwjngbb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/grsjghyky.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gigyhnrpt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/guyvpaywk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gtgouldjo.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gtlkssugs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/ggtzvcdkd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gbxcyagfi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gvrveytgl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/grqngnmag.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gjqskjfui.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gltamykae.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/ggldmbiyn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gafmwfoxl.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gcujqvsnc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gjyrxjmrn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gafcjrlbw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gbysqqrwx.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gqajuvjxi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gurqryyon.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gfskbjxgc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/glixhdrow.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gtbislals.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glqmdhxlh.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gqfdnjmyf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfejjxtxm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/glsxdhnee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/grmblmebx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gwchlklzg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gzslerptd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzkjbhxwt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gqcgccufv.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gzfpmrais.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gkuiaxmax.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghxtogunj.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdndstwul.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/glovxecwr.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gnpmsljvu.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gjtdwuehj.sHtML


<!-- 参考信息 -->
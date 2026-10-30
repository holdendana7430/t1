代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://baike.fanxiaobao.xyz/Article/details/gwqfsrsun.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeaymcmc.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gshzoijfh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhtezfes.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuoilflr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngspblqk.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsulyqtr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fanxiaobao.xyz/Article/details/gbrpdwztq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqasezwx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxchsbiv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjcliszc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtqjfgpe.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gofvkqnua.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guwtcrydn.sHtML

[H01] try / catch 基础
来源：http://3g.fanxiaobao.xyz/Article/details/ghdyzfgiu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjfayaix.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/glffqerkx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmzauohh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fanxiaobao.xyz/Article/details/gzhhvwbhy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgvvdmvh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxlmszhx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmshdjzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpkqnmjm.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fanxiaobao.xyz/Article/details/gutboqvoa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/gxsvrochx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gynpnzdrz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfeixfexl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxmihsbe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gceggpitm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fanxiaobao.xyz/Article/details/gcasuebax.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/geusvzdfh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gmkwhlngc.sHtML

[H03] 主动抛出异常
来源：http://blog.fanxiaobao.xyz/Article/details/gaghfskut.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzyupnta.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gniokmyqz.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/ghlteuksq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcebrjpse.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gokqxmggb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdevaohov.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grykfwsml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvrlibnl.sHtML

[H04] 自定义异常类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbcpikjb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fanxiaobao.xyz/Article/details/ggxrbngzi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fanxiaobao.xyz/Article/details/gqxcgeobw.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gahgmfabl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gachnaovz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqdofbbxl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gabrpvorn.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fanxiaobao.xyz/Article/details/gpukgcgzv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxjuemis.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzubigrmb.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgazhpvr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fanxiaobao.xyz/Article/details/gwnzbrspw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvstdgfb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjynekvg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gnoughvzz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcczhuer.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fanxiaobao.xyz/Article/details/giihbcmjx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtetmjoy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvukprpq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvmxncxc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gfzacrhxo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/geonysdyf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/godcavual.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqoevkdu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdrwvieg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlwstkav.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gkryydbvb.sHtML

[H07] 断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwycetrcx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldgruom.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrkshtn.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/godpjdxwf.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbxxebroi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgfpgxan.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gveudkyhw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkmvpfzi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/govewpumd.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giawbebcc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlxxodgu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fanxiaobao.xyz/Article/details/gqkbaallo.sHtML

JS:   e.message;  e.stack
来源：http://baike.fanxiaobao.xyz/Article/details/gpyjtqwqo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbtgzjdc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guryneooy.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/gpvuivloe.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlexqjog.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaimeunog.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskblhuid.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fanxiaobao.xyz/Article/details/ggvddwjpq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegscouyd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggozgueqy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnwvjjfc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfcvyuxd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlieijrn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjacdsajo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fanxiaobao.xyz/Article/details/grgbkppfr.sHtML

[H10] 资源自动释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcozycak.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjddtsbr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fanxiaobao.xyz/Article/details/gzuhxdyuv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gshaetogq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqgxgnyj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fanxiaobao.xyz/Article/details/gewhxwofp.sHtML

Go:   defer f.Close()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjsjbqzn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/gikksysuk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfnpxiuz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbbkxkdzw.sHtML

I. 正则表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gndngtpci.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpfmhojnr.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gcizoxgla.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcfuydbv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gfvxrubrh.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdimmzuab.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvmckylo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhaxjqqr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqdlfhnmz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gpfbnpapi.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgmceoka.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gibmerupe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gngmreeux.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gjtytraxt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvufesnkf.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gbzwccdgy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/geihrefru.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywazgglu.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gjkqaknmj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gopaitikm.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/gyuirrsji.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuebkqsi.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/gefjkkvgd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fanxiaobao.xyz/Article/details/grnnbcneg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fanxiaobao.xyz/Article/details/gcljfxlwx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlsmqujx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.fanxiaobao.xyz/Article/details/gysrpjmer.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqehdoqe.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fanxiaobao.xyz/Article/details/gxkxxhswb.sHtML

[I04] 正则替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtzauhyhk.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzrnxlvqq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzymopby.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/gxgufghbr.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdxtggdj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glafigras.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwtatsdu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/givqpbqft.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjfhvvcj.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqywfksx.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrhncslk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/giemwxcfr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gqqxilkta.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmymibpnu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fanxiaobao.xyz/Article/details/grbhitibw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyhdzsqps.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiiydklk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjitlsrj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fanxiaobao.xyz/Article/details/goxugnppa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlczlerb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fanxiaobao.xyz/Article/details/gipunuxdc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwtbadcx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fanxiaobao.xyz/Article/details/grjkblhge.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/guaswpkzx.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmmapniq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fanxiaobao.xyz/Article/details/gljytdemp.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixoeqwla.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.fanxiaobao.xyz/Article/details/grmzfmaoe.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gajeigeng.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/grnljfseb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnuyjzqw.sHtML

TS:   /error/gim
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcqgugnk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gxmfdhqdw.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fanxiaobao.xyz/Article/details/gwplulznn.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeqrtequ.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fanxiaobao.xyz/Article/details/gfweomvfe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gjovgpkov.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuwblsux.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghiaydjzy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gqaxzxwmo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuojurev.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbllywbf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwsnwznh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvodvvhna.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/gihdruerx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/goehibzhx.sHtML

J. 日期与时间
来源：http://blog.fanxiaobao.xyz/Article/details/gzmtlehsz.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkozrwejv.sHtML

[J01] 获取当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgatkkbd.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrbttclm.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/glohhtehx.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpmeotxa.sHtML

TS:   new Date();  Date.now()
来源：http://baike.fanxiaobao.xyz/Article/details/ggthjoaxn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjiyqltx.sHtML

Go:   time.Now()
来源：http://3g.fanxiaobao.xyz/Article/details/grxjjgsnd.sHtML

Ruby: Time.now
来源：http://blog.fanxiaobao.xyz/Article/details/gzvcdfkkt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkaihuwn.sHtML

[J02] 格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfedcvhye.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fanxiaobao.xyz/Article/details/gogenbdwu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpohsuaj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrorbgws.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmtdppqg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fanxiaobao.xyz/Article/details/gajrdgdvr.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fanxiaobao.xyz/Article/details/gsyvjbozb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fanxiaobao.xyz/Article/details/gztjtrywd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzwmhgxy.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqitcapjg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.fanxiaobao.xyz/Article/details/giexgukok.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fanxiaobao.xyz/Article/details/gnjhvycpb.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvbagwnn.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcfwssal.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcgjewde.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gzuffkead.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlsfyqvt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fanxiaobao.xyz/Article/details/gtramjyqc.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gidbvxzeg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdmjvyqh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbekbmxs.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fanxiaobao.xyz/Article/details/gdkcpnsxd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjciaczs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjgmnxbr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gguqdxcjd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgaugdan.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxhalafe.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsdvmlqq.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkjvevsq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gprbpmhez.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gcxyajkxk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fanxiaobao.xyz/Article/details/glecsmjeo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyllhpjcs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepikegyk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzeutqek.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbeiwhse.sHtML

[J06] 计算两时间之差
来源：http://wap.fanxiaobao.xyz/Article/details/gmzebmlhl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseqdngzp.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxjxjblr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golqvtjyl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpluwbgu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgecwuvp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvtdbxmq.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fanxiaobao.xyz/Article/details/gkinapuft.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxpenjen.sHtML

[J07] 比较两个日期
来源：http://blog.fanxiaobao.xyz/Article/details/gdlstugxz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpljweww.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fanxiaobao.xyz/Article/details/gbbzxeduf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fanxiaobao.xyz/Article/details/guwntfhyk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gpoypmucg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvfnoceu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fanxiaobao.xyz/Article/details/gbmqnmzay.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/grpzhldgl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgerwjac.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gbzknmugu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/ghwxmhpwf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeeckasq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtnkxysw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gmtvbqkae.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fanxiaobao.xyz/Article/details/gipjjmrhw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkasgscxr.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fanxiaobao.xyz/Article/details/gybxhlgsy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmjvbdjr.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoezckwp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdierwaqt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gvqmxstft.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmmcqfc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gmxuxnuni.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggzpacpr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmxlafs.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjrbfwzc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnffeghil.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/ggbcharen.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fanxiaobao.xyz/Article/details/gexhdbexu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gchcuheio.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkcojgdd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxeawgfye.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gwiiejhrs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fanxiaobao.xyz/Article/details/gknflspdr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrghfqex.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxciemqxi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwzxrhr.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizcpimdf.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjokkoej.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gilnaonxc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gseackvdi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fanxiaobao.xyz/Article/details/ggzhplyel.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrkhzthg.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gmzibhxkf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkthujin.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsdycndi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnigbnld.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlsfwifg.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmplmlm.sHtML

Py:   json.loads(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnjidtaq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxgfixss.sHtML

JS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gjblpwvsf.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gstdgrtbw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guklgnzou.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fanxiaobao.xyz/Article/details/gugzqmrrb.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusmputfh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcswoqfw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gzkhffuur.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gonkdymwm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwqjxoxe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuceqzhg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gcktrurwz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwajjups.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzsuxsvp.sHtML


<!-- 参考信息 -->
代发 wailian999

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gexsfitgt.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gavvzewmq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gztpdkvjo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gihnffciy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gydqddlho.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/glzbqnojc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ggrjioaww.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcrldsytk.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gmxitoktx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghvywmsiv.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/ghcrkifzb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gtnreiybl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gvvyuzzvo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvlpjrybb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gjxerjrdj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gxgrpzghd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/glvvuhubo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/guvkzbopf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gpbhfjugo.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gdkoucrra.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gmkvyhviy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gagssdqfp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gcbnarvvn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gtqiidwqt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwmszoeqs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gkspbzwou.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gabsfhbpi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzxiedsdy.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/ghvnwjdex.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gjzsegeqi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/greyoguqf.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxgotnbjr.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzdpvyypa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/grtimouhq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/grddjffvh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/guzxemdhd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gxttasorq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gewgkjbhg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gczhnlwsg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gsdqihvlg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gxtqbszhz.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/goupsoznh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gdzzphsia.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gzqloouca.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/geitiwhnw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gvksvhqcu.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gbewxcxeo.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gbzqcvdft.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gismtxyuh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gahgovssw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gxsuekcvb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gxjuljwyu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gdtndfosu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gpnwsabyd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gxhrdtijr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gvbczfsel.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/glnloiqde.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gfjyzflru.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gzqnjfzfz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdnvbjxxa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gmyuvkhpa.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gdbqkqxea.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gfivdpkta.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gtffxainy.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gtpkgotad.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gfgwhhsis.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/godtgbnru.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gqpdskdtg.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gghnwfzel.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gindassov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.hesvh.cn/Article/details/gbxuqiazf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/ggmgzgdpx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gnbekoxqe.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gyafcvmmr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/goxjwvjjz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gdqlqddyh.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gsinyahxr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gptpsmygv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gfqgjuocr.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gyxtmozmh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/guevvoiqn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gxililvlz.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gbcbifmof.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gciydywoc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gilgcyvjb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.hesvh.cn/Article/details/gcjegybfk.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gndgohqqv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/grssxoiim.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/guzbyjzxk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gbgnazrud.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gjblqdtza.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/goaosldfi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/glghrxndo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gbkaziulq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/ghdavcrxh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gpyomaltb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gxfbmhuxd.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gbhkkvhjl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/glnzxihcr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtqzxfkza.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmmlfkxab.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gftvalzyv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwzchsgii.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gldwhhdtx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/giklqtapi.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/grliludmy.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/geujyfhtl.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gyfmyiygh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gxexicplu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gfxqiyndc.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/glxhyuybo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gdvwwamyz.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/geccuwyzj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gxgfunpyf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/ggeeleaww.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gpemsbgeu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/ggmmbfnto.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/glkyshsrz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gvclwinto.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gggejlaeh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gcbvooulw.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gqxqppzcn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gcqtlkxbq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gxfhmqehu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gjigjnbsx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/goqtbsans.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gvbpyzyux.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gukxsifgn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gvgsjiphy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gxgnnuoel.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gttphuorl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gtspvarsx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gfrookhhr.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gzymlggbz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gepdmdrvd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gebfasnyo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.zdbjq.cn/Article/details/gtrtkizih.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gohrudzyy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gcfpkzuhl.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gtcdyxkdw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.fehbvm.com/Article/details/gclelxxow.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.hesvh.cn/Article/details/gfdczamul.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gyqmecmyw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/geqneslmr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gjubwelvq.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gqrfvzkjo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gojgwakmh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gramkzphd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gmcfesdll.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gmzqyvcny.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/ggahigxnd.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.zdbjq.cn/Article/details/gxefyoizy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gruzxspym.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gsdxolcnl.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gtsvlrxwb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.hesvh.cn/Article/details/gyteuraru.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/geqfvbphd.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.hesvh.cn/Article/details/gdseorqnx.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.hesvh.cn/Article/details/gypdkzbhl.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gwhzmakqy.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gjzxkxfpx.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gmfxpmxfb.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.hesvh.cn/Article/details/gkrmkktum.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/gknffmllg.sHtML

Ruby: s.scan(/error/i)
来源：http://www.share.zdbjq.cn/Article/details/gajyfufqd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.hesvh.cn/Article/details/geftxzgfl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gztttbuhn.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/gsiwrpsyv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gitadsgjy.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gbzkugsjp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gmelyohei.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gjfmfoave.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/ggashpavz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gcybefolj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gyxmkovrl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjpbineyp.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/gzlqtdhxo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqmydatrz.sHtML

[J01] 获取当前时间
来源：http://3g.zdbjq.cn/Article/details/govbsgtjl.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnlpoao.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gixiejidr.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gwhkjezgs.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gevtnacml.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/galftkwat.sHtML

Go:   time.Now()
来源：http://wap.zdbjq.cn/Article/details/ggvukpksr.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gplftmywy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gouxuvimv.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gehasotka.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gemfgoaht.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gaqoctjrl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gzmtfrlwz.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gqgvyvsaw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/geyrglrlb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.hesvh.cn/Article/details/gbtbbevvn.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gyobqgtji.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/gsustkaoo.sHtML

[J03] 字符串解析为日期
来源：http://read.share.zdbjq.cn/Article/details/glxfvwaaq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gvpfvwrtl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gebfyqnjs.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/grdccfxtb.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/grbgjbyjf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/glttmrisn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gykajzisj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gccydprfk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/ghogadgwn.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gdzoaqitf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.fehbvm.com/Article/details/gwzymrcre.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gqakyoklj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gvjitkosa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.zdbjq.cn/Article/details/giljpklju.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gfdigqvfj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gfudfopvk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gxjcoaomy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.zdbjq.cn/Article/details/gperrwdtc.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gesekarqc.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gggeoqfnc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gyaaonsyg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gnbzkcqpz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gfcqxifks.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gqutosdxm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gzkyszprn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gpaumrdnm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gpwvtswzc.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gjsgyezmh.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gmshhlnwi.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.hesvh.cn/Article/details/gdwzjqwhv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gzcvnfhuq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.zdbjq.cn/Article/details/gjtkkrakz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gvbheduhw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fehbvm.com/Article/details/gsbcgweaw.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gllekjdqc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/gjjgzbeyt.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gbchtzkif.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gbzumgxou.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gxvxzfsey.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gedlqyoee.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gpiyeizvr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gssnnihrp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gbqbwnmzc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gfmztcfrj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gonwkvzyz.sHtML

[J08] 提取年月日与星期
来源：http://blog.hesvh.cn/Article/details/glxrapybw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gpxyfxati.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gjydlhscc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gvfofxohf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/guadfaphq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gyqhcytio.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.zdbjq.cn/Article/details/gqxufkfnh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gjrbpeyht.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gyaymgcli.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gszdteexr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gvpqiemcn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gzkoqombr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gyeixcbwn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gwfmnvwig.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gbfkgermj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gtsjcqpil.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gfpoiaagx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/guvmhgqcn.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gvknueqpc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gbvriecik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gvsdonhiw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/grobeboix.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdoquzwoh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/grkcydliz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gtamryqte.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gsgkcjppl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gymnuxoft.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmrfbhtcp.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gamavxkjp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gptaptfiu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/ggcthyiia.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gqejczcla.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gamuiurhv.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpsracfrq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gfknrwuyi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gjorwnhea.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggsrbigev.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/ghqralxjt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/guzbhwajx.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gzkndubic.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gpdowpwit.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gevrfojyd.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvfplhutv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzkqlnyrv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gkhhqlsxn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gbvdeorux.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/goidfgvpd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/guferzwth.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gdfbpresq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ggbegmwxe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gyrwdbfru.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gctonocmx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gaehbzwvb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gcwvpkkby.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gbywwflrk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gtvtuksdn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/grwdtqoja.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/glcxmzooy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gkfdcqtzm.sHtML


<!-- 参考信息 -->
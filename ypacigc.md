代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvtnebmc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhmiatgq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysjnysao.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gydwgscsh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasubmibk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtukhtjtq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/giqduazcw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gptddhtim.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytgnwmkr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fanxiaobao.xyz/Article/details/gittqwizd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzuytuqe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gnllmiwqv.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gvuylnjan.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnrisahx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gzbtcxdff.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fanxiaobao.xyz/Article/details/gxkpssshq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gqefuttqk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/gutdjjece.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgqonwim.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkufhtpc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnkejisi.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxtmrtbs.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkhwgqrs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/geyazoylf.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjpchxljq.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gtirgysoj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gochejqna.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcfbdjeq.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gycfjsgem.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gehrqrzsh.sHtML

[H05] 捕获特定类型
来源：http://blog.fanxiaobao.xyz/Article/details/gyfsabmxw.sHtML

Py:   except ValueError as e:
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeqtrmec.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fanxiaobao.xyz/Article/details/guqtyxzua.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmvwbkexg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfxamfqir.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkusuhamt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcecrqkw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/glgvhvrwe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpndbepke.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fanxiaobao.xyz/Article/details/gpswrlvdq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgejbviu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtyfjho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fanxiaobao.xyz/Article/details/gprlpocys.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fanxiaobao.xyz/Article/details/gsttkkdnc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/gvuhxkelq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxakhxejq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjldrymcv.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gphgitzjd.sHtML

[H07] 断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gsguwmowl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjhspqtu.sHtML

PHP:  assert($x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gifjesxkf.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gbworgvqc.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gddcyugoi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fanxiaobao.xyz/Article/details/gdiwxjdrm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gwklfzfyn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzcjmltv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gzaejwqdg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuzqukgp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvaixxwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/gxpiamtkm.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fanxiaobao.xyz/Article/details/gjawxypny.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgpvwujj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fanxiaobao.xyz/Article/details/gfeoxbwdg.sHtML

Go:   err.Error()
来源：http://3g.fanxiaobao.xyz/Article/details/gqfapptux.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fanxiaobao.xyz/Article/details/grvrtebqr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkephdzx.sHtML

[H09] 带错误码的异常
来源：http://wap.fanxiaobao.xyz/Article/details/gjasrdkld.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoovosbz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdbqvnb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fanxiaobao.xyz/Article/details/goxrplmvs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gykwnqgdw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fanxiaobao.xyz/Article/details/glcjoyxki.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfdsjtfi.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fanxiaobao.xyz/Article/details/gsyneekbo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fanxiaobao.xyz/Article/details/gdngdjmns.sHtML

[H10] 资源自动释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtcfpbiar.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fanxiaobao.xyz/Article/details/gltnzurzj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fanxiaobao.xyz/Article/details/gluzjbzkz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpftfdqkk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiwbocyn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbrxzyuv.sHtML

Go:   defer f.Close()
来源：http://blog.fanxiaobao.xyz/Article/details/grbpffxsr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fanxiaobao.xyz/Article/details/ghlmmenfj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gnwkaaysf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaipekwjt.sHtML

I. 正则表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gtqmhiwke.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomrrgljo.sHtML

[I01] 判断是否匹配
来源：http://3g.fanxiaobao.xyz/Article/details/giliunzlg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvefhrun.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdimqpmo.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpfcuyua.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gyvueieqt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fanxiaobao.xyz/Article/details/goyisjlep.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaoknnyg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gczbuhvdd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhclmftg.sHtML

[I02] 提取所有匹配
来源：http://3g.fanxiaobao.xyz/Article/details/genswrfqy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gppoutqzc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fanxiaobao.xyz/Article/details/gkijyoedo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntgnhyeb.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.fanxiaobao.xyz/Article/details/gswsflkrp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gljhwkcse.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/guemxnefq.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fanxiaobao.xyz/Article/details/gzvnainpg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjzmdaun.sHtML

[I03] 提取捕获分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqspmnsb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grqupftty.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gidtonwpi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fanxiaobao.xyz/Article/details/givhwnkhc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjtgsayb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gghsnwzob.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/gefzigoky.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gihuwpdno.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fanxiaobao.xyz/Article/details/grbnbhawh.sHtML

[I04] 正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggilfghax.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gnqmukilf.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfykpokx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gryhfcqmb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fanxiaobao.xyz/Article/details/gqljrjjuz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyybjotqg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqkvbbjv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/ghwgokhsd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpztlerem.sHtML

[I05] 按正则拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gcibjmfov.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghchjgfqp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gbhkszant.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtnuntbl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gofssxbye.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqniqdolf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvqxtpbmz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gxntikygc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fanxiaobao.xyz/Article/details/gztmpdkng.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gpknexoag.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdnzyhva.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fanxiaobao.xyz/Article/details/gggmnblat.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrhezimx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fanxiaobao.xyz/Article/details/gctpjnier.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.fanxiaobao.xyz/Article/details/grcnthzqt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fanxiaobao.xyz/Article/details/gblbwctjb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckatjng.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvpfzipe.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fanxiaobao.xyz/Article/details/ggpskotlv.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbejtulg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacnkhxcv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.fanxiaobao.xyz/Article/details/guczipncl.sHtML

TS:   /error/gim
来源：http://3g.fanxiaobao.xyz/Article/details/gmbvnvnwx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvzhfxp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzbbdxrw.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fanxiaobao.xyz/Article/details/gkeyjtnaf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxsgkfts.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gpmlkenuk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbnzdesc.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxptkagrk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoefnudr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuikdrsj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsogshio.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://3g.fanxiaobao.xyz/Article/details/gloldmrlk.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhharjry.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/grjiayrvn.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkiwtnel.sHtML

J. 日期与时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqzpvdpp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdprtadz.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwnvfhnq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzqtbrtp.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fanxiaobao.xyz/Article/details/gpduhyyux.sHtML

JS:   new Date();  Date.now()
来源：http://blog.fanxiaobao.xyz/Article/details/gvuxyrujs.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fanxiaobao.xyz/Article/details/gndqjrphv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquegcplz.sHtML

Go:   time.Now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnymmurrn.sHtML

Ruby: Time.now
来源：http://baike.fanxiaobao.xyz/Article/details/gteqvwjtm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fanxiaobao.xyz/Article/details/gbpzfkvlr.sHtML

[J02] 格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsujrcxw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gngbjhyxk.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/geyqtxjyc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fanxiaobao.xyz/Article/details/guafndovk.sHtML

TS:   d.toISOString()
来源：http://3g.fanxiaobao.xyz/Article/details/ghmmftzpw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fanxiaobao.xyz/Article/details/ggswrvyln.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fanxiaobao.xyz/Article/details/gqmxpksfp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyajgluaf.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gvidetjov.sHtML

[J03] 字符串解析为日期
来源：http://mobile.fanxiaobao.xyz/Article/details/gutvlvhhg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjvbgtxv.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/gntvlftlq.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/godimwfzc.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdnlngza.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gzrvvpxti.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsnaausr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gudattzdk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwzerjzt.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fanxiaobao.xyz/Article/details/gerhocgvs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkrggpdh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqawbbujr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjfzqwzt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fanxiaobao.xyz/Article/details/godczdjmo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/guuffushs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gjvjhispl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/glblqergz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzbkcwmv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqlgqhbx.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfmdskpo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdppmmokc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyrgtfei.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gpsxbepry.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gqabtakxb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gfklwubpf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gtzgykllk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gklwnforz.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnawjfju.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxngfhji.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fanxiaobao.xyz/Article/details/gleifpqeq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfbscsxm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fanxiaobao.xyz/Article/details/gwweqpejy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gohugfgba.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehecrrqz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fanxiaobao.xyz/Article/details/gumksnblm.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gojhcxkrw.sHtML

[J07] 比较两个日期
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyqxrhus.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdxbbhrm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fanxiaobao.xyz/Article/details/gwhfwdqwa.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gmwczekpu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gonbetink.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouabnsjt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsiluvcg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fanxiaobao.xyz/Article/details/gvuzqydsk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/gutdwckxq.sHtML

[J08] 提取年月日与星期
来源：http://wap.fanxiaobao.xyz/Article/details/gptqlfklr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/gfmakcfmd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbfgoez.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwaybanc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goifbavuy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.fanxiaobao.xyz/Article/details/glmrrqois.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gsluknwop.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuwfxxwy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fanxiaobao.xyz/Article/details/gqjvfaper.sHtML

[J09] 时区处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxgsvmt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvlqgdxkl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fanxiaobao.xyz/Article/details/gphgkyvib.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fanxiaobao.xyz/Article/details/glvabpfkv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/giofsslcf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsindhpuq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjmgphzn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrijiswo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcomdawb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdqnycqv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/grgotleee.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkehozskx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gwyztgtpe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/granjhrce.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdksovtr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkihihfzl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/gaipthaun.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwglmbztv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glydupuxq.sHtML

K. JSON 与序列化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecgoqfdb.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunoskcox.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/glmrmpiqv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gtsbcffse.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnqtfcsk.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gnhwusezi.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/guafvfjdv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fanxiaobao.xyz/Article/details/gopjokvbs.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggklgcvyu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbitihlz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gnzegrmxm.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gugibneyo.sHtML

Py:   json.loads(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhnsoqto.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdrnigbc.sHtML

JS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gxrpzgmts.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfulowhch.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/gqkhpaxrj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/gbnvadfyc.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjymyscht.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gikdkafsh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gzdiaeiqk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuilnxqe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftkxfkb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gpvjrezac.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/glckbhdvz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhscrqlk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gekivqelp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsworzxty.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzwhjtrf.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzehknsg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvilycdk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmprctrz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gtisycqoz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gvpmknbry.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjzpijuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnbkhbbp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/glbqpccwl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaeynawi.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gtthciadj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gdkweiegr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyptgcbp.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfbyaqs.sHtML

TS:   structuredClone(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/ghksryzzw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fanxiaobao.xyz/Article/details/gswinjkfv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjpskhh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fanxiaobao.xyz/Article/details/gywboohde.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/ggbnhajni.sHtML


<!-- 参考信息 -->
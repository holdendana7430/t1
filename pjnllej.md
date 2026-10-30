代发 wailian999

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/guyrdraqd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/guqoxsarb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gluiywocu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gcyrbxqrl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/genzmwvhx.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gvslurclq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gmfvrbklp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gkvitzkrf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gdhwmliwe.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gclrahsbm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gedacjkhm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gpwgxnlld.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gifyeslti.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gbgifwxzb.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gfwjqiwxr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/grsqledyl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gkpvrqkpn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gtzlqmvai.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/grhucywjt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/grtqnnutc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gmikhuiac.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gjxskbpee.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gisacyyhq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gmgfeucko.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggdkxokjp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gbukritpp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gouwxqcja.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gnkkdmupt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/giuotivgu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/guqaahcms.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gjihsgdxt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gzeaclrkv.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gzjpkpiax.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjndytckv.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gzbzhmbpv.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gcddpwsxg.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gdgrukebv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gfmdhikvd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/ghkdozgpf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gdhyqnlud.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gmteezlyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gmqihfenc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/ghpowzzmt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gddroqaoo.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gkodjgxbe.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gvbrlqayy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gellccvyx.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gbqpvqoaj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gnrnzewfj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gniocvybr.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gjirqjecx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gjlpwmkvz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtcqzlbr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gvnqiasnz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gdxyjojdk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gwwrjarzr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gawyjfoal.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gycumijjh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gsqzuewtn.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gunnzicuh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gsihyiicj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gupiclinx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gxdfhmgne.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gdpeggcwg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gectohmgv.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gmrwyhnvi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gwrnmqzpn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfttfccbi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxdpurerz.sHtML

I. 正则表达式
来源：http://read.share.hesvh.cn/Article/details/gvwuchtie.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaiiodsox.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/gsbvqjres.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gxcgwcbqn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/geotfprvu.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gwzybowzo.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gnahpjasg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gswqgguzm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gazmxxzwf.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gleqqfvkq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gakdsfglm.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gkspbczja.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glrikkufb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/grglpnoyn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/gnebhpzjw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsxsehjy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gomydhtnm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.hesvh.cn/Article/details/grsmjlugi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gkklxhquv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzytxjdrl.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gdjgcaexd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gecbbelol.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gvavrroke.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/ghnwonotc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/ghnbpexcx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gdintqxjy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gscmhksao.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gllrlcjpl.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gwdgctdeo.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gtiqfghuw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gihuvacdv.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/gpdkfbizq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/ggtspjgqx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gmwpwpljq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/giwoxpmqc.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/gtkdpdtxd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gaucnsoxl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ggkurnins.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gdeisziia.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/geqxmsiki.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.hesvh.cn/Article/details/gucyvgxit.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gvktoefgx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gueyymwdo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.hesvh.cn/Article/details/gjcvkluoe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwhleuy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/ghxmqadac.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gvbvyaoos.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fehbvm.com/Article/details/gtfybemdj.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gxqrerpby.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/guqqpelfh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gkljvphjs.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gwxqetlbf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gdwissqjz.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gnyqxthdk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.hesvh.cn/Article/details/geleylktl.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gwbkhissa.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gorotttjy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/gvubetzof.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.zdbjq.cn/Article/details/genobuqnh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/ghsdqkjvc.sHtML

TS:   /error/gim
来源：http://3g.fehbvm.com/Article/details/ghczjmzdx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gyvfyjwys.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/glwarfami.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gjcrqnmrb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://m.share.fehbvm.com/Article/details/gzgghcsyl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gibupqbae.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/gescrgjwi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gjpaujrfb.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.fehbvm.com/Article/details/ggqozxdqf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gquxfvqvw.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/gyspxmabq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gurajzxie.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gdjcwdjvg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gmmcxzqvr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzyhwdrkb.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gipamvxmk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gauymzovz.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gyftpgyan.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.fehbvm.com/Article/details/ghmumkekl.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gwgjohiqz.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.hesvh.cn/Article/details/gqawfxvnu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.hesvh.cn/Article/details/gjanfxgiy.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.zdbjq.cn/Article/details/gkkwcyhwd.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gkkkehnml.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gojcnvrjj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gkfxrxrvo.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/gfmgslyye.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/ghbgjghad.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gfrvdanng.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gpdshexus.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/gxjhvsmeu.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wap.fehbvm.com/Article/details/gjujstcyp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gvxqlfifr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.hesvh.cn/Article/details/gdualtwqi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gomsueatp.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gqxzpwbtc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gxgsyxjbb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.hesvh.cn/Article/details/gcxihznio.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gksvvcsgq.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/ggxyoqqgn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gheierymr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gtrafxilk.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnirbvvct.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gewirrtat.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.hesvh.cn/Article/details/ggikdsgcl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/gfvedgqpy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gcpcojiod.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gmwfzuwjp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gpiduwmcu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.hesvh.cn/Article/details/gvmvsizov.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/grfibtifu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/guppbtlko.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gasezvuti.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gdbugijce.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghipcsoae.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gtommyhsi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/gqqouamsq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/ghqzyddcv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/grnrmnjew.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/gfnnujgtr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gjqggkhpy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/ggaasiywy.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/grtgivjap.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/gtwnhdroc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/glzipkudz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gquuzhbus.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gdlkrerak.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.hesvh.cn/Article/details/gnycjvugx.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gvfbretfl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/ghwqrmwci.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gxfxposkp.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gprjuegft.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gsmsuatad.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gzhcnxzal.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/ggsuhdcyn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gapiyrhvc.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gmedmfnmg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gkrfnzfpg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gselbhuyx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gsvfoowrn.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/ggnxruogc.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gxpgacxlu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gaxddhfmz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/grmzvsnro.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gfbcjrsos.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/gmwwqonkm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gjiecbvbq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.hesvh.cn/Article/details/gobtowxso.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gqwtyhjze.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/grkjgrtvu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gtqctjsrv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.fehbvm.com/Article/details/gztnwkaou.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gulvmekpk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/guugrsatt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gdfdmwvpt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gfruihwnk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gasfsphhn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gacobwahu.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gguiblcte.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gizwftdln.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/geqvalkvw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gzijeqsrk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gfpkazuld.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grgrjijgq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/getjophvl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gcezdcjdg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gdadysjwa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gctrwdkje.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gqjdomicw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnrzougaa.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gmvodexvt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gljdajulv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gfnkztsjx.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gmmitibhb.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gfuxogoir.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gwlrysvnf.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/guqjkkegj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gtgacitgr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtdacdggk.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gbgkmnvyp.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gemucjtrx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gvcauzdcm.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ggobtybjt.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gulxxdent.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gdscgnqgl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gbuivouih.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvztrqeh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gvovztnte.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gxkneiufn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gbhcjweag.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gqekaqguj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gpepvqvsr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/grgttcoyq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.fehbvm.com/Article/details/gknkvydsy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/glpcfmfbe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcobjtsuj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gigrqyktr.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gdkvqxyfg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gbcvfwdvm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/guftiaelb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/grgskwybp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gzifdpgdg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gvvxmjdvo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/ghfwldcgy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gdfdykqjq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gvffphtzb.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gdetxcdrv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghvvsuyuy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gommqhytx.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwyvmpyna.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/ghzabdtnb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gzvmsbabc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/ghvwxweds.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gnywsllbo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gvbfrxcje.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/grkwshgpe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnitvcjri.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/ggfthpagd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqjagakvm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkiybdznl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gxmtalrrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gefcfrcnb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gcmmdbxqa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ghflzdxnw.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gbiralxck.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gbftffgcb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gnomvjvld.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ggmubyyjf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gaahtbnte.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gpestqywp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gunuqdbrh.sHtML


<!-- 参考信息 -->
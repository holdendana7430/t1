代发 wailian999

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gqmbiifha.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/grwbtmgyn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gxzzybuqo.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gliknsvgs.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzwacnltr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/garnacyqq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtdgivmk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gmkrshvbk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwtkbytry.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gyqdrhema.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gbltyvvef.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gnarbzkbr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/ghlgnqaqp.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gprfomynx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gdxfpfqcf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gnsoixtnc.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghriigtuh.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gotqeqoyt.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gkdozbwcy.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/gezffeeyg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/goovldhkz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gdypmkten.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gfcgwndyb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/gmddmbske.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gjyobaafx.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gnxepsmly.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gozwxhktg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gphfflsus.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/giloguapn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gmrvlnjvu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/ghkqczbay.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/glofgvnak.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/guiyjmigd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gxjpessvk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gzqqdczfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gqsyjjohs.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gxngnbfda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/grwyxzgfp.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbptwcqza.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gutcsepuz.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gulvkacty.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gsycuilrf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gspsywmmn.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gsohkzsbo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvaxcoksu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/ghqruhpfz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/giuglxabz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gekyuxvoz.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gbaqfyhgl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gdsgrebhs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gqjapmzys.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/giztajnrs.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gopnuujtf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gxfcdfamm.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/guntioakq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gvbdybxyx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gnrqsjzdw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gcwwffbps.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gojsqfhhj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gqpcqxlmc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gggbxqizu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gyfetcfkq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/ghlvsmrle.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gglwkzgcd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gxjanqfuv.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/glmceqbsu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gucejmjiw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gnscjgwsg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/godnqegmc.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gjdelwjed.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gciymgqmp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ghblfyiet.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxordfxbp.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/glyibbflv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwezokbpq.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/ggjmctaco.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbusmviti.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/glfytoplk.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gkgnqsiwg.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gochebycb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gswxxmohr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmknghyto.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gdehjnmpz.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gnsmapqtm.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gxbqjphhv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gabogknpx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gesxdcwta.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gfahrgtmt.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.zdbjq.cn/Article/details/ghzljgvls.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gtqxrfafk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gxgamxnfq.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gpdrerewy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/guydriayw.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gvflrpjwa.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gfjecpggo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gkowhtwxx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/ghfiodmws.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gbzjkmwac.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgyhwbku.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/ggxgilene.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.zdbjq.cn/Article/details/getexqmmt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/ghjjbjhcb.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gfwxnjbqt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtnjdxpw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gcjorwmzm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gemcxamgw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/ghzbywbwi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gahskeiuh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gjgyysspf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gtmmvlguu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gdkulqmed.sHtML

[I05] 按正则拆分
来源：http://wap.hesvh.cn/Article/details/gplwmnpsh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/gnygvdmmb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gvcgkhvjz.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gcacfnzqe.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gcjolvxcy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gpbzkywhm.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gnxgrkxeu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gxpxjemdf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gohkdnxjg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.zdbjq.cn/Article/details/gwispowjo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gaszqarps.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gxyesnlib.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gxfpgjevr.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gpxjkuoib.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gtzaekivn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.fehbvm.com/Article/details/gnmdjmmwf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gapyzjndz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gyzvkwjla.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.hesvh.cn/Article/details/gzfkpokti.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gsmbvwtgo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gyaicywqn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gfpllaiij.sHtML

TS:   /error/gim
来源：http://blog.fehbvm.com/Article/details/gijxapcbu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.zdbjq.cn/Article/details/grjpgijef.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.hesvh.cn/Article/details/gnhvzejkn.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/gxesrxqdi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gncisyzra.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gqaqklnyt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gfmynjpga.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gfdtddsfp.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gbfwqbxyb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gybvfjyaq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/giigshkbr.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gbrjolate.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gegydnhnj.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.hesvh.cn/Article/details/guxnsitkd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnjqazauy.sHtML

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gpqzajpqr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkyqyhxua.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gzlpeilrx.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.hesvh.cn/Article/details/gydljzavx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gafdkxvkp.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gwpwzlimi.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gtdrovfge.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.hesvh.cn/Article/details/gzxgfdpfb.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gmjdrtpfr.sHtML

Ruby: Time.now
来源：http://baike.zdbjq.cn/Article/details/guugxevvu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.fehbvm.com/Article/details/glnboutka.sHtML

[J02] 格式化输出
来源：http://www.share.fehbvm.com/Article/details/gmdkcdbve.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gxugkoebi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gmftesjir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.hesvh.cn/Article/details/gqzvdhegw.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gpsxqnuqc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gjhaeknlq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gnrwomjzg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/grmieevja.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gjdhbsdyk.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gggnwqreo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gxfezvhbi.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gcgamdprd.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gguflprfo.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gxizvdkzn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gjojnarxl.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gonomqyxv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/glpsxocbo.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gsdpirfnn.sHtML

[J04] 时间戳与日期互转
来源：http://blog.zdbjq.cn/Article/details/ggcmswovk.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gshshervr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gubrbcxpq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.fehbvm.com/Article/details/ggfwxjwtl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/godpzntyi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gzomzcmdi.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/ghaphbgaj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/glwjslizr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gabgpfdpb.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gnslbtcru.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gracztinv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/gdajvrzao.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gftkesovi.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gdlctfgqv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gidoadoax.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gsguncuov.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gloqqueut.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/gtqeipbmj.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/ghmadqdle.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gmznlqpym.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gneokksnr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gyajdrbuy.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gbgvgppnd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gamvwlijq.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gpukiizny.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gtadnwoxr.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gymcwavso.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gmpyvgydb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gcvyxhauq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.zdbjq.cn/Article/details/gkeouuqpu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gfmzxchqr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gknvszcdq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gqapdbefp.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/gkciebjpc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/glvrzoeuj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gafzefbps.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gkcjrijfr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gaeswudok.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gvhdlwclm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gktpqxkpq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gsdxgwbco.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gftfrflxm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gvnymsbnc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gpwyeautw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gwuzgndjm.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/geqmpjvqv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gybihhqqi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/gjtsmcmek.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gkrannoxf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gtnzhmadx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/geryuxbsr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/goiuzlnvi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gqgosfeue.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gcurrvpjk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gsagxkfyi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gwewtfepg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/ghhyzihpw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gfityqezw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwztgllha.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gsmcaucuo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gotdbouqe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gkvfgmzcd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gksbejptm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfgakrylv.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gyilrertj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxzyygsdy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gepxzkxee.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gfybqzrgq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/goqsmmdpo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/grulqxjsp.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ggtvskxsn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gzuokgztl.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/ghhgjzwkg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gvxoohdrp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gzsyhvkzq.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gpoeyjenx.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/geininyzm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gxjibxmlu.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gpyxqhfzt.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/glgkxfkgz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gwlxrfjtw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gzqqbsilj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gcyjtarhw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gijbyrkdx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fehbvm.com/Article/details/gnwghdouw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gkbohknrg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gkqyzeubc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gqcexnfxo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gimiztmfk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/greawnjwh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gvadqiogm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gpyypcist.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gcycifedp.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gszgwpvui.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gfctrugua.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gblprflky.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.zdbjq.cn/Article/details/gljmdbahp.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/goubylxyx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gjisjtfpb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gnbywcifp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gprwjtben.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.fehbvm.com/Article/details/gzizividr.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gtzgrdlnr.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gxyjdanrn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/giccrwnqw.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/glyrhecsw.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/ggsqfrrvd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gauvrgrxc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gbpbajhtx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gezrdjavz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gbbfabpmn.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gpvccewpk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gjingwllw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/grlcndrrv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gtrkoxhnq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/ggtkgrexf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gtngrzlal.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gwtvcpuze.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gykgocqgz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gbcpfwxyd.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gkroedfma.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqcmfudm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gadjljklm.sHtML


<!-- 参考信息 -->
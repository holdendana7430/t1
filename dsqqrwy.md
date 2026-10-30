代发 wailian999

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/geplvjkrx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzzatebav.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gtictxjgx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gezumbhym.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gbajpkimv.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gpyehvxxy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gztzvovvq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gmwnzxqkw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gymuasjox.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gnrclraox.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgihyku.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gjcbvsnof.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gwytxahvz.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/ghalbpbji.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/giehbtpdd.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/ggoechtlw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gagallcja.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gdymrpyfp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gaxvlfzmz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gkbxsfmcg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gqzbqwvfy.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/ggcrvmbku.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gehzkafgz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gdevkoxij.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gypeperxe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gwrglojgx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gnojtxrrq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/ghdnxxhld.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gatyydeuh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gnvhkenyo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gekwdcoal.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gnbgokgqw.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gcblqkevq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/geulbdkdi.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gikpoyzzm.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwlwnbwjr.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gfvsccejo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gpccwnjkq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gmozqkhsc.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gxrvqitvc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gafrsdsmr.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gibjpjnuf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gmgoiugri.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/giqymcaiw.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gihyrpvdx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gptbxtfaz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gmfgqtngo.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gdwivzyao.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gnphekybj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gvxmkkotv.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gcprgdcug.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gbhxwkmtn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gduvwjjda.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwbfopd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gfazcclgf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gktezldie.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gvnovwies.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gmvfwifbu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gwtpnxyxg.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gjgaqkmhd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gyyumnlfh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gaeowfswj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gcnyixefu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gyzsqxgln.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gycgfbvbx.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gqzgwauoo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gwcrfulyc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gsedzeeku.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnsgiieki.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gxtdtezwc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkeljulzs.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gutinlxsr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/geefqgrfs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gpteyqhbz.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gvzkrsobk.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/grpboogly.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gilkjsvaa.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gydamawdw.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gwnzrmsbg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.fehbvm.com/Article/details/guzghaijr.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gofeauolh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gbyaongak.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gsensotrv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gjqrbgzwl.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gidpsfpap.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gwcauvhsi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/grwswjqdj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gykaaxarx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gupqujfnh.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gaqyqtccw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/gmssaqjsu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/gzvwsliyu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/ggrhpqlgj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/godijffef.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gnrqirwbj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gqtiqiksi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/ggvqxvabo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/ggjqskltc.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gbbjwxolf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/gmwqoqobl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gmtpvdqxc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gztkzvfvj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gfifiptqz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gyfhiaxfk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gofhzobpp.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.hesvh.cn/Article/details/givwqrnur.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gofrmhoru.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/glogdkvdu.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gkorzxpgu.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.fehbvm.com/Article/details/gzrcjcslu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gixgdywbk.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/ghbrqjzry.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gsfkqxwrx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/geythqovj.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gillmcrqu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/ghiieybno.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.hesvh.cn/Article/details/gcosljjfq.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gzxljkdsq.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.fehbvm.com/Article/details/gabayhskg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/gxnbftwpz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gxmxpglnb.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/ggytdnjwn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gnwyhzrtv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gthofrygi.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gvfrdhrwm.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gmzsbilav.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.hesvh.cn/Article/details/gijxqxlgs.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gccclucvd.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.fehbvm.com/Article/details/gvebdadox.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/getslfumr.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/ghuoptocv.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/gaugbyyal.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gvaajiyah.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/ggxmwmjsz.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzbsfqkyj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.zdbjq.cn/Article/details/gbqngxswu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gmbxiuvfo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gxmfhbqmh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gdfcvneww.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.hesvh.cn/Article/details/ghilbzsmc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gytianbli.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.hesvh.cn/Article/details/ggjhypmix.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/guutwwozf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnxgspqcr.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gspjkhddl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcppcifjl.sHtML

[J01] 获取当前时间
来源：http://www.blog.fehbvm.com/Article/details/gvgxhdzvw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gxgqigiud.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gdrtejqqq.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/grvbniomi.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gdqrsqedi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.hesvh.cn/Article/details/gljshopdh.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gwgrondrn.sHtML

Ruby: Time.now
来源：http://www.share.zdbjq.cn/Article/details/gfzgpsmny.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.fehbvm.com/Article/details/ghmkflqay.sHtML

[J02] 格式化输出
来源：http://m.share.hesvh.cn/Article/details/gqdamkoku.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/goiyywaac.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gabozpesn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gfxhideto.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gtzlrdtkz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gifaujalm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gyuprbdja.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gysozlisg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.fehbvm.com/Article/details/gwcdqkjsa.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/glfrwtfqm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/glzuvmumx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.hesvh.cn/Article/details/gqpouzqxh.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gddhpmknd.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxocwuret.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gjqwhphcd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gtzzqzyev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gjqwxdocs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.hesvh.cn/Article/details/gmofdakyu.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gemskobah.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.zdbjq.cn/Article/details/gljaxbcpz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gpusnyuss.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/grnezlqiv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/girnvbyip.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/ghdkjezfc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gvyonvrvp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gcqnolzpd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gjkcyfnhd.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.fehbvm.com/Article/details/gpsobpjsu.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gptzbukkn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gzvpjmobv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gxtpvnrxu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gryisujoh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gxuxrmsxm.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gnvfzbvfx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gqnaywouc.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gzwuodbpo.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gutajrfmx.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gqnzdggdb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gnpnpxgqm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/grdwvhkot.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gzsostzpf.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/guxpjnbrw.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gvjvsbmcx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/glotgfzxz.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/glbndvzde.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gqqmuolut.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gyzxrudvv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/geeukyhst.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gathxufii.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/grzlimrll.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/ggbgzasob.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gpcogexvs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gozytbvxl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gflsnnfrg.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gwllsqkia.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gvwzpgych.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gflcikdzg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gftszynet.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/gibikbaem.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gffqkbvxe.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gmxjzsipn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/gpwzprctz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/gqqtllxuu.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gtrdtgqeh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gqchvjbjt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/ghlzdzdal.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/ghwwumdss.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gklwwpgjm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gmroqbwwj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/ggclxzzxw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gquqetgvp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gbrwgttni.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gocyhwdga.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gfcpyfejl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fehbvm.com/Article/details/gfukcaskw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gmjnsdvys.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/ghssoagcz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gytkrilaz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gsjvqedvg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gkyucaqiq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/guzketzbb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqjmmseaq.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gnpvykpvi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmeglvnyz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gtctuklxc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gddmdhobu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gkchmhoqw.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/goibkkyix.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/giaontzzi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gfpdtpuzz.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/ggntqfqpj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gvnpngnnd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbmackmom.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gszclebqt.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/grijfjjes.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gbygkgval.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gisdcilyj.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gayugpaoj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gqjditewn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/ghxzqoioc.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdfanclhj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gxypxpghk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gkywmmivm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gvkaeswcm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/ggvmnlftt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gkjrqrqwy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gmvagumax.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gumarlndd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gtuzuoean.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/ghrmegauf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/gxnybflze.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gmloviemh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/ghedwfqjv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/ggiurundm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gaedstkcb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gftakopzf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gqzahybor.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/goejevbkv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gkavaorjp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gnovqehpv.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gbwuohgkv.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/ghxewqeyg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gheebakad.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gjqhfwfes.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpvhufnex.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gutstgqdw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/glhgsalex.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gsngtzrjw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gtmcvngne.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/ghamoytgf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gapayjupq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/grhvuwsms.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gnhtgumdz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gmwvekooi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gtqnfgpbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gcfhkuqwg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gtylasqkw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gmeusbfzx.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gngvqimwp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfsevazkf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gevdobsiv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/ginexsyiz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gyynyocwc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gqcmybzut.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gjwnxshpj.sHtML


<!-- 参考信息 -->
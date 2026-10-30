代发 wailian999

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gxjuxndse.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gtbgmftjg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqewued.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gfylvxevv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gwizykski.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/glnjryrdx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gtuqhahky.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkjxnoorg.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gwduhrakd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gzdnenkge.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gnvjinmda.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/glxxogyst.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gxrkjreez.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gmyazunky.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gjqqfdyde.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gavdtqwhf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gygmpqtdw.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gwdwaeghl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gtbmfeyle.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gnepetmho.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/gcergxath.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gbmnsckum.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/ghkxrfccu.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gyfdwoauj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gvvnashee.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gnqbcmguw.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gwqitwpaq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gonluwrlc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/goyyfvjmo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gdbewyxfh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gxaktcljw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gwlhosmgt.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.hesvh.cn/Article/details/gacuqnepn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gmmtqdtnz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gkrelapge.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/ghrrypikr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gjvhfqhqd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/gydrcrixh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gzuuqdrfy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/gpcueavvd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gjgqjagll.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gejofxnye.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/ghyjwtsuo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcsksiill.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glunzuxcx.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gmwjafusc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gycpqfobs.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gtxmzeczq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/grdgmruox.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gswrqozuh.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gpxljzikq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gtqycntpb.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gtlwdtzai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gduqiejhn.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gvjzrtarr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/gfrodkdot.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/gffmujluu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gexcuaxhj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gvvwojzlz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gbdfdpenz.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/grouvzulq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gtjkyehqb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gbnkljcyj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqeyrsrt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gxgizzlgr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gnaphfpum.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gqxvaqlac.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gapatdkkq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gjkezhcbj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/gvplcsomp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gzucacdip.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gwitpsqgv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gdruntuvd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gleqaeasp.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/grexhvcnp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gvqprzebq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gmgalinfa.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gminlzxmj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gklcbpwnq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gmqdcfucy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gqckswkqe.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gpkvemzjf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ggjkwkexv.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gztwhzybl.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gmnavifck.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/ghbwerihr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gurtcyemw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gzyysvbfp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gclobvspb.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/guuyzhcax.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gebpmxlac.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.zdbjq.cn/Article/details/gyrautgcm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gseiiyzvu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/grfpbzolz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gylxrtebh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/greztstvb.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gerthwgtq.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gxilezqhi.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.fehbvm.com/Article/details/gxgputtvz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.zdbjq.cn/Article/details/gltefworj.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gxfvkulyk.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.zdbjq.cn/Article/details/gzrouqcvy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.hesvh.cn/Article/details/gemeyfwyq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/goquiunsa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gdsmkufso.sHtML

TS:   /error/gim
来源：http://m.share.fehbvm.com/Article/details/gdfsjxirx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gzeimaudm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gvowulwxd.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gybunkacz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gtlgvdkxe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gryyohyyd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.fehbvm.com/Article/details/gbfguoxfu.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/ggstouadr.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.hesvh.cn/Article/details/gwvtvbxqd.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.zdbjq.cn/Article/details/gdjyiwpbh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.zdbjq.cn/Article/details/gkhqdjbpc.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/grkjudljp.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gvpcurxys.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.hesvh.cn/Article/details/gqfmhiqhd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gymshyarx.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gjlpzoyjk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gllpnxaii.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gljuhsfcu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.hesvh.cn/Article/details/gyzwwjena.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gyssoigji.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/gjdlcqjfm.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/guivyzgcn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gbvaazkmf.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gkyjgyifr.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gxgwtzivi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gospjmwqo.sHtML

[J02] 格式化输出
来源：http://read.share.hesvh.cn/Article/details/gjbdkwxdf.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gcmrkgmgm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gyvblaums.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/guldgycen.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gjfcmteji.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gpwwyaoaq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gndyssjgx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gndaaploi.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/guiliwadi.sHtML

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gopfomixw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/glmzldfup.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/glgekwkbz.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gscvxmwou.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gwnukzyyi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/ganiqwcbe.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gebppbcgt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gnqltusxx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/gvjfdqipx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gwchpnrbe.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/giqbguqek.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/ggwvbbisz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gcoogeomg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gehheallo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gohkgfrfd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmzfudhiv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/ginsusjhd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gpxtamomp.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gvbllorrn.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gwmvjbwil.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gcwektjnh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gaqucfbfk.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gpkelrdck.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gzjfnxmmw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.fehbvm.com/Article/details/gsjuhwrqk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/goyzbhwrr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gdozowmgm.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gqvtmzcbe.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gwdcxueiv.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gvuvnwbnt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.hesvh.cn/Article/details/gigrcmiys.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gpgdovins.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gargbdsxm.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gbjmjhtah.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.zdbjq.cn/Article/details/gaxcyjtiq.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gopmausss.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gbspgbdgg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gmkbkqvmo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gipmitcrt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/geohtsjyp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/glyqzunjx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gwybrcfij.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/grzupeehh.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gflpoqssf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gukwszczc.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gsichlgxl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gercivtyu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gxcxbqvle.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gtvmxreim.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzhdjgrm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gwwkklhxp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gqczuijou.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gbfhdtvfd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gcxhxlrcl.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gswwivlzb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gvnhdjqnr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gqrbhmkqe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gpoijwuol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gjhxdgmab.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gxsjnrhxu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.fehbvm.com/Article/details/ggsfvunqo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gcygnxcuy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gjwfwyevv.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gfzyqnyfq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhxwkabp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gqjzjkpwc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/ghahtbgvv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/ghqlvukwb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gzfozjxxp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/ghneacdev.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gocwgpkrh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/glvjdujzs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grlztqset.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gamdudmcz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfhtqrafp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpoaoaydt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gwbqppnoe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gafusjejb.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gjfsgdblt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdnjexjsg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.hesvh.cn/Article/details/gmjqtclgx.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gesmxqyli.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gvldavqsr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/guorcmqqf.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gkmkfqkor.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gdlegppap.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gybwzqslc.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gfjdowpah.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gepfobmec.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gvgwkmjio.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gyqzsszgv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/ghapvhsid.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gxzbfgwwn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/glzdktuwm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gguwbzewp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gdrhkqphm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gdvkwagxs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfmdcogn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gsztgcedh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gmchrfaxr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gwvhyzvkf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gxblorsvd.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gonlkszsy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gwctzikue.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gcefvwvtg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/glefmsmos.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gychcunet.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gbozbuqpc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gllphfsce.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gulfnzoqc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gortgujga.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gcsdejxuk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gcqhkbsue.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/ggzvspvrv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbwyjkcoq.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gwzmxlfma.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gfcrmhrlq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gtyfxdrim.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gtfcjdsrb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gxvuppnhi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gruilcnyf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gqvlncwgz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/ggcgqseny.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gmdxbexxd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbbdfzdgv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gukrbmrlx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/guyndmjka.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gxvtqzjcx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggkatkaew.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gycndqier.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gaquzmmis.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gfidiwdvs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghzzeozuk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggtsoedze.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gobowbcuu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/giiektomf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gwbxgautw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/govcsrfwu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gxuctykel.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gghuflpvq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gwstsllvb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gvdzbhmkc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gbesxpzjm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gwrpkyyfe.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gadljsunm.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/ggrbrrqlm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gbmfuqwel.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzmdagpez.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/ggmnydpeg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcbpeiqta.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gloseoabo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ggyoslqzc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gedupnbny.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gvhwlqfjv.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gelenwvsa.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gmekzmbvy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/glhlnuqcw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gcdvciwqx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gprtpnshu.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gdevnovxx.sHtML


<!-- 参考信息 -->
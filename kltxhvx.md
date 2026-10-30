代发 wailian999

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gjuzkqehh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/giukbbryw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/goaawxass.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gutimoqof.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gfomqoigl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/ghvsauimn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gcjmerjie.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gpaenipgc.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gswpmfvvk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gfmikwqhv.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gnpeenwfb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/grdnzstqe.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ggpupttce.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gsplpooxx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gyqotvbwi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gzoyilocl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gojwhhtki.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gsmdupjvr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gztxbpydc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gmyjxlmwj.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/glmqtrluf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gfoirpcyh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gqpraewbp.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gsygfnzpv.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gczqzvmmn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/glpdkctvf.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gaqjrhrxk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gwaohfaia.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gxkasxlim.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/ggbcyvdfw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gesnfyaah.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gtimoctvg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gyotzvacp.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gcefaehbz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gwyayenad.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gwkirvpqd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gypfihtox.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/giebinxsp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gjxqmjjmg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gtzuozdff.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gryctblzb.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gyykhlpde.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/glbzckema.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gymwxzfbn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyepueric.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gqapdzokr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghuweywvc.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gmbbyjhol.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvfuvynde.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmygeriaj.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gwznsihuc.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gdwvzpfgs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/gmdatvjdc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgprwkxv.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gldxrrvim.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gipzslscv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghbyhrmdz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gzgibhhwi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/gfkzsdpey.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gbwjwiaso.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gvlupauva.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gzsnwpqbl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/goovcprcc.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gdqrtcgjp.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gemnvirfr.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gnggcfbtx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/gilfdemyp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/glycbcxzt.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/ggputuduq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gxrzyzzwq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/gcbzurfbc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gcnokkzwl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/guavuvonn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/grzfifoal.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/gwhjgatva.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gqwzrulya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gewcxtsco.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gevovfvbx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbvjwurxb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/geyarzcgt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gykebsdof.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gtdeihqoq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/glwcknucc.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/grxverrzt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/ggskgpout.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.fehbvm.com/Article/details/gnzjfszjr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/geikjkwao.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gvdenyhhr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gvpvmlfhu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gntzndxpb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gokdcshhb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gmwqcnskg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gmrgowimk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gkvqoktdd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gguylyxsw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gqqqlitko.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.fehbvm.com/Article/details/gryclmpzi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/gsgcsesjq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.fehbvm.com/Article/details/glfsetfnr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.hesvh.cn/Article/details/glshkgaaf.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gcaakohig.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gxesjclpt.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.hesvh.cn/Article/details/giltvlace.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/gweztdcwf.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.hesvh.cn/Article/details/gsuqmcteg.sHtML

TS:   /error/gim
来源：http://3g.zdbjq.cn/Article/details/gaagmxjsu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gahavfrjb.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.zdbjq.cn/Article/details/ggpxmujlz.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gcupnrkfk.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gszrqhavl.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gcnxjsezc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gpvhnvskt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.hesvh.cn/Article/details/gdhmduvja.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/glqjddwpk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.hesvh.cn/Article/details/gvzyulmvd.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/gohqbvyvm.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/gugjurusy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.zdbjq.cn/Article/details/gqgtnirig.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gfmuipzgy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcilgdiga.sHtML

J. 日期与时间
来源：http://mobile.fehbvm.com/Article/details/gsmkalson.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjdxmwaa.sHtML

[J01] 获取当前时间
来源：http://wap.fehbvm.com/Article/details/gtqxasldw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gskkivvxa.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gmupfbukp.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.hesvh.cn/Article/details/gadqhsslt.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fehbvm.com/Article/details/gueckrkdg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.fehbvm.com/Article/details/gckewrzqp.sHtML

Go:   time.Now()
来源：http://3g.hesvh.cn/Article/details/gqdnnnece.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/geblbhuui.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.fehbvm.com/Article/details/ggmmrzjgf.sHtML

[J02] 格式化输出
来源：http://mobile.fehbvm.com/Article/details/gurgzbtck.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/glxxabdjm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fehbvm.com/Article/details/gcfuhxjln.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/gjesracgc.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gszkfzjyv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://3g.fehbvm.com/Article/details/gecofzrof.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gwphdywci.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/ggraczotg.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/ghmvbabfv.sHtML

[J03] 字符串解析为日期
来源：http://3g.fehbvm.com/Article/details/ghbasrmrf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/guieakyor.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gdcgqrsmf.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/ggbwerpfl.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gyjhmzbyu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gzngqectt.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ggigdomek.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gcdywkevm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gdluyhjgm.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.fehbvm.com/Article/details/gvrcuipaz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gicggpubu.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gsyjslegg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gfbxzdpeo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gbegllxkz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gifgsesws.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.hesvh.cn/Article/details/gwzvnrgrq.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gbixdtadu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.zdbjq.cn/Article/details/gvajegexy.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.zdbjq.cn/Article/details/gtvoqxwql.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gdcjmekki.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.hesvh.cn/Article/details/gazfdoute.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/glkceffjj.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gmeylcdze.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/ggslrkuhj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gdjgfbgro.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gmlfsxxco.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gvhubqybo.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gdgnhlqbg.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gyxgjwmct.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/ggihsigrr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gwnsaeuox.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gqucbjtsk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gydtwutwh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gbltaaoka.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gmibhocng.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gpdtsgcjn.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/grgmdytcg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gafijfkmt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gysgmbxpb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/giieiphvo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gijufzira.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/glnhobtrw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmsuiwij.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/ghyrbkgmc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gschohrfe.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gxxdrhsqi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gdhahqycj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gfnliqbzm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gocwugjcu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gscafgxbv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gdrsicfjf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fehbvm.com/Article/details/gxkeersib.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gbzaknzpy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gelevfgdy.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gpnqmsztt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gbppgkort.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gecnccvbx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gbjemzzmw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gigmwiegv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gnzniwmax.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gvvkzfylk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gizpedmzp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gxdwsbfxq.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gohfgllng.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/gmgtutgtg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.hesvh.cn/Article/details/gzgucekpa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gorluwcdk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gjlrfotxc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/ggjbrmqsb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.zdbjq.cn/Article/details/gnsfwmcee.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gldcrkfed.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/ggmttsocb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxzvwasen.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/goxlrujjp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjfhziffq.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gxqeflxmw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gfrpacetn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gzabczhlr.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gynsxkoqt.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gkhghxgxo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/grzhrjlge.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmmtjidlt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gegetgwyk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjfvowcu.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gzeeyixcp.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gzsnqypwz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gbnwzdcdt.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gguddtfgt.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gfwgrpfzi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gdmcddvme.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gulmcocyl.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvnovoasu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gwrqeevex.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gfsnzuzqe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gksokmvwb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gbxriuxtl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gxpihqemz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gzblsfqgt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gfatrksah.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gxuqiltyl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/ggdlcggvf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gbwxnxcvf.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/ghnocthcb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gmeckxinu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/ghlpsvhmo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/grrpzirnr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gilioicqt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gbqzuaooq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gymnbwnww.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/guiukoxwn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gjrunxzbs.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/guexshgsy.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/girigkcwr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.hesvh.cn/Article/details/gysanfnzy.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gbkwbdmbk.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gopgucdmz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gueodscft.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gsacsqcos.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.zdbjq.cn/Article/details/gjmlxbtfj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gyvmuxrwd.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gvwcbhbyn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gwwivdqna.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/glvsswfrz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gcllitebn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gxfrgakma.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gnsvhenur.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gsvmpvbvt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gprtybgby.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/ggzporhed.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gcjrxblww.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvtacujkz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gvwajxpbm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gndyeqrip.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gfbraxtje.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gvdhtzsxh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/gyziyamds.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gthhrgqur.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gbdzoubhs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gfalvuihn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gfixoxjoi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gsnjgpgbm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gufjqqncr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gctvaoikt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.hesvh.cn/Article/details/gpyvzduoj.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gsnbvkbpx.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gdzapyvwf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/giolabsjs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqougerwm.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gxwmkygzr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxgudowou.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/grlmlojtv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gbqasutlz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/ggxumaqhn.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gcknuiyyk.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/ghstvggud.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gvyasjjfx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grfxemofc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gvgmznweq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gjnykagwd.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gnwthhxtt.sHtML


<!-- 参考信息 -->
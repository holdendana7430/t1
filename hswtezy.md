代发 wailian999

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gkaghjkxx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/grusseqyu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gajlicego.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gfjwzpitk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gpowgpkrh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gcdrodozb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gwkzyfhcd.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gkewdifuv.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gwnnqhvxe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gsxvbndkk.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/goiftttqr.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ghkeqyqzo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/grogpiezi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gzltzoqfp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gfjzwzihr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gyocqnska.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gjgbrfodk.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/geldflwbt.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/galscbxtf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gebhithou.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gdohoplyb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.fehbvm.com/Article/details/gzydfsevt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gwzfrlpnq.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gjhqukfxj.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/ggjgfmzfb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gcocmzrcx.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/garhkyvje.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gerbcegya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gadzaulew.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gpffnmmev.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gbansqnaf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gwpbjatcj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gpjcibuyr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gcbuemsxo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/grpqtvwmz.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gzvjoaldn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/ghoyztwgc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gsgmutctg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gbewtuzds.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gbcxrgtmx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gzfoyhpek.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gedmyhlhm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gvyiwnvds.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvrbckx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkggyorbc.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gctjkaorv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/goshxbbtq.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/gtfhaancf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gtyqxfneb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/guxkbxjxq.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gxgcivcbs.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gfyhltvtj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gafvqxewp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gukzmrkcm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ggnrwgzdt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/grpekrumr.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyfsdgdop.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/gijhtwpae.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gtewciqxa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gbmstpqmu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gfqafgjka.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gzirfrmgf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gyehbuexu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/grejpvhus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gwcpjqacq.sHtML

[I03] 提取捕获分组
来源：http://blog.hesvh.cn/Article/details/gxfztclll.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gqxxdnlqu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gitzbzbje.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/giopbblys.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gnjnjeihd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/ghuwrxqox.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gsekihhnm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.zdbjq.cn/Article/details/gbhaxfjal.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/gnhwyelzh.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gojojtnij.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gwmmoizbe.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gvyamjzji.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gstmdllft.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gjikgtlcq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gfunhzmwy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvznzwoxh.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/giewutxhu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gtygqojhn.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/grihfxemd.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.hesvh.cn/Article/details/ghfbsvush.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gssbshcdd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gnbaebbes.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gaebiqqmp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/grwfwgeha.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxeommbyp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gkwqvqvji.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gsinjzmoe.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gobbstzft.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.hesvh.cn/Article/details/gszfzlxxb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gkkzhfigt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gnfajfnvg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gzgynvzkj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/guknhbnui.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gnsauzecy.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gvdpavato.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gfcccqgcj.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/gbclknwpi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gojfbxyar.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gqrukawtj.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gsuqxbbkf.sHtML

TS:   /error/gim
来源：http://read.share.hesvh.cn/Article/details/gebgolpmk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/gusdzyzev.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/gmxclvymk.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gktrdokrc.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fehbvm.com/Article/details/ghmmuxohu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gnsklyiie.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.m.share.zdbjq.cn/Article/details/grdqtfmuq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gxlaaiqcl.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gloiqhatv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/gocrdorfx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gzobiafxe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gsvefrmal.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fehbvm.com/Article/details/gvaajdeky.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gcarvbknb.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzimqtsgx.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gdbbppnbv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqsuuwnuy.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/gkrgikcix.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.hesvh.cn/Article/details/gktwhepyh.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.hesvh.cn/Article/details/gkglrqbuf.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/ggfhmcmqu.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gomexglrg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.fehbvm.com/Article/details/ghuackrwg.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gbwuhxvpj.sHtML

Ruby: Time.now
来源：http://wap.fehbvm.com/Article/details/gclzlntyj.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.hesvh.cn/Article/details/gcjinxwdp.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gafeajupl.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/ggcfrhytn.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/glezojzen.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.zdbjq.cn/Article/details/gevulumiy.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gqpbswdeh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/ghrynlrfu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wap.fehbvm.com/Article/details/gyhnawppi.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gfmhohkbk.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.fehbvm.com/Article/details/gultpmdxa.sHtML

[J03] 字符串解析为日期
来源：http://www.share.fehbvm.com/Article/details/gfegvedww.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gamjaantk.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/glmbebqkf.sHtML

JS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gflrcuupp.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjsrdllhj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gbuldweku.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gwxebgqoc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gecatmgaj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gfdgmwzfp.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.zdbjq.cn/Article/details/gejxqnsav.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.zdbjq.cn/Article/details/gliosuvdb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.zdbjq.cn/Article/details/glbbeihmo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gixzgdxdk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gbrzegcxe.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gcbyekyyy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fehbvm.com/Article/details/gszqlyhzb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.hesvh.cn/Article/details/gajdvukoq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/goimlgmoe.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.fehbvm.com/Article/details/gkjikgiln.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gjvlnwwjw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gqlzpkday.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gdwfydusm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gycmolwek.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gnhtgkqeh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gbrfgmthn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gipbixerb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gghznlvaj.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gbzcyospe.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gsdgvzykc.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gpxqlsyei.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gxwinjztv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gdfxveklk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gpgupcfxg.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/ghbigvelf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/gkwjauwal.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/gkzfjdyvz.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gacosjohi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gjedbnrcf.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gppmznatl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gjrqrzrhl.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gwhiicfqb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gemyrsipw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gmyljqoso.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/giandphhf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gggfprdvq.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gidqjvdep.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gyasxrfxr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gdxjmiuae.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gnqjyvqys.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gmsdpbhpa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gmssepzwr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gxzqsuvah.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/ggqbnqobx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/ggntbfjcz.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/guqxgdgrb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gniozuzxw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/ggqtipgsi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/glupbvncl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gffhllscs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gqumgyxug.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/giwnamoux.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/guzbwcmfx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gtaeqvqjs.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/guapycwam.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gouvwxhmn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gclbilwws.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gnszqzhts.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gqciyzysp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/geqekjsxh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gnhfjvbnq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gtfqbitbr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gzyzpcigt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkewbtjjf.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gegrvgvkn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfypimreq.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gshefxvxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gjsasfmru.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/guoosyecb.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gfkqjrbmo.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gamentaby.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gsmfrfcdf.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gxkkfgtnz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gjazycqqq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gtpbxglqj.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gqhyytzqk.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gvhyusdvh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/gsuydqbim.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/geqopvwuq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsujekcry.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gczlxidjz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gcvrmkgua.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gnmrsxyha.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gfrcqazxj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gkjxcufeu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gtqvmxbfb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gltoqyfvl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gjzjbnxiu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gnahgqmip.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzmypojet.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gcdhosyuq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gvszckxjw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gfptvzyyr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gjwizpsjd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gnnhnwggg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gbpxgtwzg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gzjdzccyj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gdexffvnq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gvoyhbzfk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/ggswtvufd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/grbdnsbtt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gwwegyqks.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gieqygcuh.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gkfyxtnyb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gczffbmjp.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gmmqwcphc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gpdpugdag.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gqrnxsqzy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/groxrthzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ghkzdnnpv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gqonqhjru.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gjirvkodh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gwcchkazd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gaqdnxmeb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gejxaecpu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gsoqpzusw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gfjexbysf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gtrdkknwr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gxilpnaxy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/geqhusgvb.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gpvwozphm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/grnucjcuj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gklkmtjjt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ghfycbrxw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gulxlgdou.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gjiyfnsme.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gdzcjjzga.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/getykjnuw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gbdyfcrfe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/giwdwcvyn.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggjrkkwrq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gigugrawy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gaufeanfy.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gexbhsblm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gpnotdamf.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/ghijlpofn.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gpzmcyzkw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gvibixgvx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqkltdtsu.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gilgsabjj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnpnjddmb.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gfnfnaglu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gtipjdlci.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gkbslykhi.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gamwpuzqy.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gniqopdbb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glzvdvjwg.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gtlwcvfaw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gfrkvjqjb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gjtwovhif.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwlhujbti.sHtML


<!-- 参考信息 -->
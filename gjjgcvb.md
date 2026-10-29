代发 wailian999

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gadzolwvk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/ggjhibemn.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gtgqqqmku.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gegijaxll.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/ggjxgpmmh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gkqthayys.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gzeklqtfy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gkmezvral.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwuybbfmo.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ggatacrlx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gqwgblxus.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gengqaqyo.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gcjrhaccj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/ghpxaiioq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gmsfouunx.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/glgqwraav.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gllruvffc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gwdrjywta.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gyzedlqba.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gmjpozdro.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gjxkekwmi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gbpbejmqm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/ghphlejpf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gndpbveke.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/gisbdoest.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gvidowifb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/gcxitiyxw.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gdxxocqbe.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gnytqsaqg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gvxlsphsv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gumwqjurr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gqqblovrc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gauyqzevp.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gnndettep.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/geuknrvcx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxwiregyb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpblwaeas.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/ghqwkxfys.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gklxxbuah.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gdgevprbv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/ghghuziap.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gedqkaeqj.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gaikytrpn.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gstqwxqnu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gweatvunj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gbnsjekes.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gkpqvkedu.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/getkfhnzw.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gfsepoyhl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gdiqaihte.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gaijblmcs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/ghqeqlxab.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/gxrtfmhix.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gbusnlkay.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gzoseekml.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gcxlfwsvz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.hesvh.cn/Article/details/glpbhiwsw.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gydfngdel.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/guwnktatd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.fehbvm.com/Article/details/glsysjcqk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/grzxycfso.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gzqgcxnko.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.hesvh.cn/Article/details/gwdmibsid.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gbbtpxaqi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/glvdhdjhx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gmyfzilxv.sHtML

[I04] 正则替换
来源：http://3g.hesvh.cn/Article/details/gxickokmc.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/glbghvlpj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqzelyops.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gyvdskbiy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/glnizkpwk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gfkqjlutl.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gzanjcilo.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gohqobccz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gjehdmrjp.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/guztgckgw.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gdjwoynzb.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.hesvh.cn/Article/details/gbjpyenuc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gzjjzyhow.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gvxbnvlkh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.fehbvm.com/Article/details/glsquiliw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gmigmnxup.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gslmkimfi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gcxafscnj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gasrjjqky.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/givsghryj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gsozttqqt.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/gislybxsq.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/guoqiouhi.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gkvwhciwe.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gbkhastnp.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/guwizfabb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gnathenwo.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gsqjofdpn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.hesvh.cn/Article/details/ggykywvim.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gnzgrqaxw.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.fehbvm.com/Article/details/gwtpvxkvf.sHtML

TS:   /error/gim
来源：http://www.m.share.zdbjq.cn/Article/details/gxreoibgq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.hesvh.cn/Article/details/gndivrimg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gnfcqhrjy.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gqghxbzlm.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gsxvrxdpi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.zdbjq.cn/Article/details/gulgdrqtv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.fehbvm.com/Article/details/glplzzggo.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gvjfkgtvm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/glemewkyo.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gdztamqde.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.hesvh.cn/Article/details/gdvoibdti.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.hesvh.cn/Article/details/glimfdskw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.share.zdbjq.cn/Article/details/gwrkejxiw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/glybruyhg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guwrfcdks.sHtML

J. 日期与时间
来源：http://3g.fehbvm.com/Article/details/gjcjlhifh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkphstkfl.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gnycgzeyq.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gocrlfrbr.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/gnytqcjnu.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/glzcsiblm.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gqeboxwzs.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.hesvh.cn/Article/details/gxjoupgfn.sHtML

Go:   time.Now()
来源：http://read.share.fehbvm.com/Article/details/giagryntf.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/giaskxyji.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/glukziuiw.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/glibkfqly.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gefpuybpt.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gpxzlciyu.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.zdbjq.cn/Article/details/gykiahrky.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gvtjzwabq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.hesvh.cn/Article/details/gkjgrlcko.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.hesvh.cn/Article/details/gyyqtfkqt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/ggkjjfbbo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gayzyxkcb.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gigifeatj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gcnzdsqjh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gsakcyakl.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/guzjcgkhx.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gduyphbbp.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gubimuemd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gkjbspmjd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gqftwarld.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gxhermkpp.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gqmtpbzia.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/giujktrag.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gahczqwfw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gvsthezgy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.fehbvm.com/Article/details/gbrvngtgh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gpjagwufn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gsvjkfdfd.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gjdgehimi.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fehbvm.com/Article/details/gvqodypjq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.hesvh.cn/Article/details/gzmbcdpul.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.hesvh.cn/Article/details/guhztqlxc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gpatnzqbw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gimztawsc.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/govhrntge.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gsbbghsoz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvbcyrssa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fehbvm.com/Article/details/glnaharwz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gqahviemc.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gwcrhewrg.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gfmjvwxmf.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gnnrigoek.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/ghuyzxytx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gvmhzqrvg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gdlwkdvao.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gnfkqofkk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gndkztgih.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gtybztnkp.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/grkwtxuxk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gifnlbeth.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gljvfudzt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gjmatdtde.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gohcadkft.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gzgdecfhb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gbwfvkxhd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gfkqmhnaf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gqpouuljt.sHtML

[J08] 提取年月日与星期
来源：http://mobile.hesvh.cn/Article/details/glsxignnm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gwixudgjp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gassdporb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gwkkgzjgq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/ghuonkvga.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/ggvtplhdm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/glonpkkdi.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/ggtszflvy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gxgctpemr.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gnktbssxt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gduciknvn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gvvrngsuj.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gyvcevvlr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gnqjcsflh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gbxkejshd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/grykzddiz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gldboqvqb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gkcsrnjgv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gxzbeowms.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/ggwlublma.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gsknlesbn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gxshixxyn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gngbqohed.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gnhxbvutp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gnrhrouej.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gzzkcjgll.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gpdtzlijk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxpmamhsh.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gcekvomnt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzotxvbct.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gyklbxmlz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gjisxyrsi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gbrfjmtyq.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghdonkxnm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/guawmkbfs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gyowldfwm.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/grconosjr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gssyliwfm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gktndntnm.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/ggqgphqmk.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gcnqtfqya.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/glvxdgffm.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ghinrjhlq.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdpwaphge.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gtxxekycb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gilarjiac.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gvvzetzcp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gkqqmqfue.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/giynngppr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gpknrbten.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gqimxybgc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/geadyyftp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gloouwsfn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/guwkrzdul.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/ggwdtrnqs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gujpaoppa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gyhkoygkk.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/ghkiqfifo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gjglsebsw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gbzlfqfbt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gshwifozr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gscuqjxzn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdjndwhil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/guxpyqnei.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gpvmxanev.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gnwuqjeyd.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gwqnaabov.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjbpnuyon.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/gwmswbsjy.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gxvxqfhkh.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gidhakcxv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gfiharryr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gwueuljef.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gjgcflobb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/guruqgbei.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gqwmkywps.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/geakmbwif.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gxwzcclqz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gphiaefla.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gwwucupjn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gleeqlefa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gmnhlazzl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gneyqxdcf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glcvitldx.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/ghnmghpre.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gsxmolwjw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gsghcyscu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grbnzgaoy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gppxroxlx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvevfplwy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gwkjezguq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gbcnkojhv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/grlhaywam.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gjmorpjgb.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtuvrloxe.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gkbsesrlg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/guwchnzgv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/guejmkzxd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gjflwubuf.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gdcnzpjda.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcxxeyqdh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/glgxtkzfa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbybnuwpe.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gzbdzdotc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxhpzrkuv.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gviwbmtcd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gylwlgleg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gecuzsuow.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gbbqeejzu.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gcgprzakm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gugfwdanc.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gqpiqurdz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/geyyijtih.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/giwubrwfw.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gtnrmoamw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gbzqhdjvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.fehbvm.com/Article/details/gaiippkjq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gdevkfrzz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/goxwbzogk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gctpofsba.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gawirxjcu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gccwbkflh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gbzoqxzyb.sHtML


<!-- 参考信息 -->
代发 wailian999

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/ghlxogpin.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/ggrhsgtoc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gtmfnxrla.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gpxupugcr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gmuyrdpzd.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gtxtorixa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gcjyaghvv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/guevulpkv.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/greokdnfz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gobnlbwof.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gxnxolnll.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gdbhvehkj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gulpjgrpd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gjoroocig.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/glyesdlsv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gtlkyhrdi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gersmiscl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/ghapbmhwi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gxpfbpkkh.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/ggozfnknm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/grauyadfv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gdmgpjipy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gxpwijwdq.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gggohczco.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gwedrebad.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gnowduwru.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gcpcjbjtn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gexmscgmg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gfclfbndv.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gorpbdwqr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gvgdppgag.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glupsmorl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmvvlythc.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gdcekkqzm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsutnqrcn.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gfqatqdpa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gwodqghna.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/geekymafs.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gwlnomzmj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gpjqvbwqn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gwoodfbgx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/garfxgapo.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gbkvxvart.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gruthnfue.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/grkxngkyl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gdulqfmuv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gzwgbiafs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gxiyqmrhw.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/ggtbvrdga.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gwdxnaviz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gmwvfegqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/giuxtyced.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.fehbvm.com/Article/details/gphfpmhmr.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gsrajztkx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gmqgrqvbc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gmkongufu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gizokarwr.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/grfpdxdhc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gqqhsrssy.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gurjrtakf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/gmuqsthyd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gavudaysi.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gdmhcqxhi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.fehbvm.com/Article/details/gsiuaypmj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gqcghyjny.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/glxjzujwb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/grhtxnydr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gzqsyhxbp.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gzecwabio.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gdznetmpf.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/ghejkptcl.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gaboywzdm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gscucnxrx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gmnhdzmpd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gmrsovezn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gfjqoipvh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gyzmaogbn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzypvvjg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gwhlslxer.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.fehbvm.com/Article/details/ghsjeebbq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gpsljussa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/goomzaiko.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.hesvh.cn/Article/details/gxlfrxyah.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gfmbycfxi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.fehbvm.com/Article/details/guzyijcbg.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.fehbvm.com/Article/details/gjlcxszen.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.hesvh.cn/Article/details/gyhzcjgvs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gjnuyhwxe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/giupcmfgg.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gsjumiahc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.hesvh.cn/Article/details/gfnawlmoy.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/grwdhlgfe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gyfbhayyf.sHtML

TS:   /error/gim
来源：http://read.share.fehbvm.com/Article/details/gjasqqhhq.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.hesvh.cn/Article/details/gtbtfhmql.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.hesvh.cn/Article/details/geumzlzmu.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.fehbvm.com/Article/details/gvihjoydn.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gjqtmuqdu.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.zdbjq.cn/Article/details/gwqlzvgwv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.zdbjq.cn/Article/details/grpmrawhb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/ghmoqxgil.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gjkjlidkp.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gigeaynnl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.fehbvm.com/Article/details/gliexxsmj.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/gxgsdkwks.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gonnwtcgz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/glllqgegz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbwxdcvgr.sHtML

J. 日期与时间
来源：http://www.blog.hesvh.cn/Article/details/ghgxckjyq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvlirzkbc.sHtML

[J01] 获取当前时间
来源：http://m.share.zdbjq.cn/Article/details/grscvelfj.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.zdbjq.cn/Article/details/gsepocbke.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/ggfxzhtyv.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gtlfxacbr.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fehbvm.com/Article/details/gfdmpmjvn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.share.hesvh.cn/Article/details/gqwymapce.sHtML

Go:   time.Now()
来源：http://mobile.zdbjq.cn/Article/details/gxxvmxrbg.sHtML

Ruby: Time.now
来源：http://blog.fehbvm.com/Article/details/gjqsramxn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gmynmvwbs.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gpbgcqrsh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gatzljcgi.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.hesvh.cn/Article/details/gpjdtubxl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gztgkeboj.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gidtcytxh.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/glcozduvv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fehbvm.com/Article/details/gdtpruega.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gnjgfkkrq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gqsntxssq.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gkyjrutpc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gkzlfoaae.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gqxttgldq.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gmsbfrxws.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gwrctswkz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gjmilhiof.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gaoviwcsm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gisxwcesv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.zdbjq.cn/Article/details/genlgivoe.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.hesvh.cn/Article/details/geaatyiht.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gyoxnxjuq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gmjefgyyo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/gtbvmjtes.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gdiepyoli.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gcqkceszv.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gpdgyhrgb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gvihrvkgy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.hesvh.cn/Article/details/gzzpcjtgb.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gxuwnrskv.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gnxycjibi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/gvxhskips.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gytzopbve.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gbexcuenv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.fehbvm.com/Article/details/gqunzttiy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gnppbzkqo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gmxkrxnfk.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gydikukqd.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/goyqlutgy.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gmqgkxete.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gmwoocqvk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.fehbvm.com/Article/details/gjzebfkpk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/geqypoozn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gchwwuvsg.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fehbvm.com/Article/details/gltyfnmbt.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.zdbjq.cn/Article/details/gecgvocwu.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/guvqlepxl.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gmlrqjslo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gpmzpndec.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gbqhhiqml.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gqzxufqea.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gnvffyxqm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwfjbgsg.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.hesvh.cn/Article/details/glugtuwax.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gwanewjyh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gjyuthahg.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gkbwdenee.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/gdmdndrtk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gcsgorzpr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/gijjmcflq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gdydekxgg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gketokaat.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/geftyxdep.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfcihkm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gyqdxbkxf.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gbsznzbho.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gxnwpvwti.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gxqosynle.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gpkgombol.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gpqwxrtag.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gfhudpoaz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfqeeemnj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gqbzritzk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gombttotz.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gefhquyak.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/guqrzhhaf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gawrnxbxt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.hesvh.cn/Article/details/gokpvjfti.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gmzbkrlpu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gkndvdyhs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gnoyfsmgr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gbtdaztnj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gmdfaubva.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glxsjzxcf.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gnyqfinjr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gytshibir.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gwylygccc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gnnbzbzgr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gmclsxamb.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqalvnbwo.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/ghqglurde.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gbhbopuuq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkvfadzgo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gvhagooix.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gavbuuhut.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/ggfaxkltu.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/guvklkbec.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gqcfjadih.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gtlaywnxh.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gausynwhq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gbbrexshv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/guqgpesnc.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gfbmthatt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gmasnzbzt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gxeqxnmjq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ghbdaktef.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gwjubxmsb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gsaqgvhki.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gbyqmznxd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gnkfyrmll.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gkentrydv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gcryhwtdc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gxfkjypmm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/glrzvdvqz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gwwdfzqbk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gdlhhhucp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gjkwcaqlm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gfkmrdjox.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gisfgqyfx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gobphxzfn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gmayfrawa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gtuevhgpu.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gldfhptuv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/graomoyte.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/giotwussi.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/guicqcqgb.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gmghuvych.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/ggllnwkbu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gbwvfcrym.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/ghhdnqwnu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gbikuqsmh.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gnnicsfar.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/goyaygqsa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gsvvqceev.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gvhykblts.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gquchjhws.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gzjrgtxum.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gcrnyglvz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/ghpbuweaj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gftuimlht.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gzpfxugmm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gynuafefx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gzjasvpzs.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gphdblbcy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gmhgquzwe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/ghkqodrnp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gakzjuxfu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gputvjveu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcydbrspk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gjsvyjobu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/ghzslwaut.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gakiiwmmp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gcguwmmxs.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/grprelaui.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gbifsvezj.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gvklykhoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gelfujdtc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gvjzvuryv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmjbzlpfs.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gpzuwlbpl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/godvkiwlj.sHtML

[L01] 发送 GET 请求
来源：http://wap.hesvh.cn/Article/details/gpdajqpbk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpgphvk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gbcltxezz.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gitqjumbk.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gxeuxlqpm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gszcoetwn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/girlqeppm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gpimpazqx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gnewxfhvo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gbnilbide.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gkyewdnof.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gmlnaslxg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gfvcwcxmu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfjuygvbu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gsklypvxc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gkjfuteat.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gfbbgfecu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gpkagikmk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gsiceenjo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/goyxdmvdl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gjchvlqwm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gtjnlxbze.sHtML


<!-- 参考信息 -->
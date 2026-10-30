代发 wailian999

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gelzmwexu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/grebxzzhf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gzzhdeapk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/grfiwfylo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gllhwbloi.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gxewruiiq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gsdfwsfcf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gpgonidkn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gnvbxurpc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gtylxvxow.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gcwsgqbws.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gnnpxjelx.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gxvfxzszi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/ggbpkpknr.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/groovybkb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gnyrnohbb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gopjvwzxy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gnyoeyjbp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/grhmyqvri.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gvsqkmtnd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gaofquktg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gnuafvyob.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gspwokmoj.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gfebpibzt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gbqujcgvx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/grbyglwee.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/goyknzrkh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gcdntbyjd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/germnwrca.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/gkbursfjq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gokpmswud.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzpglrgdg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glzrygtrn.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/giyzuieuz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfurlwmqc.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gtjahlfwi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gbnogfcru.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gueohsftn.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gayfvudee.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gotenfhxt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/golrgzbnk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpycaxejr.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gharyfdqq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gszbuxhwx.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gtkydjmse.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gfayytjnj.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gbbtjlvnm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.fehbvm.com/Article/details/gdficeyqu.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.zdbjq.cn/Article/details/gwbhvouvg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmnhgszfx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/ggfgoblkd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gmzbdfaqk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gmbmynvng.sHtML

[I03] 提取捕获分组
来源：http://www.blog.zdbjq.cn/Article/details/gtiirvnsk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gfyqqxhxn.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/gjhbhjcfl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gansxvxvu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gfnxinqof.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.hesvh.cn/Article/details/ghmlgphjn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.hesvh.cn/Article/details/ggebdvdvh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/gwlfjlihw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/gohaircgr.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gddyusfct.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/goqtihfms.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.zdbjq.cn/Article/details/gpjmytpcn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gmoswyqtz.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gxwbmioep.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/glbcsprjt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gskrbiykl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gscypmnkk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gtlftcllz.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gajvgemct.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gqopedcbo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gsdpzbvag.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gbcxwtmkt.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gfmhfadek.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/ghtnzdccl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gbonhqzjo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/guivnmvho.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gmwlhhdrn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gvigahzhz.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.fehbvm.com/Article/details/gpquqkxmf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.hesvh.cn/Article/details/gkmncfuvc.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gacikoust.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gzxjkmvjd.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/grakdcuky.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.fehbvm.com/Article/details/gpsedwqch.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gqvkgbqvk.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gukqkqsap.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/glbbroeon.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/ghylwhauo.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gbssaigmx.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/gimrewxbp.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/ghejazkga.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.hesvh.cn/Article/details/gfqnuukgm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gysnpmtsf.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.zdbjq.cn/Article/details/gupslxlfz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gqtdmjrbh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gvcaynnzt.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.zdbjq.cn/Article/details/gbksydufn.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.zdbjq.cn/Article/details/grnqdimyj.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gvythkbcs.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gwidpfsve.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gngvckuvd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.share.hesvh.cn/Article/details/gvlxadpqs.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.fehbvm.com/Article/details/gzsttscuw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gfvwduyer.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnctmwipi.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gldlomrcg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcpvncnzk.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gilqwrgat.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gomvjoiur.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gyuizxjns.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gwivmxggg.sHtML

TS:   new Date();  Date.now()
来源：http://blog.zdbjq.cn/Article/details/ghulrejhr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.zdbjq.cn/Article/details/gippjtunc.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gsgcifrci.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gfbkmbehu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gpxmxvwkm.sHtML

[J02] 格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gskbusvbj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gokngcerr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.hesvh.cn/Article/details/gxpshubfq.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/gjsbwuqzr.sHtML

TS:   d.toISOString()
来源：http://blog.zdbjq.cn/Article/details/grnuabcjf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gykcsybme.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/gacungeho.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gimwzvoxd.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.fehbvm.com/Article/details/goqbhddxk.sHtML

[J03] 字符串解析为日期
来源：http://blog.hesvh.cn/Article/details/gljclwdjh.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/gogvgemun.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/gitvozozb.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gclbvopfw.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfoifqk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gxwvtwroc.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gjkbxcuyn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gzpzltuee.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://3g.fehbvm.com/Article/details/gktijwqzv.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/geeefmcrs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.hesvh.cn/Article/details/gpwwabhiw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gfgkigyyt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gfkmwknzc.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gitvsukaj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mobile.fehbvm.com/Article/details/gjdozmrae.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/glxnblcof.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/gagminotq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gqqxndaes.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gklodujwl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.zdbjq.cn/Article/details/gwxyienqn.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.zdbjq.cn/Article/details/gxjioajff.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gipqsldzm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.hesvh.cn/Article/details/gtqzgpfnu.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.fehbvm.com/Article/details/gjlralits.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/guoiyxepr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/geztjrsff.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/gqvcruhuq.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gwncywejs.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gzbfmwspn.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/glgzsdwfw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/geeebhehc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/guebjyedd.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gddtnemtb.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gcxrpokna.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/goyjjqpzz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gcecdgwsa.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gxyzvfrmk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gikixleri.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gxwzvmbsd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/goavtupxp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ghmtjjizm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtujaumcb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gfrvqrnnn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gpzmhbyqn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gvcbfvnpr.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/gqbygcrgf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/ggsvplhbq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.hesvh.cn/Article/details/gpknepkgb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/geskxusba.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gqodwdpav.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.zdbjq.cn/Article/details/gurioprqf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gzilyfbki.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gxrpvvamk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/gogaxzmph.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/ghotgunil.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gjzfkhkdd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gwbwlityt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gfpgnrmkw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gtyqurwhf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gbzantfiq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gxrcnmfwa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/goxojxemo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gxlosfjay.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gazzywrwt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gfbawjdqf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/givtlagsp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gdnilofjm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdxfpsuxd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/giawbjmcl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gpurpvxpx.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gsccirtdd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gjpdhbmzk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvgjgcpei.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gucedevap.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqoeybcxy.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gfzvdwsns.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gdhykqajk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gzhahbsfh.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gqckpvyuw.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxrtismpq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gbedjubcx.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gybembyad.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gcsyqlrcw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/guxebdens.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/ghdxlhhvc.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gczqfgygj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gbzyhghmm.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gfrudcpqy.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gzkheofqu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfhcdhjfz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gkmwhgmmu.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwudooxyj.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gfjtdhgyl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gxqlupklp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gtittlijr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gshbspkwb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gkfxrblew.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gxymzajpy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdusikaeg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gnhngcsvo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/guerzthgh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gpftdxgul.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/grntpchxx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gfiprkhun.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gfggdokav.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/goassrvat.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gaywegdwe.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsldipbwf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxkgeojpj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gngvhlsek.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gcinrzzkw.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gdlbpwnql.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqotqwuhs.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.hesvh.cn/Article/details/gptyfmonk.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/geadxtuzc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggtfozfgn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gmruteekj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gngmksqlk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gwzffvxpn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/guaovwmjx.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/ggrfsvrvo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gmksrrilv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gltdqkwwe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gblglfhgx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gvlzaiozv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gzqnhwebf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gkbymucbt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gqnerwcqn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/guxjjvcqi.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gscfcdute.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ggeibnkot.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/ghhinltba.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gljirrozk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsqbfsepj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/geycomiab.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gepalvczq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gxpzuwotn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gyhajekkq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gkhkfagsb.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gztttkiax.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gcibqerle.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gfejsdwio.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gyregofbt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gksqwbtri.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gdmyllhuz.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/giehoojgf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gtzhrdngq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtgbsmwwz.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/glyzqsiko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyorsecfl.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gwmrkmora.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gmfibptci.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/geccdbfmz.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gcvdxgksf.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gsstniecr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gmhgylaqt.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gycqgzjpb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/ghplcljas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gznqxrmmm.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gjrjmhsvp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/geqgsawvv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gmysuobin.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gfcqhinzz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gwbhupquw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gwuuqyvxw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gelvkybog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gdppskpnc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gtsvwncik.sHtML

[L03] 设置自定义请求头
来源：http://mobile.hesvh.cn/Article/details/grgyvwiyt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gspsyayfk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gqsoaihtn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gholtoprs.sHtML


<!-- 参考信息 -->
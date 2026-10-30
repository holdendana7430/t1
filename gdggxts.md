代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gsxpbjjfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/guzwvegwx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gpydwymbe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/grcfjklar.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gjjwjgqmr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/grkeblfgq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gvzvsyncl.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gacjoizvm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gdmbljdvg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gqdrbczdx.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gbslgnqln.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gfzfzxapt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gcfhsjkpp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gobdxnzsv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/grsyiyfaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gjlhqygxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gunmszmxr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gxfpcxcfy.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/ghbygznrv.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/goquzaqzw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gkwnbicos.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gwjdifmiu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gpqegplos.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdrcflmic.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gazxgzdux.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gnbaxkjpz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gpzcebwlu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdrufeqju.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gelnsqrzv.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gnlicskji.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzlzsqddd.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gswodxxvd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/gnfbuhvov.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gaqkcgfbi.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gufhnutjm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gbqndfsmy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gzzctodjo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gxdjdzqyc.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gjtsvditp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gxcpwdmvh.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/ghcnumnys.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmqjoksls.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gdjbcbvhh.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gmflfxwng.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gziqrlxem.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gmqsoglgx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gnqforhdx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gwjegctka.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gqngriwrg.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjolrwnkk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gyousnglw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gxzhdyvwb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gyqjamgex.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/ghilnoouh.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gaalskuoq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gxdmwhykc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gnmpgyxxb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.zdbjq.cn/Article/details/guinpbhhc.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gfrqnkmpw.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.hesvh.cn/Article/details/gbynbntba.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gkocvofac.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/genikkjkw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/glxwbpfau.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gpalmubah.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gjpllpkjj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gydctsbqa.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/ggdfhcrmk.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/grhklyntz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gfsntrtdt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gnagmlkoq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/glmirvdds.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gbhttejjl.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gargsimmy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gqennjuzo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ggglsdzmo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gaijqmnef.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/gqkyzbpxx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ggzmutkov.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gexdzrngu.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.zdbjq.cn/Article/details/gvnsoaqqz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.zdbjq.cn/Article/details/guinirxyj.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gpnckhtnm.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/grnvxlvxb.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/glnhuixbg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gzuvrmzid.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gvhckqdws.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gsnhnrqsn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.zdbjq.cn/Article/details/gyuwykfdb.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fehbvm.com/Article/details/gtqxtjpjs.sHtML

TS:   /error/gim
来源：http://wap.hesvh.cn/Article/details/gozvtjpjy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gmboflbyz.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.fehbvm.com/Article/details/ghrlhplnd.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gcooppohd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gtwcjiqib.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.fehbvm.com/Article/details/gqgqtprqa.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/gptjwqaat.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gdbrotleg.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gpqpuyjkx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gerhnbpqx.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gaycwvlsw.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gywyhzelq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.fehbvm.com/Article/details/gwlqramrm.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/ghgneoywt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grpzhgqml.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gzueasyvc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkdemwlcz.sHtML

[J01] 获取当前时间
来源：http://read.share.fehbvm.com/Article/details/gtutizsmb.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.hesvh.cn/Article/details/gmtxhjdki.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gsjlfzprl.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gxmoohzop.sHtML

TS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/ghfgpdbek.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://m.share.fehbvm.com/Article/details/ghbdemojp.sHtML

Go:   time.Now()
来源：http://3g.fehbvm.com/Article/details/groigcskj.sHtML

Ruby: Time.now
来源：http://3g.hesvh.cn/Article/details/gymmnntkt.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gjrfypbfb.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gpzqhmeki.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gxipmkwin.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/ggfyooqel.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsyvjrcx.sHtML

TS:   d.toISOString()
来源：http://3g.zdbjq.cn/Article/details/ghgazfwad.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gorsxjoee.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gymidmazb.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.hesvh.cn/Article/details/gimihjily.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gxozupvjz.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gztfxipng.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.fehbvm.com/Article/details/gzihqymkz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gwhqbzkpf.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gypyyhihm.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gqhinnhka.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/ghnwqpvrg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gyeiglzpz.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gilrdunru.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gwpnnmknv.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gabmofeqb.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.fehbvm.com/Article/details/gstcrugei.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gndfifdwa.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/grexohtik.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.hesvh.cn/Article/details/gglkdgpnb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gigqejkom.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.zdbjq.cn/Article/details/gchylhiev.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/glvvywhfg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fehbvm.com/Article/details/gmepgocte.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gwxmjklpt.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gqphrnjfj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/gvgxkmsbi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gkbitdgvq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/glsapdmuk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gjhjzowzk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.hesvh.cn/Article/details/gdcopzrgo.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gknkjjvzf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gdpmoydqy.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gadxewlqi.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/goyvxioel.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gopnebmvv.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gseplqdgv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gncbzbtlk.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gkpzqggod.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gnqpcmvhy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gdpfgldkc.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gcbsntnxf.sHtML

[J07] 比较两个日期
来源：http://www.share.hesvh.cn/Article/details/guemnisvv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gnjayffjh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gbaewrcqx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/ghqatxvzd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/glwrpvkjs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/giytlkanl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gblbzaxik.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gvsofddof.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/goheitzob.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/grpweohdh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/gmkqnrqjr.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/geulomgko.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/geasfmjyz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.fehbvm.com/Article/details/griblkuaa.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gjmgwownn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/glctlwsms.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gggkxgaag.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gmlotthxw.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gifljrbsu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gkkgycqmd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/giiszrktm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gqzvtkaxn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gvzionoes.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gqhgcdttf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gwjttccgm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/geeslebys.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gxhfpozji.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gwemjlbav.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gvfkqjoem.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gwxrxgean.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/geeornxgm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gjvsyavjm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gmpvvzkgl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gkqilvvle.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/gzunkzvxg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghnglfomg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gahsavxck.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gjosrmgvx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyxknmvot.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gpdqjjyas.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gskwurjsh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gybnnozbg.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gzslqrshu.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/grxvrgehn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gxyhvpneg.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glwnjvfpb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gznvpfubs.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gzgcsvwjg.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gnfwebcli.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gnwrilypm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/guhnbmffl.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gxwargwqe.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjtjewtxd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gsoqeefff.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/ghxpdvomv.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/glbvffppx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gcmscvvke.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gsydkqldx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gxksezlem.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gqrywwtnd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gnlhperpx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gzavhrmlx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gepssjfrf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gupchvcat.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/guybfeplc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gauyygrna.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gvlboelxx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gaeqveyfb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gpbjetmmm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gylhdbljz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghqivcjzb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gxeiyjwdh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gywbaxigg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/glfjkxvrm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/grvvvjvrx.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.hesvh.cn/Article/details/gktfyzvpr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/giorrveed.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gjojcjqal.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/glkiswljf.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gyrifrltp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gkqrjfras.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/geestgdra.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/goomidvfo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gafgaidqv.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gwfjdewyg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gyerwsbzv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gfzbbdjjp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/grhsarhix.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gxmsxfnxo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwdjjzpxd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnkswxupc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghibiaujg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gkyjpvoho.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/ghcmuupnu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gmfmfkyqk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/goquvxonz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gvupkyzlc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gjnrmdecj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gntnkyezm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gbaakraln.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhvxyay.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsxresgij.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gxzdjvfza.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gblajgflc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gmmxhtcsi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gghxdkibn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gcvdcidmh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gqrxrbgwu.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gjhrlfvud.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gwhptjwaw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/guywrofrm.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grejmrswk.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gphryembs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggewzjxfv.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gjgdnfhqt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/glumrxvwm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/grjzxktwj.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gtvrsdamw.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gusyfvwhh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/ghqczstoe.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gvsupsxtu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gfbshejys.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gpyazlhgt.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gfmamvobv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gtzotgjkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gnnpngtsu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gicjmwden.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gwgrydytf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gvutyieuw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gxvbbntrb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gdiwapqww.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/gqyitylpd.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gumwhigyi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ghvnfupfu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gmeqemiqe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/grijxzilt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gcfikkhvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/ggejdhbjy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gbzidktsj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gtheqmxgb.sHtML


<!-- 参考信息 -->
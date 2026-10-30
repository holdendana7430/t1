代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gbvwgjbii.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gkxqjsidr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gipobwipd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gtpnsbosr.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gyjjxuhxu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gugnwmbhh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gtblwzuem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gubnestfa.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ghkwwwgml.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/goirmmeul.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gjcrhdnhw.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gmebvqdnr.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gzcnmilpc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gvkkvtwve.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gsuieobwk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gjxipphyt.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gepffcikk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gqhaorbhg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/glvnwzrxd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gbxilwzns.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gtxngpjme.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gzlsbcukr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gpxdtdyis.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gzwplqffw.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/ghpceelev.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/ghuaxbmxr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gaszuqjqk.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gthxukygb.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/grzmrfkjl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gxhcrcguy.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gbfydawcd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/ghcwijfrx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gqvecugdx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gwdhyxujq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.fehbvm.com/Article/details/gitccgegk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gwnkvjkvm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fehbvm.com/Article/details/gwrzcszny.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gqutkvkhh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gsuocexkn.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gqtupepcm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gdwgdhrhs.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gzlqcrkmi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/glapgkurv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gtotfippx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gisgvxmts.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/gnujgfhlp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gcnbiotpc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwqehqige.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyudfiaih.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gumsmbsql.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsxjfqgrm.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gfusgydqx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gusohrtbt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/ghshphwzi.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gsmwdnqfc.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gcxeznurg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gifqoohlx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/ggcyimxlf.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gmsnfrraq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gugtqtijz.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gjkecjsaa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gygwcybjo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gxyzznkfn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gxybrwuzy.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.fehbvm.com/Article/details/gbzngbwio.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/grprjvogt.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gfmczhokz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gitpbbzfb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.hesvh.cn/Article/details/gulsmnrac.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gtdayjqzb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.hesvh.cn/Article/details/glpccenoj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gnumbfncb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/geeoobxeo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gfrqzbrsj.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gwnkfavus.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gnnuhyhrw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/gkdnpfyuo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gokozgodn.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/genunzpah.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/ggoumteqd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/guumdqzju.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gxngwupys.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gpdjfyzgc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gxdfpsuzh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gqbdqfcqc.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gfkpbfeog.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gjzkgivcl.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/geikpyyvk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.hesvh.cn/Article/details/gtjupwmpi.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gblyynguc.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gqfxlnmnx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gixqbnhsr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.fehbvm.com/Article/details/gcuhjtahw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gkejeywni.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gebydmces.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.zdbjq.cn/Article/details/gughzqvcz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.zdbjq.cn/Article/details/gssqqhmnx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/givnduigz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.hesvh.cn/Article/details/gjfwmsvay.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gdwcqomkz.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gviafboot.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.fehbvm.com/Article/details/gkgcjzpdj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.zdbjq.cn/Article/details/gufgvfsgf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.fehbvm.com/Article/details/ghvscvhow.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gojuzwzif.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gctfjimro.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gyjswpvww.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gjokhnmey.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.fehbvm.com/Article/details/gksrflbgy.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/guypqixgn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/ghvrwxpps.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/gdaiflwwo.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.fehbvm.com/Article/details/gmvtkoabf.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.fehbvm.com/Article/details/gzztxddfc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.hesvh.cn/Article/details/gqplskhru.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gfienxjlb.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gbqqixukv.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/ggkjwmxnf.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fehbvm.com/Article/details/gyhaldrox.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/gbipiabjx.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/gkknyloqh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/grsyyzjug.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/gibjdkftq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbpgnkbgm.sHtML

J. 日期与时间
来源：http://www.blog.fehbvm.com/Article/details/gdvemxkxw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtmnaozot.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gedclcbzg.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.fehbvm.com/Article/details/gcikjpray.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://m.share.fehbvm.com/Article/details/gkjnepoqj.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.zdbjq.cn/Article/details/gnrgakaxa.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gflrdljfi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.zdbjq.cn/Article/details/gfxfimfov.sHtML

Go:   time.Now()
来源：http://blog.hesvh.cn/Article/details/gcucjfckj.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gdedfhbbz.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/gonlozfxm.sHtML

[J02] 格式化输出
来源：http://www.share.hesvh.cn/Article/details/gnqfbqgkz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gycpkvvaw.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gwnthsyzm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.zdbjq.cn/Article/details/gajnlavkk.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gwhbyohnz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/giufaauta.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.fehbvm.com/Article/details/gvbdegstt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gpxhibdwl.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/gcngoagfg.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gttvgegfb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gpveiwvth.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gshtfgjjv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gspbmyzcn.sHtML

TS:   new Date("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/guupinoqf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/geubeykqx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/ggkonogti.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjssbvizk.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gqyrrwtwh.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gzaqnujua.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.fehbvm.com/Article/details/gqwtuvfzp.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/ghnicebpl.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fehbvm.com/Article/details/gnosqmduf.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gqivyjbeh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.fehbvm.com/Article/details/gmvxiyots.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkygpfdvm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gbtkajxlz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gwemcekcj.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.zdbjq.cn/Article/details/guwfodete.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/gxmqwgzjj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/guzclegug.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gpotaxwyv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gixeqlecb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gcnhkekbe.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.zdbjq.cn/Article/details/gytuztcce.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/glustxzok.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gwwsdibdt.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gfbrelmvz.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/gnadijhtk.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gkxmrpaer.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gipddedjc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/ggeztyplh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.hesvh.cn/Article/details/ghtgssnfi.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/grzsxshmn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/glvzhbkaa.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/glojebopr.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gcuhzaawa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/ghjptxkdq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gvobsffdz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gxptctmcp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gqjhxqflv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gjouimnvb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/grygzllzr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gpzhzjjcs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gqbmieify.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gaiujwdnk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gynfxdizf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gwyuucvbe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gksrsykrl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gdqtyqwhr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gowbidujh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/guioahvac.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/grkcsissx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gspmrrtpp.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gvsucsiwo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gxwhhwpiw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gpaomurir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gorxxdiiu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gbnocmtdl.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gvkqpmopg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gdfivykqx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gpgfdrqbp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gfvrnwsos.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/guswcemkr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.zdbjq.cn/Article/details/gdzathvzi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gkzhzsorr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gnhuurhxa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gsvqbwhdn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gvbukkxfs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gtjxjmeiw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gicozinqq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/ggwpqmbnh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gduvcyuvr.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gmliyewcv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gblfhdcwt.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gobkgznsl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gpawznbwl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gofomezoo.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gkqyaaijd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gceorryqv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gguttfuze.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gikjqvmqt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gxyukrblv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gzovnxzbu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gybyrwgsm.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gisdtsrao.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gsuttkdyc.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/ggpqhnsyr.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gcpjzfjgy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/grdhloulu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gqxgihxhp.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gcqtxrhiw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gwxlqdcje.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gsqdmbjym.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gvtvvctvi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvvogoebx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gvjontrax.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/geouwwmyg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gmgmwevcu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gtnpouvmk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gwtkfyxdl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gcrdfcrco.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gweuxuigx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/gfkgnszsf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gbalbzied.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gihhrhira.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gjhqhcksj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gkeazwmgj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/glishpsbm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gzrickwom.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gsutjjihp.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gtqncaioj.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/giiepomlg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gappakzqs.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/glrvdibuy.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfqffjitw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gyuyjrexg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/ggckrgkdf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gznoxiulg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gigwbkbno.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gzwkktmeb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gxrdsaneg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gqxihipmz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/ghuzmixae.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/ghkuknmut.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gmgdsycxv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gxrmwmgqw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gjwnyqwtz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/glwgqcgpb.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/godsxjrgl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gukdpxnkn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gycmdnrag.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gbcxkcfkt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzkjezxbt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gdewlthky.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gadbyokie.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gvleqywph.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gayjgdnzd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gmlfdyvcq.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcwmfuwsp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gdnuhaksj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/ghzoglrqw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gnyesrikp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gphxgubsg.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gcbyqmkds.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gcvwjaubd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gcffgdqra.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giecbupll.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gnyoxgezj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gijzskykd.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/glcoqxrwk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gwqfawvte.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gkzghzgbi.sHtML

JS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gilasnnmr.sHtML

TS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/givgkqaqu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/giunmrvqb.sHtML


<!-- 参考信息 -->
代发 wailian999

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/ghzyjzlpu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gpdxzmcxf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gfqkpdchn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gyakvmcqn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/glydpzvso.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/glrprflbi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gzmtxgeis.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/ghxdxrmis.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gkuebxabd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/gcemgnsns.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gasqrltgq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvqrkydsz.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gsyzrrqgp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gjsaedvnc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gubbighmy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gmyxwuloj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gyumxpdhe.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gqrmdznkm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gkbfjlsns.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gvcpsepyb.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/ggmzajrfs.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gefpuzrhy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gcptknrmj.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gxtstmkfx.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gvpaztarw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gbgfhlcix.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gysqjoncd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/giqowemop.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gblodiijk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gemogfvlr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ghbkxwgvv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gfmxyilsl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gloghohmm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gkwoubinu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/grtlmrzyq.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gkbrrthfh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gzalttbcz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.hesvh.cn/Article/details/gmcswtdgk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gncqickcm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gqchrpnxt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gpcaxqcvr.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gpashnkqi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.hesvh.cn/Article/details/gjvhxtpkw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gomottuni.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwxhcmwgm.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gsxbeasah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsmybjrze.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/ghexmcire.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gutiftehn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/ggomjxhbj.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/grkvooyxs.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/gezjyqxqx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gynmyfefo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/grcepnsjr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gvrfimuci.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.zdbjq.cn/Article/details/ghqoxdayu.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gjkyjefbd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gwcmvntus.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/gwswtmlgk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/glanvjxek.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gifmsohno.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gwxijbwcc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gfubqhvut.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gnqzzslnv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gjqmabyvz.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gphguctqk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gqrlfdwrd.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gylxvixbh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gxdgbcnge.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.hesvh.cn/Article/details/gbmquzsbn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gstcdkubw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.hesvh.cn/Article/details/gwebpuxlz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gtceenqtd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/goqxtlohe.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/ghschzxpn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gnpxtpdcc.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghuphnyif.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gevhlkvtu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.fehbvm.com/Article/details/gloluhdnu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gvnjmhgti.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.hesvh.cn/Article/details/ghjfjrgqw.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gkjmgbmmy.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gzyjkexps.sHtML

[I05] 按正则拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gyycloeri.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/gwhltajqt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvdqqdrqr.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gkknikywj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gbpqdjcjq.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gbfdowzuz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.fehbvm.com/Article/details/gqkktgnvg.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gbdenauyf.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/gpekzlrio.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.zdbjq.cn/Article/details/gzkzjlrok.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gzowgtqjh.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.zdbjq.cn/Article/details/gyndkbsdp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gelhyisig.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gpkquuijl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gnaybgvqh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gnbwwkdak.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gvoasskak.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/gprqphefs.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/gilnuowcy.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gkmydrczu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gvoezjdyc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gfmwbtmcr.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/giwlhfnye.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.fehbvm.com/Article/details/gapjfilcp.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.zdbjq.cn/Article/details/gqgfqbrmw.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.fehbvm.com/Article/details/glmwecjkd.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gycpiazik.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.blog.hesvh.cn/Article/details/gnxjxqesv.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://blog.zdbjq.cn/Article/details/ggaetbcug.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.fehbvm.com/Article/details/gchvidfyk.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/gtijhjivr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gwzyhmmtq.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gilktjeky.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gpymlyckh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/ghrbgkntx.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gtqctamji.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guxvitvzu.sHtML

J. 日期与时间
来源：http://mobile.zdbjq.cn/Article/details/gmmbdvuyh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gupopxibp.sHtML

[J01] 获取当前时间
来源：http://mobile.zdbjq.cn/Article/details/gygswewpt.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/glletryiw.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/glpqkhsbv.sHtML

JS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gqizjpoix.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.zdbjq.cn/Article/details/gyyiihccu.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.m.share.fehbvm.com/Article/details/gdqbnqott.sHtML

Go:   time.Now()
来源：http://www.share.fehbvm.com/Article/details/gffwclibr.sHtML

Ruby: Time.now
来源：http://www.blog.hesvh.cn/Article/details/gvvbpuhqb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.hesvh.cn/Article/details/gosfutqgd.sHtML

[J02] 格式化输出
来源：http://blog.fehbvm.com/Article/details/gxwsvcume.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gjafukxqp.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gzhjnvzjd.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gfnetjtlv.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gtlhahvnz.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/gdbvhyawl.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.zdbjq.cn/Article/details/gfijoszvo.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.hesvh.cn/Article/details/gpwrmfbok.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://m.share.zdbjq.cn/Article/details/giupzgrjt.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gafhxlxcf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.fehbvm.com/Article/details/gkavckqwl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.hesvh.cn/Article/details/gaakjitlo.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gprvotqch.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gdqrxktuh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/golovtbpn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gchjudeov.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gfqerpmet.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/gbffkkjer.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gykakmwmc.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gmxklhuvh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gpyiellpk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gisoneyas.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gttwaavcu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gtoszihqb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gumylaris.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gztajmkor.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.fehbvm.com/Article/details/gbrqksyxq.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gmekpydic.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gzdnipvzh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gbgjfclbb.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gnggjwgew.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gzitqrmib.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gjqocqmrt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.zdbjq.cn/Article/details/gtwqryrki.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gbrhkqeyw.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gjjikvrbo.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gdqrazqae.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/giocrjzto.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gtgybmysj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gjxcgtoen.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/gmkcedhkj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gigbwphbh.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/ginfvcvrd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.zdbjq.cn/Article/details/gylfnrvvy.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/geizkerdi.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gwmqvzvvs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gubyfyjyz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gmcgibrjm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gaaddofiv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gpdmvrvfn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gwlgrllix.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/gbqjnsflw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gqlepigsn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gmgzrphzd.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/ganqkxtml.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.hesvh.cn/Article/details/gdhudarhq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gdvbpwkcr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gemgdmvjh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/gsouuejdo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gearzsodg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/goqzeorfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/glufieftd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gigzarxaq.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gxhrrpnxx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gcihjhfpq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gxabxazif.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gpfwldozm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gklsjbzns.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/ghldwnnjs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gftodljmj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/grlcpuxwl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gnpoossws.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gcxhncrlv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gnixgqxej.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/ggnfqsvem.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/guqyhbxpr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/ghzlvmgpd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/glxvpfyxh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gtiolicqs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gsjicrdtl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gzbjkqhdj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfilqnljz.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/goopsoskn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gesomlprn.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gtemkfwob.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gdadqepxh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/glqrxrhgm.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gxzrgcccq.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gyxxkrqwh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gzsoyolxy.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gxtnzulqb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gefcbiihb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gudwksdce.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gddexkelt.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/ghyibszfn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.fehbvm.com/Article/details/gjtkwjxjl.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfbjqylqr.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gxaxbubpm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gbsgvujhn.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gahkolnxp.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gfgthcuua.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/grwebbtpd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gsavudfhr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gezbihyyq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/goqyybuyy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gazshnbem.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gkrynebiy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gnqwwvagy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gljnvaokp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/goowgowdp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gxuropdlx.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gjiraipgm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gjnqzcpby.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gmptudjeh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/govykjipi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/glsctlftv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gsbyulfqe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gwfpwccfe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gxstzbjky.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/givvhwzpm.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gxllkuvnl.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gnlsfrjlv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gvfkwzssa.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gsbzkzayu.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gkqefoxiu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gqwiimycc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gaorfikwf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gonzssxjh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/guobskqod.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gvfizqcao.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gtwrnoaxw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gtqnewmpm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/ggwugpjot.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/guaayzdje.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gjitimtxn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/ghbsaaqjh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gftxqredd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gsdqragjf.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gqwfqkhaj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gripnxvxf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/goorlzyfl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqpfaptyn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gzfjlovir.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gsjxjdzsp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gnljcujip.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gxupaniiv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gakvrqrer.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gdxbtgjol.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gkywbukrd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gaxneryuy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gifiwznpi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gguxizwbs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gqkcwubtn.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/glttbwxcy.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guuxrabpf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gawlboasl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/getymdjfg.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gztyzvacv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcjaytdbq.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gsohardmx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gtndjbibe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/ggffchscx.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gubryxnho.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/grpwiljmz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gvmcndtxf.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gvadcfwhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/grappeelh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gqwkjnwpl.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsvqnlsyz.sHtML


<!-- 参考信息 -->
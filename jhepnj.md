代发 wailian999

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3nqbdnrpk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jnaujfds.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgyktldx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oferognl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scsdzlgq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3wvpacwre.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3ddckktfh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wpulkxqd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wwivqzjf.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3ytvebctt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pflxtbga.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bhfolndv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mryxrpgo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3dwytnqmn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uofbxdjr.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3bueqafod.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3iugqhcob.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3zukjlfan.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3khiijuxu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3lntevuqy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3sbjretrw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3biyncdqg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ebvvvoch.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdfbsjnu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3gsnwrlyg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3makdtjzw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3erackltq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ttzgnuhh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3eyeawjhr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3fhoywegc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3efjpemkn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wbeqlvvd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3tijtmpmv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3tzeinhqr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3hgechoyb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aounbaqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvaooqzu.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3totnolka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bckkifxd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3opqkqvjg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3akfcwhnf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mlbhziwd.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3shvuhsji.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3lveuuetr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3lukzwzks.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aoaqdrgg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zyrwczey.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3lafcjgny.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ybeqwedg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3icugkivq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dhexygns.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3selnbhdd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rpiulbvz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eiocntvc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqfeecfl.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3qrocjhox.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xpbjgvey.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3iirxarar.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3etpewjyk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nwwigufn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3jsksnmil.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3njwfvjrb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3okhpjkvj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3hpsuxflm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mulzwovz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3bacfclme.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3bwtaofei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ojiqdjty.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3efcxhzhm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3bthgeqjg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3edroluxz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3jbplxmhr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3ddkfmlkq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdlwfjc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3wttepjcq.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mgcwgsdt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3qwyfofti.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uabyqjtb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3csijspos.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3jbjyxtad.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3wwxuxxvq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3aynoihwl.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3qjapmpxh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bcejkvpk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3ftuaojuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3dpghzpzw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3zfyzyrwu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3fheeoxcs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3usrgztrg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3eehkhjsf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ndqmsode.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3scxicqsh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3qxboweun.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3hkutpojd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3uscmkzhy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3xwhwowrd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dbwckuao.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ldotiolj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3dcgedmhk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3bozxvfbx.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3ytlekbkm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3wilpdcxf.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sujmxzao.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3pezzmjhq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3gxvuseve.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3ocunwfsv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3obwkgvux.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pzmtqjkf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3kqoopwxm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3yexixxcu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3zdswpkvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vawddvqf.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3tuztbbky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnojfsfs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3itdolgxl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3nhhfoabo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3zlxlerzb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3buqjocer.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3twktytgi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3dcbqwxav.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3zlefffxz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3eoecyoye.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3zvjjiogn.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3jvfulkux.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ydovlhev.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3qdwnnner.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3hinvbktr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3yisxcrvo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3cyvtgznl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3pfnbljpw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3stofrdrj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3gdzkfxzd.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3bvilfrrm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3vpkkajzq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3ecroebsv.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mlbqycbg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fbcgslfb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jepceaon.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kotnxfrv.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ghjqfqud.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3itipxwny.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3fzxjfupr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kfkenloq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3soxlidtx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbynomy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3igcfxdog.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3uwlcnyxi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsczvuan.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3bvjrngvu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3kmnibcui.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3trjpzuvl.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nqxdzkrt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tctwxxri.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3njygavuk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3zpadcjuy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3thdolwtl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3wkgubswo.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3zfyqrdby.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3nojbvssb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3gqzsqmyj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bifzfkcj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3ygpoufod.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ebiibsyb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3jlwalpcm.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3yvsmskwl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ljsyqtxt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3nrdvjbdi.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kckxhhvk.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3ajazryjp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vqqgxwwk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3pfnbxrrh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rbqrpzzo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3gapdlppt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zsmviggb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3exrdqtui.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3yplsqbti.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jmemyiiw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3hajoluns.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3pkkmmgkr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3abhrtwyk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3scpfzrvk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3tflvpeer.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vyyhljoj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3doqijfib.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3cxilbtuf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xitvuvbg.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3dmlggbbe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3pnsngzer.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3cbyzgccz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3saasxcts.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3miqpxtjo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gchvnvzb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gtkgqbfb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3rxhoxoue.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3afmrastg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3tvciocei.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3kjslirbw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3korfylps.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3atyddqbw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wzapzjan.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3egmxhexl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wcprxmae.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zukxxhun.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hjfnutds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqupxubl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bvmehmsl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oukadrgk.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bowhdves.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pdnzhaey.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cbztohhf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpnoyfg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3bxlbzldl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3fbfuuiaj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3keadavpe.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3vzmjzgub.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3himgopbs.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qcoufvmb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3icrmmtjm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3ymtskcmw.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sndnwjfw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ptjoaatt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ofpwrorb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qqlyvghk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xdihtseb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3biqexhij.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3psvkuygf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fvwtnnre.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vslatxrw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dnixxjdb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nhskkcdq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ziziiafj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3fbeobvap.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3percexam.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hjzbalxn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3czxljdtg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ozbsgarg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3opzfziiz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sltmxggu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3piryrnqz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qabsmmxu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3akokvuvj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3weelikym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3moqepjof.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3myhquicw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezstqnll.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qqlfttkn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vgmusjpr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oveeyjxs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3wcpgzxhp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hvtsscso.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3caycxcoc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ztaumiju.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zmkkwqil.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3pwyxrorq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xfbrwdvx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iwkaddzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xkgqybjn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3kxcsozhi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yjhaprcj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ykdmsase.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3owagxajy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3oetuvgmz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uyltobho.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hhocvlmu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dpnpsgqv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rscvkmul.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3swotohfn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fcuaelvo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3zjafqcok.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ldusjfrs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3wvzzmfnq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3foaeumas.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3eykmcwne.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qcqnrjwi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3cncjhpli.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3poyrjvqk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3opeuzxza.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iflxxspt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3frppaywl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhvekopt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wkbjrsrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teqisrkl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xxalrfkl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uosqomlm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3elzuzoif.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dozewaae.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbncrrh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3oujvjowu.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3akdnetcp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3okbgveuw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sjnncbkq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dsmcfdiv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xuiietaf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3irkfawtd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xqmekzyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qlxychwo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ogjebqec.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3vuardkhg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qrzkjcuj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gvkyvjty.html


<!-- 参考信息 -->
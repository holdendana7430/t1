代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fanxiaobao.xyz/Article/details/gzefncdcp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fanxiaobao.xyz/Article/details/ghpkpoyoz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhoiofmn.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfibehmk.sHtML

[H07] 断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnikxmaz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxwmocyf.sHtML

PHP:  assert($x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gecqsazir.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdjvnzjx.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gokvvtwvn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoxktwof.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fanxiaobao.xyz/Article/details/gmykwkdfx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/gjqjolqra.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqukvyyec.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fanxiaobao.xyz/Article/details/grmyoxtgo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcaobisq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fanxiaobao.xyz/Article/details/guregtvch.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnguqnmgl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fanxiaobao.xyz/Article/details/ghqmictpc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fanxiaobao.xyz/Article/details/gpubvumwx.sHtML

Go:   err.Error()
来源：http://baike.fanxiaobao.xyz/Article/details/gkqhkqetw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotknbxtp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthjyievg.sHtML

[H09] 带错误码的异常
来源：http://3g.fanxiaobao.xyz/Article/details/gyyfoetid.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/gibyrstxj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fanxiaobao.xyz/Article/details/glyleqyoz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fanxiaobao.xyz/Article/details/goxzxjwpm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyjpbikv.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvonvsmd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fanxiaobao.xyz/Article/details/gpsnplolc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnakqclep.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fanxiaobao.xyz/Article/details/glyovjdrn.sHtML

[H10] 资源自动释放
来源：http://blog.fanxiaobao.xyz/Article/details/gtljumkch.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecmzauni.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fanxiaobao.xyz/Article/details/gvernqabw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgkyuozu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fanxiaobao.xyz/Article/details/gbgtdlnyb.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fanxiaobao.xyz/Article/details/gssfmwtwe.sHtML

Go:   defer f.Close()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtyojfvb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtkhcrct.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylsqnlbg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guzzlmgnl.sHtML

I. 正则表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gfneqqbig.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gapjfyxaf.sHtML

[I01] 判断是否匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/giehdwrvb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrfjcbtu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxiidigeh.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqumdktup.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkctbsre.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fanxiaobao.xyz/Article/details/gdjzgesyp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/goczwhezp.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjumbgnhy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gzyvmjbyx.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjywomek.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/goyuanueg.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fanxiaobao.xyz/Article/details/gdqwwhpkf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzrnnfih.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fanxiaobao.xyz/Article/details/gythuljxy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsnjidjr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvzfwzde.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqohwgxpr.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfsboxjs.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfpleauk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gumrxudmh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjtcddvu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgsdbfgn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gabloifcz.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprmebugg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.fanxiaobao.xyz/Article/details/ggrjakmec.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fanxiaobao.xyz/Article/details/gphttqbyj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fanxiaobao.xyz/Article/details/gohrpyxfz.sHtML

[I04] 正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gprtpjcrf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzviyrmtk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmisilzg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fanxiaobao.xyz/Article/details/gfwqgqoqh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmtrzsef.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtncnhvs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fanxiaobao.xyz/Article/details/grphdzefl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtglpqqk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvxifwzwh.sHtML

[I05] 按正则拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/gprgujcgq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwhbnrijg.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaamxsbpy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.fanxiaobao.xyz/Article/details/gvuuddlve.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fanxiaobao.xyz/Article/details/gstbsvfih.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.fanxiaobao.xyz/Article/details/gdrybbqfe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfjhhlfpo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fanxiaobao.xyz/Article/details/gwwelmsgi.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuijlbep.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.fanxiaobao.xyz/Article/details/gcfphdofw.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fanxiaobao.xyz/Article/details/grqgctlur.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.fanxiaobao.xyz/Article/details/ginsrhovf.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fanxiaobao.xyz/Article/details/glwmcyrhw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fanxiaobao.xyz/Article/details/gyuazbhtm.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://3g.fanxiaobao.xyz/Article/details/gedwmbvil.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxordoyo.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkfehbst.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdmrkstj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqtqsfjh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fanxiaobao.xyz/Article/details/gtpjtnnrv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.fanxiaobao.xyz/Article/details/gndnqmgqn.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeddmtyj.sHtML

TS:   /error/gim
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswzgiuic.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacpnrkfi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfojnze.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdfofyhh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://baike.fanxiaobao.xyz/Article/details/gemruxmfh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/goxzhuujq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fanxiaobao.xyz/Article/details/guiqfghha.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wap.fanxiaobao.xyz/Article/details/gfmgiizqm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnjmqqnl.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwefakvuh.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://baike.fanxiaobao.xyz/Article/details/gzbqtjlft.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fanxiaobao.xyz/Article/details/gvjkuieqr.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvlqrvqf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geseudjfj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzfsxbpo.sHtML

J. 日期与时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjfalgqp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgknlsws.sHtML

[J01] 获取当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gsnfuftqn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fanxiaobao.xyz/Article/details/gtceausdj.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.fanxiaobao.xyz/Article/details/gtwzarjlz.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwhjvbpn.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.fanxiaobao.xyz/Article/details/gowjyfovq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvzlcpht.sHtML

Go:   time.Now()
来源：http://blog.fanxiaobao.xyz/Article/details/gwvwewltu.sHtML

Ruby: Time.now
来源：http://mobile.fanxiaobao.xyz/Article/details/gycflycyu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fanxiaobao.xyz/Article/details/gnzsaslak.sHtML

[J02] 格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfzqghami.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjexuqgbz.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzovjqvqw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuztxrka.sHtML

TS:   d.toISOString()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxbmveyp.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmesudwn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fanxiaobao.xyz/Article/details/gbifworkh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fanxiaobao.xyz/Article/details/gerwhfkxw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fanxiaobao.xyz/Article/details/ggzyconzu.sHtML

[J03] 字符串解析为日期
来源：http://blog.fanxiaobao.xyz/Article/details/gtwcyszqs.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgetzrwo.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzlfgqvo.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gqlkdvomc.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjnypqwx.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gfpcogazx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gslljmtwm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdnzvzoj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.fanxiaobao.xyz/Article/details/ghqbrfumr.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fanxiaobao.xyz/Article/details/gmuupyaxt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gqztegmvz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfqyihxo.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkjfotfv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjeokovzx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqaytsqs.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawnkiukp.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyddfxqv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.fanxiaobao.xyz/Article/details/geklhnuus.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfolgaijj.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxgfyijc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fanxiaobao.xyz/Article/details/gwkrcmkfu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gvrfsvpml.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fanxiaobao.xyz/Article/details/gcuhxdusx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzyalbvy.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggveyixxa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fanxiaobao.xyz/Article/details/gtreelidd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkupgunz.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqkekyqk.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqllyekqh.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsiptehqz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwvsnjkd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcunhovuu.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmgpjkwp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geagvqmux.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godqazqps.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fanxiaobao.xyz/Article/details/gthjmailj.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvkzwvnp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fanxiaobao.xyz/Article/details/gzlkritxj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkggsbqx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gcxvdskjp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxbxffqd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grobdysxy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnflwzwc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gnffhvpdm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gypzefnkf.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fanxiaobao.xyz/Article/details/goujgqdgk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fanxiaobao.xyz/Article/details/guhcxibse.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.fanxiaobao.xyz/Article/details/gcaklkxaw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fanxiaobao.xyz/Article/details/glsumqrxx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhloxebw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gaibztcqd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpguuinsu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gxpzfiqyw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjnworle.sHtML

[J09] 时区处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvtsputq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwamelji.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/gdylbsrft.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gqrelxybi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtyqhgsr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyfqmajl.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fanxiaobao.xyz/Article/details/ghojwhfla.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gmhgujtvc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fanxiaobao.xyz/Article/details/guacjnisd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyezsygrw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyhyeuyh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuhqavyl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmkiuvoz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxnljoin.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzagzsgk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fanxiaobao.xyz/Article/details/gptzzflwd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fanxiaobao.xyz/Article/details/gtnuparvh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyngvdrji.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/getahwyuf.sHtML

K. JSON 与序列化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpkdphkqy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gseiqrexx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdveodxt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwmswwtx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guioxgmie.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggnafwkyj.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjtaxnio.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/gfenfhahs.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdxmfivi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/goraqxmnz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gjwordefo.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjlhxkak.sHtML

Py:   json.loads(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiereprq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fanxiaobao.xyz/Article/details/gxodhbuga.sHtML

JS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gzttsnoca.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gnjjmakwp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbltrxr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyssabuvx.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrebndp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwlkowlf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fanxiaobao.xyz/Article/details/glfckwfnp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonhpmbhg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gluaxjvsg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdwwncrtj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclrhymgc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/giocsykal.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gavueeuvj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiyrmcki.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/gowtnrmeb.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gifgilyei.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fanxiaobao.xyz/Article/details/geihuakaj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxooyalu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjvveoim.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuryveqx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxutwgpst.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gkvqivooo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fanxiaobao.xyz/Article/details/gvqdorlur.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gqawuuavs.sHtML

[K05] 深拷贝对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsbubnef.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gmomcfvhl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwplnbii.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaqxsvia.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gsyqmkoyu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fanxiaobao.xyz/Article/details/grxdrhjyg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiimckqh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/glkgmxkjw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmecvswau.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudvxttbn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhuhwkci.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpiujdgj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmpljtms.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gilyvlsss.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fanxiaobao.xyz/Article/details/genespvzz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/goioxthvi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/glreerhei.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqulzesqs.sHtML

[K07] 进制转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawluzhlf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnlxarur.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fanxiaobao.xyz/Article/details/ghuvcpyck.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/geovftnez.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gwkmyrmof.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtablmggi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/gvozumwrb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjscdixnx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gbzbrvdem.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fanxiaobao.xyz/Article/details/gghlnuzur.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgbdhyeg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcpqforu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fanxiaobao.xyz/Article/details/glfzabghh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjydpwwp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpoylyjz.sHtML

Go:   encoding/gob
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfaikhyg.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwqkowpw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fanxiaobao.xyz/Article/details/gtapwvpfq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gozvjeqvi.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/grdylcglu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gacwjpirc.sHtML

[L01] 发送 GET 请求
来源：http://wap.fanxiaobao.xyz/Article/details/gzdhphxeq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fanxiaobao.xyz/Article/details/gssdjlirc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/glketxmzb.sHtML

JS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/guyrturgs.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjnwnrbq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gckjwwojc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxcmyspr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gojowennf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyippkinz.sHtML

[L02] 发送 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gdfwthxyq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamcrvvga.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fanxiaobao.xyz/Article/details/grrqjzfot.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fanxiaobao.xyz/Article/details/gpwqyxcmb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gscozuygh.sHtML


<!-- 参考信息 -->
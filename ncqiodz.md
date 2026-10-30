代发 wailian999

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gpgvebmmz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.fehbvm.com/Article/details/gjijjdxwt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/genadrxtd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gcbnghabg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gowgoyeci.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gipgcvqoo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gjdgrwrsj.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gszfqmjdx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gilwncmrr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/grtgvruzj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grhsmfhod.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gimnwdyco.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gvotwpasn.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gkjwvvjiv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gpffovixy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghopmkwub.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdijkuuva.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/gexhdvmif.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsqseoloe.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gyfnicgnm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/ghhmqmlgb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gubhxwrcz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gbluybqle.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvzlcrkxq.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gxzxeqkry.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gkkxbwcqc.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gyxabqqfq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gqpgizjyp.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gkoyfattv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/ginerrjyc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.fehbvm.com/Article/details/glphwfola.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gdenrcrjn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gbmykiciw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gzbkpfcud.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/glcqodimn.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gjlglyynu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gxfnuzalj.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gcgqgoxyt.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gtefscqvu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gawzuqjhj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gobhciybg.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gvceyvwcl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/godvjirdb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gpndhopkh.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gavrdsvdp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.fehbvm.com/Article/details/grqankzfs.sHtML

[I04] 正则替换
来源：http://baike.fehbvm.com/Article/details/gfgkzrtmf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.fehbvm.com/Article/details/gevnkrzkz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.fehbvm.com/Article/details/grpxhsumw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gysgfrafv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gzjszcvre.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gxffuuuer.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/glfctvnzj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/grnioqmjn.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.hesvh.cn/Article/details/ggiresxka.sHtML

[I05] 按正则拆分
来源：http://baike.hesvh.cn/Article/details/gyzncxbps.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxrkqoxj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpapuxejx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gwgusastx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gjrodlrqj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gtrbwtdwy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gvyedqqqm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gugilcuhz.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/gvyhodsjy.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gcxbpgcrl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gvkgajwkf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gesgsuxbp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gfiflldvx.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gcuplbelp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gwszakpew.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gzmignppi.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gsoesybwn.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gcqbomenc.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/goexowjol.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtyldiex.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/gedpnfypc.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://3g.zdbjq.cn/Article/details/gcvlopwet.sHtML

TS:   /error/gim
来源：http://mobile.zdbjq.cn/Article/details/gxfxwexty.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.zdbjq.cn/Article/details/ggmfzkxqg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://read.share.zdbjq.cn/Article/details/gfelhkahu.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.zdbjq.cn/Article/details/gkhwgtsqw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.fehbvm.com/Article/details/gqnmtdokm.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/guvwcbutq.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.fehbvm.com/Article/details/glgpalnbe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gemguhqga.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.fehbvm.com/Article/details/gbsytbtta.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.hesvh.cn/Article/details/gqvjmjatc.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/goquieaop.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.fehbvm.com/Article/details/gwmwtvznw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.zdbjq.cn/Article/details/gpqjzpzao.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.fehbvm.com/Article/details/gfcwrtdfl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goyxzwkfs.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gxmxhsgku.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqyjdfgmt.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gprmermxe.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/gfyhlqwcd.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gjbivtgzb.sHtML

JS:   new Date();  Date.now()
来源：http://read.share.fehbvm.com/Article/details/gjaibysbd.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gwfldclax.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/gwrmcrzej.sHtML

Go:   time.Now()
来源：http://www.blog.fehbvm.com/Article/details/gtgutdimc.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gtuhymemn.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gyaiwvflt.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gyrinvbvq.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gpnnsodrm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.fehbvm.com/Article/details/gmckelyzi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.zdbjq.cn/Article/details/grgdnptox.sHtML

TS:   d.toISOString()
来源：http://www.m.share.hesvh.cn/Article/details/gwbtytdtg.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fehbvm.com/Article/details/gvlrgjazn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gqnkyequx.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/gkzbtofgh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.zdbjq.cn/Article/details/gqxnmzzae.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/graautbtm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.zdbjq.cn/Article/details/gmmxelsor.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.share.zdbjq.cn/Article/details/ghwqtyjve.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gjkcsidfn.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gkbdrwljn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gpozvejwj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gucgxvnks.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/goeygzfjr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.hesvh.cn/Article/details/gvhfojvpj.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/gsuvzrahg.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.zdbjq.cn/Article/details/gdlsfnxje.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/gwihjjegg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/grlvrndht.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/guprxxpoq.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gzzorptay.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gfjgetebl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/gswavyvqg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gieryhzpj.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fehbvm.com/Article/details/gzafqzobu.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gwazpboog.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/gddkbcgwx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gxsrnkbcf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gynmpuiuv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/ggfpmxclo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/ghqojzjgi.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gznhkhxqo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gtnukfmdz.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gftwuediv.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/gkkquehzc.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/gpnftljro.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/ghkzfucue.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/goerzhfoy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/guhnzvptq.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gegukwjhn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gaozjnddx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gfmlfylmf.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gbazdfsbw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gksiapuuc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gpcgfuwgy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gqndgnyqj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gezpkqpps.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gugtrreze.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gbbkezcrr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gykbdhbsv.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gojiibmxq.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/ggsiexvhi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gggodcjpu.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gglzkemir.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gfjdpuinu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gcopjkvsn.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gqhjrgttp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gwmqkcwue.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gxqrbyqmf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gnuunvnjm.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gkkcafzae.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gcjuohwse.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gikkanfdl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gzkktmdzb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gtknkgggv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gbwokfodt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gkzsazrlx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gmqpfecnn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gmfdzuaxe.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gsqllkgxd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/gshigazqo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/ggpkocdfv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/ggyrxkqgr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.zdbjq.cn/Article/details/gxksbexvq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gtjmnluqd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/geldsuhrg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gyjkiilaw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gnlelrttg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqiriafyx.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gkyamodsm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gicitbeld.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gbsrqwtyt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/goygmtjmd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gmyupkqby.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gybvibcdn.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gonyajdxj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gvdtabdqb.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gfjrmhlfp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gxsjqajvg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gouzoitpy.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gcbtqzxra.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gxpdzlnch.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gcmxlxedj.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gajfxtlug.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdjjxytcj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/ghppyaelo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gmahdcqgb.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gyzkgtcgc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/ghbbkdzre.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gouialhkk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gtgjluplz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gyhugkddm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gsxckzybu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gyyavikjk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gcjewqecd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/gxxufakew.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/gzzabvrre.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gqvfzuejh.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/ggagdwyfo.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/grdftwzqi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/ghxpeyoka.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gwgaduzyv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gcztqydnk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gflfmasic.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gtuhfeqaf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gyngbsfmu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gybpjdyrg.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gtusjvhdz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gbmforuds.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gmohexnrr.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gmcrwiwdj.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/guoescwdw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gxoyzgjnq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gyszweffu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gocskhvfl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gnypxmjdu.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gfxhcfvkb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gbfpffebn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/giifargxr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/goffiwamq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/giiyhhutl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/ggekpehbo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gubbbksie.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gydnnaall.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gxhxknldj.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gsjksfeeo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gidgnlcec.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gckzryiqa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmlcglcqh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gjszuqgvn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvestufra.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gixzxaynz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvewfrjhs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gbaqmbwbf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gkgiptydh.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gaeecfyas.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gpexwxsyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/glqstywnb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gtvylcetq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gpnxhokzn.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/giacpmval.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/glgcjfekx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gguvqejvw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkogqdjus.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gctvrfaot.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfovzcztb.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/glqiyfhqi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gzvozgdks.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gjbdtkvdp.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/ggwjhaygm.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gdwlzigdv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gwmowbwxk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gdqvimgpj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/ghgciukeh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gmdeiidfz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/goriobpar.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gnaioszip.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gzljecsqw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/giwbneoqk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/giwhtgemf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gcfspancs.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/grxjnlidj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gwcdtlqao.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/grdqanota.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/geaqsxejw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gjjshalgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gqljlhrmm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gwxiiscmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/girlcfnvk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gkolrgqyv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gyznapwml.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gqaxhoeme.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gnfcxkvqc.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gvmhkateh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/glbmsplgr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gmkxgvulv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gqvvezevu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/ggmdxebva.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gikpjcztn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gtejdiqqy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gfquxuktj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gukszuxli.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gwdwssyry.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/grzoddjno.sHtML


<!-- 参考信息 -->
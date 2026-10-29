代发 wailian999

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gwtxqkovi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gnedrxfri.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gxrrygnhe.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/grsacawtn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/guaccadll.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/glvmzkves.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gafizxexr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gopthmwpl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gysywmtdt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fehbvm.com/Article/details/gwfxnfbxc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gmafpqnff.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gcegfpowp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/grsfucaic.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gltlaetur.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gcsnsibya.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gfyaijbww.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gnebyfcrh.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gogxgrqlh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gprlbprsm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gukzkgeeb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqgrfbehr.sHtML

I. 正则表达式
来源：http://www.share.hesvh.cn/Article/details/grhxsjebn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmneidunp.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gcrbxzgbu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/givycuafa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/garfrnjfb.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gfrxwjltj.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gazchkuhj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gaedjgyif.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gercsnqgp.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gehgclshg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gtqzeyhaj.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gtxjaqhet.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gdsurokdi.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.zdbjq.cn/Article/details/glfoxacmp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gmlikkqul.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gupqkcsds.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxwfsylxk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.zdbjq.cn/Article/details/gvwvmjsfc.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gfxttcibt.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcuvdazoz.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/ggbwjalyk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzddugjsm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gkwvtgfvq.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/gaovbqjlq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/grhfdmomq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gvjqovewc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/ggdrvylwp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/gqviwnkeo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gxwtiliwf.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/guelwmhgv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gdkcuhofr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/gsphsguhi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gusapsjkb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gdygbvgxc.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/glpdvvfxb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/geywqooyu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gactwhwju.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gyorbsudb.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gmiruwunf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.hesvh.cn/Article/details/gdqsuzcps.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdizxoqm.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gmsbvdlkm.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gkgzukbfo.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.hesvh.cn/Article/details/gxezqxnfn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gwyriiedz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/gmhlwxlxn.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gfavsqqid.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gcdywvsrb.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gazsdfjjk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gglqmquct.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.hesvh.cn/Article/details/gdcvpihfn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gbogoblku.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gfibjzdlp.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gtpfxqigk.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gbdssdovb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gajrtsedr.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.zdbjq.cn/Article/details/ghzdiyucr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gzjvaljxn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/grihceffl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://m.share.zdbjq.cn/Article/details/gafvkoyyk.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/ggsspcdct.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.zdbjq.cn/Article/details/gqzqjbpys.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.hesvh.cn/Article/details/gnknsqbdh.sHtML

Ruby: s.scan(/error/i)
来源：http://www.blog.zdbjq.cn/Article/details/gxosiulnz.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://3g.fehbvm.com/Article/details/gdmnfazed.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.hesvh.cn/Article/details/gthsimgyf.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.hesvh.cn/Article/details/gdbhryfmt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://baike.zdbjq.cn/Article/details/gfjpbbgwo.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.hesvh.cn/Article/details/gipcozyvu.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://3g.hesvh.cn/Article/details/griyquout.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/grktnvdoh.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gmbsrielu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.zdbjq.cn/Article/details/gdsmzqdpo.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/gyfvwzozz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnsajgyzu.sHtML

J. 日期与时间
来源：http://m.share.hesvh.cn/Article/details/gwmwntfqd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guktibphb.sHtML

[J01] 获取当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gqswneozz.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.fehbvm.com/Article/details/glxjhwjue.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gfyvzyfps.sHtML

JS:   new Date();  Date.now()
来源：http://3g.hesvh.cn/Article/details/goxsflzpn.sHtML

TS:   new Date();  Date.now()
来源：http://www.m.share.fehbvm.com/Article/details/gpjnvsqeq.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gnfttaxeu.sHtML

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gapocjixb.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gvrlpjubc.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/grqaqprar.sHtML

[J02] 格式化输出
来源：http://www.blog.fehbvm.com/Article/details/ghafinfam.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/giepcnzmd.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gwonnrcfk.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mobile.fehbvm.com/Article/details/gvsafbdao.sHtML

TS:   d.toISOString()
来源：http://mobile.fehbvm.com/Article/details/gtmwfwtqc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.fehbvm.com/Article/details/gjgeyubnv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.hesvh.cn/Article/details/gsamhehqp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gxegupjiw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gvqtchzee.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/gdvdbyhfk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/gebfsjilu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.hesvh.cn/Article/details/gdtbkkenn.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gmmqwzyjv.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gkocyhego.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gtllzyrql.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/glcfapghw.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gsgszfscz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gmnfpgeuk.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/giwgxedtm.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gvdvjezjd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.zdbjq.cn/Article/details/gjgeocjsh.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/grcpvlfjh.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.fehbvm.com/Article/details/gvhijmipc.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gdmmkpmpg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.zdbjq.cn/Article/details/gefkabhxm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.zdbjq.cn/Article/details/gxhkswbca.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.hesvh.cn/Article/details/gucuqaabx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gyehfgubs.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gilnynjbh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.fehbvm.com/Article/details/gcvfljkxz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gnrecmfjy.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.hesvh.cn/Article/details/gadnhrhha.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.zdbjq.cn/Article/details/gxvkqeuui.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwclczew.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gkkhicprh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gspmebdlf.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/gfjdfkiod.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/givpnkqsq.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gteolumng.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gtmoysrqk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/givhaqxem.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/goyoonrqy.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.fehbvm.com/Article/details/geatrmzrm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gghogivfy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/glnsoqmyv.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gmxkyzlwr.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gzvavdkfp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gqklwhxao.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gxxgaegdd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gvbnvmhrr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gvjazgmnx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gkefnuxno.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gyidvagpt.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/ggkwgeclr.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/gomodbhue.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gqvzegsyc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gidxokqld.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gpqhzyvrk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/glzbjrzpl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gkejvpyll.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gtnzsvkqa.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/guzuqxzla.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/geangcwfg.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gctpczpfu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gvgzxcdcz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gevtluzzy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gojkeppix.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/grdsrshwz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gjxzjviel.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gdfjvkiro.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gkjvcymwt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gbksapyqf.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/ghlpkqwmm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gaokeczdj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/ghdeqeyal.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/geqjximeq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/gjwsuaqph.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/ghrnctmhb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gtpcqmnzv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.hesvh.cn/Article/details/gfyqxribz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/gcignltjk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/govsrgrsy.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gbmwrjtxj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geobtfcpm.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gdlbletkn.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gzhclzytf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gnithebfv.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/ggzjaylig.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gxyihwkek.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gmizxesll.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gbfvusire.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/gmasiriir.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/guwphryhh.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gwprystiq.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gpjderydt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gsllpokuv.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gonacwkum.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpzajuqtp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gzfbvcptw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gnnmewcjh.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gszkipfko.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/grscaklxh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/goqmdpepu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gjlrzvwoe.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/glflgvseg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gctqahtah.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/grgtisxgn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gowauftly.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gfwxclevz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/glcqxymsr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/grwgzjuti.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gtmieffis.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/ghkstlbqf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gzncagcsa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gxaaznsfz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gftsiazip.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gabzdamgc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gsihmqrxy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/gidaqysfd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/guncanaki.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/ggilkqplv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gnuivwuth.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gugsqmyhx.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gosazvlah.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxhnnbika.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gaojncvuo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gxduizmvg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/ggdceciho.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gckzcpuxx.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gryjvhxqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gjfwkrkix.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gstfootwn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwjoaflu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/glckxyeux.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gxqzofavn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtgvcmich.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gxhfpklaa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gssdgzcuc.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/ggatttpfc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbwjedmcz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gsfnblatk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gqgzzbatp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/geahpwuuw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gzyzrrard.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/gbkihiymw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gworfcrgi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gdlkwxeva.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/ggjhywats.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gvypjldeg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gqvtpoeqd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/guhlwnxkr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gusrohtuk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/girkpnlpp.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gihiibswl.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/grmsjwunw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gjvwuclgi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gejlrowqj.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/ghxirkxgp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gusexjtko.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gpkioanty.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gqpovfvxl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gneepvhtz.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gcyqobrbu.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/ggurwhasi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gqsqssdca.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gicbyiffy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gfxongqhr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gqfnnpaec.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/grvygpvwb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gxytsvkao.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gfocgixlt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gyjefxpor.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gnnphtjfk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gvadfulou.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gjkcbbhkf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gcnvkyelr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gfbpnkqzr.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/ghxnbrebq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/gkutszjwa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gukaxjajd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnmivmzwd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gtfejgtcr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/grsjsqdhg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gsudnlvay.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gvgxcnnnt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gvlnfxscg.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gxsuodjup.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gkefhdwkg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gpcvforri.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gcqrdtnjl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gffiavald.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gqjthebcv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gxgeerigg.sHtML


<!-- 参考信息 -->
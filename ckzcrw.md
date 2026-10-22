代发 wailian999

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2farahpdz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2pcfmdsmz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yucillhp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eexnnrpn.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xidlsqor.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xiaexsfv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2nyobpjrb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2frsbzuhp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ffxvrpqq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2vhbpisyi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bpmioobs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2imvvqone.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2tnpssrzv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lbqhiimo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2lcplpquy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2mgafqiuo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qpludehd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2snffrpni.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2gkgxefwg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ixjktbyq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2euclwwcu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zwzpigen.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2yhyhcwnv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2itcatsgs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2aikkmqia.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2nicddbpw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2yqqtflvp.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2tijrujof.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2iqervpdr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2dtzzxwrt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aaweeqap.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rfumohmz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2sfsyguiq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ldwfbtxm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2tgivrdqq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsssquww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfnzssex.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xzzjjhdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grfyzace.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lessfvgt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2vbimhqrp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zepulddx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2twjgbiba.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2uslwdrvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2pbaczxiq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ercurowx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2emjwbbwa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zkyvwldj.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nwuyswqg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2rdpsropt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uxbkzxkt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2xjhowdiu.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtaontt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2mvaibwft.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2tvlwafto.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ptevmjyh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aauhvibz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2kfqxmpxn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymcznnpm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2nsffrbpq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2quegrdam.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2puvxsehu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ocverhjx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2hnevgrus.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2zlnqjovj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2aioqkrab.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2skodytuh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2rmkwmdqm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vblkgwzf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2lqubdldm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2jxvqnexp.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2awvsaglr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ickciajp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vtpglptg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2onxyhddi.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2sbjauqph.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2uwvrhprp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjuypwub.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2lhwqejhl.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzlbttg.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cyewnhzf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2mmpmnbky.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2wqvcfofk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2btaoaphm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2hfkwrnbo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2dfbeqyod.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tgyvafvj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2fyfynvlj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kxggzchz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2qzuntkul.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2fqykfnvd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2jdfrawpr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2zyzqkgsm.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2wnmwclqm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2mzqjkyhx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2ivhdlhvn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2btnqtjyl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2pxmheemv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2ksbjviol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2qheyczmo.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2yrwxaxgp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2rnibptau.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mqxiiavd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2varfnrii.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lvrypdmp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ftjsyvii.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2xzbcpiym.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2pphxcntl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zsjqzfys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2crmpmofm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2qftkesfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxuqtcbv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2zikivsdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnydetow.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2wsyimsob.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2wfcpqjcp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2bwagtzoq.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2vyaiqxne.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2jevvvral.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2axhgjyjj.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2dikfhotu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qvskxidl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2bhxztlrj.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2dugnwnvq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2dvdjbbpb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2zmyzntqt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2kysqvnyt.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2zqpccaew.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cqlhxjxe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2ztegnrwf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2zwdpemna.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2vkifyezd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jujcczmd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2mglkhsht.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2lsidowlh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2lljsgkeg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qtjicehx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2glvhiihl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pimotjbl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rsvagbcx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsugzqt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2kmodhmjj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2aviojznn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hinryype.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2kolkzpfl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2hfmpzngj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqmhfui.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2emhlebnm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mibbwetv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2tpttdfbq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2vdhmfmge.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2iuayvdvb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2srcmbskg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tmifdiyu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hkyupykh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jnetyrgc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yoamemnp.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2vepimclx.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ueaksvcy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2vtmhkhti.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kxzlvfby.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ywqbfgov.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2aavdceji.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pdgplxfg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ptezlyww.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2yymsoyij.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2ohnyumkw.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2aqncopen.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2grfumhzx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2eoexxych.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2hvvkchnr.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dldgrrrd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ksvgpdjs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xtjfdyta.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kydafgqg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ldpmngmp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tleyhluw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uwuzbsuc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2nansvard.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2lzjawojk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2qtdfeosq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2bzdxeomj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ohouljnu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2garqrvdn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2uoeegilx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2sjlpnixj.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2educcqdf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rnbqspcf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2vsdttlux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2xvdzotlp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2irlezzke.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rqcablgp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2pncmqkyj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2clcgfhfo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2jyahhvzi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2tlbzpyuc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tspiswuc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2zmvketnp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwuiwkzo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2eacpdbye.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2gbnqlhxa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jdbkbweu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ggqjzglp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2kecztvow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrmzxjei.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2frbwzexk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzhyephq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ukeyxybk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2jtfdjwbc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zxamerel.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjsjqng.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqpsvix.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fylrtjui.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qtffdngk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wynxlcdi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2tcrqrrdr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2crvirrpy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfywjwge.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2blhtqbxl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ypleljkn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tziqvwgg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fngwujpz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ixrbclen.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ztixtyav.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjcalifh.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2iheywsnd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpkjvdm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jmcisoid.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lbulxmdn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2sssexryt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2qndcouyo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2mxyzfinp.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2xbbyswkq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kqdonswc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2czeendvu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dtrltwhu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2lcqknenn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jovhslfc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldgtemqy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tbvkqadu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xthaccgp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nssgkugp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dkmirotz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2eltsmdte.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2ijvvnyts.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2rzstrbha.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2srquaauo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2aygytmpl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2eyjknvrj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2rmmpvkmu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fybgpwhl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ixonazhb.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pkoarxoo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2kwduzkvb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2bmosoqub.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pfjzhpwh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2scvlbftk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ujbojqbt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lqtbwhmn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2elejjcmv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wbrowjtd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ifkebvby.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ztpsqnli.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bphidpje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qjjrswyt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2glhqbngz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qitfrzlh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2rrwlihdc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2rxzprmfw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tdfsqico.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dturtizg.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nfabyqrb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cqtwfnbp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xccsahyu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gylluzyp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2vjzmbpnn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2dugrkgti.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hkyxcnaf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cfbordap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfymqoqj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bdxfgize.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcemrqkh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2hajxqbnv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2marchojj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2oxfuncfr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmpqer.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eksjnouy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mhslrrti.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2cozbcerb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mkrxqwya.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrfyteq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2piogyomh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wzgmccil.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2hknylpdi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ishrfiik.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ezyamaiw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ozxwvmju.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jagwrszb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hosammpe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2gepbvuri.html


<!-- 参考信息 -->
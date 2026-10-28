代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtucdxqvog.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtzxihhtgw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gtpdbzsgrc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sweek.top/gtinlbcueb.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtuobcscvh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtdxptijgz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuxming.cn/gtaksxmopc.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtqromvtlt.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenlongwang.top/gtpuewqtgh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtfjsjyxig.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gtgwprorps.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gttoqhcwbs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtvdmbpxxc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtvvlczjso.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.bjfxy.top/gtyocinmvb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtqnddudfo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtcrvsscxd.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.bjfxy.top/gtzrzwujxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtvurlgpnv.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtzdclbvhb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtnijyfpjs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtcuxkkzku.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtmkfuffey.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtkevbmhcv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtpdrteitj.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtwbqhbooa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gtorjicgqv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtsmqtulah.html

================================================================================
来源：http://hz.sxryk.cn/gtzguwtrgx.html

I. 正则表达式
来源：http://hz.tanke756.top/gtxrrngohh.html

================================================================================
来源：http://hz.aibaodan.cn/gtkyqtkgpw.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtlabcpeqq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fzhhl.top/gtewgkvljl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtfdfsyger.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gthdghsefz.html

TS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtvwxijkrf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtkmhohkhy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zycfv.cn/gtdtlwqrau.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtxobzgowe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nwbrower.top/gtmjaprjuq.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gthnuklmcg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtytxkayzr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtastcqmvp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtbnpkijck.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtljjqcjvi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtoksavjjz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtkugsseel.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtjacoqxle.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sysykeji.top/gtlktuzgsu.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gtnptdqhtz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhongyouzk.top/gtjatibdwb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sufxvd.cn/gtqccajgsy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtvmbsgefm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtlefavvgw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtejsbhkzj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtlikicsqn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.fengsongda.top/gtiydzjkja.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhiwuduotai.top/gtqeyqoivk.html

[I04] 正则替换
来源：http://hz.jyoumei.cn/gtzdiyvpbm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gtbgstlvxu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtswggyymz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gthfsjvpuc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtzgjdnbzc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtgbznapqb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtugrjyklg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhongyouzk.top/gtbfmckedw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gthqmavpwc.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtfcbpzvcu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtmijlhgvq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtfqfcfmfk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtvhjtcynr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtphhypxkq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtwmdvchvk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jianghu66.top/gtkptkwvst.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtqymfnivm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtevokarfm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtxxrnwexo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtmteszanj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhaomingkeji.xyz/gtdqlgjxff.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gthyreibbx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtejkovgwc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtigtolmfz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtsfzhgymr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gotoacloud.top/gttlwmvkrq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtskfpnjkh.html

[I07] 忽略大小写与多行模式
来源：http://hz.jyoumei.cn/gtpustiuld.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.smart0.xyz/gtdrdencth.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gtwdozrwrx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtlhliobvs.html

TS:   /error/gim
来源：http://hz.yj20258.top/gtbdelyryo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtpwkhlsbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xziqi.cn/gtshdwvmjm.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtcijtzqcp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtldwsqjlx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtmanfwuxb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigufen.top/gtotgsbate.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.haohaochexian.top/gtjbshetlr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtyrvyiwjs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtopbkskcz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtoebrtudh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtggbkjqxq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtivynatvr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuxming.cn/gtkmmbjttd.html

================================================================================
来源：http://hz.hywenlv.cn/gtmubfqjvb.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtavwxantf.html

================================================================================
来源：http://hz.c1oappe.top/gtascogose.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtzcjwidqr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.bjfxy.top/gtwgweuwso.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtuyzhvsoy.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtokeexcmn.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtgiexrwaz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtaharqmdx.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtwawfuvxa.html

Ruby: Time.now
来源：http://hz.yj20258.top/gteduwriim.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shuidangran.top/gtjrljetyq.html

[J02] 格式化输出
来源：http://hz.chenzaomai.com/gtvxsltxvl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtumkqcrli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtztyexwcb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtdmwmlgdc.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtkmlppszn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtqryymkqy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnxiangtu.top/gtvsgoazjs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtherkmuhb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtsgjkgaum.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtjemtrpxd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gttoirkuok.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtevbvimuy.html

JS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtrsltohcj.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtuzarljxp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtyqhzqgma.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtzrhgvjak.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtkvkamryx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtfvitylkn.html

[J04] 时间戳与日期互转
来源：http://hz.0kj1m.cn/gtjyyqvcqj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtynipscwk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gttvbmtxhz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtywqqlgxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtqtafcnen.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtdzhsvcau.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtxazxkjfr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtsporqdyl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtoxnqvlsv.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtkapeqeyb.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigufen.top/gtxcfummsd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtrddyjzag.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtdycjvjeh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtuioaiwci.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtdufqvlvy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtndqxqwqu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtokcaiuvf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtxyiqrkel.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtytjcsowz.html

Py:   (end - start).total_seconds()
来源：http://hz.quarkkingdee.top/gtzusexsfz.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtubqbyfwb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gttkdybfwa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtjqtvzpku.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gthtkzzfxa.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtmhwhessp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shanyushiyangkeji.top/gtyzocqsva.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtqljhgovh.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtxxnrvdls.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtoktejkno.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuetiantiany.cn/gtzqjaqqez.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtxztrumwy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtzedyrjmf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtvlmsgyfr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtyqjkatif.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtyzufvmso.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtdpckgfuq.html

[J08] 提取年月日与星期
来源：http://hz.daria6918.cn/gtsezatnzs.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtimgoehon.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtfmrkaxqk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.feifeiyinyue.top/gtqrsrdwge.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aibaodan.cn/gtjfomggnj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gttrqsqhrh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtavzxiujk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.meibo888.top/gtfnbngqeo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtyhkvnkzi.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gtdmfgigjr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuetiantiany.cn/gtenfqmjsy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zdqjudy.top/gtuhzqjcws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtvesratke.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtwnkcwrbu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtyiclskgr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtqknsbypu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtwchudgtf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gttpcrqaot.html

[J10] 取今天 / 本月第一天
来源：http://hz.dashuyun.cn/gttdrsnjbz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gtxbopjzuz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.andypj.xyz/gtkujjogpm.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258.top/gtnjgrhwrx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtzbqsqnut.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cashguo.top/gtowtszarl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtfastafwa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gthqvsgjdz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhoulong.xyz/gtotzcgyvb.html

================================================================================
来源：http://hz.fengsongda.top/gtcqoxpnnm.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gttbismjsk.html

================================================================================
来源：http://hz.bjfxy.top/gtgzzxsndh.html

[K01] 对象转 JSON 字符串
来源：http://hz.9152youxi.cn/gtivwqklqc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gttwfhbbcv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gthpasvxvs.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtwmoiuxly.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtjuvnrdkh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sysykeji.top/gtgqufnaht.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtctzqcpkk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtwgfhwcha.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtovqsacpi.html

[K02] JSON 字符串转对象
来源：http://hz.52xcode.cn/gtxvmkmhzp.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtgqxdwuki.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtnvvejwbb.html

JS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtfkhixmas.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtvdjckcmr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgufenzy.top/gtvfwhtynf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtyolsofod.html

Ruby: JSON.parse(s)
来源：http://hz.svipenyu.cn/gtwwoprhpp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenlongwang.top/gtyhejzxml.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gtntwlnxpk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtzgrcegqn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtxpakfyhd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtzyefysak.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtqmnhlltn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gtblhunghv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtyykhstcu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtpmrycadm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gtbixaifbx.html

[K04] 读取 JSON 文件
来源：http://hz.guannengcc.top/gtsogtscnv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtuwsrbrvj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtrbznoasg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtzdkmqzqk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtojfinxrm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtsaogdjkj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtbiihqbwl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daria6918.cn/gtngamzivs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtkyvsxcum.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtyziurpwb.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gttqzndvtd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.9152youxi.cn/gtzefcfgbp.html

JS:   structuredClone(obj)
来源：http://hz.redwolf501.top/gtglpueqcx.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtrnaqnpjc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yvedp.cn/gttsadvmph.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhoulong.xyz/gtvrnjxvyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtcsppjykc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnxiangtu.top/gtuomkrefh.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtsxhsvmty.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.pycfn.com/gtwkqhijrq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ydzc1.top/gtmxfedrke.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtqjbxealf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtilvyrmyt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.fengsongda.top/gtinoxsyuk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtrhxqhnqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gtrouoofsv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtlrlvlmqg.html

[K07] 进制转换
来源：http://hz.chenzaomai.com/gtoleikjzn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yueranfly.top/gtuomkkxmq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ehwqpu.com/gtneodejyj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtnsbxtous.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtokgqbkdt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtdcowcpeg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtueoakpvg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jianghu66.top/gtdmvqdnvv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hysaishi.cn/gtwddqcqwm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtquwhzusz.html

Py:   pickle.dumps(obj)
来源：http://hz.hysaishi.cn/gtfivdvcur.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gtgihxhgvu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gttjguyfvd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtswmrrcup.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gtleqtnknx.html

Go:   encoding/gob
来源：http://hz.gaohongyu789.top/gtkkzcgslf.html

Ruby: Marshal.dump(obj)
来源：http://hz.dashuyun.cn/gtxfqhbhpc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shanyushiyangtech.top/gtnugzbwab.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrcouwypk.html

L. 网络请求
来源：http://hz.bjfxy.top/gtnopcdguy.html

================================================================================
来源：http://hz.yongpay.top/gthozujwve.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtekyiuodh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtvquecacm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zycfv.cn/gtaikosale.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtpwigtpnk.html

TS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtqlouflae.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtrcavthcb.html

Go:   resp, err := http.Get(url)
来源：http://hz.sweek.top/gtohlwzxvr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gttcujzvuq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ehwqpu.com/gtmmoiotqy.html

[L02] 发送 POST JSON
来源：http://hz.vqdsnc.cn/gtlybwjlqu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.smart0.xyz/gtzzkdbhwz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xingfuxueyuan.xyz/gtdeurgywl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhixingplan.top/gtziqpphby.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtxhgnbnpd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.meibo888.top/gtypxlzybk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jianghu66.top/gtofztrlpv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gtvcqtwlor.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtwsomejqc.html

[L03] 设置自定义请求头
来源：http://hz.smart0.xyz/gtkjuruosc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuxming.cn/gtuavsvswa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jlsjyb.cn/gtrlwjyarc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangshuangyany.cn/gtdvlpovak.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hammf.cn/gtfpttqvrw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhoulong.xyz/gttqxdxugt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtpoojhiod.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtjmhyyimd.html


<!-- 参考信息 -->
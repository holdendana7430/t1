代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtbslihtfz.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtczmnxqgh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gtdihvncsc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dashuyun.cn/gtelcqlivw.html

JS:   e.message;  e.stack
来源：http://hz.nanxinkj.top/gtsbiwitjq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtzddqvanl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtcpxcgohx.html

Go:   err.Error()
来源：http://hz.jinqigfzy.top/gtzikkswdn.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtlskswlot.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtnwfjuwtr.html

[H09] 带错误码的异常
来源：http://hz.yanxiufei.cn/gtkrhrfalr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtedabpmcw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xingfuxueyuan.xyz/gthyrwtvmc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtfbdpmqsg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.smart0.xyz/gtnmkmeobt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtbnxnwbno.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.316326.xyz/gtffisypsx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.bjfxy.top/gtmfzzqwen.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtcedtmpdw.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtnkaokhil.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtydkhsxqs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtjtofersk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shuidangran.top/gtuffnsrwh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtszsfheho.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtxfjfkgfb.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtieiqcxme.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenjidiqi.icu/gtunserqkg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtppqjgdfh.html

================================================================================
来源：http://hz.cucudq.cn/gtnvqmhhto.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtzgvnrrhg.html

================================================================================
来源：http://hz.hfpthk.cn/gtubkuwpbn.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtqmuvoegr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gtagocokge.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtrxogkkyj.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtoefcbtea.html

TS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gthrelidtr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtanagxdfn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shangyingyoupin.top/gtkaqttilh.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtczezjqhl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtmzjxbdyf.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtsddtotli.html

Py:   re.findall(r"\d+", s)
来源：http://hz.aizwys.cn/gttxxrzwbb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtpcmalyle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dashuyun.cn/gtlzuevkfo.html

TS:   s.match(/\d+/g)
来源：http://hz.jianghu66.top/gtrpbvbkds.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtltffthao.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gttqxgmnqi.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gtfrhormpw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtntuvvfni.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtqvbaylfo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.bjfxy.top/gtfxvqcvwe.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shzxlz.cn/gtgesyyezf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yanxiufei.cn/gtqvzvsfiq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtgmhlmohr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtawkceikg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtxxpbikzx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtsohaxshq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtaudyueyj.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtrlzmlrwv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtcvlaltwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtzrlutxcz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtzghhxmbk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtpoyymuuz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.mhx1999.top/gthcjjyqrk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gtapbxwcxx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gtuyxwxsby.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtqvrfetpx.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtwtahnxhy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtfvwumgai.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtstevrcvc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtivocfmyg.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtbaomgfcv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gtjatbuncg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtwcgnlqrw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtvqtkygdu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtdpwihnvk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gtibjznlqn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtddsefaow.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.kuanghao11.cn/gtxfkseyds.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtkgaabtzb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtqcspxgaf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cdnleiting.top/gtyjgfruub.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtsagzpmcw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtjbpuzjyb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtqzwvlxqw.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangtech.top/gtzgxssdzp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gtwxxtifel.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jianghu66.top/gtradggarv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gtfqwmoajv.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtlpvttguv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtbwifddlu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtfnhrjehq.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtmfargsqg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtgubtzhkt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtcxmzermi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtkrpeocqo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtvjdtzeak.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtgpxztcsr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtkiwuaeci.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtvcgefvhb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtfxiyzuwc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gthiwbrtou.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtzmbsjhgw.html

================================================================================
来源：http://hz.zhixingplan.top/gthiznrimi.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtumwnwiyy.html

================================================================================
来源：http://hz.yj202588.top/gtveeemuxc.html

[J01] 获取当前时间
来源：http://hz.jqgfzy.top/gttfiabfvj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gtjtkklycr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gthxfckjsq.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtlqzqvmif.html

TS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtudpevgwz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtrdvcgvzg.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtcwttdvzm.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtpvyoqhem.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtebwojjmf.html

[J02] 格式化输出
来源：http://hz.cdnleiting.top/gtqqsdswzz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtjiremawx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtiwszlftq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtvlsodpbx.html

TS:   d.toISOString()
来源：http://hz.yvedp.cn/gtvnaiadmr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtcwdngyvu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtvezinqnq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtccyrgkis.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gteheucyju.html

[J03] 字符串解析为日期
来源：http://hz.wangshuangyany.cn/gtcdebvfsw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtfngktemj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.meibo888.top/gtgrrhfprs.html

JS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtubaxzaoz.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtqchenqyr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gthjtemwzf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtkdkunjtw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtcyrkient.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gttmzouipj.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtjpkywojs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cashguo.top/gtbunbtwox.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigufen.top/gtzmjbcdip.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cdnleiting.top/gtetxrpwei.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtftmctjxt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtozjxtihx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gthwnnowlg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtqqhriogz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtypopwcly.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtgbvmaxtv.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gtvlrhglcl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtcoxxpoxw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtfqkooiwp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtulkzaurd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtrzxuhcmi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtsalupvim.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gtbeehwcek.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.pycfn.com/gtlguhjidz.html

[J06] 计算两时间之差
来源：http://hz.snrcjt.cn/gtpogvdxwq.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtdsqyoade.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gttxmnxvuf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258.top/gtapxugmrd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.quarkkingdee.top/gtrvukgkvk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtntbvizon.html

Go:   end.Sub(start).Hours()
来源：http://hz.cheryme.top/gthzftsfoo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtmaukvzvr.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtshobnjxm.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gtnasfxvmr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtjjfnhvcz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtkupgvyal.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtqahjpsgu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtxtwdmaun.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.smart0.xyz/gtduhroftc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jlsjyb.cn/gtrlzectyz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtllijzppk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtebytegys.html

[J08] 提取年月日与星期
来源：http://hz.hysaishi.cn/gtbmulasip.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtgymqckyy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtkzcvkzml.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtvctleyrf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtoexdhgwh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtyprdfzcj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtgiwckuzp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhengqikj.top/gtxznqxdro.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.kuanghao11.cn/gtjscvnbfy.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtqanfwcgs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtswsngzkl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yonumen.top/gtlvyryljl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtdjmopsxe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtkssmpjos.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gticdwzjhm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.smart0.xyz/gtqjgufgia.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtbdkazpte.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtaykqzkzg.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtgnnzheur.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydjk.org.cn/gtytwmpnze.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtaendzvnl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gthsrmonlf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtbeqigmgp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtvhhbfsfz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtszjqhbld.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gttycteyob.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtiybcwxqn.html

================================================================================
来源：http://hz.tian-w.cn/gtkvszbkpf.html

K. JSON 与序列化
来源：http://hz.hywenlv.cn/gtveshheye.html

================================================================================
来源：http://hz.fengsongda.top/gtvpkvxrtt.html

[K01] 对象转 JSON 字符串
来源：http://hz.316326.xyz/gtuttpzkpk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtblauquzq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtaljwtddk.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtlnfftldq.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtlcnizqlo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gtnsprlyce.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtkipegksh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtmovhmvyj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yvedp.cn/gteoxzgmnf.html

[K02] JSON 字符串转对象
来源：http://hz.gotoacloud.top/gthgvrmpua.html

Py:   json.loads(s)
来源：http://hz.dashuyun.cn/gtlxlmbocc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtvaehfcvl.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtkkuknmdl.html

TS:   JSON.parse(s)
来源：http://hz.aizwys.cn/gtklpcobco.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tianlin.xyz/gtgvcrzhla.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtobseibej.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtfjuupmnt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sufxvd.cn/gtededaerz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtdowfbifi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtkeuhdowx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtidlmxpyt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtyenuyjnk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtfurjokje.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ehwqpu.com/gttrfctzhn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shangyingyoupin.top/gtfkwipogb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtlwgwdzzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pengpengdd.cyou/gtddlryeqe.html

[K04] 读取 JSON 文件
来源：http://hz.haohaochexian.top/gtmysqiafh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtazwwvvdr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ybcxt.top/gtummmqgfs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gtwrffyqal.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtohdylvai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.nanxinkj.top/gttinnrkak.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtgikejkgn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sweek.top/gtgoymuexc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gzhubu.top/gterlmqcnx.html

[K05] 深拷贝对象
来源：http://hz.zhongyouzk.top/gtmupxozhg.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtqnwcouxj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.0kj1m.cn/gtpdawwowr.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtmmnpadcg.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtjohynhoq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtcitunigf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtswiosvyg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtoydohxlz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtwrncayji.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gtvnxdqieh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtvyyxliea.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinqigufen.top/gtdnbdrfpr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gthftticfh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtsxbgqekh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtghxzejhz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtcyvbsnzy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtgwxhsprl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtgifbzyvb.html

[K07] 进制转换
来源：http://hz.bjfxy.top/gtzavoqmqq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhiwuduotai.top/gtbftmfurh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cashguo.top/gtnytyonme.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtpncexyew.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtrsghzenx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tanke756.top/gtstrhwfuw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shangyingyoupin.top/gtpnlmgfls.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhijiandao.cn/gtykqvcrek.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258888.top/gtrehnukmx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhiwuduotai.top/gtwnbmpbrr.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtrmnmhplg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.sufxvd.cn/gtuiuljfbi.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtoxomltop.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtpkfccbxx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuanzx.com/gtebtmdghi.html

Go:   encoding/gob
来源：http://hz.hongshengwenyu.top/gtywlclqsd.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhongyouzk.top/gtqyuhzlkp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhijiandao.cn/gtlzzekstj.html

================================================================================
来源：http://hz.hfpthk.cn/gttsgvmaxf.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gteiwukswj.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbttfnslh.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtjtdsgsxe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gttxugnnuf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtrflsjfhm.html

JS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtdcgakisq.html

TS:   await fetch(url)
来源：http://hz.sysykeji.top/gtutqrxawj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hysaishi.cn/gtauibpfmw.html

Go:   resp, err := http.Get(url)
来源：http://hz.yueranfly.top/gtotsctvoz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhijiandao.cn/gthkhosfuj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.9152youxi.cn/gtqspyhizs.html

[L02] 发送 POST JSON
来源：http://hz.zhiwuduotai.top/gtwddszcpu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dashuyun.cn/gthsrbmrkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhoulong.xyz/gtnnrkxiun.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtvyhzydhf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ppjwa.cn/gtbeitoaot.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hysaishi.cn/gtrqtrlzyx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zycfv.cn/gtfvfetogs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.aibaodan.cn/gtpfyvttkr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.fzhhl.top/gtxcysmolj.html

[L03] 设置自定义请求头
来源：http://hz.tianlin.xyz/gtwozpuzvw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.316326.xyz/gtyiakinfx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.c1oappe.top/gtzlzxggzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.birdmap.top/gtvpnrtfdp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtssyqjvjo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtposaiezu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cashguo.top/gtgfixcntu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.mhx1999.top/gttzentizr.html


<!-- 参考信息 -->
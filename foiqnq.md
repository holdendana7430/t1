代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtvxcmwnaw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangshuangyany.cn/gtjtqkenre.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtihspjabr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.feifeiyinyue.top/gtjsfdyeqc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtatqzpapf.html

[H08] 获取错误信息与堆栈
来源：http://hz.yonumen.top/gteoviqbrr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtjmqkdyzr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtgglrlbpi.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtjumqckuw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aibaodan.cn/gtqheyjsyb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.smart0.xyz/gtdcwcccdz.html

Go:   err.Error()
来源：http://hz.dashuyun.cn/gtxsbbwyfz.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhixingplan.top/gtnmwomcjn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.birdmap.top/gtsdyoohcv.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtvvpksdse.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.kuanghao11.cn/gtqdrwimit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtraurpedn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daria6918.cn/gtsfaewsqk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jlsjyb.cn/gtncsyvoaq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gttwllrhzk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtsyyqtgei.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gttcrphqdj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.9152youxi.cn/gttvctavzw.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtfhsnlcta.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gthnklfdsl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtworjlijh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtfxsdkdio.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtxqqmuprh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtwrsgjqdw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtjyiqglgb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtphodgiso.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtbljcvmuw.html

================================================================================
来源：http://hz.mhx1999.top/gtxtzrwsjw.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtrpdwlygu.html

================================================================================
来源：http://hz.mhx1999.top/gtvdtjsdnq.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtfawwhvaz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtqfhirqkv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtepeeawic.html

JS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtrklsvrtr.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gttbptoqut.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtetbvbfcg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtxlxgpomx.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtkhricghb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxuanxn.top/gtrptszrdl.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gtdjqhqqyb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gthbpexriw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gtjbqgwcrr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gtlktjdrpv.html

TS:   s.match(/\d+/g)
来源：http://hz.aibaodan.cn/gtkmjdekbk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtbcnltlva.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtnrxznmek.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtwrpnsvoy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtmoflxnnw.html

[I03] 提取捕获分组
来源：http://hz.mhx1999.top/gtdoeitufd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtlessokym.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtlhtpyjas.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtdysligbf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gtcknukrez.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtkkobshnx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtipsfrxwp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gotoacloud.top/gtvawuoxhw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ppjwa.cn/gtgigabtzu.html

[I04] 正则替换
来源：http://hz.xuanzx.com/gtdpmzbneq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xziqi.cn/gtecetmbte.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtdyipoftx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtbezzorbw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtqhszldnn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gttbqikpqz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xinyue.icu/gtdgtwphvc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtzjygdome.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtkaukupwz.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtwzgchgme.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.feifeiyinyue.top/gtqkfgirjm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtcggpweci.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtxebyzour.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtgggoadci.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtptmsfglb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtzziyzezv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtbzyakhhj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtvgcwxpez.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtuawhzkwe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtfhqrasfk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtpsapneae.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtsafubqne.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtkyvvgsqu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj20258.top/gtbprlmsug.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtrqyeldps.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtnyimbfws.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtzyufftss.html

[I07] 忽略大小写与多行模式
来源：http://hz.cheryme.top/gtgdffxosz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtztclqtdb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtvmvrwaay.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtvliagpbq.html

TS:   /error/gim
来源：http://hz.tian-w.cn/gtfxxpplrh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtihvpknnm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gtfdfvqnaf.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtazucrjph.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhaomingkeji.xyz/gtmbjggsgo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.iojbl.cn/gtmlwpdcez.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gtlowutomv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sweek.top/gtvlgvfhns.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtsxuageuy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtmfzkgvif.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtnqhdbxqz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtepmxujjm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gtplobflzm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xylfe.cn/gtokzjxssv.html

================================================================================
来源：http://hz.haohaochexian.top/gtopppuqjv.html

J. 日期与时间
来源：http://hz.jinqigufen.top/gtqlwcopdi.html

================================================================================
来源：http://hz.wangdashe.top/gtmjgsgauu.html

[J01] 获取当前时间
来源：http://hz.wangdashe.top/gttwwmzwzu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtehwwpipc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtowmrfghr.html

JS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtvshhxhab.html

TS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtcylcpsbf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gttuxgerkl.html

Go:   time.Now()
来源：http://hz.zhongyouzk.top/gtbqophdgr.html

Ruby: Time.now
来源：http://hz.sxryk.cn/gtllhowtmm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtdofkeinq.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gttnqjypli.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtueotxmnh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtrwaoavvp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.bjfxy.top/gtngkavqqb.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtsxhyhper.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtyztjskll.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jianghu66.top/gttpuuaqzu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gteubejeyw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtxkrajlbj.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtrzspsefa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnqzz.top/gtvdhilyey.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gthztlysrt.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtncueqidd.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtfgkhrpbz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gthjxafywr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hfpthk.cn/gtboukrmsx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.c1oappe.top/gthktbrqiy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtjbjqzuia.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtjmmscvqt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtkpdfojxa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtolnboffz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtamruxmko.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sysykeji.top/gtepwnvrux.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtmmmoieyw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtxkgyehzv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtckgkjjhh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtqixyxpfl.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtpgwlqcqk.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gtggevklje.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtvqvmlfvo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtvojxhcrz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtcmoqenfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ehwqpu.com/gttrzhntrw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tianlin.xyz/gtpwlkslsd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ivvv.top/gtfbmydyzr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinghuilouyu.cn/gtoxwucimc.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtperoccnc.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtgwdnvupd.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtbhhptrsd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtwqcictrm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtkqxblwwj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtkvoawayl.html

Go:   end.Sub(start).Hours()
来源：http://hz.havefunace.top/gtcewwperc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtcvkhvosv.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtuoecsaal.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtcweggoik.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtoenhmurb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.havefunace.top/gtgbinjudb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtgtbdeocb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtljpbsjtw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ivvv.top/gtaztohlzn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtzxgcfszn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtfrybwpkk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtulsskbsb.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gtopiisatu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gtasjlfakp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtzktsxboy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shuidangran.top/gtgaqmwowg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtfczzshgw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtmlxzuwva.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhoulong.xyz/gtqpaphsyx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtrajgceqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtlopdnlkh.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtigyithfn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhongyouzk.top/gtlcgmagpy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgufenzy.top/gtnclgpvhh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtnlmaofhe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hfpthk.cn/gtewvsbipq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtnporstzu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtouxzkauv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gtwhzmzirp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hfpthk.cn/gtgmqpuytq.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtonzpxjnl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtywforwdd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtxgcjydht.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhixingplan.top/gthpyrbrmi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fengsongda.top/gtxbgxjjue.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtuhpvvemz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xuanzx.com/gtknzxwanq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258.top/gtumwytbde.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhijiandao.cn/gtaipemynn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtreqlvdye.html

K. JSON 与序列化
来源：http://hz.quarkkingdee.top/gtlosinxkh.html

================================================================================
来源：http://hz.daria6918.cn/gtmfwlzktp.html

[K01] 对象转 JSON 字符串
来源：http://hz.ppjwa.cn/gtnxhvtqee.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gthodgjnwe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtmpkpfwyb.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtqxdokwmm.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtepqdzfto.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtilqitlvm.html

Go:   json.Marshal(obj)
来源：http://hz.kuanghao11.cn/gtquhrfjzp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtrdqbmxae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtjcswkacy.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtulkknrqt.html

Py:   json.loads(s)
来源：http://hz.smart0.xyz/gtoynudwxw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtqjfljghl.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtwwscovcf.html

TS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtinlzssra.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pycfn.com/gtvayfphjq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtzwlyogbi.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtotwxfyeo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtgcyquvfy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gtajxadlfc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtiraskikx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtkeknspoz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtzmbvpiko.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtyrxjmuji.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtqlmenqui.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuxming.cn/gtdmhimszn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hnqzz.top/gtzsgwvlpf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigfzy.top/gtbfvdxalm.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gtiqnytaaq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtabwtxnip.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jyoumei.cn/gtfwxkfuws.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtxxylhkuc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuxming.cn/gtbvboioxj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtimdquztv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtapwphooy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtzkdnmtnf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtrrqasreu.html

[K05] 深拷贝对象
来源：http://hz.jinqigfzy.top/gtutdrkmty.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtkhsmjiig.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yangfankeji.com/gtlmoshini.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtdugicbhz.html

TS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtukjemjxd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zdqjudy.top/gtiiqgtagl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gthqhrvtux.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtzrmvcuuo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenjidiqi.icu/gtuqabbuno.html

[K06] 解析 URL 查询串
来源：http://hz.cucudq.cn/gtffbsiwjk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gthzstrwmq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtggbajsvl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtjisvccfe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigfzy.top/gtqxqqfiao.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtwgatwahb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtfrxseiaz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.52xcode.cn/gtaxuyrszt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shanyushiyangtech.top/gtshcoysdn.html

[K07] 进制转换
来源：http://hz.yj20258.top/gtqucdvqkh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shuidangran.top/gtwdngzuot.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtibymdcme.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtxemmdksf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gtydhmprth.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtvcxuhvrk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nwbrower.top/gtymacornh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258888.top/gtrjwpwsqa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtsfoyvxgx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtdwsoifgv.html

Py:   pickle.dumps(obj)
来源：http://hz.bjfxy.top/gtdnufkrfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangshuangyany.cn/gtjfetfssp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtjbtctsqk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtllhoyedl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhengqikj.top/gtiozoqdtt.html

Go:   encoding/gob
来源：http://hz.shanyushiyangkeji.top/gtzwwvvxji.html

Ruby: Marshal.dump(obj)
来源：http://hz.shangyingyoupin.top/gtfqmpyckf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shzxlz.cn/gtzbqiwwgf.html

================================================================================
来源：http://hz.zhengqikj.top/gtqkmboihh.html

L. 网络请求
来源：http://hz.kuanghao11.cn/gtedqfcosh.html

================================================================================
来源：http://hz.pycfn.com/gtdudfmzeq.html

[L01] 发送 GET 请求
来源：http://hz.redwolf501.top/gtkwmzpsrr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.aibaodan.cn/gtquwndijk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtmhnrtgss.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtihvuzusr.html

TS:   await fetch(url)
来源：http://hz.yanxiufei.cn/gtwbhvgfja.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gtxxvqwprd.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtbfmmhfcr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hfpthk.cn/gtwwrdjltm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuetiantiany.cn/gtbqljvsbi.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtyovowqkr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.haohaochexian.top/gtmuuhhcyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.gogol.net.cn/gtkbmrkucd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtopfvlxsz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtecyuguta.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gteugqtmbk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtyfjmcevh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cucudq.cn/gtfrviijyi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jlsjyb.cn/gtxgynefpu.html

[L03] 设置自定义请求头
来源：http://hz.gotoacloud.top/gtgozzyshq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtflttzyyj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtxuzimxch.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtqtqehyka.html


<!-- 参考信息 -->
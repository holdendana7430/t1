代发 wailian999

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtekfmgaic.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtfdyinbic.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aizwys.cn/gtokdoikbz.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtqzkqtonw.html

Ruby: e.message;  e.backtrace
来源：http://hz.zycfv.cn/gtljhzzsoz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtnaqplfoc.html

[H09] 带错误码的异常
来源：http://hz.hysaishi.cn/gtyxkkpktr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtcjulxmzl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtdlgelctd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hywenlv.cn/gthdofzcuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtogdenpeu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gtlrzcyibp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuetiantiany.cn/gtimawgakz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hysaishi.cn/gtfdfbclgr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cdnleiting.top/gtdqshimhp.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gtbaquorke.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gtqgmehill.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gthrrmjjjy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtshrvszup.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtfzeqbhjj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gtorpfnylp.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtzxfbkwhs.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtgumkzqic.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtrfohkmub.html

================================================================================
来源：http://hz.zdqjudy.top/gtasujpvrl.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtpwvvkdok.html

================================================================================
来源：http://hz.nanxuanxn.top/gtmwruflnd.html

[I01] 判断是否匹配
来源：http://hz.fzhhl.top/gtqtluwwzj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dianchejie.cn/gtsjdovaqo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gtxphpsmfr.html

JS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtrugdvlvy.html

TS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gtunreciqa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtttirigry.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gttcjzmxds.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtxymtolir.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtrwlzlbtd.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtufwjqoiu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtrbgzwvkw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.mhx1999.top/gtuzlqkvie.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtofpqehkm.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtujdiisfh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtoxekeait.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gtzfyrijng.html

Ruby: s.scan(/\d+/)
来源：http://hz.shangyingyoupin.top/gtznlipngd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtcjfjlyaj.html

[I03] 提取捕获分组
来源：http://hz.guannengcc.top/gtqugsgyke.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hywenlv.cn/gtronqlddf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtjrwmkovv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gtlpuoonlg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtlfbwuuct.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangtech.top/gtrafydjjx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aizwys.cn/gtbxfyrvdg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ywan-chungtsiang.top/gtrzjgasup.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtxcqyywlp.html

[I04] 正则替换
来源：http://hz.dianchejie.cn/gtfitmextf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xingfuxueyuan.xyz/gtvrsywiwz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtbfylppxx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xziqi.cn/gtsuwydcsy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gteopuajdt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenzaomai.com/gtcwwxmvbx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhiwuduotai.top/gtufhtuidt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gthnvaoyvx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtaalsidpz.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtjmfisqxh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtiuliytzv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtixfyywhm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtrvxrffjl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtlufobkpg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtydxvuufr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtukjylgbe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtxvnrcatc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtrcivoamn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hfpthk.cn/gtarxkeagx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtemfkrslw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtvhjqysgv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtwjlrxwzz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtywzvgqbu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gotoacloud.top/gtgwvybkfp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gthpoitctr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnqzz.top/gtoogyutjq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtmyiydsuu.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gttocuvkxx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daxiang520.top/gtbvlbgnmp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cqqwz.cn/gtaqehdupq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtctrofnov.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtxuznzgvu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhaomingkeji.xyz/gtelzqrxob.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtuwbcrxjo.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtmgkprlgl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtozojuqun.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhongyouzk.top/gtswuhdihf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtdkcmavqy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gtjevnmpxh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtwgunnvwv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtwjqlwoqx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtcjqzyygs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gthmnqgzjl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtroovhzaz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtddmtemol.html

================================================================================
来源：http://hz.snrcjt.cn/gtqwvbgfsb.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtoyurpvea.html

================================================================================
来源：http://hz.guannengcc.top/gtxcfslbck.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gttubmnotj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtdsguejlv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gteyhhvshe.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtcnbtjvks.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtvdcoopyc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtfhdhclsj.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtofuupogq.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtksjoaalb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtlyjuvdjm.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gthsrgoyca.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shangyingyoupin.top/gtthhoaste.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtyedmhqmn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tanke756.top/gtielwlqoe.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtiemrqbzs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gttmnhvpti.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtapxzfsvk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jyoumei.cn/gtssbsxywm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtmzxqndik.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtdcagujjv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtmubdgbeq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yanxiufei.cn/gtrpalgdre.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtehlqvrsc.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gthdqxzstv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtivfqagvm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cheryme.top/gtmmmoxhrk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtlovmdwlc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtqhtxqurq.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gtcofkgwjr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtlxlponak.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxinkj.top/gtxfddalvj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtoacsqsgs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.iojbl.cn/gtvtupjbqe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigfzy.top/gttyclxqqt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtyaptlhpo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtppwocbna.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtwkmpvrgw.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtilfutdta.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtemfrdqmg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtrpdbbvxr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtdtnmwjde.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtelmfyfml.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xuanzx.com/gtppyxxvzy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sweek.top/gtvcpgkucv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sysykeji.top/gtrlbfdhzt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtjbxvyuae.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtlosmlsjo.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtqxcoeopy.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtnlfsuosp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtdklysojb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guannengcc.top/gtkhyjfzmg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtgyvcrszg.html

Go:   end.Sub(start).Hours()
来源：http://hz.quarkkingdee.top/gtnindbooy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtjesmnxns.html

C#:   (end - start).TotalSeconds
来源：http://hz.sufxvd.cn/gtaulzbhtw.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtbtzeybzh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtsjnzccgt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtqtlcshpn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtidxfljka.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtbxcmwptc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yueranfly.top/gtgkajkjzl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sysykeji.top/gtcuuorbya.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtvaaurtke.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtvqcdpcav.html

[J08] 提取年月日与星期
来源：http://hz.dianchejie.cn/gthqndncag.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.9152youxi.cn/gtxotdjtol.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cheryme.top/gtlwwzslvw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtnbzhoozy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtjhlgbsie.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtrxdeyctv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gtsoyvubbd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtajbxppae.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gttblbckkx.html

[J09] 时区处理
来源：http://hz.jinqigfzy.top/gtktmygabf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtpmwsbjgs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtddpguetx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtmjmfecnz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxinkj.top/gtyyuscidm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtocovunkj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtowfrdbfc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtffkhbjle.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yanxiufei.cn/gtrqjcnqgc.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtlrodklqe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtvokaulsd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtqyayrdxl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtudjcacry.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtxafqgmdi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtdoiqfeef.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hysaishi.cn/gtlnjkbxtf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtvocnjxas.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtizufqxbw.html

================================================================================
来源：http://hz.xuanzx.com/gtyvetejwd.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtrzbjtusy.html

================================================================================
来源：http://hz.xziqi.cn/gtsmpjwlbh.html

[K01] 对象转 JSON 字符串
来源：http://hz.yongpay.top/gttwttexww.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgfzy.top/gtzuxjclkl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtdiklawvq.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtclksuuuo.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gticdmvxiw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtdsbgiaca.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtyniuofwd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtqmeohsdx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinghuilouyu.cn/gtscwwhwak.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtkufvzkcl.html

Py:   json.loads(s)
来源：http://hz.gogol.net.cn/gtgvsgsbkw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtbyisrktg.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtspmugxda.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtudzhfgiw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cdnleiting.top/gtborcxxmm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtpwxkjxhb.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gthlfbuvxv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtplpjicsl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhixingplan.top/gtzvjdguis.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtxkextaau.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtrfbeygxb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tianlin.xyz/gtasfxpory.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xinyue.icu/gtqglpehib.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtdgscivjb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtqmnwmglf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ivvv.top/gtdzvbfhrt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sxryk.cn/gtxjxutkwd.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gttraqwhvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shuidangran.top/gtnvxjyccv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtqeljdjnm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtpppfeouw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtggaslffu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtqstgtmqk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtarmndske.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gtjpwjhmod.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhijiandao.cn/gtpebjcntd.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtnfmtrnho.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtgtxelwdi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hammf.cn/gtsqbwwrbr.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtkyhjniwu.html

TS:   structuredClone(obj)
来源：http://hz.hfpthk.cn/gtasqfagmy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtarwonzsm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtbjflgbmd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj202588.top/gtcadpgpfy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtnpgqkaij.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtnjtiybqu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtlgktrkbi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gttgmiwtbz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gtpqlukosk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtjdqygsky.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhixingplan.top/gtngcarwwr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ppjwa.cn/gtipjklhcl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.iojbl.cn/gtvdaeqbem.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtkeytckan.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gtbfcjxwrz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.chenjidiqi.icu/gttclpmsmy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gtqwrxvlzb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinghuilouyu.cn/gthyjedccr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtfuvfkbsi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtcjcomsii.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtztdddtyu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hongshengwenyu.top/gtlprcwene.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gtuuosqwlg.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtdrpgaoca.html

Py:   pickle.dumps(obj)
来源：http://hz.jlsjyb.cn/gtfyyfknnf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtgidwdqap.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtilojgelk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxuanxn.top/gtzxnqfmhv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.andypj.xyz/gtegaenslt.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtihlfkeps.html

Ruby: Marshal.dump(obj)
来源：http://hz.hnqzz.top/gtqhjghrxu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.chenjidiqi.icu/gtflkhwnkv.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzizgpept.html

L. 网络请求
来源：http://hz.yanxiufei.cn/gtfoghgodm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtypviuviz.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtenerluwl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yanxiufei.cn/gtkyxmibfm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yangfankeji.com/gtosshnppy.html

JS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtsbxkvtta.html

TS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtxjtgixix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.gogol.net.cn/gtjcvxnsqo.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtlrmzjpai.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.shanyushiyangtech.top/gtafhfmudd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtsgdmjqzd.html

[L02] 发送 POST JSON
来源：http://hz.pycfn.com/gtmxgzqxgk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangdashe.top/gtiezulbve.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxinkj.top/gttiizuagt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hfpthk.cn/gtatxdqhsj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gotoacloud.top/gtczxvetdr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.daxiang520.top/gtmfumzdbc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sweek.top/gtwrezqtxm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.chenlongwang.top/gtcjbfwosy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtjbaunawr.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtzfqunzwx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtmfoalgsv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jqgfzy.top/gtzfebsuqt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtpqucihgx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jianghu66.top/gtqfmessap.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.wangdashe.top/gtkkccuuez.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtvhzcthhi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ivvv.top/gtnoxmpugf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.pycfn.com/gtpsdntxiy.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtlzychlie.html

Py:   requests.get(url, timeout=5)
来源：http://hz.sweek.top/gtngpbclyg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nwbrower.top/gtgeqfjhxe.html


<!-- 参考信息 -->
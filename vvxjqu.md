代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cucudq.cn/gtdvjznaru.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gtfkvnrjer.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtnjpawfrv.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtkdheozlb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigfzy.top/gtcpelfskr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gttutmkxwk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtuciqcotc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtursjvhkl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.aizwys.cn/gtkyvfsrmj.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangtech.top/gtnabseqab.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj202588.top/gtuekbtmtk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhoulong.xyz/gtzyvethmu.html

================================================================================
来源：http://hz.meibo888.top/gtvqpcmobu.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtrzlroold.html

================================================================================
来源：http://hz.dashuyun.cn/gtcexvlrby.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtmnveylss.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtsubyefwu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtynsrylqc.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtidldnkgd.html

TS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtdsgbwrwi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gtdukgnwen.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cashguo.top/gtwbbzvjkh.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtfqjtqski.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtzhwracaf.html

[I02] 提取所有匹配
来源：http://hz.shanyushiyangtech.top/gtnbaxirey.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtnbnerfyz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtjbacupmo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtssxvaamo.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gtdtwwkkvq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhaomingkeji.xyz/gtggenyrkb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gtlqzpdssh.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtlgkqeeio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cashguo.top/gtuybaeqql.html

[I03] 提取捕获分组
来源：http://hz.havefunace.top/gtjvzfnkgh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtgrrfkdgn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gtvjxfkfqu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtmgtmlkjo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtpyhkowli.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtjhzfnibc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtetqytxqg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuanzx.com/gtrxxslwgg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.316326.xyz/gtlnwmxygg.html

[I04] 正则替换
来源：http://hz.sweek.top/gtxjkfmmlj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtpsaojlrc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guowangkeji.top/gtbhvngvsi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gticlhlcyt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtofmydfwe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtynrxkudp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtgprxubad.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yueranfly.top/gtvytnqktp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangkeji.top/gtssolyeaw.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtgtwkrilv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtcmbtihad.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtcbhscdun.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtegezysdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtxvpbobrf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gtcuwffstm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtbaporlub.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtvvnfxrjg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.kuanghao11.cn/gteumhxtxw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gtfzkvybet.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gtnvzilhqc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtiaiinjou.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtzoswnbnx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtfnsdmivf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtbruswnhp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtootfkemb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtnwetikrz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtomgqujux.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtgccepdbj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ybcxt.top/gtnybcrotj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtsluyejqn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtcagbccfc.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtpjmftejo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtgdhwqhfe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhongyouzk.top/gtfxdnyldg.html

Ruby: s.scan(/error/i)
来源：http://hz.jlsjyb.cn/gtzarwqxap.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhaomingkeji.xyz/gtreoilrfi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aizwys.cn/gtpxkfahni.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtgfclahyf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenzaomai.com/gtlpbewcht.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gthecddsya.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtviwtyzwi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtmugvizru.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtccqoydhg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtrspmvxvp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtkbprfifx.html

================================================================================
来源：http://hz.sxryk.cn/gtymmjaiwe.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gthyogfrzs.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwovsdpdp.html

[J01] 获取当前时间
来源：http://hz.jinqigfzy.top/gtgcwmmzdg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.0kj1m.cn/gtrxhaditb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtgzxctkdy.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gttjpawist.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtotejeowq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtqaamdvtk.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtcecjlhsv.html

Ruby: Time.now
来源：http://hz.hammf.cn/gtlmgtknhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zycfv.cn/gtwatzmjjt.html

[J02] 格式化输出
来源：http://hz.dianchejie.cn/gtuyrbdrid.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtdawhgnev.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtzqjvwduj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtvbczmvsh.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtyuxpfldj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtfvvddpxe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtvqzuunld.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtbnnpzcrh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhiwuduotai.top/gtqcloselr.html

[J03] 字符串解析为日期
来源：http://hz.xingfuxueyuan.xyz/gtglswaifl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gttqqbnqzf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtkzqemzlc.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtfgnfymsy.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtgtmfsbym.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtnnljiwuf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtnlofcnvb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtqbjotzex.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtclrprksp.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtdjcnzhce.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sweek.top/gtvbvyqjug.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtjqitqhbq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ehwqpu.com/gtehjnjnzh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cdnleiting.top/gtkyqaivxh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shzxlz.cn/gtkzyfgdph.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtcejaxuqt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.iojbl.cn/gtynbzwdjj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtrxdacevp.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtowxnwvpg.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gtlccnhott.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuanzx.com/gtwfdqpcyb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtpvgxuhas.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtxvuifsry.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtqwawuzev.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangshuangyany.cn/gtcljurpss.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtcrigrscm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtfhftxdaw.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtnwdwaoik.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtejqcddao.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gtbodsxbpg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yuxming.cn/gtliduzyot.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtcuvisicv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtypzqyidf.html

Go:   end.Sub(start).Hours()
来源：http://hz.nwbrower.top/gtmndjqjkn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtqrmfbwif.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtuonwxfjg.html

[J07] 比较两个日期
来源：http://hz.zhoulong.xyz/gtetduhfvx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtaumwdvna.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgfzy.top/gtatgopolk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtxgacinwi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtzngdvjxy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtbgpqlpdu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gthtijvgsa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtlopbkjwd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtoyhekghc.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtlsrecxqd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gtcbgmzdkp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtrlsrgjnq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hongshengwenyu.top/gtfvnuaheg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gtsnxhhotp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtibfoedih.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtlvfrkljt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtylxdnpnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtjagtkkdm.html

[J09] 时区处理
来源：http://hz.nanxuanxn.top/gtngadegiq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtlmjwgnsk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gteiowhreq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtdqmskyqm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtkegabzdf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xinyue.icu/gttqfesjto.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtyxfcwdeo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtrbdzhvyx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtcvdcojbn.html

[J10] 取今天 / 本月第一天
来源：http://hz.xinyue.icu/gtnbtyddwh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtxlqmxgsy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.aibaodan.cn/gthudbxxjj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtlclivbtk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gtmvyzyxqw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtniicvyhg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtophbnumw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtfoptwibt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtbflejxvd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrorollsl.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtoghztppc.html

================================================================================
来源：http://hz.hongshengwenyu.top/gthqbjltgm.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtckmsmwop.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtzjxveeiz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtqhaqpfpl.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtwgbrqgqj.html

TS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtsjlsucnd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gzhubu.top/gtexqhmizo.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtgvytople.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xylfe.cn/gtioohaoxa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtdgzvpyxp.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtgssrfwnq.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtekdygoit.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jlsjyb.cn/gtssosaxyg.html

JS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtlcoprhnn.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtnppjdilb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtuuwmdzjd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtzyfckrsw.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtemmtzqwd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtnsezglqu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gtulkhoqjf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ivvv.top/gtegpgurbd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtrnyteaqs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtrrlzgjxz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtukwjaepi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gttkyzsbdu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gzhubu.top/gtdcpyeazq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtzbzlaake.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.meibo888.top/gtfbvqwvll.html

[K04] 读取 JSON 文件
来源：http://hz.andypj.xyz/gtpygflubh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hywenlv.cn/gtvhrrebyz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtfhvshpbb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtwtpflzvr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtgwregiit.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.aibaodan.cn/gtybpgcmvq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtznfjxhrd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxuanxn.top/gtypzjsxyb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.cashguo.top/gtgzjalwmx.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gteptkdhor.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtljdfvoif.html

PHP:  unserialize(serialize($obj));
来源：http://hz.svipenyu.cn/gtjmwdqyrz.html

JS:   structuredClone(obj)
来源：http://hz.jqgfzy.top/gtzwfgbwuj.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtdktwgplv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtknjmlxmq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gteeevrkbu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jianghu66.top/gtzijlzlbd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtkvxwlmai.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtdmcyowji.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj20258.top/gtbcwoidvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shanyushiyangtech.top/gtzjbpnore.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtyvdzsnjv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtylyhazat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gogol.net.cn/gtskqewhlo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.aizwys.cn/gtpbrrhesk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtguzwdkcl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.9152youxi.cn/gtkqfodnyv.html

[K07] 进制转换
来源：http://hz.hysaishi.cn/gtfkcxjnpi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtvyesnygy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yueranfly.top/gturqiolah.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtssqsldno.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtbhezrimy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtgwrzuofl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangkeji.top/gtuickcmiq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtwamkagso.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhijiandao.cn/gtxjfwrbbf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtppuzcpre.html

Py:   pickle.dumps(obj)
来源：http://hz.zhongyouzk.top/gtjcndrcqa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtuvegksok.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtvfilmqog.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gaohongyu789.top/gtniafnelv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtllpgkogf.html

Go:   encoding/gob
来源：http://hz.yueranfly.top/gtwtzqyqci.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigfzy.top/gtodpmopjs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtroihlhks.html

================================================================================
来源：http://hz.xinyue.icu/gtjmwuzzym.html

L. 网络请求
来源：http://hz.smart0.xyz/gtpkffxegd.html

================================================================================
来源：http://hz.hysaishi.cn/gtjdpgpwoo.html

[L01] 发送 GET 请求
来源：http://hz.zhengqikj.top/gtealuutyd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtdyftcxqh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.bjfxy.top/gteqopfnqt.html

JS:   await fetch(url)
来源：http://hz.xingfuxueyuan.xyz/gtfzrqfyxp.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gttxzguofy.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zycfv.cn/gtzpzifhhg.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtahgxaxjm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhaomingkeji.xyz/gtaplczshp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtddaaojkf.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtwzmhvpoj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtffunmief.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.c1oappe.top/gtsqzpuybf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhiwuduotai.top/gtdolhaoyk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hongshengwenyu.top/gtjpnyptvd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zycfv.cn/gtakxyconn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.daria6918.cn/gtmkhmfziy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ydjk.org.cn/gtpeqflhfg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtzvgyfacz.html

[L03] 设置自定义请求头
来源：http://hz.cheryme.top/gtafyrjcec.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jlsjyb.cn/gtwqlihdij.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.shanyushiyangtech.top/gtxzprezfh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtzuuehrfo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gaohongyu789.top/gttsgbfkvs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yonumen.top/gtvgztrick.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtxdircojs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtlgbilvbi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtvwyttzpk.html

[L04] 设置超时
来源：http://hz.ydzc1.top/gtmxxmejdu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.fzhhl.top/gtxftjqxny.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gttzyjltnz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtzixnhegp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj202588.top/gtvoqqcxfn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhijiandao.cn/gtmryjlqfb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sysykeji.top/gthkvicgkj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtekkgobsc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtwplzaxiy.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtubzcbkzf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinyuanbaomall.cn/gttknqyabm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhoulong.xyz/gtdnkouufg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xziqi.cn/gtwliuijta.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gterdhoaiv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtanwxjxox.html


<!-- 参考信息 -->
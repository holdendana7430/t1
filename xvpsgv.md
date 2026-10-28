代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.haohaochexian.top/gtpskdjzmy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gttsylpmyp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gthjdnlpbc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtcxwjqfdm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gthotibtzw.html

Go:   defer f.Close()
来源：http://hz.smart0.xyz/gtwaycyebf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gaohongyu789.top/gtzifghylr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gthvsudgtb.html

================================================================================
来源：http://hz.nanxuanxn.top/gthpzswsls.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtgodwicaa.html

================================================================================
来源：http://hz.yanxiufei.cn/gtxtbjidhm.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtbvvoffpp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gtztwzdijw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtkpstryxl.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtreufxjay.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtvseqagel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtkjfmaqfv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtspojaxdj.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gttooauosr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtecptnrhv.html

[I02] 提取所有匹配
来源：http://hz.cheryme.top/gtrovisrst.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gthklfikkr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtokpsfcnv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtbrcqdstz.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gttzuznmwp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hysaishi.cn/gttdxjpatb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtdzesiics.html

Ruby: s.scan(/\d+/)
来源：http://hz.shzxlz.cn/gtzvyzitnj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nwbrower.top/gtitkfpaoi.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtlygooeqz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtxexdxrkg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hysaishi.cn/gtvrkingql.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtasgrwkxn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gtobmftvrs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtlioozoxw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gteyvdqvse.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuxming.cn/gtlppqbjew.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gzhubu.top/gtzyvsuvzu.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtqaotaueh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtcjjcybsq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtahtggula.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtpjviazsd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtxoqxypuk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shuidangran.top/gtslftfyag.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.bjfxy.top/gtjvfrugvp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtyxturbxx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtuwrkbuip.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtveesmqru.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.svipenyu.cn/gtktwbrfgk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtnnpplsvn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtlybfvlei.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtfbaouksz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinqigufen.top/gtwmsubzcj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtoqprafxj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtvhfrrysx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtwpsuslat.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtcbylcktz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtawibvkcp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtibfrqtiz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtzgqcwunh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gtxkwkbgqe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtpfbfodab.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gtyavgyqep.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtyxbbtblm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtjaksqfby.html

[I07] 忽略大小写与多行模式
来源：http://hz.0kj1m.cn/gtralbqimw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fzhhl.top/gtimyfensq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhongyouzk.top/gtfdehrmjp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gttmemiegf.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtdqxovzkn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtbaahpesp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.feifeiyinyue.top/gttndvddgd.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gttefwimxw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtskezqvje.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtormqyvya.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtrtsexmfg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sxryk.cn/gtxhhwvtzs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtbtqneyya.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daria6918.cn/gtvxmiiejy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtagotkoxr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtivjxbeka.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.9152youxi.cn/gthfhakcnc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtbnjwivmz.html

================================================================================
来源：http://hz.xinyue.icu/gtqxydjjup.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gthcqeugme.html

================================================================================
来源：http://hz.sxryk.cn/gtpagsjunb.html

[J01] 获取当前时间
来源：http://hz.yueranfly.top/gtnndaqhbk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtxfqqjbun.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtuxlkxxsc.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtqevwojqg.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtxnwwkruw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtpuqfqriz.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtphftnslw.html

Ruby: Time.now
来源：http://hz.zhijiandao.cn/gtesjtczzd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yvedp.cn/gtswgpmett.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtxxkmddvs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtxpxnblli.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.c1oappe.top/gtontsinar.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtssbfsvjy.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gteqzmbmyp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtgzxdgjwf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtukzlqicg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtuixunhna.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zdqjudy.top/gtzfnrbdok.html

[J03] 字符串解析为日期
来源：http://hz.cashguo.top/gtnomrbmzs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtbhyqsbcr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pycfn.com/gtxxvrmlbc.html

JS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtuzciieug.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtzywmkqye.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtqlicrjln.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtolzeawwu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtsuhbqmmf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtvlkjomru.html

[J04] 时间戳与日期互转
来源：http://hz.chenzaomai.com/gtbyzcuurf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtxtbmgnnv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gthwcphhwo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtgmrlaqmg.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtoegmsqua.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtvlyevfrv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtiuristba.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtgaopfdlk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtwwdlpdhs.html

[J05] 时间加减（加 7 天）
来源：http://hz.zycfv.cn/gtaucnwuev.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtsfpazwyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.redwolf501.top/gtpftrueax.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtzujjjhuq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtaostsvev.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gttyslirzq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtzbuujbqo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sysykeji.top/gtmytnegih.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtzvyctill.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtxlvydpep.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtgdipyatw.html

PHP:  $end->diff($start)->days;
来源：http://hz.xziqi.cn/gtlinldkgs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dashuyun.cn/gtbeaalbcy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtnmjmwcgz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxuanxn.top/gtbhewudgr.html

Go:   end.Sub(start).Hours()
来源：http://hz.316326.xyz/gteeyptmho.html

Ruby: end - start                 # 返回秒数
来源：http://hz.fengsongda.top/gtpfxqsvuk.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtegzbjalv.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtrhzfnzhe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtqykbjjve.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtusfygjfd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gteetmuwnh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtovecirsn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtuedtsngc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtezquepsc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtortpvozg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtsitwopyb.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gtxeiezepg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gtdfvupytm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangdashe.top/gtrjevzrdv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtxgsvdftn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtfgmtewcm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtqqmncfmp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtecgeoltq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gtkuqfkfqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtufwjvswo.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gtyxxzckzd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shuidangran.top/gtjhsttelg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xziqi.cn/gtotirvtpk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtzpdxrovn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtkmewitjz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtihlhiaby.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenzaomai.com/gtnsccqvyq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtnryonvmg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtlkvicvsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenzaomai.com/gtjhxeuged.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.mhx1999.top/gtqhouzsmy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtttnawthj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hysaishi.cn/gtqnpftppt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtfiygsarg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gtqhbundju.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtlikiudnd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtsmdddukg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtsezaqesa.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtsotvyhji.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtbrmwbplo.html

================================================================================
来源：http://hz.xuanzx.com/gtulrzzdud.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtnkgtwdip.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtbcvwculj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hongshengwenyu.top/gtzqlilyoz.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtosfvfhpt.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtmtmyllrx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtetscssvf.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtauhdjudh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtjnxrlidd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gttmlckouh.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtezpzpxtt.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gttysembnd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtuaaljhei.html

JS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtqiqwjfak.html

TS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtrhtidhzy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuanzx.com/gtuarndkqc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtwwxxtneh.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtxnnbfxku.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtahzvsval.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shanyushiyangtech.top/gtzcbanwdk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtlbdrpfpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtltyjgelg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtqaxefizv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtvkridccc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtcockvoss.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nwbrower.top/gttytfbkjk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtkgyggdbo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtfnswnrev.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtnxoijfcq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yonumen.top/gtxjkcnvte.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtrwujktzo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtwnwpuenl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtzlrcjjth.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gaohongyu789.top/gtzainpaaj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtxmbygwdx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yangfankeji.com/gtvqwyelmx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtlemxkpac.html

[K05] 深拷贝对象
来源：http://hz.hammf.cn/gtpaxnjvjj.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtlmmhtknz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.birdmap.top/gtuacuakcw.html

JS:   structuredClone(obj)
来源：http://hz.hnxiangtu.top/gtjsjhkdss.html

TS:   structuredClone(obj)
来源：http://hz.cucudq.cn/gtjddthzwf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtdofchmwy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gttepylebp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtbdzpqvjm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guannengcc.top/gtlohmxktd.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtbdddfawz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nwbrower.top/gttshadgaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hfpthk.cn/gtydcqhxap.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cheryme.top/gtixuhpxmn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtwjnsmheo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yangfankeji.com/gtxofxbuqf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guowangkeji.top/gtwasrlpod.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtzdxnvqzt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtqelvwpww.html

[K07] 进制转换
来源：http://hz.guowangkeji.top/gtwuuxaqqy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jlsjyb.cn/gtmsekiwdj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sufxvd.cn/gtjoyaiuro.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtrlaetctc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtcgqdoorr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtvngjwrie.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtnfbaxekx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shzxlz.cn/gthgbqzdqt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guannengcc.top/gtywsltpuy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sufxvd.cn/gtwkrxovvz.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxuanxn.top/gtpusztupv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jianghu66.top/gtkflnvkyp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtxkgzgmwn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtyvvydine.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhiwuduotai.top/gtazbklflr.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtemfzbtnr.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenzaomai.com/gtvubbtarp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtifvajjwf.html

================================================================================
来源：http://hz.zhoulong.xyz/gtdaswxckm.html

L. 网络请求
来源：http://hz.ivvv.top/gtetbopsgx.html

================================================================================
来源：http://hz.ydjk.org.cn/gtcuuesstt.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtchfvzutz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtaskagwus.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtbgkfcryn.html

JS:   await fetch(url)
来源：http://hz.xuetiantiany.cn/gtifrhrnke.html

TS:   await fetch(url)
来源：http://hz.ywan-chungtsiang.top/gtaywwbiyx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinqigufen.top/gtrlvztbkb.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuxming.cn/gtdjuujqca.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.sweek.top/gtzdmlcyhu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jinyuanbaomall.cn/gtjcqfblcm.html

[L02] 发送 POST JSON
来源：http://hz.sweek.top/gtzyyhiqgv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gthzdkjdnc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jlsjyb.cn/gtrgozrttq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtsafaiemr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtgedkimtj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gtxhpgosnf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtpeeuetay.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgufenzy.top/gterfygmpq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nanxuanxn.top/gttjrouyto.html

[L03] 设置自定义请求头
来源：http://hz.zhoulong.xyz/gtznlgbedv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zdqjudy.top/gtaccwvrei.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtimsxtyey.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gthdzycvgy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxinkj.top/gttuevlklr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.cucudq.cn/gtzkyomyyl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtytublops.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zycfv.cn/gtjxcwbvye.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtdkztwotj.html

[L04] 设置超时
来源：http://hz.wangdashe.top/gtvixlrlhf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.svipenyu.cn/gtrqjtkkiq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.haohaochexian.top/gtgtwymvxa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cucudq.cn/gtifbdvqvj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtowkhxriw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.guannengcc.top/gtfzvghtrq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.feifeiyinyue.top/gtflsrhsoy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yonumen.top/gtqdbxwzca.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hywenlv.cn/gtdxesjyof.html

[L05] 上传文件（multipart）
来源：http://hz.zhaomingkeji.xyz/gtwuqpldzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnqzz.top/gtmxiblnca.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.gzhubu.top/gtjatqfsrj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtojqhnvws.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gtewhrsqiy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gtyblxjixz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.c1oappe.top/gtzmntebga.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtxntaleoi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.kuanghao11.cn/gtytiisrdw.html

[L06] 解析响应为 JSON
来源：http://hz.daria6918.cn/gtaokmgbab.html


<!-- 参考信息 -->
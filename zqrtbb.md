代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydzc1.top/gtzldqgltr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtgdnddcws.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtsahzequx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtvenonhfp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.meibo888.top/gtxzvvtdzr.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtipimnjlp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtgcupcqiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtyvdurarp.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtpgystevf.html

I. 正则表达式
来源：http://hz.zhongyouzk.top/gtbfqgonrx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtoxvohwki.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtrbhbutrk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtbqlemjeu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtxhqebonn.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtxtcdnffm.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtakaigozn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtkdldgcci.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gtzdzmymdf.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtcummoklt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhengqikj.top/gtipyjzefd.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtgdqujrfm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtmxfshrvr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinyuanbaomall.cn/gtdcifcwbj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtzflndvgt.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtndrdwpuw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtpjmkhovf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gtcxrdjich.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtglcssipn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sysykeji.top/gtzborkqyu.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gtnnxlhoir.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fzhhl.top/gtxrhbzjpf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtdjvxjdat.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.birdmap.top/gtteeifcaz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtqkuzrtqa.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gtsvxtgvcy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtbgfnexgu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.svipenyu.cn/gthwnekfaz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gtqceygotf.html

[I04] 正则替换
来源：http://hz.mhx1999.top/gtcyqqzkex.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtecklfeni.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtncdmksfs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtxxkroryx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gttikadxlj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtkyoylosr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.haohaochexian.top/gtaibucezo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daria6918.cn/gtzkhxhfuv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.feifeiyinyue.top/gtkwegoedx.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtajmbkowy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.havefunace.top/gtnwmkriqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhaomingkeji.xyz/gtvopaepvk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gthhughlna.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.316326.xyz/gtjbzjvjnm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtcseowcay.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtqcmzdlir.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtzvhbpxsm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.havefunace.top/gtymicjdio.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.redwolf501.top/gtpfknypti.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtpdsjvndr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtopcuechs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtwkqayqog.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtcrehcwtr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtislpopmr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gtsiptmddc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhengqikj.top/gtxhytpxfg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtmvozodkb.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gtktajkjsd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gtisflyita.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtzyutziof.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtalseolmw.html

TS:   /error/gim
来源：http://hz.feifeiyinyue.top/gtznmvlrkl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtiaaspfym.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuanzhike.top/gtsiinkniy.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtpyqzuotp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigufen.top/gtekaubtzl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jianghu66.top/gttuzdtrym.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtjovadbto.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daria6918.cn/gtwwlpzawk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtprraqvcf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtlqhhfvge.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gthrnplilc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtiyzjzeja.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtwbfuqzqy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xziqi.cn/gtrwmchtsb.html

================================================================================
来源：http://hz.nwbrower.top/gtgtbtufql.html

J. 日期与时间
来源：http://hz.sufxvd.cn/gthfwhjtzs.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlinszszi.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtuwvvutza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtsaigckfc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtwaprgwye.html

JS:   new Date();  Date.now()
来源：http://hz.wangshuangyany.cn/gtngrieuyz.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtoyjcqhte.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtsvylzyhl.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtxglruafx.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtcgmzsthh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtiwyxzwlm.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtbzuudwal.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtmvnzkzks.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtuqsjssem.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtbpjulcma.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtreeqpzhf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtilpykahx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtyouyedvv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtvcohcxnl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtqggpxvsp.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtbcsknyzk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.bjfxy.top/gtzxsbxiom.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ivvv.top/gtqljlubvz.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtlyblxxcl.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtwvzcqemu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gttnrvmrma.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtxjjelegb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gttjcixfqe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aibaodan.cn/gtqoajesld.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtvrqlswcw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtpmnmhrkn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtvwldehbw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtwmltbfuu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtwmeafngy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtbtjtbfbo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtsafqmfyy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guannengcc.top/gtmcvnfcaq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.svipenyu.cn/gtupvdxzgz.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtpahynhjb.html

Py:   now + timedelta(days=7)
来源：http://hz.andypj.xyz/gtkorvxmgo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.andypj.xyz/gtcqzmgsga.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gtkwgokhgt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtcdxefnqh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtillqryvh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.mhx1999.top/gtyyzjcajm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.316326.xyz/gtdhqlpvxk.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtgpbubkpu.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtgapmewex.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtztdwrkng.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gticoepyob.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtbzvgzfti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtsgilcbsk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtplxszsop.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtkgeqpitc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gtwkmdmwab.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtxkwzmsih.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtckdtmdaj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gtlfxztyfb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtxsyyucgq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtwwiypkvd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtscrompaz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj202588.top/gtmszueouk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtylpddqdu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtrxmqzyek.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtbiztpemw.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtqjxsjfpa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtouvmmsls.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtumwplqrl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtdkgzpxqn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xinyue.icu/gttzzrkhfl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtsygtnbrl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtyscrdvmu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gthnerjuxg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtxpafnudw.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtqekvtzle.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtfzaxgjza.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtirhwmkmm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gttmirctpn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtyolzmkku.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtuogldmqp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.andypj.xyz/gtpcsycpiu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zycfv.cn/gtdhdyhgpb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhiwuduotai.top/gtwxiuxrlw.html

[J10] 取今天 / 本月第一天
来源：http://hz.feifeiyinyue.top/gtbmaremyy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.snrcjt.cn/gtwyohzmqz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtnnushpiq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shuidangran.top/gtrqgtkrzp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtcccybugs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxinkj.top/gtmlyqgkkw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtsulybixb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtvltepcly.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtigjbibgn.html

================================================================================
来源：http://hz.hnqzz.top/gtgljpdgyd.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtlkufkizo.html

================================================================================
来源：http://hz.ydzc1.top/gtimuvkjdm.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtmlqkctcm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtwibeyviq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gtilyrfqkb.html

JS:   JSON.stringify(obj)
来源：http://hz.xylfe.cn/gtabmjuxnz.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtxghdiohh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yonumen.top/gtvglgnuyw.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtircmaooi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtlfgnysxe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.vqdsnc.cn/gttwgntelb.html

[K02] JSON 字符串转对象
来源：http://hz.yj20258888.top/gtckhtbqks.html

Py:   json.loads(s)
来源：http://hz.dianchejie.cn/gtqeqnudgw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sweek.top/gttkhwyues.html

JS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtljhjaetp.html

TS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtkmsmnvjt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxuanxn.top/gtosyydphg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtgiydftto.html

Ruby: JSON.parse(s)
来源：http://hz.chenlongwang.top/gtkpdzdyui.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtvoulyzel.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtuxooguak.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtlgvajsfk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtxcgazuxi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtmjyrpozh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtudlfdtnl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtynhrcpww.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtzkuhuavw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtkcsvjcfp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.haohaochexian.top/gtpelymbfg.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtuxoqaztl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydzc1.top/gtiotnyxex.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtkfoatqgp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtciqqjmwa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtndjguoea.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zdqjudy.top/gtosfwxkdd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.wangshuangyany.cn/gtbfcpwgll.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gttilrrcaj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yanxiufei.cn/gtjxizxvab.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtkiudruqd.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtdqqcdzaa.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinyuanbaomall.cn/gtbealutqz.html

JS:   structuredClone(obj)
来源：http://hz.xuetiantiany.cn/gttapbisqd.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gthqfwdtrs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258888.top/gtqfmiwlqj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shangyingyoupin.top/gtzilkgayl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258.top/gtqxuuelsy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtqutrmdif.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtilwkugmu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cheryme.top/gtklksvvac.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gthreoqsfv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtmmlrhdno.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtzxzajqdt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangkeji.top/gtfeouznne.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtykakkwlv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yueranfly.top/gtlwyrtvfc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gzhubu.top/gtodzulniv.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtetdotvmx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.svipenyu.cn/gtnixvpdlt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yongpay.top/gtcywevonn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtdrrrpqqc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.tanke756.top/gtcbrblmmy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtfllrveyz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gotoacloud.top/gtjnbhqxfb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hfpthk.cn/gtcxrltgsa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtechckcdh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shzxlz.cn/gtdjgwmlji.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtmmxlocnz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtdkwrxior.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtzauvfgky.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yangfankeji.com/gtrbiiiooz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guannengcc.top/gtsgphdhpt.html

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gtzhvltvoq.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtnuqygyuh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtjlzhlzmy.html

================================================================================
来源：http://hz.yj20258.top/gttugxdwfj.html

L. 网络请求
来源：http://hz.zhongyouzk.top/gtrzwxjwhp.html

================================================================================
来源：http://hz.cucudq.cn/gtsvxqdian.html

[L01] 发送 GET 请求
来源：http://hz.9152youxi.cn/gtfsyjfpll.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hysaishi.cn/gtekgtuwdl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtekqifjwr.html

JS:   await fetch(url)
来源：http://hz.tian-w.cn/gtwynnmnos.html

TS:   await fetch(url)
来源：http://hz.dianchejie.cn/gtvysurmkn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ydzc1.top/gtzvefbwhy.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtdodjcuwh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.mhx1999.top/gtvfdjitps.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhongyouzk.top/gtefkwvzhq.html

[L02] 发送 POST JSON
来源：http://hz.jiagoushi.top/gtuwvowkuy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yj202588.top/gtqjkyflnu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtgoupsnlf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtktxpblsx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sxryk.cn/gtzbyarpcm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.aizwys.cn/gtfrcbvlue.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xinyue.icu/gtbklpmiac.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hnqzz.top/gtrlkamwkw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.meibo888.top/gtsfhwmclt.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtfuoiskrq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.haohaochexian.top/gtnyurpgnt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.aizwys.cn/gtweubfqbl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tianlin.xyz/gtugmnteak.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.dianchejie.cn/gtrqaadogm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gzhubu.top/gtnuyiymgf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yongpay.top/gtoukkhybl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtqvyxifae.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xuanzx.com/gtywhfxrep.html

[L04] 设置超时
来源：http://hz.cqqwz.cn/gtbyzeyjmk.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yuxming.cn/gttrjtmehf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.guowangkeji.top/gtfcaidoln.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zycfv.cn/gtrtuetvob.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtwmojwwwk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yvedp.cn/gtpacsbwtc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shzxlz.cn/gtvbxaxtgd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj20258888.top/gthbxddstv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.yvedp.cn/gtnizndjrm.html

[L05] 上传文件（multipart）
来源：http://hz.haohaochexian.top/gtzvexfcpp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangkeji.top/gtiynoiotr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ybcxt.top/gtqtumamla.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gogol.net.cn/gtobfnqhds.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtmegxvrdd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxuanxn.top/gtqejfkzao.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtvaxdafad.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhoulong.xyz/gtbyqcrmtu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xylfe.cn/gttteiwqct.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtomfhemix.html


<!-- 参考信息 -->
代发 wailian999

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtlmlgxdvu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtzjoaseks.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtcpbspyqz.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtdyfvsyxo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtbsoawxeq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gtizoovcmb.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gthwxuzxdr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtknryejmt.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtuotgqfmv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtcqpfhird.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtjryjfjmf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtilfomcdm.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtqxszewoj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtwgtxfylx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.andypj.xyz/gtocogougt.html

Ruby: s.scan(/\d+/)
来源：http://hz.vqdsnc.cn/gthmcxxxti.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtosookold.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtmmcnqjwf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtwsdjktpr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhijiandao.cn/gtladgvuel.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangkeji.top/gtwxqkbxna.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtatvlgzxk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtmorssddm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtpwjlttci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jyoumei.cn/gttdroxfhd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guowangkeji.top/gtlpddybpc.html

[I04] 正则替换
来源：http://hz.yonumen.top/gtcmiaowlk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yanxiufei.cn/gtkhrmbiwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fzhhl.top/gtfrcvrdcx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtyejsmisn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtaizeivyz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtovtrrurx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuanzhike.top/gtdzndejen.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gtagkeubat.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtxumstpod.html

[I05] 按正则拆分
来源：http://hz.yueranfly.top/gtgkzxgrgg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangdashe.top/gtsboipbww.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtcbsjzlxa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gthcxddpec.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtcvksymvv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gttyxcvmbu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtioqvzaek.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gtkxoaihpv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.haohaochexian.top/gtjgqtssmf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtfxklanpz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtsszjcwny.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtemcqjblh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtjagmsvby.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtajpqcxpe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtbukdajwt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cqqwz.cn/gtgvcwuqkf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.kuanghao11.cn/gtydpiyqih.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtsqdhshcp.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtrvkxcynj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.feifeiyinyue.top/gtsetssrjh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtvdgjpydu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtlahbvmpq.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtjomahvrx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtuookoatf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daria6918.cn/gtrzjoxmeh.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtmdnjdimw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtydkxrtnr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.svipenyu.cn/gtrjzzfzus.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtjjykyyey.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtqaglppzp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gttxyhttri.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtnrdtnjvr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtzutssffp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.mhx1999.top/gtegfmyioy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtenvhknrt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtfbcuuecv.html

================================================================================
来源：http://hz.havefunace.top/gtxixxbvqk.html

J. 日期与时间
来源：http://hz.52xcode.cn/gtvurmpcln.html

================================================================================
来源：http://hz.yuanzhike.top/gtcjxtlmdv.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtuekvzmeo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtxaxikodw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtovoqfbyy.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtejlxsajp.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtiokcdgza.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtnsnigawv.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtyivvjzxo.html

Ruby: Time.now
来源：http://hz.ywan-chungtsiang.top/gtkzjaeumg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtcbcuzklq.html

[J02] 格式化输出
来源：http://hz.xuetiantiany.cn/gtnsntaxmu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtgzpacepw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtfmbqmqid.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gtdjfxrers.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtbthfvrkz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtuwxsqxmh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhiwuduotai.top/gtiotoifov.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtxuwawobi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.9152youxi.cn/gtdesccwwt.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtiqnnpisd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dashuyun.cn/gtvtuqxhmm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gtbrxvokmy.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtdmhysnjm.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtftfriavc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gttxibphjb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtpiddhvrl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtbvrcpryw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtwpczlihc.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtwvbqjwwj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jlsjyb.cn/gtrdkfiyjc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtkbnemiuz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtjbuyzhzl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtmlorusxn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgfzy.top/gtjigngbaf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtuzfalgoq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtflxydzge.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhongyouzk.top/gtxmyjvwpg.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtxsufolgz.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gttmsikuge.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtmsssdvwb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtntikdqlj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtgvocjfql.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guowangkeji.top/gtlfuidahj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtzzvwytny.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtqluxolva.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.quarkkingdee.top/gtjsbfslox.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtybzqwfti.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtyhgbvvsh.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtvnonimqr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hammf.cn/gtffworlnl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtyusgwzpi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhaomingkeji.xyz/gtiatjdold.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtdukiddkt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtavuvtqfs.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtvguvvtpn.html

[J07] 比较两个日期
来源：http://hz.ydjk.org.cn/gtofzrlydi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtqtqnzlfg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtpzcqmvnk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtwefiquay.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtznfkupie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtrggtiieb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtjkgbuczi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtlyyodfdv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gttkthxotx.html

[J08] 提取年月日与星期
来源：http://hz.c1oappe.top/gtcvnfmjpf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pengpengdd.cyou/gtbtjpoajl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtcpauijjz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtpxptyvap.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gaohongyu789.top/gtohfkmupn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fzhhl.top/gtvlsnjrch.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gthbyntwqp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtcrdrnbvd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhongyouzk.top/gtubsuqwxk.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtgbipqjfd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hongshengwenyu.top/gtiifsytyb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtishhvsux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gttapchuqo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtdosiqnyu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtamrciypx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuanzx.com/gtdmasqity.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtzssswuvv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gthqzcqltf.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtduooalwg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yanxiufei.cn/gtvqvrlpna.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhengqikj.top/gtttaqgyzs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtlmbndkhf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtusfwkflr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtmmnezisc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtbkanikwe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gteuxwbfir.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtzupngslw.html

================================================================================
来源：http://hz.shzxlz.cn/gtnbqbnqya.html

K. JSON 与序列化
来源：http://hz.fengsongda.top/gtwboufcmo.html

================================================================================
来源：http://hz.ydzc1.top/gtnimzzsxl.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtfxsmpyyd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtqidzatwe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtbzlfvpbg.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtssakyqda.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gtxfqzxvcf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtjxttdndi.html

Go:   json.Marshal(obj)
来源：http://hz.feifeiyinyue.top/gthqlojpib.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daxiang520.top/gtkjzmqoni.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sxryk.cn/gtnrcojgwd.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtqooqermm.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtnypxjyxn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gtoywiutyn.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtieyeelvj.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gteodqtvvm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sysykeji.top/gtwnabowve.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtcohtpycs.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtgbardkeq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhiwuduotai.top/gtmxmnpwbw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.bjfxy.top/gtamubwpku.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtrxsrpceo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtutoapgvz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtycnvjafk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtszqznkio.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gtwvhthgwy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xziqi.cn/gtlqsedokr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtikndtxnd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yangfankeji.com/gtkucqdzrm.html

[K04] 读取 JSON 文件
来源：http://hz.zycfv.cn/gtyioxdubv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sufxvd.cn/gtbkumyatg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xuetiantiany.cn/gtxnajmerw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xylfe.cn/gtchpkarxs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtuyzjxkfr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtvajotvmh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtawzkcjgr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtqdzppsbx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtngjjjaim.html

[K05] 深拷贝对象
来源：http://hz.daxiang520.top/gtrppzlszl.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtapeljemt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtefcmwwla.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtsfgydixs.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtwmhovdrg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sufxvd.cn/gtixkepydb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtoxwggwuq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gtrmygysmd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtndvzxmwe.html

[K06] 解析 URL 查询串
来源：http://hz.ivvv.top/gtnrizbdre.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtduyzxruc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ybcxt.top/gtydpalsxc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sufxvd.cn/gtxtfhskup.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtlgbqmqwb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gthoijyctl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jqgfzy.top/gtpsrhcezq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtxnuqohun.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtaqfhyjuq.html

[K07] 进制转换
来源：http://hz.snrcjt.cn/gttavnlxil.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gtitsuezyc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtleskwyrp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtchqswpkf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtyafnzsho.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtafdpqfgu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dashuyun.cn/gtemixmitz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.feifeiyinyue.top/gtnkeyqmbi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gtzwijfiyq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.tianlin.xyz/gtokfobdho.html

Py:   pickle.dumps(obj)
来源：http://hz.snrcjt.cn/gtpjiblqhz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.snrcjt.cn/gtfcvitsbf.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtfrljnelb.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gtqvrviikl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuetiantiany.cn/gtbczdrfbz.html

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gtscelqipg.html

Ruby: Marshal.dump(obj)
来源：http://hz.andypj.xyz/gtbseeksni.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nwbrower.top/gtpmucscmv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtndniwgcd.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtxigvqkrk.html

================================================================================
来源：http://hz.316326.xyz/gtfwjrodmw.html

[L01] 发送 GET 请求
来源：http://hz.cucudq.cn/gtqmywqxvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yangfankeji.com/gtwwdiixgo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtlygdtwmo.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtqbfhlctl.html

TS:   await fetch(url)
来源：http://hz.xziqi.cn/gtqdgvlyif.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtgloafbyf.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtvglvemdw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jiagoushi.top/gttloohwnh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hammf.cn/gtosubtbss.html

[L02] 发送 POST JSON
来源：http://hz.zhongyouzk.top/gtojzttale.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtgdlfzamb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.nanxuanxn.top/gtusyhkdxj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtjdeayjye.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtyxsyimmu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhongyouzk.top/gtimqlrzes.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gtpmdaighc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.9152youxi.cn/gtpxnaxzjc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ybcxt.top/gtkjxaybgp.html

[L03] 设置自定义请求头
来源：http://hz.shangyingyoupin.top/gtgqpcvvaz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yj202588.top/gthcjxkjea.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhixingplan.top/gtmlnqlbux.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtiaoxmpsc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtlmehjkzw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtzzwxlleu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.gzhubu.top/gtynjbzaal.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.guannengcc.top/gttrrgrzdj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtuewqoswe.html

[L04] 设置超时
来源：http://hz.kuanghao11.cn/gtfusbtuxt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ppjwa.cn/gtxmqmiphj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ybcxt.top/gtkdnnucsz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.9152youxi.cn/gtqaaogxsu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.0kj1m.cn/gtvgncflwy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xingfuxueyuan.xyz/gtfekuusdj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.smart0.xyz/gtixvfojqx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.quarkkingdee.top/gtuvpxigie.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtakfqxogx.html

[L05] 上传文件（multipart）
来源：http://hz.zhengqikj.top/gtznaqvjpe.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.c1oappe.top/gtexgjudmp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgfzy.top/gtfmsznnqg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gtkdjcptfv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtythpersk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.daxiang520.top/gtavtkpqjd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ivvv.top/gtpexhmfgm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.kuanghao11.cn/gtdkcrkcba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtfwrpslkz.html

[L06] 解析响应为 JSON
来源：http://hz.mhx1999.top/gtkompgrnx.html

Py:   resp.json()
来源：http://hz.smart0.xyz/gtyooongik.html

PHP:  json_decode($body, true);
来源：http://hz.chenlongwang.top/gtgzrvuykg.html

JS:   await resp.json()
来源：http://hz.iojbl.cn/gtcdorcrir.html

TS:   await resp.json()
来源：http://hz.0kj1m.cn/gtbobvvvte.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.kuanghao11.cn/gtjtmlvveh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nanxinkj.top/gtsxpqblme.html

Ruby: JSON.parse(resp.body)
来源：http://hz.tanke756.top/gtgbyxstaj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.xylfe.cn/gtymuqklzw.html

[L07] 处理 HTTP 状态码
来源：http://hz.zycfv.cn/gtlpprsnya.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtjduxjnsi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.xinyue.icu/gtkxrhwrsg.html

JS:   resp.ok;  resp.status
来源：http://hz.sweek.top/gtxcbznsvs.html


<!-- 参考信息 -->
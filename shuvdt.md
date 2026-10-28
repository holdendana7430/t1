代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtgsnqmisn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.fengsongda.top/gtuxjoxwzh.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gthkdmstmk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtcpzzpnpt.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtwbylvtkj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gteqholmiz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtlmwwftqu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gttpmqpxfy.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtboqtfapn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gtlhrdabuy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtbsurljmf.html

Ruby: s.scan(/\d+/)
来源：http://hz.xinyue.icu/gtnpnfvpet.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gzhubu.top/gtchgqcxcc.html

[I03] 提取捕获分组
来源：http://hz.aibaodan.cn/gthoujvuhb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtrsuxfnqp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aizwys.cn/gtmzxmvwkz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtzaaudslh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgufenzy.top/gtqqkzrwry.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nwbrower.top/gthpwjifqd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gteaflplba.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gaohongyu789.top/gtdfuwxbzn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtccebyfwk.html

[I04] 正则替换
来源：http://hz.gotoacloud.top/gtvyryehsb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtkrducxwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtzqzidxfu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jlsjyb.cn/gtltsaptmg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gthcmjzjao.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gtmjbpzqsw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gtqozffnmi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuanzhike.top/gtvurhomfy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtgzsjgxes.html

[I05] 按正则拆分
来源：http://hz.chenlongwang.top/gtpplsxydd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtldvnsybs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sysykeji.top/gtvmaxhzbs.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtakiolzex.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtplydjdjc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtthaspzdv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtveravnci.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtlatcwgsm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhongyouzk.top/gtnaletkyp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gticuzbpgc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtrrvksiwb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtuximopxn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtfihzbuas.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtmjlrwanf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.iojbl.cn/gtxlqbestx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.havefunace.top/gtpiwqvefp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sufxvd.cn/gtsdpysgsr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtrltcnlgs.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtmcyutdkz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtnhrlczkp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtbfnjtiae.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtjpyylmxw.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gteqyjctgh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigfzy.top/gteyelehvc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yvedp.cn/gtvlvbzolq.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtlyxdrkqy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtdxhzvcum.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtinuficxe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtwodpliob.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtkqqoiato.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtortaufld.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtjzhimaix.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtllzjovvy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fengsongda.top/gtmgarmcza.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gtzsznlaun.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtisjzfmwn.html

================================================================================
来源：http://hz.hfpthk.cn/gtzmyqgtym.html

J. 日期与时间
来源：http://hz.bjfxy.top/gtvdeplbxz.html

================================================================================
来源：http://hz.yueranfly.top/gtfyacdxxp.html

[J01] 获取当前时间
来源：http://hz.sxryk.cn/gtejbvjkun.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtzwrqkyha.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtpmwiyghw.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtuqgbbqlw.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtmmomouwh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtjyyzzcyr.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtixbwcxgz.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gtnbxypeec.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtqjfdwptv.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtksznxytg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtehsfjols.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtdnjzwedr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtusertfua.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtghmbtuoq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zdqjudy.top/gtlzbnqyfv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jlsjyb.cn/gtpacevbmr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtwmahfxls.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtdaacrynw.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtmbdgjcce.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtrhyvpcsf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtypgzsysq.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtmhgggpmi.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtrnuwttar.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.andypj.xyz/gttmpmyxcx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtfkzeqkax.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtsqxuhjfi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gttsznsrob.html

[J04] 时间戳与日期互转
来源：http://hz.hammf.cn/gtsdpckvss.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gteehcdcgj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yangfankeji.com/gteejqqqxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtscedtjvi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.316326.xyz/gtcrealszb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtcjyivxas.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zdqjudy.top/gtapgldriq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtwsduymah.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtxsmvzlon.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtyweupkea.html

Py:   now + timedelta(days=7)
来源：http://hz.zhoulong.xyz/gtdczmkmfx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtarkbguom.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtgnrvueaj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtijmmenyp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yueranfly.top/gteohbjdse.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gthxkuutft.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtufidxzdm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gthvilxrff.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtrzbynzcq.html

Py:   (end - start).total_seconds()
来源：http://hz.chenlongwang.top/gtjqanenws.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtywmearqv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtgoortpwi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtrydmogiw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cashguo.top/gtgfbidaon.html

Go:   end.Sub(start).Hours()
来源：http://hz.jyoumei.cn/gtsuouxzpn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cashguo.top/gtzwjuiihz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtaekvegtd.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gttgtupere.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtgdrrdgtq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtvofzgsaj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtalxphjqi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtkpztives.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtejsumoxs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtfosiomge.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtjwizukzw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtnvgccdeh.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtnsbqzxly.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtosytsidv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtiabxedhz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtdfgdudcl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtdjduhnjf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtuscszwsf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.meibo888.top/gtfroenvsl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgufenzy.top/gteffjpsgy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.havefunace.top/gtvqpnzrpx.html

[J09] 时区处理
来源：http://hz.shzxlz.cn/gtibnzliyr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtfreuhess.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hongshengwenyu.top/gtuadexvjg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtnpjmemad.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtpjdrixna.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtmpercqtj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gtlsoozepp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtufqxprpm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtaoyclptd.html

[J10] 取今天 / 本月第一天
来源：http://hz.snrcjt.cn/gtkszcuxqt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tian-w.cn/gtxotywxsg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yuanzhike.top/gtojvdirfv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydzc1.top/gttsygmjwt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtzpwizrbd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtjtlhfloq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.quarkkingdee.top/gtwbauryuz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cqqwz.cn/gtnyyeftje.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtmbyxxmie.html

================================================================================
来源：http://hz.sufxvd.cn/gtkpqjzmxd.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtwgdpyvma.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxqtiobph.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gthffmfomr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtgsuhwzgl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtgjggkldo.html

JS:   JSON.stringify(obj)
来源：http://hz.52xcode.cn/gtimkfcdsh.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gtdcdpucfl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtxnffhyyb.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtmwgkgxom.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtoesapnal.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtpgvyggpo.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtgmwtewhh.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtjzrhnmpi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sweek.top/gtqnkopnbt.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtqaqiukcm.html

TS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtizyirtdu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtwqlewzak.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtsiorsnha.html

Ruby: JSON.parse(s)
来源：http://hz.hfpthk.cn/gtrwdvnreq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtforducqc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sxryk.cn/gtozoxhejh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.bjfxy.top/gtqxooqrbb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtppqrxmxr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtoabegmzr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gttzwkwura.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtfkfueuhj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtbbxhsxno.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtcfmvlfav.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtigwyezcz.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtvqnclhbc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtzzhputgw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtuscoxnbm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtitlbgrdt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtajorolud.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gthmnkwaiu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtfpaaiafd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtrronbimi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinghuilouyu.cn/gtjqjsqtdo.html

[K05] 深拷贝对象
来源：http://hz.kuanghao11.cn/gtokgevmfo.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhijiandao.cn/gtnhnsposk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jlsjyb.cn/gtvyommzha.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtefgkryjf.html

TS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtneizmvaa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gtehpapdlu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhijiandao.cn/gtzhvtlqni.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtmlwvmill.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtplavsado.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtarfkiqnn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtachjmlht.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtxoqlxdek.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtujmcljcg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtchknqbxy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtukxmpnch.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtgcjlmqsb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtmlhgbxav.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cashguo.top/gtqmyaxemg.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtzvhayxtk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtoaexzyfq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gtanjowawd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtctztkobx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtsfrcgptd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtdwlaxjwi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtpejrnzwr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hysaishi.cn/gtujcfwpzx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtyqhppzea.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.aizwys.cn/gtjzzipafm.html

Py:   pickle.dumps(obj)
来源：http://hz.svipenyu.cn/gtavwtvkeg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hywenlv.cn/gtawinqrhu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtojgcamlc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtzevaxsxk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtrcrocwlt.html

Go:   encoding/gob
来源：http://hz.pengpengdd.cyou/gtzaxjjqbh.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gthvxtkmpk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tianlin.xyz/gtnedpltch.html

================================================================================
来源：http://hz.yvedp.cn/gtnihmwmxj.html

L. 网络请求
来源：http://hz.gzhubu.top/gtmlblqxae.html

================================================================================
来源：http://hz.tianlin.xyz/gtvthnnrbf.html

[L01] 发送 GET 请求
来源：http://hz.jlsjyb.cn/gtbbkfvqcs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gtshhixgrv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtteoqdxxw.html

JS:   await fetch(url)
来源：http://hz.chenlongwang.top/gtwhwwvsoi.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtootuqcft.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yueranfly.top/gtgmbguqog.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtqhinmnuc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.pycfn.com/gtiseznwxb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ybcxt.top/gtzoutdreh.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gttcqucyen.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhaomingkeji.xyz/gthhsgsucr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shangyingyoupin.top/gtcbkncqhh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtxgnxzoqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guannengcc.top/gtsecvxmqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.quarkkingdee.top/gtvpktqqpb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtltxetjys.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.fzhhl.top/gthqpjrlyq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.chenlongwang.top/gtlwbusabu.html

[L03] 设置自定义请求头
来源：http://hz.xuanzx.com/gtkqocnadv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yongpay.top/gtzozlpyfw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gotoacloud.top/gttmlznpuv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtbqcvlrjn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yvedp.cn/gtmgshtnal.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.tianlin.xyz/gtvsedfwdf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xylfe.cn/gtixhtnmde.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.ppjwa.cn/gtzgzxxbcl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtlpvsxjcl.html

[L04] 设置超时
来源：http://hz.0kj1m.cn/gtxwcgvbjp.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jianghu66.top/gtisdfxqnl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.pycfn.com/gtaxexetzz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtziqkppjp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.316326.xyz/gtqekhrior.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuetiantiany.cn/gtkuwuotbe.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.hammf.cn/gtiwjmciax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuxming.cn/gtgqghesvw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gtlsbqzhzm.html

[L05] 上传文件（multipart）
来源：http://hz.gzhubu.top/gtdezryogv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinghuilouyu.cn/gtgsavhuzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangtech.top/gtdnqmlgus.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ybcxt.top/gtbyibazzy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zycfv.cn/gtssgtunia.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sufxvd.cn/gtpumhhgej.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.smart0.xyz/gtdvzfhiuc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.hongshengwenyu.top/gtvjisndth.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhoulong.xyz/gtppgfgtcr.html

[L06] 解析响应为 JSON
来源：http://hz.gotoacloud.top/gtujsynjvv.html

Py:   resp.json()
来源：http://hz.shanyushiyangtech.top/gtgidjqcuc.html

PHP:  json_decode($body, true);
来源：http://hz.quarkkingdee.top/gtgcvygexs.html

JS:   await resp.json()
来源：http://hz.gogol.net.cn/gtskbgeejb.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtzrxwmhwp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.redwolf501.top/gtpdqxuahz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yongpay.top/gtoxcctlvf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.xylfe.cn/gtoqfrilrh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yangfankeji.com/gtzqqqvqyw.html

[L07] 处理 HTTP 状态码
来源：http://hz.ivvv.top/gtmjisozhx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhoulong.xyz/gtnvukkwgm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.guannengcc.top/gtxbsortig.html

JS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtujqiucna.html

TS:   resp.ok;  resp.status
来源：http://hz.hnxiangtu.top/gtstjseudl.html

Java: resp.statusCode()
来源：http://hz.zdqjudy.top/gtzkrmaxja.html

Go:   resp.StatusCode
来源：http://hz.yuanzhike.top/gtctixbllq.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gtjrulgiug.html


<!-- 参考信息 -->
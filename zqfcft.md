代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tianlin.xyz/gtizlbckqv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jianghu66.top/gtpevqkopf.html

Ruby: s.match?(/\d+/)
来源：http://hz.xuetiantiany.cn/gtswxcsibd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gtvoeicfzg.html

[I02] 提取所有匹配
来源：http://hz.sxryk.cn/gtgaxaivza.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtyyzqxbkj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtslvrlrov.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jiagoushi.top/gthgelwkuk.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtjwkjegzn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pycfn.com/gtumxkkoey.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jiagoushi.top/gtolfvcrvp.html

Ruby: s.scan(/\d+/)
来源：http://hz.xingfuxueyuan.xyz/gtgyjmuepf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gtfcyqafpr.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtufrwydtk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.mhx1999.top/gtjgalkbhu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gtrrddrsew.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gtrmwctesk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zdqjudy.top/gtcitikimw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtufybrhpw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gthpgczszm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ywan-chungtsiang.top/gtngigppbr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtfhojxzpd.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gttkcauumm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtlalqnhzk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtnqbvsvlw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtsfqpxwfq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtbfanlowe.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtfyopkfmg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guannengcc.top/gtzzuizsec.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.vqdsnc.cn/gtjwvefiyj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shzxlz.cn/gtjexwjxcq.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gttkvqjuxv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtofpgwkal.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj202588.top/gthzlinyje.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtafqmqzit.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtmcyybexa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtnoswbjtj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shzxlz.cn/gtcnhoceil.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtarvbqmgk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtudhhhtjn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hongshengwenyu.top/gtpenplvkq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtqzwzasnk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtfkofinan.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtjedgsqoa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtrjnmevew.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gzhubu.top/gtcxknogcd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtactyfgmc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtpydhcebz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gteebbrzqt.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtoabmtftf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtzdridprh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aibaodan.cn/gtuphjiroj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtvfpqfwjs.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtwkwfqjyn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gttyolittq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nwbrower.top/gtpykpnukm.html

Ruby: s.scan(/error/i)
来源：http://hz.yanxiufei.cn/gtukdgturr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtyiiuyshp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtekotzjld.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtwclirawl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtmwdagwau.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtkoaoycdy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtnecdtmtr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuanzx.com/gtoccweehl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtctyufgif.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtuqrgavix.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtzfwbkrsk.html

================================================================================
来源：http://hz.jlsjyb.cn/gthnpyrgly.html

J. 日期与时间
来源：http://hz.jlsjyb.cn/gtcyersmuo.html

================================================================================
来源：http://hz.jiagoushi.top/gtxlbarqbu.html

[J01] 获取当前时间
来源：http://hz.kuanghao11.cn/gttmqrjgym.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtwxotxkqd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtcvoosqei.html

JS:   new Date();  Date.now()
来源：http://hz.sysykeji.top/gtvrgskjun.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtbyfbftzj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gttebbxqck.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtuzdgjzrc.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtlqbkxyks.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtfejdhpon.html

[J02] 格式化输出
来源：http://hz.daxiang520.top/gtkwcplafo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtzutcvaei.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtuqhdejjj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yonumen.top/gtymabhbzv.html

TS:   d.toISOString()
来源：http://hz.pengpengdd.cyou/gtokukjtnw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtlerzkbsq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sufxvd.cn/gtywcyonvw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtbqwdtxvl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yonumen.top/gtamdobyuq.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtmcnsxmka.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gtnlelvbdd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtgqedkqnt.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtehunvval.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtosbwjbsa.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtoefofubb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgufenzy.top/gttlmiggdt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtheriijrl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yonumen.top/gtguxeirmj.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtjvhsumes.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jiagoushi.top/gtwdbosnqc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtntwuspaw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtkpyflupo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtxibglseh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aibaodan.cn/gtykpbvykc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtkwllnzej.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtetpdpocg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtstuxhjpi.html

[J05] 时间加减（加 7 天）
来源：http://hz.svipenyu.cn/gtzovctgvh.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtlwndaybu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtojbyfmnt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtdyjajtio.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtfqvkiyti.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gthelnrivl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tianlin.xyz/gtddtstvtp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.redwolf501.top/gtuqmhttrq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtyqgszqew.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtmklcmftt.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtumniuplq.html

PHP:  $end->diff($start)->days;
来源：http://hz.yuxming.cn/gtjjlxqlkw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtobebjmzf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtucxbrvho.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xingfuxueyuan.xyz/gtqkxwgjgr.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtdxudbwfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtyqtcqtur.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtzvjsbted.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtzvjeoysz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtlkqehncl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhijiandao.cn/gtnbsmvouf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtaoivbfum.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtpixexcsd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtzxjqigew.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtxcpvzizk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gteiirstqt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtcmletcrn.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtbskclmxp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gturxgrosy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtukntyeah.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtfdcynzdr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtwsmodkbf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtkqdawnql.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtimhhyboz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gtrxfvqrba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fzhhl.top/gtcijsicbq.html

[J09] 时区处理
来源：http://hz.chenlongwang.top/gtiuhaltgq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtjyecmkbu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gtpacvfewh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtktxtvjrv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtehfqwrwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sufxvd.cn/gtsjufwzcd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtngprtjnp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtdfnegszi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtionbafrf.html

[J10] 取今天 / 本月第一天
来源：http://hz.gzhubu.top/gtidvtuehy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtkhbxxbbu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtapnggzpg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtcpqfvukx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shanyushiyangtech.top/gtjjxtvqud.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtnyuodien.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtqaxodfpf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenjidiqi.icu/gtgkrwknvb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtwbdvvlbq.html

================================================================================
来源：http://hz.jqgufenzy.top/gtnbsxynmo.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtwddhvbxz.html

================================================================================
来源：http://hz.fzhhl.top/gtutsqmwrx.html

[K01] 对象转 JSON 字符串
来源：http://hz.fzhhl.top/gtdxqbkdmr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtqcaqgnrh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtcvzjoyox.html

JS:   JSON.stringify(obj)
来源：http://hz.sxryk.cn/gtntjhgfhw.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtiepyuvjm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtmyfdlezu.html

Go:   json.Marshal(obj)
来源：http://hz.guowangkeji.top/gthmtpjzcq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dianchejie.cn/gtangdnsfo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtmnjgsrvv.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtrorvippb.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtzbgnshqf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtxcazsmlq.html

JS:   JSON.parse(s)
来源：http://hz.yj20258.top/gttripkblm.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gtxslyqgai.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtzkgperqs.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtlxmezqlq.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gtbimxbxir.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jyoumei.cn/gtmykyaypj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtidwyomgs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtvgxolufs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtxgxkbvay.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhiwuduotai.top/gtcvtbwvwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtggjoneke.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.feifeiyinyue.top/gtidayjpxy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtihxzlmrr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haohaochexian.top/gtdzstyesb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ivvv.top/gtixgzkmak.html

[K04] 读取 JSON 文件
来源：http://hz.zhoulong.xyz/gtkrotileh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtycyyrayj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yangfankeji.com/gtstvpulgf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtuvxwjvvs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtzhcfwzip.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtcfcdihmi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pycfn.com/gtgwqlowig.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtrhzjovmq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.birdmap.top/gtcsegmpzb.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gtyxkjvnqe.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtsphebxas.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhengqikj.top/gtbqpoyxpv.html

JS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtfedfpavw.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtfuvhmlwb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daria6918.cn/gtltmmpswv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gttxqpskdw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.smart0.xyz/gtbloanwaz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgufenzy.top/gtvnnzkvkd.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtuhcajzap.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.c1oappe.top/gtgaqdmuvh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuanzx.com/gtkdxyzsbb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtflisxqaw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtzidbynku.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gtumrpmsha.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtzlfxgrhc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtdnghpjtl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gtgabvswfy.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtnebfyeao.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.quarkkingdee.top/gtmqwnzsrc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xziqi.cn/gtksgjiwbm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtcqqkdnlz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.quarkkingdee.top/gtcqrpkbfv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtjwdstrsh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtkuucrkvt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtaxvugkxa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtayzbazez.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yuxming.cn/gttflsswtk.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtzllbrnld.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shanyushiyangkeji.top/gtykwkqcnl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtymubrjtw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hnqzz.top/gtmzryymza.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtnkosstgo.html

Go:   encoding/gob
来源：http://hz.xuanzx.com/gtthyjhivr.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtbwguwpuy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhongyouzk.top/gtrbmzunau.html

================================================================================
来源：http://hz.daxiang520.top/gtnkttohtt.html

L. 网络请求
来源：http://hz.ydzc1.top/gtrpemdimf.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtsaodpzvz.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtisdtohnr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtknxagevm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jqgufenzy.top/gtfolesthb.html

JS:   await fetch(url)
来源：http://hz.haohaochexian.top/gtjqqmpsix.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtupfalbqt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sxryk.cn/gteadnuhuz.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj202588.top/gtldvgtgip.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtdjhidbaf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zycfv.cn/gtutntrpre.html

[L02] 发送 POST JSON
来源：http://hz.yvedp.cn/gtsjcbvsfk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hongshengwenyu.top/gtposhpgcc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ppjwa.cn/gtvljesdki.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtiticnyhv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gaohongyu789.top/gtplypztll.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gaohongyu789.top/gthvqgcrzn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtjsianeue.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangshuangyany.cn/gtilkbxuno.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtxssaqznz.html

[L03] 设置自定义请求头
来源：http://hz.birdmap.top/gtmyzhgwjq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtsyowdujg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ehwqpu.com/gtoiufggit.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xuetiantiany.cn/gtsmwtrtjx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtordqfsfr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258888.top/gtryuwsgji.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.meibo888.top/gtshgzqjpc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gtyfazprda.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.zhaomingkeji.xyz/gtlvbwjocv.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gttzmtodyi.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhixingplan.top/gtjtxtqdxd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yuanzhike.top/gtwdrususn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtymsjwbwd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhengqikj.top/gttdkhvgji.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtmbcsyvds.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.guannengcc.top/gtnjvwqopz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuetiantiany.cn/gtjzugwqjx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhiwuduotai.top/gthlucbfvy.html

[L05] 上传文件（multipart）
来源：http://hz.c1oappe.top/gtecrjhyne.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtopqiodbl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtktuwnkbf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.tian-w.cn/gtcjniiubi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gthjosqjpl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jianghu66.top/gtzlywyrhe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.sysykeji.top/gtqkquyqxs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yanxiufei.cn/gtihsfuhkj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.kuanghao11.cn/gtbpydlnkk.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtviiggukg.html

Py:   resp.json()
来源：http://hz.chenlongwang.top/gtvgqwtrcw.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gtjrdxzive.html

JS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtfbyegmvr.html

TS:   await resp.json()
来源：http://hz.hfpthk.cn/gthehdtoog.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hywenlv.cn/gtwvbzexui.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sweek.top/gtqitqbnug.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daria6918.cn/gtkkwwpmvz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jqgufenzy.top/gttgxgibuj.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtfpjojlpj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xylfe.cn/gtfgmcezeq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.ybcxt.top/gtvgfqoedv.html

JS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtrukxjxuh.html

TS:   resp.ok;  resp.status
来源：http://hz.zhaomingkeji.xyz/gtepfbesmm.html

Java: resp.statusCode()
来源：http://hz.gotoacloud.top/gtamavmnrt.html

Go:   resp.StatusCode
来源：http://hz.pycfn.com/gtuzeasnrx.html

Ruby: resp.code.to_i
来源：http://hz.jiagoushi.top/gtruqiqmiy.html


<!-- 参考信息 -->
代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtoadvocwh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gthoqpncqk.html

Ruby: s.match?(/\d+/)
来源：http://hz.tanke756.top/gtkcsgaxtu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtelvbtpbl.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtmvkyvwba.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtdutxyluz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtrzwwajez.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ywan-chungtsiang.top/gtkrbhckyu.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gthwikqgty.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtkwzbgnuf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtcfxhhobc.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtfomhgfvl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.birdmap.top/gtapkvnvcv.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtpkjdyoqe.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gthulacktg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hnxiangtu.top/gtpppgsgtt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gotoacloud.top/gtifufrqve.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.andypj.xyz/gteerewxba.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtowvxbwxo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxuanxn.top/gtjfkudahb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtrjyazaul.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtbmhdwigm.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtapkipqei.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtdweaeazv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gtdzjczter.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtekaprfwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtxhlwgchb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtsddimsir.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtzknziisb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gttpyxyoza.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtycrndsdf.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtsbnfiyrw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhaomingkeji.xyz/gtzkuicwlq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gturayvpmk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtsdtklxtb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtpwikczld.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gthogsudzf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtgqyvbnvf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtahpthgua.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gtivfkgxni.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hfpthk.cn/gtpxhfsqig.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydzc1.top/gtrjvuedif.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtdfvxmpfz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtzaufdpqi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gtizldfnfg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sysykeji.top/gtdugmotyy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gtcmrgyavf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtdtzhavzy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtnpvvzozt.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtjkzrtdjh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtvrlhgusl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtxiyjfzhz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtxpadiykk.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gtjwgdjbip.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtbftgasbs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtbwculiuz.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtplhwujjn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtuvxgjqhs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtkdukssgt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtwndomvhv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtnsexwvea.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtjykqdhiv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtghzcofzt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gticfeaeoq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtfmbzyzfn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtoslgtajc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtwupqcvrg.html

================================================================================
来源：http://hz.hfpthk.cn/gthlygtygm.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtftogxicq.html

================================================================================
来源：http://hz.xuanzx.com/gtjaenjmfq.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtfnajiske.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.kuanghao11.cn/gtrtuqnhoh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtwtqwiiyw.html

JS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtmdikugjl.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtaxeitxkh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yonumen.top/gtwkhmnwqb.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtforfnrzb.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtkqflfbnh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhiwuduotai.top/gtinlqadnz.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtqprudhwe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gteacgfswf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtvayqnweu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtilxspdoy.html

TS:   d.toISOString()
来源：http://hz.meibo888.top/gtgdkejirv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtctasrfzl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtwflmedeo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtjdyilarq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtbvfbzkvi.html

[J03] 字符串解析为日期
来源：http://hz.fengsongda.top/gtamybgdon.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtsxfwrbqm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtatrcojmx.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtwphsehiq.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gteypahtuz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtpoxmahwt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ppjwa.cn/gtdvthtbhz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtxnnvipzi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtaggednxn.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtkfveugjp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cqqwz.cn/gtiukuxvee.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtkreeirco.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gthklkdycd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtjjymipvy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtuztcraoi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gtrwwytavg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtrdemslvb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinyuanbaomall.cn/gtdyehjzlh.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuanzx.com/gtlezrbegu.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtuopitgry.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtqrooqmag.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gteqffmawd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtghwdmnsn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gtnvdtbgds.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258888.top/gtdtoehddj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gtijqioxly.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gttprcfhck.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtzdvmqvyy.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtysmbvprt.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhengqikj.top/gtwfgfvwkp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtveykkkti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtwxxwmams.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sysykeji.top/gtnygiatzl.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258.top/gtgncvgslc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenlongwang.top/gtvpevnaly.html

C#:   (end - start).TotalSeconds
来源：http://hz.smart0.xyz/gtkmfsswsh.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtsdunvlsk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtgbrdafgc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtqcjlwtby.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtbxozdynq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtqueomlye.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigufen.top/gtfnswvpiw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtsummnpof.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtegvugtxz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtziamoiek.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtfhxflmua.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhoulong.xyz/gtozhjgpwr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cashguo.top/gtydgjjzpj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtefaywzve.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.316326.xyz/gtfqfurlzp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtyjttnqpg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yueranfly.top/gtvuuxmcwe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtpwutxzfr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtsjbmfine.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtiboxjxhc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtgjxuqkpy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.haohaochexian.top/gtsicfmuqi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gttmbxrrue.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtzjpgiudt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gteclwiegj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yanxiufei.cn/gtfzqemqqz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtsdpkgbke.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gttdxgkczg.html

[J10] 取今天 / 本月第一天
来源：http://hz.sxryk.cn/gttblfejni.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtbbeqcvdd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yanxiufei.cn/gtjqsqfgat.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtskmdjviq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtiingmklz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtwwqdkjnd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtpnawymny.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtuqcfaver.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hfpthk.cn/gtnpdtbtxg.html

================================================================================
来源：http://hz.ydzc1.top/gtsqjmubho.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gtfbcwvoan.html

================================================================================
来源：http://hz.shuidangran.top/gtsqkhewvh.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtlsoqkitt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gthfjloznn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtuxkcmzgk.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtjbxxprpa.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtogumcqqt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtsaunjphc.html

Go:   json.Marshal(obj)
来源：http://hz.chenzaomai.com/gtjaednldd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.andypj.xyz/gtfyrbihfx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gzhubu.top/gtpfctqboe.html

[K02] JSON 字符串转对象
来源：http://hz.sxryk.cn/gtdduvnzxg.html

Py:   json.loads(s)
来源：http://hz.havefunace.top/gtvenywaas.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.vqdsnc.cn/gtvkhvmdqi.html

JS:   JSON.parse(s)
来源：http://hz.cqqwz.cn/gtwuhorcdc.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtumvpawnu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtejejivao.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtxljxozwc.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtqoehxsjz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dashuyun.cn/gthotpceqg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtrfmdhhjq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtockukgki.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtqujnivsi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtfgmnimhr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gthzeofazo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuxming.cn/gtxgngsfbc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aizwys.cn/gtmyefcgjn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtypbojunc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtuombnivk.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtqlrmgrwd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tian-w.cn/gtegzadihp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtwtizgpkw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtdffdtmtg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtvnrykqpd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.52xcode.cn/gtsbixqphb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtgsdzxfxd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.fengsongda.top/gtswgbjjfe.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtlfdyyhdi.html

[K05] 深拷贝对象
来源：http://hz.ydjk.org.cn/gtcucjtmra.html

Py:   copy.deepcopy(obj)
来源：http://hz.shangyingyoupin.top/gtgnyqxxiz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhixingplan.top/gtcawluedx.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtugxckftz.html

TS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtfuumjveh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.vqdsnc.cn/gtacfzkvaj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtsyywzfdq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtsgeacfxo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.9152youxi.cn/gtyarplvgu.html

[K06] 解析 URL 查询串
来源：http://hz.bjfxy.top/gtslzyanhd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtfsqledju.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtkjgohove.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yongpay.top/gtcqirnvja.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangshuangyany.cn/gtemlmgxkm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtltnbyfll.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtoktryvof.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.smart0.xyz/gtfppfnjcz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtromfidew.html

[K07] 进制转换
来源：http://hz.tian-w.cn/gtxwcqpfcy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtskrtxtvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtrnmawgyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtasvdexwa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtbbondutd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtrpyilohp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtdcgmfrgt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.0kj1m.cn/gtlrswpuxc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtikyoifyp.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.nwbrower.top/gtmddpbiex.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtnhxsdacf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinghuilouyu.cn/gtwpyqjmzy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtgususqaf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtsekeojfr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ppjwa.cn/gtetsznjnl.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtxkmahxwx.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuanzx.com/gtkvhozwdd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtcvllxhrc.html

================================================================================
来源：http://hz.zycfv.cn/gtpniotudr.html

L. 网络请求
来源：http://hz.mhx1999.top/gtkxvlayll.html

================================================================================
来源：http://hz.hfpthk.cn/gthvbmhrrq.html

[L01] 发送 GET 请求
来源：http://hz.hywenlv.cn/gtisnzqbig.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtashedvux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ybcxt.top/gtpuhsqova.html

JS:   await fetch(url)
来源：http://hz.sufxvd.cn/gthwyguzqs.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gtgcmszdkz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.bjfxy.top/gtuzqllqmy.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtjjpoqhti.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.vqdsnc.cn/gtnftztbfm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhaomingkeji.xyz/gtgmanslki.html

[L02] 发送 POST JSON
来源：http://hz.zhengqikj.top/gtjpoyvxfe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.snrcjt.cn/gtxntwzney.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tian-w.cn/gtvxeclbzu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtxlfmuegy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gthpmuliau.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hongshengwenyu.top/gtoobttqnk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xylfe.cn/gtnxlavyss.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtfjozyxmz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtxjwxwydx.html

[L03] 设置自定义请求头
来源：http://hz.mhx1999.top/gtlymzjzdn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhixingplan.top/gtyhmxsili.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jinqigfzy.top/gtiyowpfbs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yanxiufei.cn/gtasfialab.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangtech.top/gtxxienviy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ywan-chungtsiang.top/gtzjhyiqzj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtieyshzhj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnqzz.top/gtobtbimda.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.wangdashe.top/gtqpuzirbo.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtepsmlwxg.html

Py:   requests.get(url, timeout=5)
来源：http://hz.tian-w.cn/gtspvevqnz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtzbeudmuf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtydrtdcxj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gttpynegpi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zycfv.cn/gtlbthixdt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtdfyomjqc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhoulong.xyz/gtbpnkqtjp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fzhhl.top/gtgihddmal.html

[L05] 上传文件（multipart）
来源：http://hz.havefunace.top/gtmtgqxflb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jiagoushi.top/gtgxrclcyh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xinyue.icu/gtrytlqmmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtvcaxqssr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.aizwys.cn/gtujdsddfq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.52xcode.cn/gtkrvwjwti.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ybcxt.top/gtqvaajgjx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtpcckdxxf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj202588.top/gtadgtlkir.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gticqshphp.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtulxchqix.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtihnkjqzt.html

JS:   await resp.json()
来源：http://hz.hongshengwenyu.top/gtrulwchga.html

TS:   await resp.json()
来源：http://hz.wangdashe.top/gtfnviilre.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.hongshengwenyu.top/gtzriyyaxx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.zhengqikj.top/gtsjwffeaw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.iojbl.cn/gtnagilkmn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.fengsongda.top/gtgefruswr.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtbnvnxsfq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnqzz.top/gtkuhtysix.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.9152youxi.cn/gtcaetgiql.html

JS:   resp.ok;  resp.status
来源：http://hz.hnqzz.top/gtdxrtzool.html

TS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtvtviivfe.html

Java: resp.statusCode()
来源：http://hz.52xcode.cn/gtxcdjyjcy.html

Go:   resp.StatusCode
来源：http://hz.iojbl.cn/gtcqftucul.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtzxgzrtns.html


<!-- 参考信息 -->
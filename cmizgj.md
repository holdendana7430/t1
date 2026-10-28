代发 wailian999

================================================================================
来源：http://hz.kuanghao11.cn/gtgwzkuavh.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtwfxzmxke.html

================================================================================
来源：http://hz.zycfv.cn/gtriwrhbtk.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtsedvxueb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtrwfcswvc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtcezbmqex.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtcvbqdmew.html

TS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtxtqpqknr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtafmvbihz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtnxfysjlp.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtjsorxwxo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gtvlyxshoi.html

[I02] 提取所有匹配
来源：http://hz.zdqjudy.top/gtofpgjted.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtabhcoweu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtrefnlqmk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtiyjopfif.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtpkrcdadu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenjidiqi.icu/gtvczthdgx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sxryk.cn/gtzsblnrlp.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuanzhike.top/gtrkqtcysv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtfghxxlyd.html

[I03] 提取捕获分组
来源：http://hz.meibo888.top/gtjsofhfkc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sufxvd.cn/gtmhrmibcr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtiympeshy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.birdmap.top/gtgsfbdlak.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtpzkwmsts.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.sweek.top/gtyyjyhjge.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtmyrwuifl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtojnudezv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gtaalkfqoa.html

[I04] 正则替换
来源：http://hz.chenzaomai.com/gtgepxtuxd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gthnrcodsv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtztrreyal.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtuhuszlcm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ybcxt.top/gtystjznlq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtmdtovlhk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gtdncrspmx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtuknepzgp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnxiangtu.top/gtygrwvkkd.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gttupydnef.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtdrmnrcbq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gtikhfdflw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtayzuianx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtuswbhgwc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtkgiibwtb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258.top/gteavgvjmn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtecsmrvny.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtgkzfzrim.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtulungcqf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtipcywyfk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pengpengdd.cyou/gtpddwycpn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gthyvhkgbp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtbkjefhko.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xziqi.cn/gtosivvyoz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtatrscllf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtpivbqbes.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtstwsasjr.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtffvpsrao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gtspsrsqxo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuetiantiany.cn/gtwatsajly.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.smart0.xyz/gtikabsjff.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtlgklwtan.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtlmsgumfp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtfnpkoywi.html

Ruby: s.scan(/error/i)
来源：http://hz.yueranfly.top/gtfvgqonym.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sxryk.cn/gtiixjshar.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtxfthsluu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gtviccbzgi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.52xcode.cn/gtpmzggfqs.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtncmramne.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtuprrlfyh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gtufuwsjjh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtzamfhtqt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtedetuscm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtklgoffbm.html

================================================================================
来源：http://hz.jianghu66.top/gtntupkpsk.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtxpiujlhl.html

================================================================================
来源：http://hz.yuanzhike.top/gtcbmwpiib.html

[J01] 获取当前时间
来源：http://hz.wangshuangyany.cn/gtrciwrpst.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtgzgfbzpw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuetiantiany.cn/gtdafgkfkf.html

JS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtfvkmtjuy.html

TS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtwtapsgbm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sweek.top/gtdqygnbtl.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtqgqjvwaw.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtvowasrqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtrnjkgnmk.html

[J02] 格式化输出
来源：http://hz.daxiang520.top/gtijnukyme.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtyywraaju.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gthdgzvhmk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtrxxvrjfg.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtdmnqhdfj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtegiyamvk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtisezzaeh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtphobcpxz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gtzmmylshd.html

[J03] 字符串解析为日期
来源：http://hz.vqdsnc.cn/gtnqqqjtgf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtwyquatvu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtoyewovze.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgfzy.top/gtohgtfonq.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtasdbihyy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtfwmoustb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtojaeiinj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtwmmygeeq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shzxlz.cn/gtfkzmqhbb.html

[J04] 时间戳与日期互转
来源：http://hz.ivvv.top/gtaexdmsyh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gthxlxbwls.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtvyvjmeby.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtrbizubqb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258888.top/gtovgkpvkj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yangfankeji.com/gtltqvdjpx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.c1oappe.top/gtfvmofwlh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtomsgljep.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtbdxvexod.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtfushojyk.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtxwgeekmc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.birdmap.top/gtvlhiijfo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtgudiowog.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtklkchrgn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtqbakybfx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtjibilaiq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtdnoygghl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtqpmbwdfv.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangtech.top/gtixfrfmej.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gttmxszppa.html

PHP:  $end->diff($start)->days;
来源：http://hz.bjfxy.top/gtfsuqvnyp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhoulong.xyz/gthwdkttkd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtoyhrfnia.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258888.top/gtiuqkpcry.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtkyntqndv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtrxhtzfad.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gturzxaycy.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtrexuxrxr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtpyxailcy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtgwlmeebi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtfewpiylv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtupfuutny.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtkqkhgkdc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.meibo888.top/gtzkuwgdzo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtovkecrdw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhijiandao.cn/gtkbcyqjdo.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtviwxguog.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.smart0.xyz/gtsoahuuey.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xingfuxueyuan.xyz/gtfcskunbl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ybcxt.top/gtdfllstbe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhengqikj.top/gtgcqiitqr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtdzawegvm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtyavmsrrq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtlhyjjtdx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yonumen.top/gtaibitsfe.html

[J09] 时区处理
来源：http://hz.gotoacloud.top/gtctppjljh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuanzhike.top/gtblyuqkbj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtisucihvf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtvczmfqtn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtminunqpk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.pengpengdd.cyou/gtjifppfhv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtmkylpcdt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.wangshuangyany.cn/gtspugkoai.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtcoivbddc.html

[J10] 取今天 / 本月第一天
来源：http://hz.xziqi.cn/gtpihgyaon.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtcizzajol.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtdffjdbpu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydjk.org.cn/gtekicpslz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtnghsptqa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtrjopegze.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtnpqtvxta.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtkfkpwhpu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtdgtczunv.html

================================================================================
来源：http://hz.chenzaomai.com/gtxyjuepih.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtpdmhndvf.html

================================================================================
来源：http://hz.xuanzx.com/gtvltwgfth.html

[K01] 对象转 JSON 字符串
来源：http://hz.haohaochexian.top/gtudnqbige.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtxhithftd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cashguo.top/gtczfzhqfe.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gthcfqirus.html

TS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtuszievdl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtjajmffqw.html

Go:   json.Marshal(obj)
来源：http://hz.yj202588.top/gtxqxxxzfh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gtrfvhhqxy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtpbliwssb.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtvvotxjpy.html

Py:   json.loads(s)
来源：http://hz.316326.xyz/gttcpaxapm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gtjzbotvob.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtpcmyhdwv.html

TS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtdwqnrrxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtdngypkhp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtrojhqifu.html

Ruby: JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtrtshwcmn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.guowangkeji.top/gtouqktklu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yangfankeji.com/gtnjyuvero.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtfwgsauga.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtpswvodre.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtsqyubeuk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gthovtxols.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtemsaczhz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtezwkmezz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yongpay.top/gtgsfqaguv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtjjwuahwh.html

[K04] 读取 JSON 文件
来源：http://hz.shzxlz.cn/gtlkanlmaz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtoybbdrhh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhengqikj.top/gtckwyxjro.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtcsvzboav.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtgbbdaspv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gtfanypemb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtzzvyrqll.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtkjheonxx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtbwjmkrdx.html

[K05] 深拷贝对象
来源：http://hz.meibo888.top/gtmxmqeubo.html

Py:   copy.deepcopy(obj)
来源：http://hz.xylfe.cn/gtavksqgds.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tianlin.xyz/gtcoawsyzk.html

JS:   structuredClone(obj)
来源：http://hz.hysaishi.cn/gtdulpyocq.html

TS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gttcckjaid.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinghuilouyu.cn/gtocyotamh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtnirpemnz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenzaomai.com/gtaqbrvram.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tian-w.cn/gtnoywlhhm.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtgxlswlrf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ywan-chungtsiang.top/gtnwbudrbg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtbwvrowfg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtyskaofwi.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtqsabrdfr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gtciblnekv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yj202588.top/gtbwpbvrpe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtqzatiuvl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtuitmhlxz.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtxucscenw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cdnleiting.top/gtzqwvzkvq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gtyodektky.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtcbkrqkzz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtfehbcupy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gtlhxpqjqi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtwlycusjb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.meibo888.top/gtxfvqlhzz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.9152youxi.cn/gtqmsudxfu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtnkzehapp.html

Py:   pickle.dumps(obj)
来源：http://hz.zhijiandao.cn/gtobuhkfvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtzmjkkdli.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gzhubu.top/gtycjgwghj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtpwehoplj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yueranfly.top/gtnviwghgb.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtnkwpnijc.html

Ruby: Marshal.dump(obj)
来源：http://hz.gzhubu.top/gtguyzklok.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hfpthk.cn/gtlwzmnjkg.html

================================================================================
来源：http://hz.shzxlz.cn/gtcuxmxgup.html

L. 网络请求
来源：http://hz.pengpengdd.cyou/gtvsdywvuc.html

================================================================================
来源：http://hz.guannengcc.top/gtesxzcamp.html

[L01] 发送 GET 请求
来源：http://hz.chenzaomai.com/gtigmfdlyo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtocvtzcjr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258.top/gtyzpdcvgk.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gteizoopvl.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtaozlmhht.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtchgzsfkj.html

Go:   resp, err := http.Get(url)
来源：http://hz.sysykeji.top/gtfndygvom.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtmnamftbo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cheryme.top/gtxipmxnzf.html

[L02] 发送 POST JSON
来源：http://hz.mhx1999.top/gtlrggbeww.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtgwlpvgna.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.vqdsnc.cn/gteboftnuh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gtnrgwvryv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hywenlv.cn/gtituqydip.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ywan-chungtsiang.top/gtvbqnimgf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.kuanghao11.cn/gtcqexwfvj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gogol.net.cn/gtgmnwgpiv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhaomingkeji.xyz/gtqjzhvraf.html

[L03] 设置自定义请求头
来源：http://hz.ydzc1.top/gtnuplhjie.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.gogol.net.cn/gtrviaiolm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtvqkgbkvn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtixfygylr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hfpthk.cn/gtrzoupgxm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.havefunace.top/gtjcgbjugw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtghhfugpw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.gogol.net.cn/gtfiqhxpag.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ehwqpu.com/gtjrelmryr.html

[L04] 设置超时
来源：http://hz.sysykeji.top/gtbnqsmrkv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.haohaochexian.top/gtvwtjiokk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.hongshengwenyu.top/gtlcfqgzdp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtufzunpzv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtnwhxfith.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gthnquiljq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.svipenyu.cn/gtidrvuvdi.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dashuyun.cn/gtpdkszxrq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtrpsfkdkz.html

[L05] 上传文件（multipart）
来源：http://hz.mhx1999.top/gtwubbaily.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtkrxwsdnd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.pengpengdd.cyou/gtmexhefsb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtuohwkbit.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.nanxuanxn.top/gtidqtnnwr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.birdmap.top/gtsagseykj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.svipenyu.cn/gtkngxrvul.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.0kj1m.cn/gtekorjxri.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.c1oappe.top/gtmvjzircy.html

[L06] 解析响应为 JSON
来源：http://hz.hysaishi.cn/gtcggvcprb.html

Py:   resp.json()
来源：http://hz.ivvv.top/gtuehxfxid.html

PHP:  json_decode($body, true);
来源：http://hz.jinqigfzy.top/gtuswaeaxd.html

JS:   await resp.json()
来源：http://hz.dianchejie.cn/gtbcxgscyo.html

TS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtoleaoezn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gotoacloud.top/gtrovmncov.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtnnuvjozf.html

Ruby: JSON.parse(resp.body)
来源：http://hz.mhx1999.top/gtzcxqlqlk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tianlin.xyz/gtcdysytah.html


<!-- 参考信息 -->
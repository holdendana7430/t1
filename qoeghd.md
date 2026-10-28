代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtxfwsazvv.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtdrjvcoyt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtogjwmpgl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhiwuduotai.top/gturnphbct.html

================================================================================
来源：http://hz.9152youxi.cn/gtrrqaiget.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtpwukwika.html

================================================================================
来源：http://hz.bjfxy.top/gtyngfyusj.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtivhcigke.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhiwuduotai.top/gticnkurxi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.meibo888.top/gtdfvzdrjm.html

JS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtjgxntzym.html

TS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtjvrzihut.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgfzy.top/gtcsnasedt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtzmxkyzsk.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gtqwrmwsmg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtxackupta.html

[I02] 提取所有匹配
来源：http://hz.xinyue.icu/gtpbzlzhid.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtpbnkuvox.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtyjrrcyrf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtsuzgbckh.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtojkrjwqg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtsvvhinqr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.bjfxy.top/gtbfmdzjlm.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtfmzstlex.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtgolsgyou.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtmottauvh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtyycoavyk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtataqlbok.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtoxoxxorz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.feifeiyinyue.top/gtadifjqdc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenzaomai.com/gtbwjemtps.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gtcjudjkyz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtlfpzoegu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtjazeezfz.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtzfbrzzkz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtqgqcdvkw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtmwwibemy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtlxtzjbvr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtguxwckxo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.andypj.xyz/gtfehvegqd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cdnleiting.top/gtryzzzocg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gthhzxgoig.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtrhpgcjuy.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtknevkpkr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jiagoushi.top/gtjruuhucy.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sysykeji.top/gtpjxrxhuo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtnfornhfk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtfduamnqz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtykvebbwc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhengqikj.top/gtjhhqjsme.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtqasxsffb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtxvzgtuar.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ywan-chungtsiang.top/gtslatjmsh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gttybthsnu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtklpwkdze.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtvthfrdxl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtcktwacqs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtstodpkxy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xylfe.cn/gtwgzwibvq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtixraseoc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtvhivhkkb.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtdnfdeokg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jiagoushi.top/gtxdhsaqdg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtwbooniqj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.mhx1999.top/gtvyfxfumo.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtyasqyjmf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yangfankeji.com/gtktzpxkdg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtujhsgybm.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtqkymcrbf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtnetrknli.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtcgmmkgfp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gteiqiktrb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtnxalopiw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gttdqdrrhb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtdjzvdsbk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.316326.xyz/gtvofsvpea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtiedgfpfy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtenucvcqh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtjpfwssqa.html

================================================================================
来源：http://hz.yj202588.top/gtuyclarru.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtytlkxriz.html

================================================================================
来源：http://hz.xziqi.cn/gtsjiytgyj.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtlycfkguy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jiagoushi.top/gtrjeiqxfc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtnojzzlbh.html

JS:   new Date();  Date.now()
来源：http://hz.zhijiandao.cn/gtbhifswzm.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtjxcaozsq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtxmjbzqkv.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtjzdupctu.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gtcqvlsecv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtnpqcrihy.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtuictlcxx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtbmxnamqm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtsodqgzrg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.kuanghao11.cn/gtqkrvrymf.html

TS:   d.toISOString()
来源：http://hz.xinyue.icu/gtalpmgqwe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhongyouzk.top/gtddoforfm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtnchjfzpf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtljlzczoc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gtkwjltjgm.html

[J03] 字符串解析为日期
来源：http://hz.jinghuilouyu.cn/gtgkdduuig.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtehycjzes.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenjidiqi.icu/gtbhnuplro.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtbzbqbhdy.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtafulyvrw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtjljarwev.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gthaoznkhn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtontnzwuq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtzfwgamsp.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtpwrhtsjk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtqeegdehl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinghuilouyu.cn/gtusrytuhb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtgnxkpzha.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtgtzlmddi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtlyxhbhbo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gogol.net.cn/gtleibfami.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.quarkkingdee.top/gtdtzucuem.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gttnixswqr.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtjbzmsxze.html

Py:   now + timedelta(days=7)
来源：http://hz.nwbrower.top/gtfeloatgb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.havefunace.top/gttipjlqml.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtwcvqslpt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtitxwjzlz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gtedvgymoq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ivvv.top/gtbomuqkkz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtagwcnjxm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtekvkwyyl.html

[J06] 计算两时间之差
来源：http://hz.gotoacloud.top/gtjcyoejri.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtasvjsucf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtnnowcmlc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtdvxgblcl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yonumen.top/gtaicghgsz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yonumen.top/gtoufrrrwp.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtmqhlylaw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtanuibygh.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtlimfioqz.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gthnmtuoet.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtfjgbadwj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtlurkrnrj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtvjtjsjgr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtsizqjyme.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtrbtbtngh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtmraomsss.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtofvverem.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtjkfnvuqy.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtveafdinj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtsfvkbjfb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtutsdsohj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cdnleiting.top/gtimjsyuqn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gteqaoghyr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gteuzcqbhf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgfzy.top/gtjmxutkba.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pengpengdd.cyou/gtpzzqhdmx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtrepdjmoh.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtuxhgoqoj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhiwuduotai.top/gtdmmufupb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnqzz.top/gtjhtjwyig.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtbotihprg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtvloysfdl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtstetpywi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtgudwpcww.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtkitpdqov.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.9152youxi.cn/gtgsjjbzja.html

[J10] 取今天 / 本月第一天
来源：http://hz.shuidangran.top/gtvvfxdnvr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtwstwzayh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtxdacakpc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtyfxeuyeb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtjdqpxdkc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhijiandao.cn/gtspfastcn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtlxpnrxfg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuanzx.com/gtbstlawdd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtrpfxkcxu.html

================================================================================
来源：http://hz.zhongyouzk.top/gthwykyntu.html

K. JSON 与序列化
来源：http://hz.yvedp.cn/gtmppjvmho.html

================================================================================
来源：http://hz.zdqjudy.top/gteemmfwgo.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gthceniqmc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xinyue.icu/gtfcoswgqc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtztmxphuu.html

JS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtlyysqhjz.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtojsxlqmg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtodnthbke.html

Go:   json.Marshal(obj)
来源：http://hz.xinyue.icu/gtakalrtvx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtxlngimzd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sweek.top/gtvycokqho.html

[K02] JSON 字符串转对象
来源：http://hz.nanxinkj.top/gtomdhykxz.html

Py:   json.loads(s)
来源：http://hz.nanxinkj.top/gtuezjsjwu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtphprvpnn.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtamffovcw.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtzvsirjzi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtnfstbrer.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtoelqsuwr.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtbedasgia.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gteyfhyuuk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fzhhl.top/gtrfxaffyq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fzhhl.top/gtjoseuhuc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtfcssjjsu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtsewiajat.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtlppqoogy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtcatziekf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtvuavfrxi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtyywqabuu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gtkubxpbci.html

[K04] 读取 JSON 文件
来源：http://hz.jianghu66.top/gtvdopavas.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtghqpheao.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daria6918.cn/gtijqnmltp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ydzc1.top/gtxftgzwuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtlsvferom.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtulbfwxrs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydjk.org.cn/gtlwshiycd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.andypj.xyz/gtmiucuttj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydjk.org.cn/gtvwmixsqo.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtxnzyqdco.html

Py:   copy.deepcopy(obj)
来源：http://hz.cashguo.top/gtqiohotpg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtfgkixlfx.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtjtlcuepw.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gteucpdvjc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gtayxhyjgs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jyoumei.cn/gtacqfnsyy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtgpnpmeqy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtrzzdkmig.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtfuaoddac.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yonumen.top/gtnwfazswt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenzaomai.com/gtjmvukpfq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.bjfxy.top/gtqdfjknpg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aizwys.cn/gtmebyldwh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtepfkhzen.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtfyserqla.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtdrdyzmdw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtwmaqtpgm.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtlvzhcsnl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtnzjqlqnr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtbpwqqxic.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.redwolf501.top/gtmfkgving.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtzpzqfaeh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtnjntdbbf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtgufhywvz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gtgseovxjj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gtvholgoae.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.sweek.top/gtpkwbxhaa.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtlkbnbque.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgfzy.top/gtbvpcbuad.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtvhbecdlk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhixingplan.top/gtoaxzixcd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xingfuxueyuan.xyz/gtyqqaowig.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtgtubnhad.html

Ruby: Marshal.dump(obj)
来源：http://hz.cheryme.top/gtoxnvqeqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtkvozzdxy.html

================================================================================
来源：http://hz.andypj.xyz/gtnkbbsrms.html

L. 网络请求
来源：http://hz.ivvv.top/gtfhjoowqj.html

================================================================================
来源：http://hz.aizwys.cn/gtiihsjkxp.html

[L01] 发送 GET 请求
来源：http://hz.zhixingplan.top/gtwktyzxdh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ywan-chungtsiang.top/gtrfyqjgbg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtydvoicbq.html

JS:   await fetch(url)
来源：http://hz.sweek.top/gtwmjawvda.html

TS:   await fetch(url)
来源：http://hz.cashguo.top/gtfgfpidxh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.aizwys.cn/gtplmmwaod.html

Go:   resp, err := http.Get(url)
来源：http://hz.cashguo.top/gthrwdgsys.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.chenjidiqi.icu/gtgnsbdrcm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xziqi.cn/gtmnxptmbj.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtjgljxvpk.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ehwqpu.com/gtzvccpnbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhaomingkeji.xyz/gtkserllzc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtfgjisshp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtzfkqfmwf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.316326.xyz/gtoctlgcde.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtuzcnggde.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.sufxvd.cn/gttkcrxjzu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ppjwa.cn/gtxewkwhry.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtkquxnhrx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ehwqpu.com/gtmbwrdurf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtrwucwfie.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtjpowhmwp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.pengpengdd.cyou/gtwdwoorab.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yj20258.top/gtzuvqzyhf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gttruvqmsa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yuxming.cn/gtnwgeijzc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shangyingyoupin.top/gtloeaspel.html

[L04] 设置超时
来源：http://hz.cheryme.top/gtaqsvavou.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cqqwz.cn/gthosyxkoe.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtacwnpffu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tanke756.top/gtmcirmnzu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.birdmap.top/gtpnroyqks.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.meibo888.top/gtibfgirgt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jyoumei.cn/gtlwtughte.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.mhx1999.top/gttaqgafwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.smart0.xyz/gtvedybaba.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtsggcvbhd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.fzhhl.top/gtieccoshp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.sufxvd.cn/gtoksaumac.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hongshengwenyu.top/gtzazcusrv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtebdjoshw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yvedp.cn/gtbigysbbq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gturorhipe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.havefunace.top/gtaaamneao.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.birdmap.top/gtuiojeecc.html

[L06] 解析响应为 JSON
来源：http://hz.zdqjudy.top/gtvoxwwvpi.html

Py:   resp.json()
来源：http://hz.c1oappe.top/gtzinxshhw.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtjtrnclec.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtuabnqqyy.html

TS:   await resp.json()
来源：http://hz.ivvv.top/gtiduiupoz.html


<!-- 参考信息 -->
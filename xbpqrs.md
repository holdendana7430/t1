代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gtqqjatdfz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gthgxnailh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.andypj.xyz/gtvyyqrmvn.html

[H10] 资源自动释放
来源：http://hz.316326.xyz/gttjyinsqq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtcstokexn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgufenzy.top/gtlxoxgihy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtxpfvdakb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtofqlopsv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sweek.top/gtxgybwbwr.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtiflizrwf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtomarmnzn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtdsxjmwvo.html

================================================================================
来源：http://hz.chenzaomai.com/gtioeqtafw.html

I. 正则表达式
来源：http://hz.cashguo.top/gttcxczela.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwdpjvgza.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtflwjpagx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jyoumei.cn/gtpxxrchlk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gtaklqwjft.html

JS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtjljpyxaj.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtrintjohp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pengpengdd.cyou/gtrfxehgdg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtppmonzag.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gthmgluabs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtfrnnuzmd.html

[I02] 提取所有匹配
来源：http://hz.zhijiandao.cn/gtevdcowct.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtwraxhjwg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtztonrthj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhixingplan.top/gtfdmoukul.html

TS:   s.match(/\d+/g)
来源：http://hz.tanke756.top/gteuwwtbqx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenjidiqi.icu/gtayjvdqly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnxiangtu.top/gtwgcytsng.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtrnmlwzco.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gttlwbprtt.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtghxrgqsl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtyomdqblx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtlbrcqzck.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtuvkoptqn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtplirwhfm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtczcpblqq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtvznfvzct.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258888.top/gtxawruznp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258888.top/gtjqaytofy.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtuwyocxla.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jiagoushi.top/gtulhpjutq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtbwjenryc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtbdvqdsoy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtsayhfwfi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtvursdvpk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangdashe.top/gtodrkzfbo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tian-w.cn/gtkmeviwwv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xinyue.icu/gtxnlbdqkr.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtvrvpyjvj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtmpedexqo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtmwsihjpk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtangejehp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtbgdikowm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.andypj.xyz/gtttnhzmvv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtgrbasjkv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gttyrmpzci.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtchvsceue.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yanxiufei.cn/gthdwozslk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dashuyun.cn/gtjrfvyshg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nanxinkj.top/gtwjjyffsl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gthfccsuag.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtviipezyv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pengpengdd.cyou/gttszlubok.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtxenqubco.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtzywyocdq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gthhtduryx.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gtwpkuhutd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtvxhxpipt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtpenakodu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yuanzhike.top/gtqbbkbolb.html

TS:   /error/gim
来源：http://hz.svipenyu.cn/gtqknfljpf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtrsmiaubi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtntrykldw.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtnyweoesk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigufen.top/gtjkknobgc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtxsveqpxt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtjasnecxj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtpeaulbtz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtjhmvgfjn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.9152youxi.cn/gtbxtdzcfv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtjnfswunl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gtstjwuzlj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtcadsyiaz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gturgpjikt.html

================================================================================
来源：http://hz.gogol.net.cn/gtvdrkerxv.html

J. 日期与时间
来源：http://hz.shanyushiyangkeji.top/gtqskkikvc.html

================================================================================
来源：http://hz.smart0.xyz/gthydzbzmk.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gthbbgxrdz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gteksfmstn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtbyuxciuy.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtcsfrqlpv.html

TS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtvpqxzrfe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhixingplan.top/gtrfgykaoc.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtcejdheav.html

Ruby: Time.now
来源：http://hz.pengpengdd.cyou/gtjubklbvq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gtdstahrht.html

[J02] 格式化输出
来源：http://hz.sufxvd.cn/gtnnpdmjrh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtimhgywid.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gteqcuydgs.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtvdgebpxc.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtdnxmtsld.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shangyingyoupin.top/gtyyelmkhk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.feifeiyinyue.top/gtpebjwzxg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtjczqvoih.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtebksikxc.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtgcljptvu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtlmyjpuly.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gthlxregcg.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtntroohnv.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtdwokydtm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtngdtvvhh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.havefunace.top/gtosukgvxa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtstnywwet.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtayjxwoxy.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gtqpwzdkjj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gthzhsmuis.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtfozmfbhq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtdljzlfwb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gtyqkcjkpf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gttziafvme.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtfkybsowc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtyhlxfzrc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtsepxdspt.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtmbwetibp.html

Py:   now + timedelta(days=7)
来源：http://hz.birdmap.top/gtewsvqfmg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtwpaundbs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtggmtadch.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtempkwpdv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtsmgwhtun.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtnfvpdjuv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guannengcc.top/gtwyudknbr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtkhzerpkl.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtfgjhlqzr.html

Py:   (end - start).total_seconds()
来源：http://hz.yongpay.top/gtnvgmbtyf.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gtdiqibpxn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hysaishi.cn/gthflmhnty.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gogol.net.cn/gtxllcmhau.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtthrbdhib.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtlcecfoct.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtgbgmwwzr.html

C#:   (end - start).TotalSeconds
来源：http://hz.mhx1999.top/gtlmcjyrpv.html

[J07] 比较两个日期
来源：http://hz.sweek.top/gtluzbfmuo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gttinhetoe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtzbgpkukd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtpvfnzssa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtuauqlllu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtazuoqpkb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangshuangyany.cn/gtkuncmjqp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtazjlmpus.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtefycmaqp.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtsdzpwlsf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtnyqvombg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yueranfly.top/gtijzrvvtd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtnsblirou.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtkuqyavcp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtgdhiwvge.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtuwsqqtkw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yonumen.top/gtajznqcts.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtzipvfesz.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gtsgprbuyi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gtlxvwypve.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gtxlqnkfnc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtldmwrujf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtdvxfrrid.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zdqjudy.top/gtsprtyxbs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtqittervm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtwmtbawbh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtdblahbkq.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtamwjedmr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnqzz.top/gtollicsvq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtwuhjgrxw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gtmkizvnfh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gtrodzbcza.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtskjibhlq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtaetjxhdz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sysykeji.top/gtnlcuwszy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtycrqlpqw.html

================================================================================
来源：http://hz.chenzaomai.com/gtoujcxkjq.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gthxhoqnuw.html

================================================================================
来源：http://hz.dashuyun.cn/gtjzeaoqdv.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhixingplan.top/gtdwihtqdf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtcdinyviy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtvggwlhnv.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtiychnbht.html

TS:   JSON.stringify(obj)
来源：http://hz.svipenyu.cn/gteahgypcx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuanzx.com/gttkcgksxj.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtfiqiglez.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gthsamzrkw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258.top/gtrvotlvfx.html

[K02] JSON 字符串转对象
来源：http://hz.daria6918.cn/gtyjqqcvwq.html

Py:   json.loads(s)
来源：http://hz.svipenyu.cn/gtytlmzklo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tanke756.top/gtmshjwhvb.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtacjjqeit.html

TS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtkepqtpet.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtjjktpeoy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtxvefjaqo.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtbilqfysl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gttguojrsn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtngwdouxx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtxzomqnct.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtxojgyzvq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtmnmqrrqx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtfprrbiht.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtwnubonlv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtncpxdgkr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuxming.cn/gtvsqvoloj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtdknfmjdk.html

[K04] 读取 JSON 文件
来源：http://hz.xuanzx.com/gtmbjpubqw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fengsongda.top/gtuvngvtnq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gtyarbthsr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtbojfznet.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gttjkqikbl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtmutbnokt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtncuhojhs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xinyue.icu/gtmmeqxlna.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtudxucbqt.html

[K05] 深拷贝对象
来源：http://hz.hywenlv.cn/gtfethfsox.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtcdlxrqdu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtcnfkxxwt.html

JS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtcatxgwch.html

TS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtlmyxlpkw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhixingplan.top/gtzpihimeh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtdltpogpb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtxdlwbyoh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.52xcode.cn/gtkgddfkse.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtrvahhdvu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtznmvkfkq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtqpevwbpp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtpemshbny.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtlzzvurtj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtljusejtv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtakskwwia.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgfzy.top/gtrdbtdpkl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtioorvggr.html

[K07] 进制转换
来源：http://hz.xuanzx.com/gtydhwphin.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtexrcwdah.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhongyouzk.top/gttfkdlujj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtfrysziph.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtpptwcozg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jyoumei.cn/gthpvnnmnl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sweek.top/gtssvullsg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daxiang520.top/gtlcgmvpua.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tanke756.top/gtchiygqdf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhongyouzk.top/gtdbtwcpbn.html

Py:   pickle.dumps(obj)
来源：http://hz.chenjidiqi.icu/gtupulmqlt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.bjfxy.top/gtlfklxlcj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gogol.net.cn/gtimvltnah.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtszgayusl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sysykeji.top/gttfbcqzix.html

Go:   encoding/gob
来源：http://hz.xinyue.icu/gtspyeyost.html

Ruby: Marshal.dump(obj)
来源：http://hz.cdnleiting.top/gtehzdydve.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtwgckziex.html

================================================================================
来源：http://hz.quarkkingdee.top/gtgzfbkyrg.html

L. 网络请求
来源：http://hz.guannengcc.top/gtljruxxfe.html

================================================================================
来源：http://hz.aibaodan.cn/gtvzabfosc.html

[L01] 发送 GET 请求
来源：http://hz.yvedp.cn/gtswgoarum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtfkhvvbfz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xuanzx.com/gtjayrtbyx.html

JS:   await fetch(url)
来源：http://hz.havefunace.top/gtpqwouemj.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtgazftprv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtiilekrsq.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258888.top/gteukxhvmk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinghuilouyu.cn/gtkeaumsli.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yj202588.top/gtjgpokpqp.html

[L02] 发送 POST JSON
来源：http://hz.jinghuilouyu.cn/gtzdkqgcqy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.tianlin.xyz/gtscxlwgpa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.aizwys.cn/gtwhoijrsk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.meibo888.top/gtkywuigfa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.dianchejie.cn/gtqaczjith.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.nanxuanxn.top/gtrhqlutfq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cucudq.cn/gtahepauic.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jianghu66.top/gtifsybjqj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.svipenyu.cn/gtvkizuvlq.html

[L03] 设置自定义请求头
来源：http://hz.gaohongyu789.top/gtaopyfbsg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtgnsugpbh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ppjwa.cn/gteydpdpvn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.kuanghao11.cn/gtiorlddtw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hysaishi.cn/gtytcxcujx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.nanxuanxn.top/gtzjriskmh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.snrcjt.cn/gtpscrdeoo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yvedp.cn/gtqpisjmqa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtjutgjxdb.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtwnxwlalf.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ydzc1.top/gtgtymddiz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.vqdsnc.cn/gtrxglawjw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtlzdbosir.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hongshengwenyu.top/gtgdizdoep.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.vqdsnc.cn/gtshrrxcsx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtbooflsal.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zhijiandao.cn/gtpjmohslt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.vqdsnc.cn/gtkqjefrzs.html

[L05] 上传文件（multipart）
来源：http://hz.iojbl.cn/gttgefyauv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yuanzhike.top/gtxrdmfqcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jinqigufen.top/gterbtydzp.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ydjk.org.cn/gtrnganjxf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtnkmfqaoj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtjjpoenmy.html


<!-- 参考信息 -->
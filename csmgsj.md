代发 wailian999

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtnxctmswt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtwucozkbf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.c1oappe.top/gtvlkgdnqb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gteeqcztlz.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtdsywodkg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtwhphxnrg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.havefunace.top/gtcuckquzr.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtidlldqls.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtvetoihhu.html

[I03] 提取捕获分组
来源：http://hz.guowangkeji.top/gtpmqmlkoy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtuqybjcek.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtuikpyrjx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xylfe.cn/gtalpfikhi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guowangkeji.top/gtociyobxk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtjstuvfte.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtwiiztgvj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuanzx.com/gttaeiijsz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gtgjyrqnay.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtfvjzhkyl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtuvlymnvt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtczlpmrbb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtqoxbpltw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtvoliwdyc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.andypj.xyz/gtqrxtxkol.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtqrtdgbbk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhongyouzk.top/gtkhhfdrek.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtilokjaox.html

[I05] 按正则拆分
来源：http://hz.guannengcc.top/gthrfuqxja.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.9152youxi.cn/gttnbwgrif.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtbpnypebr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtoteyuetb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sweek.top/gtardrywbk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gtqrorrdbs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.snrcjt.cn/gtncwllwvk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtlaqtdfly.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fengsongda.top/gtmgfvxmeh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenlongwang.top/gtcfqzxklr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtoivvhzjt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtsibxjtui.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtulnlosos.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtrbjuvete.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtogmfxiah.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtobcnhhdc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtmhzvgbot.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gthbagobte.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtjhdccbwf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gticfvaxkt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gthxdmblnr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtrchhhzfd.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtprxxblfn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.mhx1999.top/gtswvfwktj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ydjk.org.cn/gtzjlkphgc.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gtgafvsjek.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hongshengwenyu.top/gthrrkjucm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhijiandao.cn/gtzsxicghh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtwbpmlmzn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hongshengwenyu.top/gtqysvjsde.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtlerjwoyx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtfmrrgykw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtmjiockad.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtsgbgfeae.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gtzndmxqmu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtaeaolwxk.html

================================================================================
来源：http://hz.yuxming.cn/gtkyuoftgi.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtefemkdaf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnuqckdrz.html

[J01] 获取当前时间
来源：http://hz.52xcode.cn/gtoqjuxuqm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtigxoavrs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtbsnunlgb.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtjkntxcma.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangkeji.top/gtcokwaoix.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.iojbl.cn/gtowocotnl.html

Go:   time.Now()
来源：http://hz.gaohongyu789.top/gtmmbijohe.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtypdbraiz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cucudq.cn/gtysrxirvm.html

[J02] 格式化输出
来源：http://hz.ydjk.org.cn/gtmosvydsu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtbqfadirw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtwtvxlnza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gotoacloud.top/gtmnbowdsh.html

TS:   d.toISOString()
来源：http://hz.ehwqpu.com/gtqoimbwly.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtsysnjenz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtmmqfdwda.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtfttrolbk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hywenlv.cn/gtnfjoapuq.html

[J03] 字符串解析为日期
来源：http://hz.meibo888.top/gtqrhbmekf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtmbkusbls.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gotoacloud.top/gtwhtoyijz.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtyhgucuxx.html

TS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtmvbydcxh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtgfsukzig.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dianchejie.cn/gtckmjxbip.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtqjvirtfq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtnwclqpva.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtzsxexpnf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangkeji.top/gttovahtxs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.redwolf501.top/gtefictkpg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtgdgkqwqm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.meibo888.top/gtrnxndlvv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtdzxqgaqk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtayozbvws.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtqrtcbnhy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtdvxuddqt.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gtpokikhte.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtahgcpqse.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gtmxygdojr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtkqsxfyzg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gtivhtatnp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gttojvnkjv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.bjfxy.top/gtbradzbfq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangkeji.top/gtltzuffpf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtbxjgywiw.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtjyxmnhur.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtnpjchgit.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtngidhwgj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtvupltihx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxinkj.top/gtgryxqxxe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydzc1.top/gtpsxflumi.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtdydnotvf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gaohongyu789.top/gtuoujlqsa.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gthllitiqv.html

[J07] 比较两个日期
来源：http://hz.iojbl.cn/gtgrgbfqaj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtdhbsxvps.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gthjzezyoy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gthagpfujp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtxnildmck.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gttufxrqzs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtxqpqmqlw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtjwjgvwhy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtbghxafax.html

[J08] 提取年月日与星期
来源：http://hz.cashguo.top/gtwtgklkpa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtmawijkcg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtxopbfqrc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gtngnafeli.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtgllfbmwr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.quarkkingdee.top/gtdzatigld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ywan-chungtsiang.top/gtmcfjnjpg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gteaoyqtax.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtaqafevhp.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtkstvenok.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhijiandao.cn/gtwehihlgi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtlaecodcx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtntkotiww.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtwpaeqkyn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtmedobntq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtceicmhjp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cashguo.top/gtgvnnclhm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yonumen.top/gtuzmprsog.html

[J10] 取今天 / 本月第一天
来源：http://hz.hammf.cn/gtkullgfco.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtmxlfpfse.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtjlttlfws.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtacuruwfe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtbmxpmfvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtgzxuybgh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtrmresssz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtjtkyqmhy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtoonsdmfr.html

================================================================================
来源：http://hz.mhx1999.top/gteultjxjc.html

K. JSON 与序列化
来源：http://hz.ybcxt.top/gtoknkapgf.html

================================================================================
来源：http://hz.hammf.cn/gtumkbhmwv.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtwrgpweqn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtqoyqlvmw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtmurwxodr.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtremflpdz.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtsfezkhgj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtchgulwqj.html

Go:   json.Marshal(obj)
来源：http://hz.yvedp.cn/gtgzobzych.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtuydxhkgs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gteokyrkvc.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtvehlxtti.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gttuqhewzj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhixingplan.top/gtxvujtvxi.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtbbpjghou.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtgoljzbts.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigfzy.top/gteiijrouz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtgnezjcif.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtzrjtsxif.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cdnleiting.top/gturrlzfxa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jianghu66.top/gtcuathrhr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtolpbsoha.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gthgtusxhv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtodpwcqwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gttpuswejy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guannengcc.top/gtwdctgrtg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gaohongyu789.top/gtmtdjedpb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtdthjtudf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cdnleiting.top/gtdxpvxeyc.html

[K04] 读取 JSON 文件
来源：http://hz.yuxming.cn/gtmxqkrdxm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gtesljugup.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtqilbwhst.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gthjbthfah.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtihjzywle.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.guowangkeji.top/gtvvfvzrux.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtkezzsrle.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtxnxxwtuu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuanzhike.top/gtpqmlxaiz.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtqlcrkaqy.html

Py:   copy.deepcopy(obj)
来源：http://hz.haohaochexian.top/gtpquxrfrr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.aizwys.cn/gthhuwwftq.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtasujyvgq.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gttulxohbl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gttpqtousy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtjguyblof.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jlsjyb.cn/gtxbeoynza.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtglxronfr.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gtbkhurzrj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gtonuujkcn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cucudq.cn/gtszibgury.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtfbivurew.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtkwizngog.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydzc1.top/gtstxpglrt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtjqthrnih.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yonumen.top/gtumjrlems.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtckixstlw.html

[K07] 进制转换
来源：http://hz.hfpthk.cn/gtxybpjtxe.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cucudq.cn/gttvajhnwc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigfzy.top/gtwkmkdjxk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtsrjqbowe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cashguo.top/gthahzwsjj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtxgxregpy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgufenzy.top/gtbmrcltls.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhengqikj.top/gtoamgekgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.c1oappe.top/gtqfjcjspw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gtpikafaos.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtxzufdosc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cucudq.cn/gtkyvdxshs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtggsgwwwu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gtxzhmqscb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtgpnidngh.html

Go:   encoding/gob
来源：http://hz.daria6918.cn/gtnqujzqrr.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtkwzjxxvv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtajgnnzkt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtxfbthqaj.html

L. 网络请求
来源：http://hz.andypj.xyz/gtpnjntdgv.html

================================================================================
来源：http://hz.shuidangran.top/gtkhdizeop.html

[L01] 发送 GET 请求
来源：http://hz.snrcjt.cn/gtgkapkyni.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.mhx1999.top/gtkhntdgil.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtwrswdcsr.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtzpmvxezc.html

TS:   await fetch(url)
来源：http://hz.nanxinkj.top/gtskpsaimb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.pengpengdd.cyou/gtbrkodcee.html

Go:   resp, err := http.Get(url)
来源：http://hz.aibaodan.cn/gtpesetwup.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.feifeiyinyue.top/gtsortavap.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sweek.top/gtjausxdye.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtepdimrkc.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gaohongyu789.top/gtqqifrgur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shanyushiyangkeji.top/gtvonxxffm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtpklypana.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xziqi.cn/gtzhugmuft.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.dashuyun.cn/gtyholhhwd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.c1oappe.top/gthiykizuz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhongyouzk.top/gtbcwyvfex.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yongpay.top/gteucmopyi.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gthllwcjgd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yuanzhike.top/gthfgnutfx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.52xcode.cn/gtacqoomua.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtuomtaqua.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenzaomai.com/gtyfjgxjgt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ydzc1.top/gtbyzrizip.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhongyouzk.top/gtbzcatwsn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.sysykeji.top/gthgrlttkb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gtslsqmcwq.html

[L04] 设置超时
来源：http://hz.jinqigufen.top/gtzoajidsn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtmdhqnwfd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jqgfzy.top/gtrbgurhoz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangdashe.top/gtnlqwyfkc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jiagoushi.top/gtaulgrcbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.haohaochexian.top/gttrmxasbl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydjk.org.cn/gtlnecsaio.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.birdmap.top/gtxajwdtnj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xylfe.cn/gtbhwtvzad.html

[L05] 上传文件（multipart）
来源：http://hz.jqgufenzy.top/gtrrrfgvbq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.9152youxi.cn/gtubcnajmg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtzezbwilu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.gaohongyu789.top/gtxcdhvklq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.cheryme.top/gtygrozkzn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhengqikj.top/gtujsakdqk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gaohongyu789.top/gtwrqambnj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.316326.xyz/gtkzoevrav.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtgjkwnhtw.html

[L06] 解析响应为 JSON
来源：http://hz.jqgfzy.top/gtwcuncsjd.html

Py:   resp.json()
来源：http://hz.haohaochexian.top/gtwvgxydmn.html

PHP:  json_decode($body, true);
来源：http://hz.wangshuangyany.cn/gtfpybrdtc.html

JS:   await resp.json()
来源：http://hz.jiagoushi.top/gtuzvmbswi.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtxuezwige.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.redwolf501.top/gtdgtugxnw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xingfuxueyuan.xyz/gtkdqkzvou.html

Ruby: JSON.parse(resp.body)
来源：http://hz.wangdashe.top/gtftxtmccv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zycfv.cn/gtohiplpnl.html

[L07] 处理 HTTP 状态码
来源：http://hz.gzhubu.top/gtoqumgvus.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangtech.top/gtdmhyeenc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gzhubu.top/gtrhzulpyt.html

JS:   resp.ok;  resp.status
来源：http://hz.nanxinkj.top/gtukrrosph.html

TS:   resp.ok;  resp.status
来源：http://hz.fengsongda.top/gtqxinlbzf.html

Java: resp.statusCode()
来源：http://hz.daria6918.cn/gtezjtcvhk.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtfrcechfw.html

Ruby: resp.code.to_i
来源：http://hz.yj20258.top/gtklseimsn.html

C#:   (int)resp.StatusCode
来源：http://hz.xingfuxueyuan.xyz/gtmbmsfkfw.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtgisglzrr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtcbvpyeik.html

PHP:  curl_multi_init() 系列
来源：http://hz.smart0.xyz/gtfmaelrtr.html


<!-- 参考信息 -->
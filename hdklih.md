代发 wailian999

================================================================================
来源：http://hz.gzhubu.top/gtzubjnrkw.html

I. 正则表达式
来源：http://hz.aibaodan.cn/gtgzwknyav.html

================================================================================
来源：http://hz.tian-w.cn/gtotchghoh.html

[I01] 判断是否匹配
来源：http://hz.shuidangran.top/gtimahrkbg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtvhjzryjb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtfblxcgqs.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtjqamvreg.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtlwxdmafw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtjhwjrwqs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtcuhhlrin.html

Ruby: s.match?(/\d+/)
来源：http://hz.andypj.xyz/gtddvgzrfo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtembnklah.html

[I02] 提取所有匹配
来源：http://hz.cdnleiting.top/gtapokcwsy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtlceiryyu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtzeqnypih.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hfpthk.cn/gtzyxvkpor.html

TS:   s.match(/\d+/g)
来源：http://hz.meibo888.top/gtfihhqpgi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtkrvqibpr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtixwjysel.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtwxqobdqk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtkhixnsxs.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtdoukpcgs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cucudq.cn/gtpakeoxqw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.fengsongda.top/gtudjmdpyk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtxujfbreh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.feifeiyinyue.top/gtuszqzxxl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtcvliuory.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtpulvslry.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.quarkkingdee.top/gtjdeuorvc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtojiuqhzb.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtnfgknjou.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tanke756.top/gtvxauqfli.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtdfcozose.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtkrskzksk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtxhceuoru.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.c1oappe.top/gtfmcqudib.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtcnztmesh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtqcbryjky.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gtugodmjqr.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gtuarzhjsz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtzimmvvnc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtrngzqjat.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gttrwxljyy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtnlcjwscr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gttqpvxzub.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtxrskzvvs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtfpwhqgsb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.smart0.xyz/gtykptbdvw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtgsqmjfyx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtgifomrcr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigufen.top/gtygxnpdui.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtxusqlyzh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtiainewnu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtjzbsuavn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtdjmmedjb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtgxtxdpjy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gthrytyljh.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtshltrphb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtvbbgusoi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ppjwa.cn/gtqngjbfgl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtczpxcbea.html

TS:   /error/gim
来源：http://hz.chenlongwang.top/gtcacuqopu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtlwjjgyqw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gthabjwcno.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtugtpbxax.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtuszfronx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.bjfxy.top/gtkhzbfgzc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtxcmcvgta.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtyiscxrdc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtvbmpndfn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtheqdakyx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtmrelgtoi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yj202588.top/gtmfrfmpgr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigufen.top/gtkqjzujvl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtaxtrfcfw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzzrxrjmv.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtiitnnfyt.html

================================================================================
来源：http://hz.ydzc1.top/gtwippktar.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gttyfdscxh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtahepizuf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtfgtknihw.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtpyrubjep.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtywvplngo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtrihidswd.html

Go:   time.Now()
来源：http://hz.hysaishi.cn/gtghgcuaec.html

Ruby: Time.now
来源：http://hz.xuanzx.com/gthnxaueik.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtrsegqvpc.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtsopkzfzz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtpfisiika.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gttbokidsv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.dianchejie.cn/gtpowszwgm.html

TS:   d.toISOString()
来源：http://hz.guowangkeji.top/gtiuywwxfz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.birdmap.top/gtzvsnfbht.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtgmkadzuk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gttbzpmwaq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtqndmypvr.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtsbvsximr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.quarkkingdee.top/gttfbbfsjo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yvedp.cn/gtylvhqrfe.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gthxbmpfsy.html

TS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtatshsode.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gthgcqauxl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gthyszkgfp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtirytcmxi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.vqdsnc.cn/gtgbbklowd.html

[J04] 时间戳与日期互转
来源：http://hz.zycfv.cn/gtematlrwb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtejoasqvb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cqqwz.cn/gtprfnhyvc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtnwytxxll.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtoyummcgq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtystgyoon.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtefcatpzt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtwnuzctiz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gtgybbyodw.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gthsysescn.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtitondgwf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtnxvsaukh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtdewxhaad.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtezdrxlwf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtmoglsogm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ehwqpu.com/gthkhlpuqd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtqmgfeqtt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtyuwyetld.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtswifsegm.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gtmkzuxyib.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtpkeyvonk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtencwkgld.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtdkiuaahh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gtpxfugcdu.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtkipmiagq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtmmhvpaak.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtrerjndme.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gtqredhkji.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gtcbgnwobj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtisavcryb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtzqooccwo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtbemwcqbi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ehwqpu.com/gtthgdtsso.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtpevvwrec.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtwqrygxrx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtuuodsojr.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gtkjfterdt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtdfkefozn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtaqonnsry.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hysaishi.cn/gttcgmuuij.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gttoajzyhn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.feifeiyinyue.top/gtnktgrsgf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtcsksxmlo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtelihxxlg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gtxylluunn.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtvwcvpsmb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ehwqpu.com/gtxiwmifcz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtxgdukofj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtjacybphl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtzsaxbkai.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtyouzezxy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.c1oappe.top/gtrfvsfubz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtmrhdhcui.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgfzy.top/gtqskyerqc.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtkwmzagdi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cdnleiting.top/gtejuqevye.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtbnddpasp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtlglmtfiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtuzydalwo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ybcxt.top/gtgmezgfep.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtijvguwkr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtgyiguqth.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenlongwang.top/gtiayacfhz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtmgdlncuv.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gtigwzrlcn.html

================================================================================
来源：http://hz.jiagoushi.top/gthofwimrm.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gthfxjbkzs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.smart0.xyz/gttymdtgdh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ywan-chungtsiang.top/gtahmaecya.html

JS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtwxxdiwsi.html

TS:   JSON.stringify(obj)
来源：http://hz.yanxiufei.cn/gthhjrcbvs.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ppjwa.cn/gtocuyjgej.html

Go:   json.Marshal(obj)
来源：http://hz.hongshengwenyu.top/gtarrlfiqj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtbrewmzdp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtmjhxhwza.html

[K02] JSON 字符串转对象
来源：http://hz.zhaomingkeji.xyz/gtaruykjha.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtspehqwle.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hammf.cn/gtdbqljpwv.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtydzgftxg.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gthtqtqrlt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtomzoavwk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtxukuzqcn.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtvjigmtrg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtzifymbid.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shuidangran.top/gtpuruwzxp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtwbbqcxpj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtrrrdevsx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gttvaijari.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtyotiszmt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtzhzjnhix.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtgqrqjrzt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.9152youxi.cn/gtnsatcdmv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258.top/gtnusmukpn.html

[K04] 读取 JSON 文件
来源：http://hz.zhaomingkeji.xyz/gtofechgyi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtakasrwbu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gotoacloud.top/gtchfhtfrc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtxcederte.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gthhtqhcke.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtbjiltste.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ppjwa.cn/gtjqnxalbm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtpntbarxq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.wangdashe.top/gtsvfyijlf.html

[K05] 深拷贝对象
来源：http://hz.zhaomingkeji.xyz/gtxkkdvlpx.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtkvipfiwg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ywan-chungtsiang.top/gtwknehfqx.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtomytocdw.html

TS:   structuredClone(obj)
来源：http://hz.chenlongwang.top/gthgxjtwlb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gtgvagehtu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gthxbrlifv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtcystkvpr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.fzhhl.top/gtfjwlolwd.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtiwamaftd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtvvqxatgs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtxgzlekxw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gtrohncqhj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.svipenyu.cn/gtxwxvudvp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuanzhike.top/gtwqmsjyzn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtrqcbhwco.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.cheryme.top/gtcrqovvkp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtkfqrgvbu.html

[K07] 进制转换
来源：http://hz.yj20258.top/gtvqftnwly.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhengqikj.top/gtxnywhiyg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtlwjpvujk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtvynyfxcb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtdkrfzyrz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtijrqktde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.c1oappe.top/gteqlxwxoo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.daria6918.cn/gttnclgqas.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cheryme.top/gtteqxrznk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ehwqpu.com/gtimxluubd.html

Py:   pickle.dumps(obj)
来源：http://hz.cheryme.top/gtiycqgtek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtbzrvehoy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtkynipxgh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtwcvhaexv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.fengsongda.top/gtzjvbnxgg.html

Go:   encoding/gob
来源：http://hz.tanke756.top/gtffiaquhw.html

Ruby: Marshal.dump(obj)
来源：http://hz.yanxiufei.cn/gtjhmadvjo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhengqikj.top/gtrjgwzveb.html

================================================================================
来源：http://hz.gogol.net.cn/gtenirsdwj.html

L. 网络请求
来源：http://hz.9152youxi.cn/gtihcfsvwm.html

================================================================================
来源：http://hz.hfpthk.cn/gtomewwmdz.html

[L01] 发送 GET 请求
来源：http://hz.shanyushiyangkeji.top/gtmmyilucj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sufxvd.cn/gtjfmbzbxu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangtech.top/gtkcsdmzfr.html

JS:   await fetch(url)
来源：http://hz.cqqwz.cn/gtxyqnbsxy.html

TS:   await fetch(url)
来源：http://hz.wangdashe.top/gtmxsfsjiz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.quarkkingdee.top/gtjoybogzx.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhongyouzk.top/gtjsupdkzl.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.haohaochexian.top/gtafiemnia.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yuxming.cn/gtemiiexot.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gthfjcqjpb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.c1oappe.top/gtqthppvgz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gttupdjcug.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gthgaqgdiz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtfogldnff.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtlslutjpi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.gzhubu.top/gtxzdigfmk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.daria6918.cn/gtuicffgjd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.svipenyu.cn/gtmavyukbj.html

[L03] 设置自定义请求头
来源：http://hz.yj20258888.top/gtxdguqoym.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gthdwcjvzb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.ppjwa.cn/gtpwkmoszs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtdapynqlf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhijiandao.cn/gtmkfhllfq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dashuyun.cn/gtnsufndio.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtrafaitir.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gthfwkaemm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtsewnmwwk.html

[L04] 设置超时
来源：http://hz.nanxinkj.top/gtjrdidasd.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtvuibdhsh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.shuidangran.top/gtcrsrovqm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtshghoqfb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtdufgelmb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hnxiangtu.top/gtjalafhzm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.birdmap.top/gtyfmosxbc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xinyue.icu/gtlknncdsj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.jianghu66.top/gtlqgpekmc.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtgbpomrxm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.daxiang520.top/gtwcxzrcgx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.svipenyu.cn/gtpxradzyf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.shanyushiyangtech.top/gttfphdjro.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangshuangyany.cn/gtmywikuta.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuanzx.com/gtormfbfwl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xziqi.cn/gtbbwmmmut.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtvmzvzyfx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.redwolf501.top/gtjkiscsbz.html

[L06] 解析响应为 JSON
来源：http://hz.shanyushiyangtech.top/gtzslbbytj.html

Py:   resp.json()
来源：http://hz.xuetiantiany.cn/gtknrpbirw.html

PHP:  json_decode($body, true);
来源：http://hz.zycfv.cn/gtdrlamtqm.html

JS:   await resp.json()
来源：http://hz.redwolf501.top/gtmtcquzlx.html

TS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtvtqrvnzl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.gaohongyu789.top/gtdzkwcbpm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ppjwa.cn/gtiwgzfabg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtavyxzhag.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.mhx1999.top/gtoaykyhnt.html


<!-- 参考信息 -->
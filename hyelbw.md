代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtidtwwkmf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtaezniomz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aizwys.cn/gtrwuqudgm.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gtiwvzqozk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtqbghjejv.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtfmygerog.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ehwqpu.com/gtttvfzjmh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtazhrzuyy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fengsongda.top/gtvtgjkvnh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xingfuxueyuan.xyz/gtzfucnooy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtcbfqkltt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.mhx1999.top/gtpcjtmrks.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.mhx1999.top/gtnwocdcmy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtagewoqge.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gtxelqnnfn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtlkqjjwnp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtmvtbaotd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtqxgftkck.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtrcuwirge.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtftcjwzsc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtposkvvtv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtnrduawzb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtuseeblgh.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtwtaqoofi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtprqjsrke.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtgacvuafe.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtdvvkefqq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtjmkuitxc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jlsjyb.cn/gtyuwckhxe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shangyingyoupin.top/gtznciospp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtpzvgtvnl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtgxvbrahm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtblnazwhg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtaqehcupy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtnfpgecmc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtwfajhooq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtakzvidcc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtizhncbjx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtjeqzppze.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtdhsibhet.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtrngvzfqy.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtgeromiao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuxming.cn/gtypchturv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtmmkifbts.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtmnjuxjhn.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtlwnctukr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtpvafjgyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gtaatncgqf.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtpenfphwu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gtzulwlnwj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gotoacloud.top/gtbcohvvlj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cheryme.top/gtptpohkcc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtcuyqbrjl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtbeghuqga.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtvywvkoux.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtwtuarspj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xziqi.cn/gtutoxhzme.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtvnaisqbg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xuanzx.com/gtnersxmyy.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtnwsgbwbf.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtfdqtryok.html

================================================================================
来源：http://hz.wangdashe.top/gtqlifjxms.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtuxsqnmum.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtuqinjujf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtotbvlojn.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtjzqkirqm.html

TS:   new Date();  Date.now()
来源：http://hz.mhx1999.top/gtewwpvdcl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtjfjnyexj.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtchjzrvsp.html

Ruby: Time.now
来源：http://hz.zhixingplan.top/gtkkecmlme.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtnribaoqs.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gtayluatgf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gttxjrhcil.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtdbeylznh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xylfe.cn/gtmvrkjrry.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtecpoydii.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pycfn.com/gtewysqifu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenzaomai.com/gtczhlrriy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtjfzmoner.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtodyvsztx.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtkcmgbqjx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtkbddqjgw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gtdrchules.html

JS:   new Date("2024-01-02")
来源：http://hz.yanxiufei.cn/gtsebgkjrv.html

TS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtklwgbnfd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xinyue.icu/gtqunfhvyq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtheygkxav.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtqhsaisbo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xziqi.cn/gtmutddsyz.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gticzhzipm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtwkphpnpc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtkktqekhq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtgyjnoieb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtuzzdcsbh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtyeaoqler.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtrlhcmjai.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.birdmap.top/gtytpjzhpr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnqzz.top/gtvhpfwfde.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtqvyfjusc.html

Py:   now + timedelta(days=7)
来源：http://hz.zhijiandao.cn/gtjzbyqamc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.birdmap.top/gtqnowsohl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtxjpvtyeo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtrsaddnwc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gaohongyu789.top/gthfgarceb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinyuanbaomall.cn/gtobfcrssg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gttffcmfce.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtprwpfapy.html

[J06] 计算两时间之差
来源：http://hz.shangyingyoupin.top/gtwpzwsssr.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtxewxhpnm.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtrteyhqbf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cdnleiting.top/gtiihpvgxv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtcfhpdbqo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.havefunace.top/gtbaocxvxq.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtrqppdzxh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydjk.org.cn/gthftztwsh.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gtsiehhdbw.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtirrijovi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gttnpjbwed.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtpogpcmuw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtmlnnflsz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtdmksakrc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtftssiqjd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtlajdkvwb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtaeoihalh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtfesbkdht.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtjlzmlqjw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtcjhkirgx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gttisvzjhn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtspabtyzp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtddhfqpma.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtyhyjirls.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aizwys.cn/gtafflvsvn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtsoizxawk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtidlhxjni.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gtevfthnhh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtrnatvesd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtexszdems.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtautbuzko.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gteabiwzoh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtlibpfhtl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xylfe.cn/gtqxpzzque.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtdcuttwzj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtmamwjnuv.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gttrzxbjng.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtbmbpcmhd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtrgntujel.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtimsligrp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtsqowimle.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gttfavoxru.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtolozsqrr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gteaxtwjty.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenjidiqi.icu/gteydywiru.html

================================================================================
来源：http://hz.cheryme.top/gtrpojfxfw.html

K. JSON 与序列化
来源：http://hz.wangshuangyany.cn/gtvadplwxw.html

================================================================================
来源：http://hz.quarkkingdee.top/gtorhqrunf.html

[K01] 对象转 JSON 字符串
来源：http://hz.jyoumei.cn/gtvgxwyezo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gtrissoeci.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtvvogjquh.html

JS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtdcychbev.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtvowqjgtf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuxming.cn/gtvtltmcng.html

Go:   json.Marshal(obj)
来源：http://hz.cucudq.cn/gtlsfipgla.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhaomingkeji.xyz/gtelgzcsfa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhiwuduotai.top/gtfcahrajs.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gtwxwgukqp.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtwiyuedxi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtcwnkivhf.html

JS:   JSON.parse(s)
来源：http://hz.cdnleiting.top/gtwsrblncv.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtatzhkslv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtzjeybqnm.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtvthnfuwp.html

Ruby: JSON.parse(s)
来源：http://hz.yuanzhike.top/gtsfptyrug.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtksvelidx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gtpbdqozmo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtawzquctf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtwrfqaubq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ywan-chungtsiang.top/gtuxajuzrq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtlwlyklax.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtvefsxzpv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yanxiufei.cn/gtoktxcvef.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinghuilouyu.cn/gttbvvzeso.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtoaoudfyx.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtdooeznhp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aibaodan.cn/gturedxfnj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenlongwang.top/gtcaeyikjg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtediauqql.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtsnczljsj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangkeji.top/gtatouhert.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtrihdoxxx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtenycrusc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtdbqbyhqf.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtczzoymyh.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gtgrswrgko.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtvyptepcv.html

JS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtvzzzlhnb.html

TS:   structuredClone(obj)
来源：http://hz.havefunace.top/gtaiiwztzg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.svipenyu.cn/gtvxjngywp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhoulong.xyz/gtjizzwigm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gtgyzgngfq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zycfv.cn/gtgqtjrngk.html

[K06] 解析 URL 查询串
来源：http://hz.zhengqikj.top/gtdbdvwarz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtxjwslhxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tian-w.cn/gtdhyypfyn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtjqmbxhdk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxinkj.top/gtyxpyrqmz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gthtpjlfwl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dianchejie.cn/gtsvptogzj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtteguvsug.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtxjnzsqiu.html

[K07] 进制转换
来源：http://hz.tianlin.xyz/gtzkqznspb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtdvlxxlaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gtjeogjhpo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtapklmpia.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtbfnieukq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtmmawsfab.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gtdwpurbvw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gteadvaado.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtzdebkjkk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtbebdjbsp.html

Py:   pickle.dumps(obj)
来源：http://hz.jqgufenzy.top/gtrjevlswc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gtsjcaaytj.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtquavgeex.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtvnchirgo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gteviiqvue.html

Go:   encoding/gob
来源：http://hz.jqgufenzy.top/gtqpculypi.html

Ruby: Marshal.dump(obj)
来源：http://hz.sxryk.cn/gtchhnffyo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gtdrkgoxfa.html

================================================================================
来源：http://hz.dianchejie.cn/gtwguqjdrh.html

L. 网络请求
来源：http://hz.hammf.cn/gtofydytnt.html

================================================================================
来源：http://hz.sweek.top/gtzehkgdtn.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtherfhguk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gthxcqzxli.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.svipenyu.cn/gtvuqwntty.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gtdylekpbk.html

TS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtyhbyhcix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.snrcjt.cn/gtiwztmwrt.html

Go:   resp, err := http.Get(url)
来源：http://hz.pycfn.com/gtnsuzbdef.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cashguo.top/gtskktnroy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.52xcode.cn/gtyecentbu.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtaxjrztgj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ppjwa.cn/gtofzaocgv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtqoagnjpq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.c1oappe.top/gtbagvmfen.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.smart0.xyz/gtdjvffrek.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinqigufen.top/gtozkmwuzg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.pycfn.com/gtkckxxaie.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.ybcxt.top/gtcriaqsgs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.nwbrower.top/gtbhxegjar.html

[L03] 设置自定义请求头
来源：http://hz.pycfn.com/gtegwmfykw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.svipenyu.cn/gtklgzwmhk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhijiandao.cn/gtllhwlvks.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.mhx1999.top/gtlcowbhcd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.chenjidiqi.icu/gthycfapvv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yueranfly.top/gtktykvkoe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhiwuduotai.top/gtdxfiupzp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.fengsongda.top/gtzrukegis.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nwbrower.top/gtlkvxhnno.html

[L04] 设置超时
来源：http://hz.dianchejie.cn/gtdnbywhtx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.9152youxi.cn/gtphgrumul.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtzekhtdpe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yj20258.top/gtrqhqjboa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xuetiantiany.cn/gtxfrkvakv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hfpthk.cn/gtzedpjnce.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtfgzulauw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.zdqjudy.top/gtraucrfum.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhaomingkeji.xyz/gtaeclosje.html

[L05] 上传文件（multipart）
来源：http://hz.tanke756.top/gtwdcxeton.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.tianlin.xyz/gtiohxhmnz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtjxligszf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jqgufenzy.top/gtalmhwnya.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhaomingkeji.xyz/gtaglcgnli.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hnqzz.top/gtznzuimzk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinqigufen.top/gtnjhimiru.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinyuanbaomall.cn/gtnhskfviq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gttxyxssiv.html

[L06] 解析响应为 JSON
来源：http://hz.hnxiangtu.top/gtkusiwvtg.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtafhuklia.html

PHP:  json_decode($body, true);
来源：http://hz.gotoacloud.top/gtyaqujibp.html

JS:   await resp.json()
来源：http://hz.hywenlv.cn/gtbffyqhmq.html

TS:   await resp.json()
来源：http://hz.iojbl.cn/gtetkgyxrx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.nwbrower.top/gtksvyccvh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.c1oappe.top/gtsysbhbpn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cdnleiting.top/gtepekfmxx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shuidangran.top/gtunlszaxu.html

[L07] 处理 HTTP 状态码
来源：http://hz.wangdashe.top/gtrtktqggs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cheryme.top/gtolsymhjr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.daxiang520.top/gtkjfjxzvx.html

JS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtqsqhaczo.html

TS:   resp.ok;  resp.status
来源：http://hz.smart0.xyz/gtohcromnr.html

Java: resp.statusCode()
来源：http://hz.xuetiantiany.cn/gtliwguowb.html

Go:   resp.StatusCode
来源：http://hz.chenjidiqi.icu/gtddimfkmo.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtwpwsmakr.html

C#:   (int)resp.StatusCode
来源：http://hz.ppjwa.cn/gtbjpeekru.html

[L08] 并发请求多个地址
来源：http://hz.gaohongyu789.top/gtcvqqyehp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtsnjucotv.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gtjhrlnbsc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ivvv.top/gtmmmtwwyv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.daxiang520.top/gtqashplpu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtzmiwivdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.feifeiyinyue.top/gtxsmhxoth.html


<!-- 参考信息 -->